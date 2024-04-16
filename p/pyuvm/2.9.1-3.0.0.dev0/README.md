# Comparing `tmp/pyuvm-2.9.1.tar.gz` & `tmp/pyuvm-3.0.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyuvm-2.9.1.tar", last modified: Wed Apr 19 17:06:25 2023, max compression
+gzip compressed data, was "pyuvm-3.0.0.dev0.tar", last modified: Tue Apr 16 19:36:56 2024, max compression
```

## Comparing `pyuvm-2.9.1.tar` & `pyuvm-3.0.0.dev0.tar`

### file list

```diff
@@ -1,28 +1,38 @@
-drwxr-xr-x   0 raysalemi   (501) staff       (20)        0 2023-04-19 17:06:25.882977 pyuvm-2.9.1/
--rw-r--r--   0 raysalemi   (501) staff       (20)      567 2022-10-09 18:34:56.000000 pyuvm-2.9.1/LICENSE
--rw-r--r--   0 raysalemi   (501) staff       (20)       16 2020-12-06 19:42:29.000000 pyuvm-2.9.1/MANIFEST.in
--rw-r--r--   0 raysalemi   (501) staff       (20)    20550 2023-04-19 17:06:25.882763 pyuvm-2.9.1/PKG-INFO
--rw-r--r--   0 raysalemi   (501) staff       (20)    19929 2023-04-19 16:03:03.000000 pyuvm-2.9.1/README.md
--rw-r--r--   0 raysalemi   (501) staff       (20)      104 2021-08-13 21:06:37.000000 pyuvm-2.9.1/pyproject.toml
-drwxr-xr-x   0 raysalemi   (501) staff       (20)        0 2023-04-19 17:06:25.876292 pyuvm-2.9.1/pyuvm/
--rw-r--r--   0 raysalemi   (501) staff       (20)      638 2022-02-12 22:21:28.000000 pyuvm-2.9.1/pyuvm/__init__.py
--rw-r--r--   0 raysalemi   (501) staff       (20)      899 2021-09-28 10:54:51.000000 pyuvm-2.9.1/pyuvm/error_classes.py
--rw-r--r--   0 raysalemi   (501) staff       (20)     1286 2023-04-19 17:04:52.000000 pyuvm-2.9.1/pyuvm/extension_classes.py
--rw-r--r--   0 raysalemi   (501) staff       (20)    12500 2023-04-19 16:03:03.000000 pyuvm-2.9.1/pyuvm/s05_base_classes.py
--rw-r--r--   0 raysalemi   (501) staff       (20)     3535 2023-04-19 16:03:03.000000 pyuvm-2.9.1/pyuvm/s06_reporting_classes.py
--rw-r--r--   0 raysalemi   (501) staff       (20)    19313 2021-12-09 21:54:48.000000 pyuvm-2.9.1/pyuvm/s08_factory_classes.py
--rw-r--r--   0 raysalemi   (501) staff       (20)     4549 2022-01-03 13:27:06.000000 pyuvm-2.9.1/pyuvm/s09_phasing.py
--rw-r--r--   0 raysalemi   (501) staff       (20)    26702 2022-10-09 16:34:56.000000 pyuvm-2.9.1/pyuvm/s12_uvm_tlm_interfaces.py
--rw-r--r--   0 raysalemi   (501) staff       (20)     3442 2021-12-22 15:16:43.000000 pyuvm-2.9.1/pyuvm/s13_predefined_component_classes.py
--rw-r--r--   0 raysalemi   (501) staff       (20)    21777 2022-02-09 13:32:30.000000 pyuvm-2.9.1/pyuvm/s13_uvm_component.py
--rw-r--r--   0 raysalemi   (501) staff       (20)    11424 2022-10-09 16:34:56.000000 pyuvm-2.9.1/pyuvm/s14_15_python_sequences.py
--rw-r--r--   0 raysalemi   (501) staff       (20)     3673 2021-10-22 12:50:53.000000 pyuvm-2.9.1/pyuvm/s18_register_model.py
--rw-r--r--   0 raysalemi   (501) staff       (20)     9374 2022-10-15 13:59:54.000000 pyuvm-2.9.1/pyuvm/utility_classes.py
-drwxr-xr-x   0 raysalemi   (501) staff       (20)        0 2023-04-19 17:06:25.882533 pyuvm-2.9.1/pyuvm.egg-info/
--rw-r--r--   0 raysalemi   (501) staff       (20)    20550 2023-04-19 17:06:25.000000 pyuvm-2.9.1/pyuvm.egg-info/PKG-INFO
--rw-r--r--   0 raysalemi   (501) staff       (20)      559 2023-04-19 17:06:25.000000 pyuvm-2.9.1/pyuvm.egg-info/SOURCES.txt
--rw-r--r--   0 raysalemi   (501) staff       (20)        1 2023-04-19 17:06:25.000000 pyuvm-2.9.1/pyuvm.egg-info/dependency_links.txt
--rw-r--r--   0 raysalemi   (501) staff       (20)       14 2023-04-19 17:06:25.000000 pyuvm-2.9.1/pyuvm.egg-info/requires.txt
--rw-r--r--   0 raysalemi   (501) staff       (20)        6 2023-04-19 17:06:25.000000 pyuvm-2.9.1/pyuvm.egg-info/top_level.txt
--rw-r--r--   0 raysalemi   (501) staff       (20)       38 2023-04-19 17:06:25.883032 pyuvm-2.9.1/setup.cfg
--rwxr-xr-x   0 raysalemi   (501) staff       (20)      931 2023-04-19 17:04:52.000000 pyuvm-2.9.1/setup.py
+drwxr-xr-x   0 raysalemi   (501) staff       (20)        0 2024-04-16 19:36:56.085060 pyuvm-3.0.0.dev0/
+-rw-r--r--   0 raysalemi   (501) staff       (20)      567 2022-10-09 18:34:56.000000 pyuvm-3.0.0.dev0/LICENSE
+-rw-r--r--   0 raysalemi   (501) staff       (20)       16 2020-12-06 19:42:29.000000 pyuvm-3.0.0.dev0/MANIFEST.in
+-rw-r--r--   0 raysalemi   (501) staff       (20)    21675 2024-04-16 19:36:56.084803 pyuvm-3.0.0.dev0/PKG-INFO
+-rw-r--r--   0 raysalemi   (501) staff       (20)    21020 2024-02-19 21:32:50.000000 pyuvm-3.0.0.dev0/README.md
+-rw-r--r--   0 raysalemi   (501) staff       (20)      104 2021-08-13 21:06:37.000000 pyuvm-3.0.0.dev0/pyproject.toml
+drwxr-xr-x   0 raysalemi   (501) staff       (20)        0 2024-04-16 19:36:56.083442 pyuvm-3.0.0.dev0/pyuvm/
+-rw-r--r--   0 raysalemi   (501) staff       (20)     1186 2024-02-19 21:32:50.000000 pyuvm-3.0.0.dev0/pyuvm/__init__.py
+-rw-r--r--   0 raysalemi   (501) staff       (20)      899 2021-09-28 10:54:51.000000 pyuvm-3.0.0.dev0/pyuvm/error_classes.py
+-rw-r--r--   0 raysalemi   (501) staff       (20)     1286 2023-04-19 17:04:52.000000 pyuvm-3.0.0.dev0/pyuvm/extension_classes.py
+-rw-r--r--   0 raysalemi   (501) staff       (20)    14873 2023-08-06 13:06:58.000000 pyuvm-3.0.0.dev0/pyuvm/s05_base_classes.py
+-rw-r--r--   0 raysalemi   (501) staff       (20)     3534 2023-08-06 13:06:58.000000 pyuvm-3.0.0.dev0/pyuvm/s06_reporting_classes.py
+-rw-r--r--   0 raysalemi   (501) staff       (20)    19321 2024-04-16 19:17:42.000000 pyuvm-3.0.0.dev0/pyuvm/s08_factory_classes.py
+-rw-r--r--   0 raysalemi   (501) staff       (20)     4549 2022-01-03 13:27:06.000000 pyuvm-3.0.0.dev0/pyuvm/s09_phasing.py
+-rw-r--r--   0 raysalemi   (501) staff       (20)    26702 2022-10-09 16:34:56.000000 pyuvm-3.0.0.dev0/pyuvm/s12_uvm_tlm_interfaces.py
+-rw-r--r--   0 raysalemi   (501) staff       (20)     3442 2021-12-22 15:16:43.000000 pyuvm-3.0.0.dev0/pyuvm/s13_predefined_component_classes.py
+-rw-r--r--   0 raysalemi   (501) staff       (20)    22334 2024-04-16 19:17:42.000000 pyuvm-3.0.0.dev0/pyuvm/s13_uvm_component.py
+-rw-r--r--   0 raysalemi   (501) staff       (20)    11424 2022-10-09 16:34:56.000000 pyuvm-3.0.0.dev0/pyuvm/s14_15_python_sequences.py
+-rw-r--r--   0 raysalemi   (501) staff       (20)     8165 2024-02-19 21:32:50.000000 pyuvm-3.0.0.dev0/pyuvm/s17_uvm_reg_enumerations.py
+-rw-r--r--   0 raysalemi   (501) staff       (20)     9431 2024-02-19 21:32:50.000000 pyuvm-3.0.0.dev0/pyuvm/s18_uvm_reg_block.py
+-rw-r--r--   0 raysalemi   (501) staff       (20)    23076 2024-02-19 21:32:50.000000 pyuvm-3.0.0.dev0/pyuvm/s19_uvm_reg_field.py
+-rw-r--r--   0 raysalemi   (501) staff       (20)    11781 2024-02-19 21:32:50.000000 pyuvm-3.0.0.dev0/pyuvm/s20_uvm_reg.py
+-rw-r--r--   0 raysalemi   (501) staff       (20)    15353 2024-02-19 21:32:50.000000 pyuvm-3.0.0.dev0/pyuvm/s21_uvm_reg_map.py
+-rw-r--r--   0 raysalemi   (501) staff       (20)      353 2024-02-19 21:32:50.000000 pyuvm-3.0.0.dev0/pyuvm/s22_uvm_mem.py
+-rw-r--r--   0 raysalemi   (501) staff       (20)     5722 2024-02-19 21:32:50.000000 pyuvm-3.0.0.dev0/pyuvm/s23_uvm_reg_item.py
+-rw-r--r--   0 raysalemi   (501) staff       (20)     4696 2024-02-19 21:32:50.000000 pyuvm-3.0.0.dev0/pyuvm/s24_uvm_reg_includes.py
+-rw-r--r--   0 raysalemi   (501) staff       (20)     3929 2024-02-19 21:32:50.000000 pyuvm-3.0.0.dev0/pyuvm/s25_uvm_adapter.py
+-rw-r--r--   0 raysalemi   (501) staff       (20)      202 2024-02-19 21:32:50.000000 pyuvm-3.0.0.dev0/pyuvm/s26_uvm_predictor.py
+-rw-r--r--   0 raysalemi   (501) staff       (20)      449 2024-02-19 21:32:50.000000 pyuvm-3.0.0.dev0/pyuvm/s27_uvm_reg_pkg.py
+-rw-r--r--   0 raysalemi   (501) staff       (20)     9374 2022-10-15 13:59:54.000000 pyuvm-3.0.0.dev0/pyuvm/utility_classes.py
+drwxr-xr-x   0 raysalemi   (501) staff       (20)        0 2024-04-16 19:36:56.084534 pyuvm-3.0.0.dev0/pyuvm.egg-info/
+-rw-r--r--   0 raysalemi   (501) staff       (20)    21675 2024-04-16 19:36:56.000000 pyuvm-3.0.0.dev0/pyuvm.egg-info/PKG-INFO
+-rw-r--r--   0 raysalemi   (501) staff       (20)      819 2024-04-16 19:36:56.000000 pyuvm-3.0.0.dev0/pyuvm.egg-info/SOURCES.txt
+-rw-r--r--   0 raysalemi   (501) staff       (20)        1 2024-04-16 19:36:56.000000 pyuvm-3.0.0.dev0/pyuvm.egg-info/dependency_links.txt
+-rw-r--r--   0 raysalemi   (501) staff       (20)       14 2024-04-16 19:36:56.000000 pyuvm-3.0.0.dev0/pyuvm.egg-info/requires.txt
+-rw-r--r--   0 raysalemi   (501) staff       (20)        6 2024-04-16 19:36:56.000000 pyuvm-3.0.0.dev0/pyuvm.egg-info/top_level.txt
+-rw-r--r--   0 raysalemi   (501) staff       (20)       38 2024-04-16 19:36:56.085111 pyuvm-3.0.0.dev0/setup.cfg
+-rwxr-xr-x   0 raysalemi   (501) staff       (20)      936 2024-04-16 19:25:26.000000 pyuvm-3.0.0.dev0/setup.py
```

### Comparing `pyuvm-2.9.1/LICENSE` & `pyuvm-3.0.0.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyuvm-2.9.1/PKG-INFO` & `pyuvm-3.0.0.dev0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: pyuvm
-Version: 2.9.1
-Summary: A Python implementation of the UVM using cocotb
-Home-page: https://github.com/pyuvm/pyuvm
-Author: Ray Salemi
-Author-email: ray@raysalemi.com
-Project-URL: Bug Tracker, https://github.com/pyuvm/pyuvm/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Operating System :: OS Independent
-Classifier: Topic :: Scientific/Engineering :: Electronic Design Automation (EDA)
-Classifier: Framework :: cocotb
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # PyUVM
 
 ## Description
 
 **pyuvm** is the Universal Verification Methodology implemented in Python instead of SystemVerilog. **pyuvm** uses cocotb to interact with the simulator and schedule simulation events.
 
 **pyuvm** implements the most often-used parts of the UVM while taking advantage of the fact that Python does not have strict typing and does not require parameterized classes. The project refactors pieces of the UVM that were either overly complicated due to typing or legacy code.
@@ -32,14 +15,25 @@
 |5|Base Classes|uvm_object does not capture transaction timing information|
 |6|Reporting Classes|Leverages logging, controlled using UVM hierarchy|
 |8|Factory Classes|All uvm_void classes automatically registered|
 |9|Phasing|Simplified to only common phases. Supports objection system|
 |12|UVM TLM Interfaces|Fully implemented|
 |13|Predefined Component Classes|Implements uvm_component with hierarchy, uvm_root singleton,run_test(), simplified ConfigDB, uvm_driver, etc|
 |14 & 15|Sequences, sequencer, sequence_item|Refactored sequencer functionality leveraging Python language capabilities. Simpler and more direct implementation|
+|17|UVM Regfister Enum|All the basic Enum types to be used in the whole PYUVM Ral|
+|18|UVM Register Block|Main Register Block class|
+|19|UVM Register Field|Regsister Filed there are still few functionalities missing like atomic Backdoor access amd Field byte access or single Field access during read or write operation|
+|20|UVM Register|Main register class, still missing Backdoor and used Backdoor to be leveraged from cocotb force. Byte access and single field access yet to be implemeneted|
+|21|UVM Register Map|Main register map class, should be refatored to guarantee simplicity and backdoor access, extension class in Read and Write to be implemeneted|
+|22|UVM Memory|Not Implemented|
+|23|Register Item|Register Item used across multiple classes|
+|24|Register include file|Includes other Enum and typeds to be merged with s17|
+|25|UVM register adapter|Main register adapter|
+|26|UVM register predictor|Main register predictor, should be disabled if auto_prediction is not set|
+|27|Register Package|Main PKG if included and flake8 is not active should behave similarly to uvm_reg_pkg|
 
 ### Installation
 
 You can install **pyuvm** using `pip`. This will also install **cocotb** as a requirement for **pyuvm**.
 
 ```bash
 % pip install pyuvm
```

### Comparing `pyuvm-2.9.1/README.md` & `pyuvm-3.0.0.dev0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,7 +1,25 @@
+Metadata-Version: 2.1
+Name: pyuvm
+Version: 3.0.0.dev0
+Summary: A Python implementation of the UVM using cocotb
+Home-page: https://github.com/pyuvm/pyuvm
+Author: Ray Salemi
+Author-email: ray@raysalemi.com
+Project-URL: Bug Tracker, https://github.com/pyuvm/pyuvm/issues
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: Apache Software License
+Classifier: Operating System :: OS Independent
+Classifier: Topic :: Scientific/Engineering :: Electronic Design Automation (EDA)
+Classifier: Framework :: cocotb
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: cocotb>=1.6.0
+
 # PyUVM
 
 ## Description
 
 **pyuvm** is the Universal Verification Methodology implemented in Python instead of SystemVerilog. **pyuvm** uses cocotb to interact with the simulator and schedule simulation events.
 
 **pyuvm** implements the most often-used parts of the UVM while taking advantage of the fact that Python does not have strict typing and does not require parameterized classes. The project refactors pieces of the UVM that were either overly complicated due to typing or legacy code.
@@ -15,14 +33,25 @@
 |5|Base Classes|uvm_object does not capture transaction timing information|
 |6|Reporting Classes|Leverages logging, controlled using UVM hierarchy|
 |8|Factory Classes|All uvm_void classes automatically registered|
 |9|Phasing|Simplified to only common phases. Supports objection system|
 |12|UVM TLM Interfaces|Fully implemented|
 |13|Predefined Component Classes|Implements uvm_component with hierarchy, uvm_root singleton,run_test(), simplified ConfigDB, uvm_driver, etc|
 |14 & 15|Sequences, sequencer, sequence_item|Refactored sequencer functionality leveraging Python language capabilities. Simpler and more direct implementation|
+|17|UVM Regfister Enum|All the basic Enum types to be used in the whole PYUVM Ral|
+|18|UVM Register Block|Main Register Block class|
+|19|UVM Register Field|Regsister Filed there are still few functionalities missing like atomic Backdoor access amd Field byte access or single Field access during read or write operation|
+|20|UVM Register|Main register class, still missing Backdoor and used Backdoor to be leveraged from cocotb force. Byte access and single field access yet to be implemeneted|
+|21|UVM Register Map|Main register map class, should be refatored to guarantee simplicity and backdoor access, extension class in Read and Write to be implemeneted|
+|22|UVM Memory|Not Implemented|
+|23|Register Item|Register Item used across multiple classes|
+|24|Register include file|Includes other Enum and typeds to be merged with s17|
+|25|UVM register adapter|Main register adapter|
+|26|UVM register predictor|Main register predictor, should be disabled if auto_prediction is not set|
+|27|Register Package|Main PKG if included and flake8 is not active should behave similarly to uvm_reg_pkg|
 
 ### Installation
 
 You can install **pyuvm** using `pip`. This will also install **cocotb** as a requirement for **pyuvm**.
 
 ```bash
 % pip install pyuvm
```

### Comparing `pyuvm-2.9.1/pyuvm/error_classes.py` & `pyuvm-3.0.0.dev0/pyuvm/error_classes.py`

 * *Files identical despite different names*

### Comparing `pyuvm-2.9.1/pyuvm/extension_classes.py` & `pyuvm-3.0.0.dev0/pyuvm/extension_classes.py`

 * *Files identical despite different names*

### Comparing `pyuvm-2.9.1/pyuvm/s05_base_classes.py` & `pyuvm-3.0.0.dev0/pyuvm/s05_base_classes.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 """
 import sys
 
 try:
     import pyuvm.error_classes as error_classes
     import pyuvm.utility_classes as utility_classes
     from pyuvm.s08_factory_classes import uvm_factory
+    from cocotb.utils import get_sim_time
 except ModuleNotFoundError as mnf:
     print(mnf)
     sys.exit(1)
 
 
 # 5.3.1
 class uvm_object(utility_classes.uvm_void):
@@ -349,14 +350,17 @@
         """
         :param name: Object name
         :param initiator: component that is initiator
         """
         super().__init__(name)
         self.set_initiator(initiator)
         self.transaction_id = id(self)
+        self._accept_time: int = None
+        self._begin_time: int = None
+        self._end_time: int = None
 
     def set_id_info(self, other):
         """
         Set transaction_id from other
         :param other: uvm_transaction
         :return: None
         """
@@ -378,54 +382,102 @@
         return self._initiator
 
     def __not_implemented(self):
         raise error_classes.UVMNotImplemented(
             'This method is not implemented at this time.')
 
     # 5.4.2.2
-    def accept_tr(self, time):
+    def accept_tr(self, accept_time=0):
         """
-        Not implemented
+        5.4.2.2
+        :param time: simulation time
         """
-        self.__not_implemented()
+        if (accept_time is not None) and (accept_time != 0):
+            self._accept_time = accept_time
+        else:
+            self._accept_time = get_sim_time()
+        # TODO Call 'accept' event pool triggers
+        self.do_accept_tr()
 
     # 5.4.2.3
     def do_accept_tr(self):
         """
-        Not implemented
+        User definable method
         """
-        self.__not_implemented()
+        pass
 
     # 5.4.2.5
-    def begin_tr(self, begin_time=0, parent_handle=None):
-        """
-        Not implemented
-        """
-        self.__not_implemented()
+    def begin_tr(self,
+                 begin_time=0,
+                 parent_handle=None) -> int:
+        """
+        :param begin_time: Simulation time at which
+                           the transaction is acted upon by the driver
+        :param parent_handle:
+        """
+        if (begin_time is not None) and (begin_time != 0):
+            # begin_time must be greater than or equal to accept_time
+            if begin_time < self._accept_time:
+                raise error_classes.UVMFatalError(
+                    f"""begin_time : {begin_time} is less than
+                        accept_time: {self._accept_time} for
+                        the transaction : {self.get_name()}
+                     """)
+            else:
+                self._begin_time = begin_time
+        else:
+            self._begin_time = get_sim_time()
+        # TODO: update recodring API calls
+        self.do_begin_tr()
+        # TODO Call 'begin' event pool triggers
+        # Update return value when recording is enabled
+        return 0
 
     # 5.4.2.5
     def do_begin_tr(self):
         """
-        Not implemented
+        User definable method
         """
-        self.__not_implemented()
+        pass
 
     # 5.4.2.6
-    def end_tr(self, end_time=0, free_handle=True):
-        """
-        Not implemented
+    def end_tr(self, end_time=0, free_handle=True) -> None:
         """
-        self.__not_implemented()
+        :param end_time: Simulation time at which the transaction
+                         is marked as acted upon
+        :param free_handle:
+        """
+        if end_time is not None and end_time != 0:
+            # end_time must be greater than or equal to
+            # accept_time and begin_time
+            if end_time < self._accept_time:
+                raise error_classes.UVMFatalError(
+                    """end_time : {end_time} is less than
+                       accept_time : {self._accept_time}
+                       for the transaction : {self.get_name()}""")
+            elif end_time < self._begin_time:
+                raise error_classes.UVMFatalError(
+                    """end_time : {end_time} is less than
+                    accept_time : {self._begin_time}
+                    for the transaction : {self.get_name()}""")
+            else:
+                self._end_time = end_time
+        else:
+            self._end_time = get_sim_time()
+        # TODO: update recodring API calls
+        self.do_end_tr()
+        # TODO Call 'end' event pool triggers
+        # Update return value when recording is enabled
 
     # 5.4.2.7
     def do_end_tr(self):
         """
         Not implemented
         """
-        self.__not_implemented()
+        pass
 
     # 5.4.2.8
     def get_tr_handle(self):
         """
         Not implemented
         """
         self.__not_implemented()
@@ -462,33 +514,31 @@
     def get_event_pool(self):
         """
         Not implemented
         """
         self.__not_implemented()
 
     # 5.4.2.16
-    def get_accept_time(self):
+    def get_accept_time(self) -> int:
         """
-        Not implemented
+        Returns the Accept time of transaction
         """
-        self.__not_implemented()
+        return self._accept_time
 
-    # 5.4.2.16
-    def get_begin_time(self):
+    def get_begin_time(self) -> int:
         """
-        Not implemented
+        Returns the Begin time of transaction
         """
-        self.__not_implemented()
+        return self._begin_time
 
-    # 5.4.2.16
-    def get_end_time(self):
+    def get_end_time(self) -> int:
         """
-        Not implemented
+        Returns the End time of transaction
         """
-        self.__not_implemented()
+        return self._end_time
 
     # 5.4.2.17
     def set_transaction_id(self, txn_id):
         """
         Sets  variable transaction_id
         """
         assert (isinstance(txn_id, int)), "Transaction ID must be an integer."
```

### Comparing `pyuvm-2.9.1/pyuvm/s06_reporting_classes.py` & `pyuvm-3.0.0.dev0/pyuvm/s06_reporting_classes.py`

 * *Files 4% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 class PyuvmFormatter(SimColourLogFormatter):
     def __init__(self, full_name):
         self.full_name = full_name
         super().__init__()
 
     def format(self, record):
-        new_msg = f"[{self.full_name}]: " + record.msg
+        new_msg = f"[{self.full_name}]: {record.msg}"
         record.msg = new_msg
         name_temp = record.name
         record.name = f"{record.pathname}({record.lineno})"
         if want_color_output():
             formatted_msg = super().format(record)
         else:
             formatted_msg = SimLogFormatter.format(self, record)
```

### Comparing `pyuvm-2.9.1/pyuvm/s08_factory_classes.py` & `pyuvm-3.0.0.dev0/pyuvm/s08_factory_classes.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 import fnmatch
 
 
 # pyuvm refactors the factory, taking advantage Python's
 # superiority in terms of OOP features and lack of types.
 
 # Implementing section 8 in the IEEE Specification
+#
 # The IEEE spec assumes that UVM is being written in SystemVerilog,
 # a language that does not allow you to control how classes get defined.
 # Python has more control in this area. With Python we can set things up
 # so that any class that extends uvm_void automatically gets registered
 # into the factory.
 
 # Therefore there is no need for 8.2.2 the type_id, that
@@ -74,18 +75,18 @@
         # We capture this by storing the original and override types as a
         # tuple at the full inst path.  Later we'll retrieve the tuple
         # and check the type of the object at the full_inst_path.
         #
         # instance_overrides is an OrderedDict, so we will check
         # the paths in the order they are registered later.
 
-        assert issubclass(original_type, utility_classes.uvm_void),\
+        assert issubclass(original_type, utility_classes.uvm_void), \
             "You tried to override a non-uvm_void class"
         assert issubclass(override_type,
-                          utility_classes.uvm_void),\
+                          utility_classes.uvm_void), \
             "You tried to use a non-uvm_void class as an override"
         self.__set_override(original_type, override_type, full_inst_path)
 
     # 8.3.1.4.1
     def set_inst_override_by_name(self, original_type_name,
                                   override_type_name, full_inst_path):
         """
@@ -133,18 +134,18 @@
                                   replace=True):
         """
         Override one type with another type globally
         :param original_type: The original type to be overridden
         :param override_type: The new type that will override it
         :param replace: If the override exists, only replace it if this is True
         """
-        assert issubclass(original_type, utility_classes.uvm_void),\
+        assert issubclass(original_type, utility_classes.uvm_void), \
             "You tried to override a non-uvm_void class"
         assert issubclass(override_type,
-                          utility_classes.uvm_void),\
+                          utility_classes.uvm_void), \
             "You tried to use a non-uvm_void class as an override"
         if (original_type not in self.fd.overrides) or replace:
             self.__set_override(original_type, override_type)
 
     # 8.3.1.4.2
     def set_type_override_by_name(self, original_type_name,
                                   override_type_name, replace=True):
@@ -156,17 +157,17 @@
         overridden or an arbitrary string.
         :param override_type_name: The name of the overriding type.
         It must have been declared.
         :param replace: If the override already exists only
         replace if this is True
         :return:
         """
-        assert isinstance(original_type_name, str),\
+        assert isinstance(original_type_name, str), \
             "Original_name must be a string"
-        assert isinstance(override_type_name, str),\
+        assert isinstance(override_type_name, str), \
             "Override_name must be a string"
         try:
             override_type = self.fd.classes[override_type_name]
         except KeyError:
             raise error_classes.UVMFactoryError(
                 f"{override_type_name}" + " has not been defined.")
```

### Comparing `pyuvm-2.9.1/pyuvm/s09_phasing.py` & `pyuvm-3.0.0.dev0/pyuvm/s09_phasing.py`

 * *Files identical despite different names*

### Comparing `pyuvm-2.9.1/pyuvm/s12_uvm_tlm_interfaces.py` & `pyuvm-3.0.0.dev0/pyuvm/s12_uvm_tlm_interfaces.py`

 * *Files identical despite different names*

### Comparing `pyuvm-2.9.1/pyuvm/s13_predefined_component_classes.py` & `pyuvm-3.0.0.dev0/pyuvm/s13_predefined_component_classes.py`

 * *Files identical despite different names*

### Comparing `pyuvm-2.9.1/pyuvm/s13_uvm_component.py` & `pyuvm-3.0.0.dev0/pyuvm/s13_uvm_component.py`

 * *Files 2% similar despite different names*

```diff
@@ -432,14 +432,15 @@
 # as defined by fnmatch().
 #
 # To avoid confusion with the full uvm_config_db
 # our class is named ConfigDB.
 
 
 class ConfigDB(metaclass=utility_classes.Singleton):
+    default_get = object()
     default_precedence = 1000
     legal_chars = set(string.ascii_letters) | set(string.digits) | set("_.")
     """
     A path-based singleton storage system
     """
 
     # The ConfigDB is a dual-level dict. The outer dict is a
@@ -530,85 +531,93 @@
         if uvm_root().running_phase is uvm_build_phase:
             precedence = self.default_precedence - context.get_depth()
 
         self._path_dict[inst_name][field_name][precedence] = value
 
         self.trace("SET", context, inst_name, field_name, value)
 
-    def get(self, context, inst_name, field_name):
+    def get(self, context, inst_name, field_name, default=default_get):
         """
         The component path matches against the paths in the ConfigDB. The path
         cannot have wildcards, but can match against keys with wildcards.
-        Return the value stored at key. Raise UVMConfigError if there is no key
+        Return the value stored at key. If the key is missing, returns default
+        or raises UVMConfigItemNotFound.
 
+        :param context: The component making the call
         :param inst_name: component full path with no wildcards
         :param field_name: the field_name being retrieved
-        :param context: The component making the call
+        :param default: the value to return if there is no key, defaults to
+            default_get
         :return: value found at location
         """
         if not set(inst_name).issubset(self.legal_chars):
             raise error_classes.UVMError(
                 f'"{inst_name}" is illegal: '
                 f'inst_name wildcards only allowed when storing.')
 
         context, inst_name = self._get_context_inst_name(context, inst_name)
 
-        key_matches = []  # Make the linter happy by setting this.
         try:
-            # key_matches = [dk for dk in self._path_dict.keys()
-            #                if fnmatch.fnmatch(inst_name, dk)]
-            for dk in self._path_dict.keys():
-                if fnmatch.fnmatch(inst_name, dk):
-                    key_matches.append(dk)
-
-        except TypeError:
-            raise error_classes.UVMConfigItemNotFound(
-                f'"{inst_name}" is not in ConfigDB().')
-        finally:
-            if len(key_matches) == 0:
+            key_matches = []  # Make the linter happy by setting this.
+            try:
+                # key_matches = [dk for dk in self._path_dict.keys()
+                #                if fnmatch.fnmatch(inst_name, dk)]
+                for dk in self._path_dict.keys():
+                    if fnmatch.fnmatch(inst_name, dk):
+                        key_matches.append(dk)
+
+            except TypeError:
                 raise error_classes.UVMConfigItemNotFound(
                     f'"{inst_name}" is not in ConfigDB().')
-        # Here we sort the list of paths by which paths are "in" other
-        # paths. That is A comes before '*'  A.B comes before A.*, etc.
-        # We use an insertion sort. A path is inserted in front of the
-        # first path it is "in"
-        sorted_paths = []
-        try:
-            sorted_paths.append(key_matches.pop())
-        except IndexError:
-            raise error_classes.UVMConfigItemNotFound(
-                f"{inst_name} not in ConfigDB()")
-
-        # Sort the matching keys from most specific to
-        # most greedy. A.B.C before A.B.* before A.* before *
-        for path in key_matches:
-            inserted = False
-            for ii in range(len(sorted_paths)):
-                if fnmatch.fnmatch(path, sorted_paths[ii]):
-                    sorted_paths.insert(ii, path)
-                    inserted = True
-                    break
-            if not inserted:
-                sorted_paths.append(path)
-        value = None
-        for path in sorted_paths:
+            finally:
+                if len(key_matches) == 0:
+                    raise error_classes.UVMConfigItemNotFound(
+                        f'"{inst_name}" is not in ConfigDB().')
+            # Here we sort the list of paths by which paths are "in" other
+            # paths. That is A comes before '*'  A.B comes before A.*, etc.
+            # We use an insertion sort. A path is inserted in front of the
+            # first path it is "in"
+            sorted_paths = []
             try:
-                component_fields = self._path_dict[path]
-                matching_path_fields = component_fields[field_name]
-                max_precedence = max(matching_path_fields.keys())
-                value = matching_path_fields[max_precedence]
-                break
-            except KeyError:
-                pass
-        if value is not None:
-            self.trace("GET", context, inst_name, field_name, value)
-            return value
-        else:
-            raise error_classes.UVMConfigItemNotFound(
-                f'"Component {inst_name} has no key: {field_name}')
+                sorted_paths.append(key_matches.pop())
+            except IndexError:
+                raise error_classes.UVMConfigItemNotFound(
+                    f"{inst_name} not in ConfigDB()")
+
+            # Sort the matching keys from most specific to
+            # most greedy. A.B.C before A.B.* before A.* before *
+            for path in key_matches:
+                inserted = False
+                for ii in range(len(sorted_paths)):
+                    if fnmatch.fnmatch(path, sorted_paths[ii]):
+                        sorted_paths.insert(ii, path)
+                        inserted = True
+                        break
+                if not inserted:
+                    sorted_paths.append(path)
+            value = None
+            for path in sorted_paths:
+                try:
+                    component_fields = self._path_dict[path]
+                    matching_path_fields = component_fields[field_name]
+                    max_precedence = max(matching_path_fields.keys())
+                    value = matching_path_fields[max_precedence]
+                    break
+                except KeyError:
+                    pass
+            if value is not None:
+                self.trace("GET", context, inst_name, field_name, value)
+                return value
+            else:
+                raise error_classes.UVMConfigItemNotFound(
+                    f'"Component {inst_name} has no key: {field_name}')
+        except error_classes.UVMConfigItemNotFound as e:
+            if default is self.default_get:
+                raise e
+            return default
 
     def exists(self, context, inst_name, field_name):
         """
         Returns true if there is data in the database at this location
         :param context: None or uvm_component
         :param inst_name: instance name string in context
         :param field_name: key name for location
```

### Comparing `pyuvm-2.9.1/pyuvm/s14_15_python_sequences.py` & `pyuvm-3.0.0.dev0/pyuvm/s14_15_python_sequences.py`

 * *Files identical despite different names*

### Comparing `pyuvm-2.9.1/pyuvm/utility_classes.py` & `pyuvm-3.0.0.dev0/pyuvm/utility_classes.py`

 * *Files identical despite different names*

### Comparing `pyuvm-2.9.1/pyuvm.egg-info/PKG-INFO` & `pyuvm-3.0.0.dev0/pyuvm.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: pyuvm
-Version: 2.9.1
+Version: 3.0.0.dev0
 Summary: A Python implementation of the UVM using cocotb
 Home-page: https://github.com/pyuvm/pyuvm
 Author: Ray Salemi
 Author-email: ray@raysalemi.com
 Project-URL: Bug Tracker, https://github.com/pyuvm/pyuvm/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Scientific/Engineering :: Electronic Design Automation (EDA)
 Classifier: Framework :: cocotb
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: cocotb>=1.6.0
 
 # PyUVM
 
 ## Description
 
 **pyuvm** is the Universal Verification Methodology implemented in Python instead of SystemVerilog. **pyuvm** uses cocotb to interact with the simulator and schedule simulation events.
 
@@ -32,14 +33,25 @@
 |5|Base Classes|uvm_object does not capture transaction timing information|
 |6|Reporting Classes|Leverages logging, controlled using UVM hierarchy|
 |8|Factory Classes|All uvm_void classes automatically registered|
 |9|Phasing|Simplified to only common phases. Supports objection system|
 |12|UVM TLM Interfaces|Fully implemented|
 |13|Predefined Component Classes|Implements uvm_component with hierarchy, uvm_root singleton,run_test(), simplified ConfigDB, uvm_driver, etc|
 |14 & 15|Sequences, sequencer, sequence_item|Refactored sequencer functionality leveraging Python language capabilities. Simpler and more direct implementation|
+|17|UVM Regfister Enum|All the basic Enum types to be used in the whole PYUVM Ral|
+|18|UVM Register Block|Main Register Block class|
+|19|UVM Register Field|Regsister Filed there are still few functionalities missing like atomic Backdoor access amd Field byte access or single Field access during read or write operation|
+|20|UVM Register|Main register class, still missing Backdoor and used Backdoor to be leveraged from cocotb force. Byte access and single field access yet to be implemeneted|
+|21|UVM Register Map|Main register map class, should be refatored to guarantee simplicity and backdoor access, extension class in Read and Write to be implemeneted|
+|22|UVM Memory|Not Implemented|
+|23|Register Item|Register Item used across multiple classes|
+|24|Register include file|Includes other Enum and typeds to be merged with s17|
+|25|UVM register adapter|Main register adapter|
+|26|UVM register predictor|Main register predictor, should be disabled if auto_prediction is not set|
+|27|Register Package|Main PKG if included and flake8 is not active should behave similarly to uvm_reg_pkg|
 
 ### Installation
 
 You can install **pyuvm** using `pip`. This will also install **cocotb** as a requirement for **pyuvm**.
 
 ```bash
 % pip install pyuvm
```

### Comparing `pyuvm-2.9.1/setup.py` & `pyuvm-3.0.0.dev0/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyuvm",
-    version="2.9.1",
+    version="3.0.0.dev0",
     author="Ray Salemi",
     author_email="ray@raysalemi.com",
     description="A Python implementation of the UVM using cocotb",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/pyuvm/pyuvm",
     project_urls={
```

