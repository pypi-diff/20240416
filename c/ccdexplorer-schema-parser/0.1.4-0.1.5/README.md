# Comparing `tmp/ccdexplorer_schema_parser-0.1.4.tar.gz` & `tmp/ccdexplorer_schema_parser-0.1.5.tar.gz`

## Comparing `ccdexplorer_schema_parser-0.1.4.tar` & `ccdexplorer_schema_parser-0.1.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0      425 1970-01-01 00:00:00.000000 ccdexplorer_schema_parser-0.1.4/Cargo.toml
--rw-r--r--   0     1001      127        4 2024-04-16 10:04:53.000000 ccdexplorer_schema_parser-0.1.4/.dockerignore
--rw-r--r--   0     1001      127     2452 2024-04-16 10:04:53.000000 ccdexplorer_schema_parser-0.1.4/.github/workflows/CI.yml
--rw-r--r--   0     1001      127      690 2024-04-16 10:04:53.000000 ccdexplorer_schema_parser-0.1.4/.gitignore
--rw-r--r--   0     1001      127    11357 2024-04-16 10:04:53.000000 ccdexplorer_schema_parser-0.1.4/LICENSE.md
--rw-r--r--   0     1001      127        0 2024-04-16 10:04:53.000000 ccdexplorer_schema_parser-0.1.4/Parser/__init__.py
--rw-r--r--   0     1001      127     1080 2024-04-16 10:04:53.000000 ccdexplorer_schema_parser-0.1.4/Parser/schema.py
--rw-r--r--   0     1001      127     1421 2024-04-16 10:04:53.000000 ccdexplorer_schema_parser-0.1.4/README.md
--rw-r--r--   0     1001      127       10 2024-04-16 10:04:53.000000 ccdexplorer_schema_parser-0.1.4/requirements.txt
--rw-r--r--   0     1001      127     3672 2024-04-16 10:04:53.000000 ccdexplorer_schema_parser-0.1.4/src/lib.rs
--rw-r--r--   0     1001      127    50137 2024-04-16 10:04:57.000000 ccdexplorer_schema_parser-0.1.4/Cargo.lock
--rw-r--r--   0     1001      127      442 2024-04-16 10:04:53.000000 ccdexplorer_schema_parser-0.1.4/pyproject.toml
--rw-r--r--   0        0        0     1790 1970-01-01 00:00:00.000000 ccdexplorer_schema_parser-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0      425 1970-01-01 00:00:00.000000 ccdexplorer_schema_parser-0.1.5/Cargo.toml
+-rw-r--r--   0     1001      127        4 2024-04-16 10:22:00.000000 ccdexplorer_schema_parser-0.1.5/.dockerignore
+-rw-r--r--   0     1001      127     2452 2024-04-16 10:22:00.000000 ccdexplorer_schema_parser-0.1.5/.github/workflows/CI.yml
+-rw-r--r--   0     1001      127      690 2024-04-16 10:22:00.000000 ccdexplorer_schema_parser-0.1.5/.gitignore
+-rw-r--r--   0     1001      127    11357 2024-04-16 10:22:00.000000 ccdexplorer_schema_parser-0.1.5/LICENSE.md
+-rw-r--r--   0     1001      127     1421 2024-04-16 10:22:00.000000 ccdexplorer_schema_parser-0.1.5/README.md
+-rw-r--r--   0     1001      127     1246 2024-04-16 10:22:00.000000 ccdexplorer_schema_parser-0.1.5/python/ccdexplorer_schema_parser/Schema.py
+-rw-r--r--   0     1001      127        0 2024-04-16 10:22:00.000000 ccdexplorer_schema_parser-0.1.5/python/ccdexplorer_schema_parser/__init__.py
+-rw-r--r--   0     1001      127       10 2024-04-16 10:22:00.000000 ccdexplorer_schema_parser-0.1.5/requirements.txt
+-rw-r--r--   0     1001      127     3672 2024-04-16 10:22:00.000000 ccdexplorer_schema_parser-0.1.5/src/lib.rs
+-rw-r--r--   0     1001      127    50137 2024-04-16 10:22:03.000000 ccdexplorer_schema_parser-0.1.5/Cargo.lock
+-rw-r--r--   0     1001      127      430 2024-04-16 10:22:00.000000 ccdexplorer_schema_parser-0.1.5/pyproject.toml
+-rw-r--r--   0        0        0     1790 1970-01-01 00:00:00.000000 ccdexplorer_schema_parser-0.1.5/PKG-INFO
```

### Comparing `ccdexplorer_schema_parser-0.1.4/.github/workflows/CI.yml` & `ccdexplorer_schema_parser-0.1.5/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `ccdexplorer_schema_parser-0.1.4/.gitignore` & `ccdexplorer_schema_parser-0.1.5/.gitignore`

 * *Files identical despite different names*

### Comparing `ccdexplorer_schema_parser-0.1.4/LICENSE.md` & `ccdexplorer_schema_parser-0.1.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ccdexplorer_schema_parser-0.1.4/Parser/schema.py` & `ccdexplorer_schema_parser-0.1.5/python/ccdexplorer_schema_parser/Schema.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,27 +1,31 @@
-from Parser import parser
+from ccdexplorer_schema_parser import ccdexplorer_schema_parser
 import json
 
 
 class Schema:
     def __init__(self, source, version=None):
         """Construct a new schema by extracting it from a module source. The
         module source can be either provided as a serialized versioned module,
         or a pair of a Wasm module together with a version (which can be either
         0 or 1). If the optional `version` argument is supplied then this
         assumes that the `source` is only the Wasm module.
 
         """
         if version is not None:
-            self.schema = parser.extract_schema_pair_ffi(version, source)
+            self.schema = ccdexplorer_schema_parser.extract_schema_pair_ffi(
+                version, source
+            )
         else:
-            self.schema = parser.extract_schema_ffi(source)
+            self.schema = ccdexplorer_schema_parser.extract_schema_ffi(source)
 
     def event_to_json(self, contractName, eventData):
-        response = parser.parse_event_ffi(self.schema, contractName, eventData)
+        response = ccdexplorer_schema_parser.parse_event_ffi(
+            self.schema, contractName, eventData
+        )
         return json.loads(response)
 
     def return_value_to_json(self, contractName, functionName, returnValueData):
-        response = parser.parse_return_value_ffi(
+        response = ccdexplorer_schema_parser.parse_return_value_ffi(
             self.schema, contractName, functionName, returnValueData
         )
         return json.loads(response)
```

### Comparing `ccdexplorer_schema_parser-0.1.4/README.md` & `ccdexplorer_schema_parser-0.1.5/README.md`

 * *Files identical despite different names*

### Comparing `ccdexplorer_schema_parser-0.1.4/src/lib.rs` & `ccdexplorer_schema_parser-0.1.5/src/lib.rs`

 * *Files identical despite different names*

### Comparing `ccdexplorer_schema_parser-0.1.4/Cargo.lock` & `ccdexplorer_schema_parser-0.1.5/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -299,15 +299,15 @@
 name = "cc"
 version = "1.0.90"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8cd6604a82acf3039f1144f54b8eb34e91ffba622051189e71b781822d5ee1f5"
 
 [[package]]
 name = "ccdexplorer-schema-parser"
-version = "0.1.4"
+version = "0.1.5"
 dependencies = [
  "concordium-contracts-common",
  "concordium-smart-contract-engine",
  "concordium_base",
  "pyo3",
 ]
```

### Comparing `ccdexplorer_schema_parser-0.1.4/PKG-INFO` & `ccdexplorer_schema_parser-0.1.5/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ccdexplorer-schema-parser
-Version: 0.1.4
+Version: 0.1.5
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE.md
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
```

