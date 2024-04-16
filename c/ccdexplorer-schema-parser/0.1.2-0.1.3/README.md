# Comparing `tmp/ccdexplorer_schema_parser-0.1.2.tar.gz` & `tmp/ccdexplorer_schema_parser-0.1.3.tar.gz`

## Comparing `ccdexplorer_schema_parser-0.1.2.tar` & `ccdexplorer_schema_parser-0.1.3.tar`

### file list

```diff
@@ -1,11 +1,13 @@
--rw-r--r--   0        0        0      425 1970-01-01 00:00:00.000000 ccdexplorer_schema_parser-0.1.2/Cargo.toml
--rw-r--r--   0     1001      127        4 2024-04-16 09:07:34.000000 ccdexplorer_schema_parser-0.1.2/.dockerignore
--rw-r--r--   0     1001      127     2452 2024-04-16 09:07:34.000000 ccdexplorer_schema_parser-0.1.2/.github/workflows/CI.yml
--rw-r--r--   0     1001      127      690 2024-04-16 09:07:34.000000 ccdexplorer_schema_parser-0.1.2/.gitignore
--rw-r--r--   0     1001      127    11357 2024-04-16 09:07:34.000000 ccdexplorer_schema_parser-0.1.2/LICENSE.md
--rw-r--r--   0     1001      127     1421 2024-04-16 09:07:34.000000 ccdexplorer_schema_parser-0.1.2/README.md
--rw-r--r--   0     1001      127       10 2024-04-16 09:07:34.000000 ccdexplorer_schema_parser-0.1.2/requirements.txt
--rw-r--r--   0     1001      127     3672 2024-04-16 09:07:34.000000 ccdexplorer_schema_parser-0.1.2/src/lib.rs
--rw-r--r--   0     1001      127    50137 2024-04-16 09:07:41.000000 ccdexplorer_schema_parser-0.1.2/Cargo.lock
--rw-r--r--   0     1001      127      405 2024-04-16 09:07:34.000000 ccdexplorer_schema_parser-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1790 1970-01-01 00:00:00.000000 ccdexplorer_schema_parser-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0      425 1970-01-01 00:00:00.000000 ccdexplorer_schema_parser-0.1.3/Cargo.toml
+-rw-r--r--   0     1001      127        4 2024-04-16 09:55:17.000000 ccdexplorer_schema_parser-0.1.3/.dockerignore
+-rw-r--r--   0     1001      127     2452 2024-04-16 09:55:17.000000 ccdexplorer_schema_parser-0.1.3/.github/workflows/CI.yml
+-rw-r--r--   0     1001      127      690 2024-04-16 09:55:17.000000 ccdexplorer_schema_parser-0.1.3/.gitignore
+-rw-r--r--   0     1001      127    11357 2024-04-16 09:55:17.000000 ccdexplorer_schema_parser-0.1.3/LICENSE.md
+-rw-r--r--   0     1001      127        0 2024-04-16 09:55:17.000000 ccdexplorer_schema_parser-0.1.3/Parser/__init__.py
+-rw-r--r--   0     1001      127     1080 2024-04-16 09:55:17.000000 ccdexplorer_schema_parser-0.1.3/Parser/schema.py
+-rw-r--r--   0     1001      127     1421 2024-04-16 09:55:17.000000 ccdexplorer_schema_parser-0.1.3/README.md
+-rw-r--r--   0     1001      127       10 2024-04-16 09:55:17.000000 ccdexplorer_schema_parser-0.1.3/requirements.txt
+-rw-r--r--   0     1001      127     3672 2024-04-16 09:55:17.000000 ccdexplorer_schema_parser-0.1.3/src/lib.rs
+-rw-r--r--   0     1001      127    50137 2024-04-16 09:55:23.000000 ccdexplorer_schema_parser-0.1.3/Cargo.lock
+-rw-r--r--   0     1001      127      405 2024-04-16 09:55:17.000000 ccdexplorer_schema_parser-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1790 1970-01-01 00:00:00.000000 ccdexplorer_schema_parser-0.1.3/PKG-INFO
```

### Comparing `ccdexplorer_schema_parser-0.1.2/.github/workflows/CI.yml` & `ccdexplorer_schema_parser-0.1.3/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `ccdexplorer_schema_parser-0.1.2/.gitignore` & `ccdexplorer_schema_parser-0.1.3/.gitignore`

 * *Files identical despite different names*

### Comparing `ccdexplorer_schema_parser-0.1.2/LICENSE.md` & `ccdexplorer_schema_parser-0.1.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ccdexplorer_schema_parser-0.1.2/README.md` & `ccdexplorer_schema_parser-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `ccdexplorer_schema_parser-0.1.2/src/lib.rs` & `ccdexplorer_schema_parser-0.1.3/src/lib.rs`

 * *Files identical despite different names*

### Comparing `ccdexplorer_schema_parser-0.1.2/Cargo.lock` & `ccdexplorer_schema_parser-0.1.3/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -299,15 +299,15 @@
 name = "cc"
 version = "1.0.90"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8cd6604a82acf3039f1144f54b8eb34e91ffba622051189e71b781822d5ee1f5"
 
 [[package]]
 name = "ccdexplorer-schema-parser"
-version = "0.1.2"
+version = "0.1.3"
 dependencies = [
  "concordium-contracts-common",
  "concordium-smart-contract-engine",
  "concordium_base",
  "pyo3",
 ]
```

### Comparing `ccdexplorer_schema_parser-0.1.2/PKG-INFO` & `ccdexplorer_schema_parser-0.1.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: ccdexplorer-schema-parser
-Version: 0.1.2
+Version: 0.1.3
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE.md
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
```

