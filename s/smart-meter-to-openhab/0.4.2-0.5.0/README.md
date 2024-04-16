# Comparing `tmp/smart_meter_to_openhab-0.4.2.tar.gz` & `tmp/smart_meter_to_openhab-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "smart_meter_to_openhab-0.4.2.tar", max compression
+gzip compressed data, was "smart_meter_to_openhab-0.5.0.tar", max compression
```

## Comparing `smart_meter_to_openhab-0.4.2.tar` & `smart_meter_to_openhab-0.5.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1211 2024-04-11 19:28:35.047443 smart_meter_to_openhab-0.4.2/LICENSE
--rw-r--r--   0        0        0     4580 2024-04-11 19:28:35.047443 smart_meter_to_openhab-0.4.2/README.md
--rw-r--r--   0        0        0      793 2024-04-11 19:28:35.047443 smart_meter_to_openhab-0.4.2/pyproject.toml
--rw-r--r--   0        0        0      543 2024-04-11 19:28:35.047443 smart_meter_to_openhab-0.4.2/smart_meter_to_openhab/.env.example
--rw-r--r--   0        0        0      349 2024-04-11 19:28:35.047443 smart_meter_to_openhab-0.4.2/smart_meter_to_openhab/__init__.py
--rw-r--r--   0        0        0     8849 2024-04-11 19:28:35.047443 smart_meter_to_openhab-0.4.2/smart_meter_to_openhab/interfaces.py
--rw-r--r--   0        0        0     7314 2024-04-11 19:28:35.047443 smart_meter_to_openhab-0.4.2/smart_meter_to_openhab/openhab.py
--rw-r--r--   0        0        0     8594 2024-04-11 19:28:35.047443 smart_meter_to_openhab-0.4.2/smart_meter_to_openhab/sml_iskra_mt175.py
--rw-r--r--   0        0        0     3531 2024-04-11 19:28:35.047443 smart_meter_to_openhab-0.4.2/smart_meter_to_openhab/sml_reader.py
--rw-r--r--   0        0        0      301 2024-04-11 19:28:35.047443 smart_meter_to_openhab-0.4.2/smart_meter_to_openhab/utils.py
--rw-r--r--   0        0        0     7084 2024-04-11 19:28:35.047443 smart_meter_to_openhab-0.4.2/smart_meter_to_openhab_scripts/main.py
--rw-r--r--   0        0        0     5253 1970-01-01 00:00:00.000000 smart_meter_to_openhab-0.4.2/PKG-INFO
+-rw-r--r--   0        0        0     1211 2024-04-15 19:52:48.196297 smart_meter_to_openhab-0.5.0/LICENSE
+-rw-r--r--   0        0        0     4580 2024-04-15 19:52:48.196297 smart_meter_to_openhab-0.5.0/README.md
+-rw-r--r--   0        0        0      793 2024-04-15 19:52:48.200296 smart_meter_to_openhab-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0      543 2024-04-15 19:52:48.200296 smart_meter_to_openhab-0.5.0/smart_meter_to_openhab/.env.example
+-rw-r--r--   0        0        0      349 2024-04-15 19:52:48.200296 smart_meter_to_openhab-0.5.0/smart_meter_to_openhab/__init__.py
+-rw-r--r--   0        0        0     8806 2024-04-15 19:52:48.200296 smart_meter_to_openhab-0.5.0/smart_meter_to_openhab/interfaces.py
+-rw-r--r--   0        0        0     7714 2024-04-15 19:52:48.200296 smart_meter_to_openhab-0.5.0/smart_meter_to_openhab/openhab.py
+-rw-r--r--   0        0        0     7647 2024-04-15 19:52:48.200296 smart_meter_to_openhab-0.5.0/smart_meter_to_openhab/sml_iskra_mt175.py
+-rw-r--r--   0        0        0     3531 2024-04-15 19:52:48.200296 smart_meter_to_openhab-0.5.0/smart_meter_to_openhab/sml_reader.py
+-rw-r--r--   0        0        0      420 2024-04-15 19:52:48.200296 smart_meter_to_openhab-0.5.0/smart_meter_to_openhab/utils.py
+-rw-r--r--   0        0        0     6063 2024-04-15 19:52:48.200296 smart_meter_to_openhab-0.5.0/smart_meter_to_openhab_scripts/main.py
+-rw-r--r--   0        0        0     5253 1970-01-01 00:00:00.000000 smart_meter_to_openhab-0.5.0/PKG-INFO
```

### Comparing `smart_meter_to_openhab-0.4.2/LICENSE` & `smart_meter_to_openhab-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `smart_meter_to_openhab-0.4.2/README.md` & `smart_meter_to_openhab-0.5.0/README.md`

 * *Files identical despite different names*

### Comparing `smart_meter_to_openhab-0.4.2/pyproject.toml` & `smart_meter_to_openhab-0.5.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "smart_meter_to_openhab"
-version = "0.4.2"
+version = "0.5.0"
 description = "Pushing data of ISKRA MT175 smart meter to openhab"
 authors = ["Heiko Bauer <heiko_bauer@icloud.com>"]
 repository = "https://github.com/die-bauerei/smart-meter-to-openhab"
 readme = "README.md"
 packages = [
     {include = "smart_meter_to_openhab"},
     {include = "smart_meter_to_openhab_scripts"}
```

### Comparing `smart_meter_to_openhab-0.4.2/smart_meter_to_openhab/.env.example` & `smart_meter_to_openhab-0.5.0/smart_meter_to_openhab/.env.example`

 * *Files identical despite different names*

### Comparing `smart_meter_to_openhab-0.4.2/smart_meter_to_openhab/interfaces.py` & `smart_meter_to_openhab-0.5.0/smart_meter_to_openhab/interfaces.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,16 +60,16 @@
                     this_value.value = new_value.value
                     break
 
     def __iter__(self) -> Iterator[OhItemAndValue]:
         return iter(self._oh_items_and_values)
     
     def is_invalid(self) -> bool:
-        # consider only the values that really will be used (oh_item name not empty)
-        return all(oh_item_value.value is None for oh_item_value in self._oh_items_and_values if oh_item_value.oh_item)
+        number_values=[value for value in self.value_list() if value is not None]
+        return (not number_values) or any(value < 0 for value in number_values)
     
     def is_valid(self) -> bool:
         return not self.is_invalid()
     
     def value_list(self) -> List[Any]:
         # consider only the values that really will be used (oh_item name not empty)
         return [oh_item_value.value for oh_item_value in self._oh_items_and_values  if oh_item_value.oh_item]
```

### Comparing `smart_meter_to_openhab-0.4.2/smart_meter_to_openhab/openhab.py` & `smart_meter_to_openhab-0.5.0/smart_meter_to_openhab/openhab.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,38 +8,46 @@
 from statistics import median
 from .interfaces import *
 
 # disable warnings about insecure requests because ssl verification is disabled
 import urllib3
 urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
 
+PersistenceValuesType = List[List[float]]
 def _convert_list_to_smart_meter_values(oh_item_names : SmartMeterOhItemNames, 
-                                       list_values : List[List[float]]) -> List[SmartMeterValues]:
+                                       list_values : PersistenceValuesType) -> List[SmartMeterValues]:
     smart_meter_values : List[SmartMeterValues] = []
     valid_items=[item for item in oh_item_names if item]
     for value_index in range(len(list_values[0]) if list_values else 0):
         item_value_list : List[OhItemAndValue] = []
         for item_index, item in enumerate(valid_items):
             item_value_list.append(OhItemAndValue(item, list_values[item_index][value_index]))
         smart_meter_values.append(SmartMeterValues.create(item_value_list))
     return smart_meter_values
 
-def _check_if_updated(values : List[SmartMeterValues]) -> bool:
-    valid_values : List[SmartMeterValues] = [value for value in values if value.is_valid()]
-    if len(valid_values) < 2:
-        return False
-
-    # no consumption is good and considered as updated
-    if all((value.overall_consumption.value is not None and value.overall_consumption.value == 0) for value in valid_values):
-        return True
-    
-    # for all other cases, at least one value has to be different
-    if any(value != valid_values[0] for value in valid_values):
-        return True
-    
+def _convert_smart_meter_values_to_list(values : List[SmartMeterValues]) -> PersistenceValuesType:
+    list_values : PersistenceValuesType = []
+    for i in range(len(SmartMeterValues().value_list())):
+        list_values.append([0]*len(values))
+    for index_set, value_set in enumerate(values):
+         for index_value, value in enumerate(value_set.value_list()):
+             list_values[index_set][index_value]=value
+    return list_values
+
+# TODO: add to sml interface and implement for iskra mt175
+# NOTE: Use List[List[float]] as input to consider that the count of values can potentially be different per item.
+# This could be some data optimization in openhab or similar. Whatever the reason is, we have to support it.
+def _check_if_updated(pers_values : PersistenceValuesType) -> bool:
+    for values in pers_values:
+        # no consumption is good and considered as updated. All values are same and very very low (but not necessarily 0)
+        if all(value == values[0] for value in values) and all(value < 20 for value in values):
+            return True
+        # for all other cases, at least one value has to be different
+        if any(value != values[0] for value in values):
+            return True
     return False
 
 def _get_median(oh_item_names : SmartMeterOhItemNames, list_values : List[List[float]]) -> SmartMeterValues:
     smart_meter_values : List[OhItemAndValue] = []
     value_index=0
     for item in oh_item_names:
         if item:
@@ -89,15 +97,14 @@
 
     def get_values_from_items(self, oh_item_names : SmartMeterOhItemNames) -> SmartMeterValues:
         return SmartMeterValues.create(self.get_item_value_list_from_items(oh_item_names))
     
     def get_extended_values_from_items(self, oh_item_names : ExtendedSmartMeterOhItemNames) -> ExtendedSmartMeterValues:
         return ExtendedSmartMeterValues.create(self.get_item_value_list_from_items(oh_item_names))
 
-    PersistenceValuesType = List[List[float]]
     def _get_persistence_values(self, oh_item_names : Tuple[str, ...], start_time : datetime.datetime, end_time : datetime.datetime) -> PersistenceValuesType:
         pers_values = []
         for item in oh_item_names:
             if item:
                 values=[]
                 try:
                     with self._session.get(
@@ -111,22 +118,20 @@
                 except requests.exceptions.RequestException as e:
                     self._logger.warning("Caught Exception while getting persistence data from openHAB: " + str(e))
                 pers_values.append(values)
         return pers_values
 
     def check_if_persistence_values_updated(self, oh_item_names : SmartMeterOhItemNames, start_time : datetime.datetime, end_time : datetime.datetime) -> bool:
         pers_values=self._get_persistence_values(oh_item_names, start_time, end_time)
-        if pers_values and any(len(values) != len(pers_values[0]) for values in pers_values):
-            # return True in case the input lists are of unequal size
-            # NOTE: This happens if the GET/POST requests to Openhab have not been completely successful.
-            self._logger.warning("Persistence values are of unequal size. Assuming they have been updated.")
-            return True
-        
-        smart_meter_values=_convert_list_to_smart_meter_values(oh_item_names, pers_values)
-        return _check_if_updated(smart_meter_values)
+        updated=_check_if_updated(pers_values)
+        if not updated:
+            self._logger.warning("Persistence values have not been updated.")
+            for index, values in enumerate(pers_values):
+                self._logger.warning(f"Values for index {index}: {values}")
+        return updated
 
     def get_median_from_items(self, oh_item_names : SmartMeterOhItemNames, 
                               timedelta : datetime.timedelta = datetime.timedelta(minutes=30)) -> SmartMeterValues:
         end_time=datetime.datetime.now()
         start_time=end_time-timedelta
         pers_values=self._get_persistence_values(oh_item_names, start_time, end_time)
         return _get_median(oh_item_names, pers_values)
```

### Comparing `smart_meter_to_openhab-0.4.2/smart_meter_to_openhab/sml_iskra_mt175.py` & `smart_meter_to_openhab-0.5.0/smart_meter_to_openhab/sml_iskra_mt175.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,32 +1,24 @@
 import serial
 import os
 import logging
 from datetime import timedelta, datetime
 from logging import Logger
 from typing import Protocol, List, Any, Optional
-from functools import cached_property
 from pathlib import Path
 from .interfaces import SmartMeterValues
 
 MIN_REF_VALUE_IN_WATT=50
 def _has_outlier(value_list : List[Any], ref_value_list : List[Any]) -> bool:
     for i in range(len(value_list)):
         if value_list[i] is not None and ref_value_list[i] is not None and value_list[i]*0.001 > max(ref_value_list[i], MIN_REF_VALUE_IN_WATT):
             return True
     return False
 
 class SmartMeterReader(Protocol):
-    @cached_property
-    def default(self) -> SmartMeterValues:
-        ...
-    @cached_property
-    def estimated_max_read_time_in_sec(self) -> int:
-        ...
-    
     # TODO:  this function can already be implemented in an abstract class
     def read(self, ref_values : SmartMeterValues) -> SmartMeterValues:
         ...
 
 # supporting OBIS code 1.8.0 only
 def _decode_sml_iskra_mt175_one_way(raw_data : str) -> SmartMeterValues:
     def _convert_to_float(pos_begin : int, pos_end : int) -> Optional[float]:
@@ -61,84 +53,67 @@
     return smart_meter_values
 
 # The smart meter supports consumption only. No electricity feed-in support! (German: Zweirichtungszähler)
 class SmlIskraMt175OneWay():
     # Data reading will be canceled after this time period.
     #      NOTE: Take care that this is longer then the specified transmission time of your smart meter.
     _read_raw_time_out_in_sec : int = 5
-    # try n times to get a valid raw read
-    # TODO: rm this when a value of 1 works
-    _max_read_attempts : int = 1
 
     def __init__(self, serial_port : str, logger : Logger, raw_data_dump_dir : Optional[Path] = None) -> None:
         self._port=serial.Serial(baudrate=9600, bytesize=serial.EIGHTBITS, parity=serial.PARITY_NONE, stopbits=serial.STOPBITS_ONE)
         self._serial_port=serial_port
         self._logger=logger
         self._latest_raw_data=''
         self._raw_data_dump_dir=raw_data_dump_dir
         self._raw_data_dump_invalid_counter=0
         self._raw_data_dump_outlier_counter=0
         self._raw_data_dump_valid_counter=0
         if self._raw_data_dump_dir:
             os.makedirs(self._raw_data_dump_dir, exist_ok=True)
             self._logger.info(f"Using directory {self._raw_data_dump_dir} for raw data dumps.")
 
-    @cached_property
-    def default(self) -> SmartMeterValues:
-        return SmartMeterValues(overall_consumption=0, phase_1_consumption=0, phase_2_consumption=0, phase_3_consumption=0)
-    
-    @cached_property
-    def estimated_max_read_time_in_sec(self) -> int:
-        return self._read_raw_time_out_in_sec*self._max_read_attempts
-
     def read(self, ref_values : SmartMeterValues) -> SmartMeterValues:
         """Read data from the smart meter via SML and try to validate them
 
         Parameters
         ----------
         ref_values : SmartMeterValues
             Values that are used as baseline to detect outliers
         
         Returns
         -------
         SmartMeterValues
             Contains the data read from the smart meter
         """
         ref_value_list=ref_values.value_list()
-        values=SmartMeterValues()
-        for i in range(self._max_read_attempts):
-            values=self._read_raw()
-            if values.is_invalid():
-                self._logger.info(f"Detected invalid values during SML read. Trying again")
-                if self._raw_data_dump_dir:
-                    with open(self._raw_data_dump_dir / f"raw_data_dump_invalid_{self._raw_data_dump_invalid_counter}.sml", 'w') as f:
-                        f.write(self._latest_raw_data)
-                    self._raw_data_dump_invalid_counter+=1
-                continue
-            value_list=values.value_list()
-            if _has_outlier(value_list, ref_value_list):
-                self._logger.info(f"Detected unrealistic values during SML read. Trying again")
-                if self._raw_data_dump_dir:
-                    with open(self._raw_data_dump_dir / f"raw_data_dump_outlier_{self._raw_data_dump_outlier_counter}.sml", 'w') as f:
-                        f.write(self._latest_raw_data)
-                    self._raw_data_dump_outlier_counter+=1
-                continue
-            break
-
+        values=self._read_raw()
+        if values.is_invalid():
+            self._logger.info(f"Detected invalid values during SML read. Trying again")
+            if self._raw_data_dump_dir:
+                with open(self._raw_data_dump_dir / f"raw_data_dump_invalid_{self._raw_data_dump_invalid_counter}.sml", 'w') as f:
+                    f.write(self._latest_raw_data)
+                self._raw_data_dump_invalid_counter+=1
         value_list=values.value_list()
+        if _has_outlier(value_list, ref_value_list):
+            self._logger.info(f"Detected unrealistic values during SML read. Trying again")
+            if self._raw_data_dump_dir:
+                with open(self._raw_data_dump_dir / f"raw_data_dump_outlier_{self._raw_data_dump_outlier_counter}.sml", 'w') as f:
+                    f.write(self._latest_raw_data)
+                self._raw_data_dump_outlier_counter+=1
+
         if values.is_invalid() or _has_outlier(value_list, ref_value_list):
             self._logger.warning(f"Unable to read and validate SML data. Ignoring following values: {values}")
             values.reset()
 
         if self._raw_data_dump_dir and self._logger.level == logging.DEBUG and values.is_valid():
             with open(self._raw_data_dump_dir / f"raw_data_dump_valid_{self._raw_data_dump_valid_counter}.sml", 'w') as f:
                 f.write(self._latest_raw_data)
             self._raw_data_dump_valid_counter+=1
 
-        return values if values.is_valid() else self.default
+        return values
 
     def _read_raw(self) -> SmartMeterValues:
         """Read raw data from the smart meter via SML
 
         Parameters
         ----------
         time_out : timedelta
```

### Comparing `smart_meter_to_openhab-0.4.2/smart_meter_to_openhab/sml_reader.py` & `smart_meter_to_openhab-0.5.0/smart_meter_to_openhab/sml_reader.py`

 * *Files identical despite different names*

### Comparing `smart_meter_to_openhab-0.4.2/smart_meter_to_openhab_scripts/main.py` & `smart_meter_to_openhab-0.5.0/smart_meter_to_openhab_scripts/main.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import argparse
 import logging
 import os
 import sys
 import subprocess
-from datetime import timedelta, datetime
+from datetime import datetime
 from pathlib import Path
-from time import sleep
 from dotenv import load_dotenv
 from typing import Union, List
 
 try:
     import importlib.metadata
     __version__ = importlib.metadata.version('smart_meter_to_openhab')
 except:
@@ -34,100 +33,82 @@
     
 def create_args_parser() -> argparse.ArgumentParser:
     parser=argparse.ArgumentParser(description=f"A tool to push data of ISKRA MT175 smart meter to openHAB. Version {__version__}")
     parser.add_argument("--dotenv_path", type=Path, required=False, help=f"Provide the required environment variables in this .env file \
                         or by any other means (e.g. in your ~/.profile)")
     parser.add_argument("-c", "--smart_meter_read_count", type=int, required=False, default=5, 
                         help="Specifies the number of performed reads that are averaged per interval. Between each read is a sleep of 1 sec.")
-    parser.add_argument("--max_reinit", type=int, required=False, default=5, help="Exit process with Return Code 1 when pinging stays unsuccessful.")
-    parser.add_argument('--uhubctl', action='store_true', help="Use uhubctl to power off and on the usb port on reinit")
+    parser.add_argument('--uhubctl', action='store_true', help="Use uhubctl to power off and on the usb port on when process is unsuccessful.")
     parser.add_argument("--logfile", type=Path, required=False, help="Write logging to this file instead of to stdout")
     parser.add_argument("--raw_data_dump_dir", type=Path, required=False, help="Dump raw data of unsuccessful reads to this folder.")
     parser.add_argument('-v', '--verbose', action='count', default=0)
     return parser
 
 def _exec_process(params : List[str]) -> None:
     result = subprocess.run(params, stdout=subprocess.PIPE, stderr=subprocess.STDOUT)
     rc=result.returncode
     if rc != 0:
         raise Exception("Failed to execute command "+ ' '.join(params)+". Return code was: "+str(result.returncode))
 
-def _run(logger : logging.Logger, read_count : int, use_uhubctl : bool, raw_data_dump_dir : Union[Path, None] = None) -> bool:
+def _run(logger : logging.Logger, read_count : int, raw_data_dump_dir : Union[Path, None] = None) -> None:
     from smart_meter_to_openhab.openhab import OpenhabConnection
     from smart_meter_to_openhab.sml_iskra_mt175 import SmlIskraMt175OneWay
     from smart_meter_to_openhab.sml_reader import SmlReader
     from smart_meter_to_openhab.interfaces import SmartMeterValues
-    from smart_meter_to_openhab.utils import add_value_to_rolling_list
+    from smart_meter_to_openhab.utils import manage_rolling_list
 
     oh_user=os.getenv('OH_USER') if 'OH_USER' in os.environ else ''
     oh_passwd=os.getenv('OH_PASSWD') if 'OH_PASSWD' in os.environ else ''
     oh_connection = OpenhabConnection(os.getenv('OH_HOST'), oh_user, oh_passwd, logger) # type: ignore
     sml_iskra = SmlIskraMt175OneWay('/dev/ttyUSB0', logger, raw_data_dump_dir)
     sml_reader = SmlReader(logger)
     logger.info("Connections established. Starting to transfer smart meter values to openhab.")
-    desired_number_of_persistence_values=4
-    datetimes_before_post_to_oh=[datetime.now()]*desired_number_of_persistence_values
-    ping_timedelta = timedelta(seconds=read_count*sml_iskra.estimated_max_read_time_in_sec*desired_number_of_persistence_values)
-    logger.info(f"Calculated ping_timedelta is {ping_timedelta}. Process will be reinit if no data change is detected in the openHAB DB in the given timeframe.")
-    run_start_time=datetime.now()
-    ping_succeeded=False
+    desired_number_of_persistence_values=6
+    datetimes_before_post_to_oh : List[datetime] =[]
     while True:
         logger.info("Reading SML data")
         ref_smart_meter_value=oh_connection.get_median_from_items(SmartMeterValues.oh_item_names())
         values, extended_values=sml_reader.read_avg_from_sml_and_compute_extended_values(sml_iskra, read_count, 
                                                                                          ref_values=ref_smart_meter_value)
         logger.info(f"current values: {values}")
         logger.info(f"current extended values: {extended_values}")
-        datetimes_before_post_to_oh=add_value_to_rolling_list(datetimes_before_post_to_oh, datetime.now())
+        datetimes_before_post_to_oh=manage_rolling_list(datetimes_before_post_to_oh, desired_number_of_persistence_values, datetime.now())
         oh_connection.post_to_items(values)
         oh_connection.post_to_items(extended_values)
         logger.info("Values posted to openHAB")
-        # start pinging after running for the specified time
-        if (datetime.now() - run_start_time) > ping_timedelta:
+        if len(datetimes_before_post_to_oh) == desired_number_of_persistence_values:
             # NOTE: exclude the latest values since oh sometimes has not handled the post requests from above yet.
             if not oh_connection.check_if_persistence_values_updated(SmartMeterValues.oh_item_names(), 
                                                                      start_time=datetimes_before_post_to_oh[0], 
                                                                      end_time=datetimes_before_post_to_oh[-1]):
                 break
-            ping_succeeded=True
             logger.info("openHAB items ping successful.")
-    
-    if use_uhubctl:
-        logger.error("openHAB items seem to have not been updated - Power off and on usb ports and reinit process")
-        # TODO: sudo reboot seems to help a lot more. But lets try this first
-        _exec_process(["sudo", "uhubctl", "-a", "cycle", "-d", "10", "-p", "1-5"])
-        sleep(1)
-    else:
-        logger.error("openHAB items seem to have not been updated - reinit process")
-    
-    return ping_succeeded
 
 def main() -> None:
     parser=create_args_parser()
     args = parser.parse_args()
     if args.dotenv_path:
         load_dotenv(dotenv_path=args.dotenv_path)
     logger=create_logger(args.logfile)
     logger.setLevel(logging.INFO)
     logger.info(f"Starting smart_meter_to_openhab version {__version__}")
     logger.setLevel(log_level_from_arg(args.verbose))
     try:
         raw_data_dump_dir=args.raw_data_dump_dir if args.raw_data_dump_dir else None
-        # TODO: remove the reinit thingy. Let it fail and restart by systemd or so
-        unsuccessful_reinit_count=0
-        while unsuccessful_reinit_count < args.max_reinit:
-            if _run(logger, args.smart_meter_read_count, args.uhubctl, raw_data_dump_dir):
-                unsuccessful_reinit_count=0
-            else:
-                unsuccessful_reinit_count+=1
-                logger.error("No improvement after reinit. Trying again.")
+        _run(logger, args.smart_meter_read_count, raw_data_dump_dir)
 
+        if args.uhubctl:
+            logger.error("openHAB items seem to have not been updated - Power off and on usb ports and exiting process")
+            # TODO: sudo reboot seems to help a lot more. But lets try this first
+            _exec_process(["sudo", "uhubctl", "-a", "cycle", "-d", "10", "-p", "1-5"])
+        else:
+            logger.error("openHAB items seem to have not been updated - exiting process")
     except Exception as e:
         logger.exception("Caught Exception: " + str(e))
     except:
         logger.exception("Caught unknow exception")
-    
+
     logger.error("Unable to upload valid data to openHAB. Exiting Process with Return Code 1.")
     sys.exit(1)
 
 if __name__ == '__main__':
     main()
```

### Comparing `smart_meter_to_openhab-0.4.2/PKG-INFO` & `smart_meter_to_openhab-0.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: smart_meter_to_openhab
-Version: 0.4.2
+Version: 0.5.0
 Summary: Pushing data of ISKRA MT175 smart meter to openhab
 Home-page: https://github.com/die-bauerei/smart-meter-to-openhab
 Author: Heiko Bauer
 Author-email: heiko_bauer@icloud.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

