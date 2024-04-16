# Comparing `tmp/pyqcisim-1.2.1.tar.gz` & `tmp/pyqcisim-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyqcisim-1.2.1.tar", last modified: Wed Dec 13 07:12:17 2023, max compression
+gzip compressed data, was "pyqcisim-1.3.0.tar", last modified: Tue Apr 16 12:13:49 2024, max compression
```

## Comparing `pyqcisim-1.2.1.tar` & `pyqcisim-1.3.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxrwxr-x   0 xiangfu   (1005) xiangfu   (1005)        0 2023-12-13 07:12:17.678982 pyqcisim-1.2.1/
--rw-rw-r--   0 xiangfu   (1005) xiangfu   (1005)    11547 2023-07-09 01:45:11.000000 pyqcisim-1.2.1/LICENSE
--rw-r--r--   0 xiangfu   (1005) xiangfu   (1005)     9527 2023-12-13 07:12:17.678982 pyqcisim-1.2.1/PKG-INFO
--rw-rw-r--   0 xiangfu   (1005) xiangfu   (1005)     8836 2023-12-13 03:42:09.000000 pyqcisim-1.2.1/README.md
--rw-rw-r--   0 xiangfu   (1005) xiangfu   (1005)      108 2023-07-09 01:45:11.000000 pyqcisim-1.2.1/pyproject.toml
--rw-rw-r--   0 xiangfu   (1005) xiangfu   (1005)      783 2023-12-13 07:12:17.678982 pyqcisim-1.2.1/setup.cfg
--rw-rw-r--   0 xiangfu   (1005) xiangfu   (1005)       38 2023-07-09 01:45:11.000000 pyqcisim-1.2.1/setup.py
-drwxrwxr-x   0 xiangfu   (1005) xiangfu   (1005)        0 2023-12-13 07:12:17.674982 pyqcisim-1.2.1/src/
-drwxrwxr-x   0 xiangfu   (1005) xiangfu   (1005)        0 2023-12-13 07:12:17.678982 pyqcisim-1.2.1/src/pyqcisim/
--rw-rw-r--   0 xiangfu   (1005) xiangfu   (1005)     4808 2023-07-09 01:45:11.000000 pyqcisim-1.2.1/src/pyqcisim/QCIS_inst.py
--rw-rw-r--   0 xiangfu   (1005) xiangfu   (1005)     3618 2023-07-09 01:45:11.000000 pyqcisim-1.2.1/src/pyqcisim/QCIS_lexer.py
--rw-rw-r--   0 xiangfu   (1005) xiangfu   (1005)     6134 2023-12-13 03:42:09.000000 pyqcisim-1.2.1/src/pyqcisim/QCIS_parser.py
--rw-rw-r--   0 xiangfu   (1005) xiangfu   (1005)        0 2023-07-09 01:45:11.000000 pyqcisim-1.2.1/src/pyqcisim/__init__.py
--rw-rw-r--   0 xiangfu   (1005) xiangfu   (1005)     8520 2023-07-09 01:45:11.000000 pyqcisim-1.2.1/src/pyqcisim/circuit_executor.py
--rw-rw-r--   0 xiangfu   (1005) xiangfu   (1005)     3710 2023-12-13 07:10:41.000000 pyqcisim-1.2.1/src/pyqcisim/circuit_executor_tequila.py
--rw-rw-r--   0 xiangfu   (1005) xiangfu   (1005)     7983 2023-11-06 02:26:48.000000 pyqcisim-1.2.1/src/pyqcisim/parsetab.py
--rw-rw-r--   0 xiangfu   (1005) xiangfu   (1005)     2055 2023-12-13 03:42:09.000000 pyqcisim-1.2.1/src/pyqcisim/simulate_qcis.py
--rw-rw-r--   0 xiangfu   (1005) xiangfu   (1005)     5518 2023-12-13 03:42:09.000000 pyqcisim-1.2.1/src/pyqcisim/simulator.py
--rw-rw-r--   0 xiangfu   (1005) xiangfu   (1005)     5932 2023-12-13 07:10:41.000000 pyqcisim-1.2.1/src/pyqcisim/utils.py
-drwxrwxr-x   0 xiangfu   (1005) xiangfu   (1005)        0 2023-12-13 07:12:17.678982 pyqcisim-1.2.1/src/pyqcisim.egg-info/
--rw-r--r--   0 xiangfu   (1005) xiangfu   (1005)     9527 2023-12-13 07:12:17.000000 pyqcisim-1.2.1/src/pyqcisim.egg-info/PKG-INFO
--rw-rw-r--   0 xiangfu   (1005) xiangfu   (1005)      513 2023-12-13 07:12:17.000000 pyqcisim-1.2.1/src/pyqcisim.egg-info/SOURCES.txt
--rw-rw-r--   0 xiangfu   (1005) xiangfu   (1005)        1 2023-12-13 07:12:17.000000 pyqcisim-1.2.1/src/pyqcisim.egg-info/dependency_links.txt
--rw-rw-r--   0 xiangfu   (1005) xiangfu   (1005)       45 2023-12-13 07:12:17.000000 pyqcisim-1.2.1/src/pyqcisim.egg-info/requires.txt
--rw-rw-r--   0 xiangfu   (1005) xiangfu   (1005)        9 2023-12-13 07:12:17.000000 pyqcisim-1.2.1/src/pyqcisim.egg-info/top_level.txt
+drwxrwxr-x   0 xiangfu   (1005) xiangfu   (1005)        0 2024-04-16 12:13:49.412116 pyqcisim-1.3.0/
+-rw-rw-r--   0 xiangfu   (1005) xiangfu   (1005)    11547 2023-07-09 01:45:11.000000 pyqcisim-1.3.0/LICENSE
+-rw-rw-r--   0 xiangfu   (1005) xiangfu   (1005)     9407 2024-04-16 12:13:49.412116 pyqcisim-1.3.0/PKG-INFO
+-rw-rw-r--   0 xiangfu   (1005) xiangfu   (1005)     8836 2023-12-13 03:42:09.000000 pyqcisim-1.3.0/README.md
+-rw-rw-r--   0 xiangfu   (1005) xiangfu   (1005)      108 2023-07-09 01:45:11.000000 pyqcisim-1.3.0/pyproject.toml
+-rw-rw-r--   0 xiangfu   (1005) xiangfu   (1005)      783 2024-04-16 12:13:49.416117 pyqcisim-1.3.0/setup.cfg
+-rw-rw-r--   0 xiangfu   (1005) xiangfu   (1005)       38 2023-07-09 01:45:11.000000 pyqcisim-1.3.0/setup.py
+drwxrwxr-x   0 xiangfu   (1005) xiangfu   (1005)        0 2024-04-16 12:13:49.408116 pyqcisim-1.3.0/src/
+drwxrwxr-x   0 xiangfu   (1005) xiangfu   (1005)        0 2024-04-16 12:13:49.412116 pyqcisim-1.3.0/src/pyqcisim/
+-rw-rw-r--   0 xiangfu   (1005) xiangfu   (1005)     4808 2023-07-09 01:45:11.000000 pyqcisim-1.3.0/src/pyqcisim/QCIS_inst.py
+-rw-rw-r--   0 xiangfu   (1005) xiangfu   (1005)     3618 2023-07-09 01:45:11.000000 pyqcisim-1.3.0/src/pyqcisim/QCIS_lexer.py
+-rw-rw-r--   0 xiangfu   (1005) xiangfu   (1005)     6134 2023-12-13 03:42:09.000000 pyqcisim-1.3.0/src/pyqcisim/QCIS_parser.py
+-rw-rw-r--   0 xiangfu   (1005) xiangfu   (1005)        0 2023-07-09 01:45:11.000000 pyqcisim-1.3.0/src/pyqcisim/__init__.py
+-rw-rw-r--   0 xiangfu   (1005) xiangfu   (1005)     8520 2024-04-16 08:15:55.000000 pyqcisim-1.3.0/src/pyqcisim/circuit_executor.py
+-rw-rw-r--   0 xiangfu   (1005) xiangfu   (1005)     4893 2024-04-16 08:34:57.000000 pyqcisim-1.3.0/src/pyqcisim/circuit_executor_tequila.py
+-rw-rw-r--   0 xiangfu   (1005) xiangfu   (1005)     7983 2023-11-06 02:26:48.000000 pyqcisim-1.3.0/src/pyqcisim/parsetab.py
+-rw-rw-r--   0 xiangfu   (1005) xiangfu   (1005)     2055 2023-12-13 03:42:09.000000 pyqcisim-1.3.0/src/pyqcisim/simulate_qcis.py
+-rw-rw-r--   0 xiangfu   (1005) xiangfu   (1005)     6387 2024-04-16 11:50:46.000000 pyqcisim-1.3.0/src/pyqcisim/simulator.py
+-rw-rw-r--   0 xiangfu   (1005) xiangfu   (1005)     5967 2024-04-16 08:24:26.000000 pyqcisim-1.3.0/src/pyqcisim/utils.py
+drwxrwxr-x   0 xiangfu   (1005) xiangfu   (1005)        0 2024-04-16 12:13:49.412116 pyqcisim-1.3.0/src/pyqcisim.egg-info/
+-rw-r--r--   0 xiangfu   (1005) xiangfu   (1005)     9407 2024-04-16 12:13:49.000000 pyqcisim-1.3.0/src/pyqcisim.egg-info/PKG-INFO
+-rw-rw-r--   0 xiangfu   (1005) xiangfu   (1005)      513 2024-04-16 12:13:49.000000 pyqcisim-1.3.0/src/pyqcisim.egg-info/SOURCES.txt
+-rw-rw-r--   0 xiangfu   (1005) xiangfu   (1005)        1 2024-04-16 12:13:49.000000 pyqcisim-1.3.0/src/pyqcisim.egg-info/dependency_links.txt
+-rw-rw-r--   0 xiangfu   (1005) xiangfu   (1005)       45 2024-04-16 12:13:49.000000 pyqcisim-1.3.0/src/pyqcisim.egg-info/requires.txt
+-rw-rw-r--   0 xiangfu   (1005) xiangfu   (1005)        9 2024-04-16 12:13:49.000000 pyqcisim-1.3.0/src/pyqcisim.egg-info/top_level.txt
```

### Comparing `pyqcisim-1.2.1/LICENSE` & `pyqcisim-1.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyqcisim-1.2.1/PKG-INFO` & `pyqcisim-1.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,21 @@
 Metadata-Version: 2.1
 Name: pyqcisim
-Version: 1.2.1
+Version: 1.3.0
 Summary: A Python-based Quantum Control Instruction Set (QCIS) simulator
 Home-page: https://gitee.com/hpcl_quanta/pyqcisim
 Author: Zhihao Wu, Xiang Fu, Wenjin Chen
 Author-email: gtaifu@gmail.com
 Project-URL: Bug Tracker, https://gitee.com/hpcl_quanta/pyqcisim/issues
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: quantumsim==0.2.0
-Requires-Dist: bitstring
-Requires-Dist: ply
-Requires-Dist: numpy
-Requires-Dist: pytest
 
 # PyQCISim
 
 ## Introduction
 
 A Python-based Quantum Control Instruction Set (QCIS) simulator developed by Zhihao Wu and Xiang Fu from QUANTA@NUDT.
```

### Comparing `pyqcisim-1.2.1/README.md` & `pyqcisim-1.3.0/README.md`

 * *Files identical despite different names*

### Comparing `pyqcisim-1.2.1/setup.cfg` & `pyqcisim-1.3.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pyqcisim
-version = 1.2.1
+version = 1.3.0
 author = Zhihao Wu, Xiang Fu, Wenjin Chen
 author_email = gtaifu@gmail.com
 use_2to3 = False
 description = A Python-based Quantum Control Instruction Set (QCIS) simulator
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://gitee.com/hpcl_quanta/pyqcisim
```

### Comparing `pyqcisim-1.2.1/src/pyqcisim/QCIS_inst.py` & `pyqcisim-1.3.0/src/pyqcisim/QCIS_inst.py`

 * *Files identical despite different names*

### Comparing `pyqcisim-1.2.1/src/pyqcisim/QCIS_lexer.py` & `pyqcisim-1.3.0/src/pyqcisim/QCIS_lexer.py`

 * *Files identical despite different names*

### Comparing `pyqcisim-1.2.1/src/pyqcisim/QCIS_parser.py` & `pyqcisim-1.3.0/src/pyqcisim/QCIS_parser.py`

 * *Files identical despite different names*

### Comparing `pyqcisim-1.2.1/src/pyqcisim/circuit_executor.py` & `pyqcisim-1.3.0/src/pyqcisim/circuit_executor.py`

 * *Files identical despite different names*

### Comparing `pyqcisim-1.2.1/src/pyqcisim/circuit_executor_tequila.py` & `pyqcisim-1.3.0/src/pyqcisim/circuit_executor_tequila.py`

 * *Files 20% similar despite different names*

```diff
@@ -43,22 +43,34 @@
         self._qubit_name_number_dict = dict()
         for i, name in enumerate(self._names):
             self._qubit_name_number_dict[name] = i
 
     def reset(self):
         pass
 
-    def execute(self, instructions, num_shots):
+    def execute(self, instructions, mode, num_shots):
+
+        assert mode in ["one_shot", "state_vector", "final_result"]
+
         # prepare qubits
         q = qubit(len(self._names))
 
         msmt_qubits = []
 
+        insns_to_simulate = instructions
+        first_msmt_idx = len(instructions)
+        if mode == "state_vector":
+            for i, inst in enumerate(instructions):
+                if inst.op_code.is_measure_op():
+                    first_msmt_idx = i
+                    break
+        insns_to_simulate = instructions[:first_msmt_idx]
+
         # apply gates
-        for inst in instructions:
+        for inst in insns_to_simulate:
             if inst.op_code not in (
                 set(SINGLE_QUBIT_CODE_TENSOR_DICT.keys())
                 | set(TWO_QUBIT_CODE_TENSOR_DICT.keys())
                 | set([QCISOpCode.MEASURE, QCISOpCode.M])
             ):
                 raise ValueError(
                     "Unsupported instruction for TEQUILA backend: {}".format(
@@ -84,16 +96,36 @@
 
             if inst.op_code.is_measure_op():
                 msmt_qubits.extend(
                     list(
                         map(lambda q: self._qubit_name_number_dict[q], inst.qubits_list)
                     )
                 )
-        num_msmt_qubits = len(msmt_qubits)
-        msmt_qubit_names = list(map(lambda q: self._names[q], msmt_qubits))
-        msmts = []
-        for i in range(num_shots):
+
+        if mode == "one_shot":
+            num_msmt_qubits = len(msmt_qubits)
+            msmt_qubit_names = list(map(lambda q: self._names[q], msmt_qubits))
+            msmts = []
+            for i in range(num_shots):
+                """meas_rej returns result in a dict format: {'11000': 2, '00100': 3}"""
+                bit_str_res = list(q.meas_rej(msmt_qubits, 1).keys())[0]
+                res = [int(bit_str_res[j], 2) for j in range(num_msmt_qubits)]
+                msmts.append(res)
+
+            return (msmt_qubit_names, msmts)
+
+        if mode == "final_result":
+            num_msmt_qubits = len(msmt_qubits)
+            msmt_qubit_names = list(map(lambda q: self._names[q], msmt_qubits))
+            msmts = []
             """meas_rej returns result in a dict format: {'11000': 2, '00100': 3}"""
             bit_str_res = list(q.meas_rej(msmt_qubits, 1).keys())[0]
             res = [int(bit_str_res[i], 2) for i in range(num_msmt_qubits)]
             msmts.append(res)
-        return (msmt_qubit_names, msmts)
+
+            result = {}
+            result["classical"] = (msmt_qubit_names, msmts)
+            result["quantum"] = (self._names, q.vec())
+            return result
+
+        if mode == "state_vector":
+            return (self._names, q.vec())
```

### Comparing `pyqcisim-1.2.1/src/pyqcisim/parsetab.py` & `pyqcisim-1.3.0/src/pyqcisim/parsetab.py`

 * *Files identical despite different names*

### Comparing `pyqcisim-1.2.1/src/pyqcisim/simulate_qcis.py` & `pyqcisim-1.3.0/src/pyqcisim/simulate_qcis.py`

 * *Files identical despite different names*

### Comparing `pyqcisim-1.2.1/src/pyqcisim/simulator.py` & `pyqcisim-1.3.0/src/pyqcisim/simulator.py`

 * *Files 27% similar despite different names*

```diff
@@ -45,27 +45,27 @@
         if not success:
             print(self._parser.error_list)
             raise ValueError("QCIS parser failed to compile the given QCIS program.")
         self._compile_success = success
         self._instructions = instructions
         self._names = names
 
-    def simulate(self, mode="one_shot", num_shots=1000):
+    def simulate(self, mode="one_shot", num_shots=1):
         if self._backend == "quantumsim":
             return self.simulate_quantumsim(mode, num_shots)
         elif self._backend == "tequila":
             return self.simulate_tequila(mode, num_shots)
         else:
             raise ValueError(
                 "Invalid backend: '{}' (supported are: 'quantumsim' and 'tequila').".format(
                     self._backend
                 )
             )
 
-    def simulate_quantumsim(self, mode="one_shot", num_shots=1000):
+    def simulate_quantumsim(self, mode="one_shot", num_shots=1):
         """Simulate the compiled QCIS program by QuantumSim.
 
         Args:
           - mode (string): the simulation mode to use:
               - "one_shot":
                 The output is a tuple of two elements:
                     - the first element is a list of qubit names `names`
@@ -88,54 +88,77 @@
           - num_shots (int): the number of iterations performed in `one_shot` mode.
         """
         from pyqcisim.circuit_executor import CircuitExecutor
 
         if not self._compile_success:
             raise ValueError("Failed to simulate due to compilation error.")
 
+        supported_modes = ["one_shot", "state_vector", "final_result"]
+        if mode not in supported_modes:
+            raise ValueError(
+                "Invalid simulation mode '{}' for PyQCISim-QuantumSim (supported is: {})".format(
+                    mode, supported_modes
+                )
+            )
+
         self._circuit_executor = CircuitExecutor(self._names)
 
         if mode == "one_shot":
             one_shot_msmts = []
             for i in range(num_shots):
                 self._circuit_executor.reset()  # Reset the quantum state simulator
 
                 for inst in self._instructions:  # Execute instructions one by one.
                     self._circuit_executor.execute(inst)
 
                 # Pending operations will not be done!
                 # As they do not contribute to the measurement results!
                 one_shot_msmts.append(self._circuit_executor.res)
 
-            # final_result = count_final_result(one_shot_msmts)
-            final_result = format_result(one_shot_msmts)
+            return format_result(one_shot_msmts)
 
-        elif mode == "final_state":
+        if mode in ["state_vector", "final_result"]:
             self._circuit_executor.reset()  # Reset the quantum state simulator
-            for inst in self._instructions:  # Execute instructions one by one.
-                self._circuit_executor.execute(inst)
-            final_result = self._circuit_executor.get_quantum_state()
 
-        else:
-            raise ValueError(
-                "Invalid simulation mode: '{}' (supported are: 'one_shot' and "
-                "'final_state').".format(mode)
-            )
+            insns_to_simulate = self._instructions
+            first_msmt_idx = len(insns_to_simulate)
+            if mode == "state_vector":
+                for i, inst in enumerate(insns_to_simulate):
+                    if inst.op_code.is_measure_op():
+                        first_msmt_idx = i
+                        break
+
+            insns_to_simulate = insns_to_simulate[:first_msmt_idx]
+
+            for inst in insns_to_simulate:  # Execute instructions one by one.
+                self._circuit_executor.execute(inst)
 
-        return final_result
+            if mode == "state_vector":
+                return self._circuit_executor.get_quantum_state(separate=False)
+            else:
+                return self._circuit_executor.get_quantum_state()
+
+        raise ValueError(
+            "Invalid simulation mode: '{}' (supported are: 'one_shot' and "
+            "'state').".format(mode)
+        )
 
     def simulate_tequila(self, mode="one_shot", num_shots=1000):
         """Simulate the compiled QCIS program by Tequila."""
 
         from pyqcisim.circuit_executor_tequila import CircuitExecutorTequila
 
         if not self._compile_success:
             raise ValueError("Failed to simulate due to compilation error.")
-        if not (mode == "one_shot"):
+
+        supported_modes = ["one_shot", "state_vector", "final_result"]
+        if mode not in supported_modes:
             raise ValueError(
-                "Invalid simulation mode: '{}' (supported is: 'one_shot')".format(mode)
+                "Invalid simulation mode '{}' for PyQCISim-TEQUILA (supported is: {]})".format(
+                    mode, supported_modes
+                )
             )
 
         self._circuit_executor = CircuitExecutorTequila(self._names)
         self._circuit_executor.reset()
-        ret = self._circuit_executor.execute(self._instructions, num_shots)
+        ret = self._circuit_executor.execute(self._instructions, mode, num_shots)
         return ret
```

### Comparing `pyqcisim-1.2.1/src/pyqcisim/utils.py` & `pyqcisim-1.3.0/src/pyqcisim/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,17 +20,15 @@
     """
     if not is_number(x):
         raise ValueError("get_bin: parameter {} is not a number.".format(x))
 
     if Unsigned is True:
         return "{0:{fill}{width}b}".format(int(x), fill="0", width=n)
     else:
-        return "{0:{fill}{width}b}".format(
-            (int(x) + 2**n) % 2**n, fill="0", width=n
-        )
+        return "{0:{fill}{width}b}".format((int(x) + 2**n) % 2**n, fill="0", width=n)
 
 
 def format_result(final_results):
     """
     Format the one shot simulation results of multiple iterations.
 
     Input: [{'Q3': 1, 'Q4': 1, 'Q5': 0, 'Q6': 0, 'Q7': 0}, {'Q3': 1, 'Q4': 1, 'Q5': 0, 'Q6': 0, 'Q7': 0}, {'Q3': 1, 'Q4': 1, 'Q5': 0, 'Q6': 0, 'Q7': 0}]
@@ -38,16 +36,19 @@
     The output is a tuple of two elements:
     - the first element is a list of qubit names `names`
     - the second element is the collection of all measurement results, with the i-th
       element in each measurement result being that of the i-th qubit in `names`.
     Note: the qubit names will be sorted. Example:
     (['Q3', 'Q4', 'Q5', 'Q6', 'Q7'], [[1, 1, 0, 0, 0], [1, 1, 0, 0, 0], [1, 1, 0, 0, 0]])
     """
-    if len(final_results) == 0 or len(final_results[0]) == 0:
-        return None
+    if len(final_results) == 0:
+        return ([], [])
+
+    if len(final_results[0]) == 0:
+        return ([], [[]] * len(final_results))
 
     first_shot_result = final_results[0]
     num_qubits = len(first_shot_result)
     names = list(first_shot_result.keys())
     names.sort()
 
     assert all(isinstance(one_shot, dict) for one_shot in final_results)
```

### Comparing `pyqcisim-1.2.1/src/pyqcisim.egg-info/PKG-INFO` & `pyqcisim-1.3.0/src/pyqcisim.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,21 @@
 Metadata-Version: 2.1
 Name: pyqcisim
-Version: 1.2.1
+Version: 1.3.0
 Summary: A Python-based Quantum Control Instruction Set (QCIS) simulator
 Home-page: https://gitee.com/hpcl_quanta/pyqcisim
 Author: Zhihao Wu, Xiang Fu, Wenjin Chen
 Author-email: gtaifu@gmail.com
 Project-URL: Bug Tracker, https://gitee.com/hpcl_quanta/pyqcisim/issues
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: quantumsim==0.2.0
-Requires-Dist: bitstring
-Requires-Dist: ply
-Requires-Dist: numpy
-Requires-Dist: pytest
 
 # PyQCISim
 
 ## Introduction
 
 A Python-based Quantum Control Instruction Set (QCIS) simulator developed by Zhihao Wu and Xiang Fu from QUANTA@NUDT.
```

### Comparing `pyqcisim-1.2.1/src/pyqcisim.egg-info/SOURCES.txt` & `pyqcisim-1.3.0/src/pyqcisim.egg-info/SOURCES.txt`

 * *Files identical despite different names*

