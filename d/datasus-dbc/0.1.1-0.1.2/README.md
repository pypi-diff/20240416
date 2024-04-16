# Comparing `tmp/datasus_dbc-0.1.1.tar.gz` & `tmp/datasus_dbc-0.1.2.tar.gz`

## Comparing `datasus_dbc-0.1.1.tar` & `datasus_dbc-0.1.2.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0      502 1970-01-01 00:00:00.000000 datasus_dbc-0.1.1/Cargo.toml
--rw-r--r--   0     1001      127     2825 2023-12-06 20:06:24.000000 datasus_dbc-0.1.1/.github/workflows/CI.yml
--rw-r--r--   0     1001      127      686 2023-12-06 20:06:24.000000 datasus_dbc-0.1.1/.gitignore
--rw-r--r--   0     1001      127     1111 2023-12-06 20:06:24.000000 datasus_dbc-0.1.1/LISCENSE
--rw-r--r--   0     1001      127      910 2023-12-06 20:06:24.000000 datasus_dbc-0.1.1/README.md
--rw-r--r--   0     1001      127      236 2023-12-06 20:06:24.000000 datasus_dbc-0.1.1/datasus_dbc.pyi
--rw-r--r--   0     1001      127     1196 2023-12-06 20:06:24.000000 datasus_dbc-0.1.1/src/lib.rs
--rw-r--r--   0     1001      127     8090 2023-12-06 20:06:24.000000 datasus_dbc-0.1.1/Cargo.lock
--rw-r--r--   0     1001      127      718 2023-12-06 20:06:24.000000 datasus_dbc-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1546 1970-01-01 00:00:00.000000 datasus_dbc-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      502 1970-01-01 00:00:00.000000 datasus_dbc-0.1.2/Cargo.toml
+-rw-r--r--   0     1001      127     2825 2024-04-16 20:52:27.000000 datasus_dbc-0.1.2/.github/workflows/CI.yml
+-rw-r--r--   0     1001      127      686 2024-04-16 20:52:27.000000 datasus_dbc-0.1.2/.gitignore
+-rw-r--r--   0     1001      127     1111 2024-04-16 20:52:27.000000 datasus_dbc-0.1.2/LISCENSE
+-rw-r--r--   0     1001      127     1316 2024-04-16 20:52:27.000000 datasus_dbc-0.1.2/README.md
+-rw-r--r--   0     1001      127      236 2024-04-16 20:52:27.000000 datasus_dbc-0.1.2/datasus_dbc.pyi
+-rw-r--r--   0     1001      127     1196 2024-04-16 20:52:27.000000 datasus_dbc-0.1.2/src/lib.rs
+-rw-r--r--   0     1001      127     8090 2024-04-16 20:52:31.000000 datasus_dbc-0.1.2/Cargo.lock
+-rw-r--r--   0     1001      127      718 2024-04-16 20:52:27.000000 datasus_dbc-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1952 1970-01-01 00:00:00.000000 datasus_dbc-0.1.2/PKG-INFO
```

### Comparing `datasus_dbc-0.1.1/.github/workflows/CI.yml` & `datasus_dbc-0.1.2/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `datasus_dbc-0.1.1/.gitignore` & `datasus_dbc-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `datasus_dbc-0.1.1/LISCENSE` & `datasus_dbc-0.1.2/LISCENSE`

 * *Files identical despite different names*

### Comparing `datasus_dbc-0.1.1/README.md` & `datasus_dbc-0.1.2/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,28 +1,40 @@
 # datasus-dbc-py
 
+[![PyPI version](https://badge.fury.io/py/datasus-dbc.svg)](https://pypi.org/project/datasus-dbc/)
+
 Decompress `*.dbc` files usually found in Brazil's DATASUS ftp server into `*.dbf` files in python.
 
 This are python bindings of the sibling library [datasus-dbc](https://crates.io/crates/datasus-dbc) which is written in rust. This library should be **compatible with most platforms**.
 
+## Instalation
+
+```
+pip install datasus-dbc
+```
+
 ## Examples
 
-To decompress a `*.dbc` file into a `*.dbf` use `decompress` function:
+To decompress a `*.dbc` file into a `*.dbf` use the `decompress` function:
 
 ```python
 import datasus_dbc
 
-datasus_dbc.decompress("input.dbc", "output.dbc")
+datasus_dbc.decompress("input.dbc", "output.dbf")
 ```
 
 If you have a `*.dbc` file's raw bytes, you can use `decompress_bytes` to get the decompressed `*.dbf` raw bytes in memory:
 
 ```python
 import datasus_dbc
 
 with open("input.dbc", "rb") as file:
     dbf_bytes = datasus_dbc.decompress_bytes(file.read())
     print(dbf_bytes)
 ```
 
+## Reading *.dbf files
+
+This library does not support reading the contents of a `*.dbf` file, but you can still use one of the following libraries: [simpledbf](https://pypi.org/project/simpledbf/) or [dbfread](https://pypi.org/project/dbfread/1.0.6/).
+
 ## Found a bug?
 Feel free to create an [issue](https://github.com/mymatsubara/datasus-dbc-py/issues/new) here if you found a bug or if you want a new feature!
```

### Comparing `datasus_dbc-0.1.1/src/lib.rs` & `datasus_dbc-0.1.2/src/lib.rs`

 * *Files identical despite different names*

### Comparing `datasus_dbc-0.1.1/Cargo.lock` & `datasus_dbc-0.1.2/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 checksum = "6d271fe7d81346c0f41089c1427f3558dc31719a59a816b54ceb0f3667942e1a"
 dependencies = [
  "explode",
 ]
 
 [[package]]
 name = "datasus-dbc-py"
-version = "0.1.1"
+version = "0.1.2"
 dependencies = [
  "datasus-dbc",
  "pyo3",
 ]
 
 [[package]]
 name = "explode"
```

### Comparing `datasus_dbc-0.1.1/pyproject.toml` & `datasus_dbc-0.1.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `datasus_dbc-0.1.1/PKG-INFO` & `datasus_dbc-0.1.2/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: datasus-dbc
-Version: 0.1.1
+Version: 0.1.2
 Classifier: Programming Language :: Rust
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: System :: Archiving :: Compression
 Summary: Decompress DATASUS's dbc files into dbf files
 Keywords: dbc,dbf,datasus,compression,blast
 Author: Murilo Matsubara <murilo.matsubara@gmail.com>
@@ -12,33 +12,45 @@
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 Project-URL: Source, https://github.com/mymatsubara/datasus-dbc-py
 
 # datasus-dbc-py
 
+[![PyPI version](https://badge.fury.io/py/datasus-dbc.svg)](https://pypi.org/project/datasus-dbc/)
+
 Decompress `*.dbc` files usually found in Brazil's DATASUS ftp server into `*.dbf` files in python.
 
 This are python bindings of the sibling library [datasus-dbc](https://crates.io/crates/datasus-dbc) which is written in rust. This library should be **compatible with most platforms**.
 
+## Instalation
+
+```
+pip install datasus-dbc
+```
+
 ## Examples
 
-To decompress a `*.dbc` file into a `*.dbf` use `decompress` function:
+To decompress a `*.dbc` file into a `*.dbf` use the `decompress` function:
 
 ```python
 import datasus_dbc
 
-datasus_dbc.decompress("input.dbc", "output.dbc")
+datasus_dbc.decompress("input.dbc", "output.dbf")
 ```
 
 If you have a `*.dbc` file's raw bytes, you can use `decompress_bytes` to get the decompressed `*.dbf` raw bytes in memory:
 
 ```python
 import datasus_dbc
 
 with open("input.dbc", "rb") as file:
     dbf_bytes = datasus_dbc.decompress_bytes(file.read())
     print(dbf_bytes)
 ```
 
+## Reading *.dbf files
+
+This library does not support reading the contents of a `*.dbf` file, but you can still use one of the following libraries: [simpledbf](https://pypi.org/project/simpledbf/) or [dbfread](https://pypi.org/project/dbfread/1.0.6/).
+
 ## Found a bug?
 Feel free to create an [issue](https://github.com/mymatsubara/datasus-dbc-py/issues/new) here if you found a bug or if you want a new feature!
```

