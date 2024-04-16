# Comparing `tmp/sentry_ophio-0.2.6.tar.gz` & `tmp/sentry_ophio-0.2.7.tar.gz`

## Comparing `sentry_ophio-0.2.6.tar` & `sentry_ophio-0.2.7.tar`

### file list

```diff
@@ -1,26 +1,30 @@
--rw-r--r--   0     1001      127      528 2024-03-27 09:32:32.000000 sentry_ophio-0.2.6/rust/Cargo.toml
--rw-r--r--   0     1001      127     2841 2024-03-27 09:32:32.000000 sentry_ophio-0.2.6/rust/benches/enhancers.rs
--rw-r--r--   0     1001      127    11734 2024-03-27 09:32:32.000000 sentry_ophio-0.2.6/rust/src/enhancers/actions.rs
--rw-r--r--   0     1001      127     4286 2024-03-27 09:32:32.000000 sentry_ophio-0.2.6/rust/src/enhancers/cache.rs
--rw-r--r--   0     1001      127     6596 2024-03-27 09:32:32.000000 sentry_ophio-0.2.6/rust/src/enhancers/config_structure.rs
--rw-r--r--   0     1001      127     1459 2024-03-27 09:32:32.000000 sentry_ophio-0.2.6/rust/src/enhancers/families.rs
--rw-r--r--   0     1001      127     3807 2024-03-27 09:32:32.000000 sentry_ophio-0.2.6/rust/src/enhancers/frame.rs
--rw-r--r--   0     1001      127    12775 2024-03-27 09:32:32.000000 sentry_ophio-0.2.6/rust/src/enhancers/grammar.rs
--rw-r--r--   0     1001      127    20908 2024-03-27 09:32:32.000000 sentry_ophio-0.2.6/rust/src/enhancers/matchers.rs
--rw-r--r--   0     1001      127    10578 2024-03-27 09:32:32.000000 sentry_ophio-0.2.6/rust/src/enhancers/mod.rs
--rw-r--r--   0     1001      127     4347 2024-03-27 09:32:32.000000 sentry_ophio-0.2.6/rust/src/enhancers/rules.rs
--rw-r--r--   0     1001      127       19 2024-03-27 09:32:32.000000 sentry_ophio-0.2.6/rust/src/lib.rs
--rw-r--r--   0        0        0      440 1970-01-01 00:00:00.000000 sentry_ophio-0.2.6/bindings/Cargo.toml
--rw-r--r--   0     1001      127     6193 2024-03-27 09:32:32.000000 sentry_ophio-0.2.6/bindings/src/enhancers.rs
--rw-r--r--   0     1001      127      419 2024-03-27 09:32:32.000000 sentry_ophio-0.2.6/bindings/src/lib.rs
--rw-r--r--   0     1001      127     2804 2024-03-27 09:32:32.000000 sentry_ophio-0.2.6/bindings/src/proguard.rs
--rw-r--r--   0     1001      127    31902 2024-03-27 09:32:32.000000 sentry_ophio-0.2.6/Cargo.lock
--rw-r--r--   0        0        0       79 1970-01-01 00:00:00.000000 sentry_ophio-0.2.6/Cargo.toml
--rw-r--r--   0     1001      127      724 2024-03-27 09:32:32.000000 sentry_ophio-0.2.6/pyproject.toml
--rw-r--r--   0     1001      127      129 2024-03-27 09:32:32.000000 sentry_ophio-0.2.6/python/sentry_ophio/proguard.py
--rw-r--r--   0     1001      127        0 2024-03-27 09:32:32.000000 sentry_ophio-0.2.6/python/sentry_ophio/__init__.py
--rw-r--r--   0     1001      127      203 2024-03-27 09:32:32.000000 sentry_ophio-0.2.6/python/sentry_ophio/enhancers.py
--rw-r--r--   0     1001      127        0 2024-03-27 09:32:32.000000 sentry_ophio-0.2.6/python/sentry_ophio/py.typed
--rw-r--r--   0     1001      127     3089 2024-03-27 09:32:32.000000 sentry_ophio-0.2.6/python/sentry_ophio/enhancers.pyi
--rw-r--r--   0     1001      127      582 2024-03-27 09:32:32.000000 sentry_ophio-0.2.6/python/sentry_ophio/proguard.pyi
--rw-r--r--   0        0        0      298 1970-01-01 00:00:00.000000 sentry_ophio-0.2.6/PKG-INFO
+-rw-r--r--   0     1001      127      583 2024-04-16 11:16:34.000000 sentry_ophio-0.2.7/rust/Cargo.toml
+-rw-r--r--   0     1001      127     2841 2024-04-16 11:16:34.000000 sentry_ophio-0.2.7/rust/benches/enhancers.rs
+-rw-r--r--   0     1001      127    11734 2024-04-16 11:16:34.000000 sentry_ophio-0.2.7/rust/src/enhancers/actions.rs
+-rw-r--r--   0     1001      127     4286 2024-04-16 11:16:35.000000 sentry_ophio-0.2.7/rust/src/enhancers/cache.rs
+-rw-r--r--   0     1001      127     6596 2024-04-16 11:16:35.000000 sentry_ophio-0.2.7/rust/src/enhancers/config_structure.rs
+-rw-r--r--   0     1001      127     1459 2024-04-16 11:16:35.000000 sentry_ophio-0.2.7/rust/src/enhancers/families.rs
+-rw-r--r--   0     1001      127     3807 2024-04-16 11:16:35.000000 sentry_ophio-0.2.7/rust/src/enhancers/frame.rs
+-rw-r--r--   0     1001      127    12775 2024-04-16 11:16:35.000000 sentry_ophio-0.2.7/rust/src/enhancers/grammar.rs
+-rw-r--r--   0     1001      127    20908 2024-04-16 11:16:35.000000 sentry_ophio-0.2.7/rust/src/enhancers/matchers.rs
+-rw-r--r--   0     1001      127    10578 2024-04-16 11:16:35.000000 sentry_ophio-0.2.7/rust/src/enhancers/mod.rs
+-rw-r--r--   0     1001      127     4347 2024-04-16 11:16:35.000000 sentry_ophio-0.2.7/rust/src/enhancers/rules.rs
+-rw-r--r--   0     1001      127     5369 2024-04-16 11:16:35.000000 sentry_ophio-0.2.7/rust/src/ketama.rs
+-rw-r--r--   0     1001      127       35 2024-04-16 11:16:35.000000 sentry_ophio-0.2.7/rust/src/lib.rs
+-rw-r--r--   0        0        0      440 1970-01-01 00:00:00.000000 sentry_ophio-0.2.7/bindings/Cargo.toml
+-rw-r--r--   0     1001      127     6193 2024-04-16 11:16:34.000000 sentry_ophio-0.2.7/bindings/src/enhancers.rs
+-rw-r--r--   0     1001      127      747 2024-04-16 11:16:34.000000 sentry_ophio-0.2.7/bindings/src/ketama.rs
+-rw-r--r--   0     1001      127      473 2024-04-16 11:16:34.000000 sentry_ophio-0.2.7/bindings/src/lib.rs
+-rw-r--r--   0     1001      127     2804 2024-04-16 11:16:34.000000 sentry_ophio-0.2.7/bindings/src/proguard.rs
+-rw-r--r--   0     1001      127    33332 2024-04-16 11:16:34.000000 sentry_ophio-0.2.7/Cargo.lock
+-rw-r--r--   0        0        0       79 1970-01-01 00:00:00.000000 sentry_ophio-0.2.7/Cargo.toml
+-rw-r--r--   0     1001      127      724 2024-04-16 11:16:34.000000 sentry_ophio-0.2.7/pyproject.toml
+-rw-r--r--   0     1001      127     3089 2024-04-16 11:16:34.000000 sentry_ophio-0.2.7/python/sentry_ophio/enhancers.pyi
+-rw-r--r--   0     1001      127       68 2024-04-16 11:16:34.000000 sentry_ophio-0.2.7/python/sentry_ophio/ketama.py
+-rw-r--r--   0     1001      127        0 2024-04-16 11:16:34.000000 sentry_ophio-0.2.7/python/sentry_ophio/__init__.py
+-rw-r--r--   0     1001      127      203 2024-04-16 11:16:34.000000 sentry_ophio-0.2.7/python/sentry_ophio/enhancers.py
+-rw-r--r--   0     1001      127      582 2024-04-16 11:16:34.000000 sentry_ophio-0.2.7/python/sentry_ophio/proguard.pyi
+-rw-r--r--   0     1001      127        0 2024-04-16 11:16:34.000000 sentry_ophio-0.2.7/python/sentry_ophio/py.typed
+-rw-r--r--   0     1001      127      607 2024-04-16 11:16:34.000000 sentry_ophio-0.2.7/python/sentry_ophio/ketama.pyi
+-rw-r--r--   0     1001      127      129 2024-04-16 11:16:34.000000 sentry_ophio-0.2.7/python/sentry_ophio/proguard.py
+-rw-r--r--   0        0        0      298 1970-01-01 00:00:00.000000 sentry_ophio-0.2.7/PKG-INFO
```

### Comparing `sentry_ophio-0.2.6/rust/Cargo.toml` & `sentry_ophio-0.2.7/rust/Cargo.toml`

 * *Files 7% similar despite different names*

```diff
@@ -5,16 +5,19 @@
 edition = "2021"
 
 [features]
 testing = ["dep:serde_json"]
 
 [dependencies]
 anyhow = "1.0.79"
+crc32fast = "1.4.0"
 globset = "0.4.14"
+indexmap = "2.2.6"
 lru = "0.12.1"
+md-5 = "0.10.6"
 regex = "1.10.2"
 rmp-serde = "1.1.2"
 serde = { version = "1.0.195", features = ["derive"] }
 serde_json = { version = "1.0.111", optional = true }
 smol_str = { version = "0.2.0", features = ["serde"] }
 
 [dev-dependencies]
```

### Comparing `sentry_ophio-0.2.6/rust/benches/enhancers.rs` & `sentry_ophio-0.2.7/rust/benches/enhancers.rs`

 * *Files identical despite different names*

### Comparing `sentry_ophio-0.2.6/rust/src/enhancers/actions.rs` & `sentry_ophio-0.2.7/rust/src/enhancers/actions.rs`

 * *Files identical despite different names*

### Comparing `sentry_ophio-0.2.6/rust/src/enhancers/cache.rs` & `sentry_ophio-0.2.7/rust/src/enhancers/cache.rs`

 * *Files identical despite different names*

### Comparing `sentry_ophio-0.2.6/rust/src/enhancers/config_structure.rs` & `sentry_ophio-0.2.7/rust/src/enhancers/config_structure.rs`

 * *Files identical despite different names*

### Comparing `sentry_ophio-0.2.6/rust/src/enhancers/families.rs` & `sentry_ophio-0.2.7/rust/src/enhancers/families.rs`

 * *Files identical despite different names*

### Comparing `sentry_ophio-0.2.6/rust/src/enhancers/frame.rs` & `sentry_ophio-0.2.7/rust/src/enhancers/frame.rs`

 * *Files identical despite different names*

### Comparing `sentry_ophio-0.2.6/rust/src/enhancers/grammar.rs` & `sentry_ophio-0.2.7/rust/src/enhancers/grammar.rs`

 * *Files identical despite different names*

### Comparing `sentry_ophio-0.2.6/rust/src/enhancers/matchers.rs` & `sentry_ophio-0.2.7/rust/src/enhancers/matchers.rs`

 * *Files identical despite different names*

### Comparing `sentry_ophio-0.2.6/rust/src/enhancers/mod.rs` & `sentry_ophio-0.2.7/rust/src/enhancers/mod.rs`

 * *Files identical despite different names*

### Comparing `sentry_ophio-0.2.6/rust/src/enhancers/rules.rs` & `sentry_ophio-0.2.7/rust/src/enhancers/rules.rs`

 * *Files identical despite different names*

### Comparing `sentry_ophio-0.2.6/bindings/src/enhancers.rs` & `sentry_ophio-0.2.7/bindings/src/enhancers.rs`

 * *Files identical despite different names*

### Comparing `sentry_ophio-0.2.6/bindings/src/proguard.rs` & `sentry_ophio-0.2.7/bindings/src/proguard.rs`

 * *Files identical despite different names*

### Comparing `sentry_ophio-0.2.6/Cargo.lock` & `sentry_ophio-0.2.7/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -74,14 +74,23 @@
 [[package]]
 name = "bitflags"
 version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "cf4b9d6a944f767f8e5e0db018570623c85f3d925ac718db4e06d0187adb21c1"
 
 [[package]]
+name = "block-buffer"
+version = "0.10.4"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3078c7629b62d3f0439517fa394996acacc5cbc91c5a20d8c658e77abd503a71"
+dependencies = [
+ "generic-array",
+]
+
+[[package]]
 name = "brownstone"
 version = "3.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c5839ee4f953e811bfdcf223f509cb2c6a3e1447959b0bff459405575bc17f22"
 dependencies = [
  "arrayvec",
 ]
@@ -152,24 +161,44 @@
 [[package]]
 name = "crossbeam-utils"
 version = "0.8.19"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "248e3bacc7dc6baa3b21e405ee045c3047101a49145e7e9eca583ab4c2ca5345"
 
 [[package]]
+name = "crypto-common"
+version = "0.1.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "1bfb12502f3fc46cca1bb51ac28df9d618d813cdc3d2f25b9fe775a34af26bb3"
+dependencies = [
+ "generic-array",
+ "typenum",
+]
+
+[[package]]
 name = "debugid"
 version = "0.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef552e6f588e446098f6ba40d89ac146c8c7b64aade83c051ee00bb5d2bc18d"
 dependencies = [
  "serde",
  "uuid",
 ]
 
 [[package]]
+name = "digest"
+version = "0.10.7"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9ed9a281f7bc9b7576e61468ba615a66a5c8cfdff42420a70aa82701a3b1e292"
+dependencies = [
+ "block-buffer",
+ "crypto-common",
+]
+
+[[package]]
 name = "divan"
 version = "0.1.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a0d567df2c9c2870a43f3f2bd65aaeb18dbce1c18f217c3e564b4fbaeb3ee56c"
 dependencies = [
  "cfg-if",
  "clap",
@@ -249,14 +278,24 @@
 checksum = "46303f565772937ffe1d394a4fac6f411c6013172fadde9dcdb1e147a086940e"
 dependencies = [
  "crc32fast",
  "miniz_oxide",
 ]
 
 [[package]]
+name = "generic-array"
+version = "0.14.7"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "85649ca51fd72272d7821adaf274ad91c288277713d9c18820d8499a7ff69e9a"
+dependencies = [
+ "typenum",
+ "version_check",
+]
+
+[[package]]
 name = "gimli"
 version = "0.28.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4271d37baee1b8c7e4b708028c57d816cf9d2434acb33a549475f78c181f6253"
 dependencies = [
  "fallible-iterator 0.3.0",
  "stable_deref_trait",
@@ -397,14 +436,24 @@
 [[package]]
 name = "maybe-owned"
 version = "0.3.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4facc753ae494aeb6e3c22f839b158aebd4f9270f55cd3c79906c45476c47ab4"
 
 [[package]]
+name = "md-5"
+version = "0.10.6"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d89e7ee0cfbedfc4da3340218492196241d89eefb6dab27de5df917a6d2e78cf"
+dependencies = [
+ "cfg-if",
+ "digest",
+]
+
+[[package]]
 name = "memchr"
 version = "2.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "523dc4f511e55ab87b694dc30d0f820d60906ef06413f93d4d7a1385599cc149"
 
 [[package]]
 name = "memmap2"
@@ -481,15 +530,15 @@
 name = "once_cell"
 version = "1.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3fdb12b2476b595f9358c5161aa467c2438859caa136dec86c26fdd2efe17b92"
 
 [[package]]
 name = "ophio-bindings"
-version = "0.2.6"
+version = "0.2.7"
 dependencies = [
  "anyhow",
  "proguard",
  "pyo3",
  "rust-ophio",
  "smol_str",
  "symbolic",
@@ -747,17 +796,20 @@
 ]
 
 [[package]]
 name = "rust-ophio"
 version = "0.0.0"
 dependencies = [
  "anyhow",
+ "crc32fast",
  "divan",
  "globset",
+ "indexmap",
  "lru",
+ "md-5",
  "regex",
  "rmp-serde",
  "serde",
  "serde_json",
  "smol_str",
 ]
 
@@ -1004,14 +1056,20 @@
 dependencies = [
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
+name = "typenum"
+version = "1.17.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "42ff0bf0c66b8238c6f3b578df37d0b7848e55df8577b3f74f92a69acceeb825"
+
+[[package]]
 name = "unicode-ident"
 version = "1.0.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3354b9ac3fae1ff6755cb6db53683adb661634f67557942dea4facebec0fee4b"
 
 [[package]]
 name = "unindent"
```

### Comparing `sentry_ophio-0.2.6/pyproject.toml` & `sentry_ophio-0.2.7/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sentry_ophio-0.2.6/python/sentry_ophio/enhancers.pyi` & `sentry_ophio-0.2.7/python/sentry_ophio/enhancers.pyi`

 * *Files identical despite different names*

### Comparing `sentry_ophio-0.2.6/python/sentry_ophio/proguard.pyi` & `sentry_ophio-0.2.7/python/sentry_ophio/proguard.pyi`

 * *Files identical despite different names*

