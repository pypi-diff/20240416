# Comparing `tmp/pyrevm_contract-0.2.8.tar.gz` & `tmp/pyrevm_contract-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrevm_contract-0.2.8.tar", last modified: Wed Jan  3 19:36:01 2024, max compression
+gzip compressed data, was "pyrevm_contract-0.3.0.tar", last modified: Tue Apr 16 00:52:56 2024, max compression
```

## Comparing `pyrevm_contract-0.2.8.tar` & `pyrevm_contract-0.3.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 jcalb      (501) staff       (20)        0 2024-01-03 19:36:01.422451 pyrevm_contract-0.2.8/
--rw-r--r--   0 jcalb      (501) staff       (20)     1071 2023-09-28 23:14:04.000000 pyrevm_contract-0.2.8/LICENSE
--rw-r--r--   0 jcalb      (501) staff       (20)     1961 2024-01-03 19:36:01.422205 pyrevm_contract-0.2.8/PKG-INFO
--rw-r--r--   0 jcalb      (501) staff       (20)     1429 2023-10-23 23:44:56.000000 pyrevm_contract-0.2.8/README.md
-drwxr-xr-x   0 jcalb      (501) staff       (20)        0 2024-01-03 19:36:01.421027 pyrevm_contract-0.2.8/pyrevm_contract/
--rw-r--r--   0 jcalb      (501) staff       (20)       96 2023-10-20 23:42:17.000000 pyrevm_contract-0.2.8/pyrevm_contract/__init__.py
--rw-r--r--   0 jcalb      (501) staff       (20)     3551 2024-01-03 19:35:07.000000 pyrevm_contract-0.2.8/pyrevm_contract/abi.py
--rw-r--r--   0 jcalb      (501) staff       (20)     2895 2023-12-04 02:40:44.000000 pyrevm_contract-0.2.8/pyrevm_contract/contract.py
--rw-r--r--   0 jcalb      (501) staff       (20)     1444 2023-11-15 07:20:16.000000 pyrevm_contract-0.2.8/pyrevm_contract/revm.py
-drwxr-xr-x   0 jcalb      (501) staff       (20)        0 2024-01-03 19:36:01.421991 pyrevm_contract-0.2.8/pyrevm_contract.egg-info/
--rw-r--r--   0 jcalb      (501) staff       (20)     1961 2024-01-03 19:36:01.000000 pyrevm_contract-0.2.8/pyrevm_contract.egg-info/PKG-INFO
--rw-r--r--   0 jcalb      (501) staff       (20)      346 2024-01-03 19:36:01.000000 pyrevm_contract-0.2.8/pyrevm_contract.egg-info/SOURCES.txt
--rw-r--r--   0 jcalb      (501) staff       (20)        1 2024-01-03 19:36:01.000000 pyrevm_contract-0.2.8/pyrevm_contract.egg-info/dependency_links.txt
--rw-r--r--   0 jcalb      (501) staff       (20)       25 2024-01-03 19:36:01.000000 pyrevm_contract-0.2.8/pyrevm_contract.egg-info/requires.txt
--rw-r--r--   0 jcalb      (501) staff       (20)       16 2024-01-03 19:36:01.000000 pyrevm_contract-0.2.8/pyrevm_contract.egg-info/top_level.txt
--rw-r--r--   0 jcalb      (501) staff       (20)       38 2024-01-03 19:36:01.422494 pyrevm_contract-0.2.8/setup.cfg
--rw-r--r--   0 jcalb      (501) staff       (20)      788 2024-01-03 19:35:56.000000 pyrevm_contract-0.2.8/setup.py
-drwxr-xr-x   0 jcalb      (501) staff       (20)        0 2024-01-03 19:36:01.421801 pyrevm_contract-0.2.8/tests/
--rw-r--r--   0 jcalb      (501) staff       (20)     3569 2023-11-02 23:50:21.000000 pyrevm_contract-0.2.8/tests/test_contract.py
+drwxr-xr-x   0 jcalb      (501) staff       (20)        0 2024-04-16 00:52:56.880999 pyrevm_contract-0.3.0/
+-rw-r--r--   0 jcalb      (501) staff       (20)     1071 2023-09-28 23:14:04.000000 pyrevm_contract-0.3.0/LICENSE
+-rw-r--r--   0 jcalb      (501) staff       (20)     2006 2024-04-16 00:52:56.880778 pyrevm_contract-0.3.0/PKG-INFO
+-rw-r--r--   0 jcalb      (501) staff       (20)     1429 2023-10-23 23:44:56.000000 pyrevm_contract-0.3.0/README.md
+drwxr-xr-x   0 jcalb      (501) staff       (20)        0 2024-04-16 00:52:56.876941 pyrevm_contract-0.3.0/pyrevm_contract/
+-rw-r--r--   0 jcalb      (501) staff       (20)       96 2023-10-20 23:42:17.000000 pyrevm_contract-0.3.0/pyrevm_contract/__init__.py
+-rw-r--r--   0 jcalb      (501) staff       (20)     3481 2024-04-16 00:50:03.000000 pyrevm_contract-0.3.0/pyrevm_contract/abi.py
+-rw-r--r--   0 jcalb      (501) staff       (20)     2656 2024-04-16 00:50:14.000000 pyrevm_contract-0.3.0/pyrevm_contract/contract.py
+-rw-r--r--   0 jcalb      (501) staff       (20)     1357 2024-04-16 00:33:09.000000 pyrevm_contract-0.3.0/pyrevm_contract/revm.py
+drwxr-xr-x   0 jcalb      (501) staff       (20)        0 2024-04-16 00:52:56.880506 pyrevm_contract-0.3.0/pyrevm_contract.egg-info/
+-rw-r--r--   0 jcalb      (501) staff       (20)     2006 2024-04-16 00:52:56.000000 pyrevm_contract-0.3.0/pyrevm_contract.egg-info/PKG-INFO
+-rw-r--r--   0 jcalb      (501) staff       (20)      346 2024-04-16 00:52:56.000000 pyrevm_contract-0.3.0/pyrevm_contract.egg-info/SOURCES.txt
+-rw-r--r--   0 jcalb      (501) staff       (20)        1 2024-04-16 00:52:56.000000 pyrevm_contract-0.3.0/pyrevm_contract.egg-info/dependency_links.txt
+-rw-r--r--   0 jcalb      (501) staff       (20)       55 2024-04-16 00:52:56.000000 pyrevm_contract-0.3.0/pyrevm_contract.egg-info/requires.txt
+-rw-r--r--   0 jcalb      (501) staff       (20)       16 2024-04-16 00:52:56.000000 pyrevm_contract-0.3.0/pyrevm_contract.egg-info/top_level.txt
+-rw-r--r--   0 jcalb      (501) staff       (20)       38 2024-04-16 00:52:56.881070 pyrevm_contract-0.3.0/setup.cfg
+-rw-r--r--   0 jcalb      (501) staff       (20)      828 2024-04-16 00:50:28.000000 pyrevm_contract-0.3.0/setup.py
+drwxr-xr-x   0 jcalb      (501) staff       (20)        0 2024-04-16 00:52:56.880156 pyrevm_contract-0.3.0/tests/
+-rw-r--r--   0 jcalb      (501) staff       (20)     3564 2024-04-16 00:50:58.000000 pyrevm_contract-0.3.0/tests/test_contract.py
```

### Comparing `pyrevm_contract-0.2.8/LICENSE` & `pyrevm_contract-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrevm_contract-0.2.8/PKG-INFO` & `pyrevm_contract-0.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: pyrevm_contract
-Version: 0.2.8
+Version: 0.3.0
 Summary: Minimal Brownie like contract wrapper for Pyrevm
 Home-page: https://github.com/jalbrekt85/pyrevm_contract
 Author: jalbrekt85
 Author-email: jcalbrecht85@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: pyrevm
+Requires-Dist: pyrevm==0.3.0
 Requires-Dist: eth-abi
 Requires-Dist: eth-utils
+Requires-Dist: eth-hash[pycryptodome]
 
 # pyrevm_contract
 Minimal Brownie like contract wrapper for Pyrevm
 
 ```
 pip install pyrevm_contract
 ```
```

### Comparing `pyrevm_contract-0.2.8/README.md` & `pyrevm_contract-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `pyrevm_contract-0.2.8/pyrevm_contract/abi.py` & `pyrevm_contract-0.3.0/pyrevm_contract/abi.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,17 +46,15 @@
         return selector + encoded_inputs
 
     def decode_outputs(self, output_data: bytes) -> Any:
         if not output_data or not self.outputs:
             return None
 
         if isinstance(output_data, str):
-            output_data = bytes.fromhex(
-                output_data[2:] if output_data.startswith("0x") else output_data
-            )
+            output_data = bytes.fromhex(output_data.lstrip("0x"))
 
         try:
             decoded = decode(self.outputs, output_data)
             decoded = [
                 to_checksum_address(value) if typ == "address" else value
                 for value, typ in zip(decoded, self.outputs)
             ]
```

### Comparing `pyrevm_contract-0.2.8/pyrevm_contract/contract.py` & `pyrevm_contract-0.3.0/pyrevm_contract/contract.py`

 * *Files 8% similar despite different names*

```diff
@@ -50,35 +50,28 @@
 
         return parse_json_abi(abi)
 
     def call_function(self, func: ABIFunction, args: tuple, kwargs: dict = {}):
         value = kwargs.get("value", 0)
         caller = kwargs.get("caller", self.caller)
         ignore_outputs = kwargs.get("ignore_outputs", False)
-
         calldata = func.encode_inputs(args)
 
-        if func.constant:
-            raw_output = self.revm.call_raw(
-                caller=caller, to=self.address, data=calldata
-            )
-            if not ignore_outputs:
-                return func.decode_outputs(raw_output)
-        else:
-            if not func.payable and value > 0:
-                raise ValueError("Cannot send value to a non-payable function")
-
-            if caller == ZERO_ADDRESS:
-                raise ValueError("Cannot call a non-constant function without a caller")
-
-            raw_output = self.revm.call_raw_committing(
-                caller=caller,
-                to=self.address,
-                data=calldata,
-                value=value,
-            )
+        if not func.payable and value > 0:
+            raise ValueError("Cannot send value to a non-payable function")
+
+        if not func.constant and caller == ZERO_ADDRESS:
+            raise ValueError("Cannot call a non-constant function without a caller")
+
+        raw_output = self.revm.message_call(
+            caller=self.caller,
+            to=self.address,
+            calldata=calldata,
+            value=value,
+            is_static=func.constant,
+        )
 
-            if not ignore_outputs:
-                return func.decode_outputs(raw_output)
+        if not ignore_outputs:
+            return func.decode_outputs(raw_output)
 
     def balance(self):
         return self.revm.get_balance(self.address)
```

### Comparing `pyrevm_contract-0.2.8/pyrevm_contract/revm.py` & `pyrevm_contract-0.3.0/pyrevm_contract/revm.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,43 +1,39 @@
 from pyrevm import *
 
 
 class Revm:
     _instance = None
 
-    def __new__(cls, fork_url="", block_number=0, *args, **kwargs):
+    def __new__(cls, fork_url="", block_number="latest", *args, **kwargs):
         if cls._instance is None:
             cls._instance = super(Revm, cls).__new__(cls)
             cls._instance.fork_url = fork_url
             cls._instance.block_number = block_number
             cls._instance.revm = EVM(
                 fork_url=fork_url,
                 tracing=False,
-                fork_block_number=block_number,
+                fork_block=str(block_number),
             )
         return cls._instance
 
     def __init__(self, fork_url="", block_number=0):
         pass
 
-    def update_fork(self, new_block_number, fork_url=""):
+    def update_fork(self, new_block_number=None, fork_url=None):
         fork_url = fork_url if fork_url else self.fork_url
+        self.block_number = new_block_number if new_block_number else self.block_number
         self.revm = EVM(
             fork_url=fork_url,
             tracing=False,
-            fork_block_number=new_block_number,
+            fork_block=str(new_block_number),
         )
-        self.block_number = new_block_number
-        self.fork_url = fork_url
 
-    def call_raw(self, *args, **kwargs):
-        return self.revm.call_raw(*args, **kwargs)
-
-    def call_raw_committing(self, *args, **kwargs):
-        return self.revm.call_raw_committing(*args, **kwargs)
+    def message_call(self, *args, **kwargs):
+        return self.revm.message_call(*args, **kwargs)
 
     def get_balance(self, address):
         return self.revm.get_balance(address)
 
     def set_balance(self, address, value):
         return self.revm.set_balance(address, value)
```

### Comparing `pyrevm_contract-0.2.8/pyrevm_contract.egg-info/PKG-INFO` & `pyrevm_contract-0.3.0/pyrevm_contract.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: pyrevm_contract
-Version: 0.2.8
+Version: 0.3.0
 Summary: Minimal Brownie like contract wrapper for Pyrevm
 Home-page: https://github.com/jalbrekt85/pyrevm_contract
 Author: jalbrekt85
 Author-email: jcalbrecht85@gmail.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: pyrevm
+Requires-Dist: pyrevm==0.3.0
 Requires-Dist: eth-abi
 Requires-Dist: eth-utils
+Requires-Dist: eth-hash[pycryptodome]
 
 # pyrevm_contract
 Minimal Brownie like contract wrapper for Pyrevm
 
 ```
 pip install pyrevm_contract
 ```
```

### Comparing `pyrevm_contract-0.2.8/setup.py` & `pyrevm_contract-0.3.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="pyrevm_contract",
-    version="0.2.8",
+    version="0.3.0",
     author="jalbrekt85",
     author_email="jcalbrecht85@gmail.com",
     description="Minimal Brownie like contract wrapper for Pyrevm",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/jalbrekt85/pyrevm_contract",
     packages=find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
     python_requires=">=3.9",
     install_requires=[
-        "pyrevm",
+        "pyrevm==0.3.0",
         "eth-abi",
         "eth-utils",
+        "eth-hash[pycryptodome]"
     ],
 )
```

### Comparing `pyrevm_contract-0.2.8/tests/test_contract.py` & `pyrevm_contract-0.3.0/tests/test_contract.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,24 +13,23 @@
         self.vault_addr = "0xBA12222222228d8Ba445958a75a0704d566BF2C8"
         self.weth_addr = "0xC02aaA39b223FE8D0A0e5C4F27eAD9083C756Cc2"
         self.bal_addr = "0xba100000625a3754423978a60c9317c58a424e3D"
         self.pool_id = (
             "0x5c6ee304399dbdb9c8ef030ab642b10820db8f56000200000000000000000014"
         )
 
-        Revm("https://eth.llamarpc.com", 18000000)
+        self.revm = Revm("http://eth.llamarpc.com", 18000000)
         self.vault = Contract(self.vault_addr, vault_abi)
 
     def test_init(self):
         self.assertEqual(
             self.vault.address, "0xBA12222222228d8Ba445958a75a0704d566BF2C8"
         )
-        self.assertEqual(len(self.vault.abi.functions), 1)
-        batch_swap = self.vault.abi.functions[0]
-        self.assertEqual(batch_swap.name, "queryBatchSwap")
+        self.assertEqual(len(self.vault.abi.functions), 26)
+        batch_swap = [f for f in self.vault.abi.functions if f.name == "queryBatchSwap"][0]
         self.assertEqual(
             batch_swap.inputs,
             [
                 "uint8",
                 "(bytes32,uint256,uint256,uint256,bytes)[]",
                 "address[]",
                 "(address,bool,address,bool)",
```

