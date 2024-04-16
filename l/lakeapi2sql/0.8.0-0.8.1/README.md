# Comparing `tmp/lakeapi2sql-0.8.0.tar.gz` & `tmp/lakeapi2sql-0.8.1.tar.gz`

## Comparing `lakeapi2sql-0.8.0.tar` & `lakeapi2sql-0.8.1.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1420 1970-01-01 00:00:00.000000 lakeapi2sql-0.8.0/Cargo.toml
--rw-r--r--   0     1001      127      118 2023-11-21 06:51:29.000000 lakeapi2sql-0.8.0/.editorconfig
--rw-r--r--   0     1001      127     2966 2023-11-21 06:51:29.000000 lakeapi2sql-0.8.0/.github/workflows/CI.yml
--rw-r--r--   0     1001      127     3110 2023-11-21 06:51:29.000000 lakeapi2sql-0.8.0/.gitignore
--rw-r--r--   0     1001      127       76 2023-11-21 06:51:29.000000 lakeapi2sql-0.8.0/.vscode/settings.json
--rw-r--r--   0     1001      127     1081 2023-11-21 06:51:29.000000 lakeapi2sql-0.8.0/LICENSE
--rw-r--r--   0     1001      127     1388 2023-11-21 06:51:29.000000 lakeapi2sql-0.8.0/README.md
--rw-r--r--   0     1001      127        0 2023-11-21 06:51:29.000000 lakeapi2sql-0.8.0/lakeapi2sql/__init__.py
--rw-r--r--   0     1001      127     3102 2023-11-21 06:51:29.000000 lakeapi2sql-0.8.0/lakeapi2sql/bulk_insert.py
--rw-r--r--   0     1001      127        0 2023-11-21 06:51:29.000000 lakeapi2sql-0.8.0/py.typed
--rw-r--r--   0     1001      127    21563 2023-11-21 06:51:29.000000 lakeapi2sql-0.8.0/src/arrow_convert.rs
--rw-r--r--   0     1001      127     6809 2023-11-21 06:51:29.000000 lakeapi2sql-0.8.0/src/bulk_insert.rs
--rw-r--r--   0     1001      127     1519 2023-11-21 06:51:29.000000 lakeapi2sql-0.8.0/src/connect.rs
--rw-r--r--   0     1001      127     5190 2023-11-21 06:51:29.000000 lakeapi2sql-0.8.0/src/lib.rs
--rw-r--r--   0     1001      127        0 2023-11-21 06:51:29.000000 lakeapi2sql-0.8.0/test/__init__.py
--rw-r--r--   0     1001      127     1649 2023-11-21 06:51:29.000000 lakeapi2sql-0.8.0/test/test_insert.py
--rw-r--r--   0     1001      127     1663 2023-11-21 06:51:29.000000 lakeapi2sql-0.8.0/test/test_insert_reader.py
--rw-r--r--   0     1001      127    66860 2023-11-21 06:51:37.000000 lakeapi2sql-0.8.0/Cargo.lock
--rw-r--r--   0     1001      127      693 2023-11-21 06:51:29.000000 lakeapi2sql-0.8.0/pyproject.toml
--rw-r--r--   0        0        0     1852 1970-01-01 00:00:00.000000 lakeapi2sql-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1420 1970-01-01 00:00:00.000000 lakeapi2sql-0.8.1/Cargo.toml
+-rw-r--r--   0     1001      127      118 2024-04-16 07:04:28.000000 lakeapi2sql-0.8.1/.editorconfig
+-rw-r--r--   0     1001      127     2966 2024-04-16 07:04:28.000000 lakeapi2sql-0.8.1/.github/workflows/CI.yml
+-rw-r--r--   0     1001      127     3110 2024-04-16 07:04:28.000000 lakeapi2sql-0.8.1/.gitignore
+-rw-r--r--   0     1001      127       76 2024-04-16 07:04:28.000000 lakeapi2sql-0.8.1/.vscode/settings.json
+-rw-r--r--   0     1001      127     1081 2024-04-16 07:04:28.000000 lakeapi2sql-0.8.1/LICENSE
+-rw-r--r--   0     1001      127     1388 2024-04-16 07:04:28.000000 lakeapi2sql-0.8.1/README.md
+-rw-r--r--   0     1001      127        0 2024-04-16 07:04:28.000000 lakeapi2sql-0.8.1/lakeapi2sql/__init__.py
+-rw-r--r--   0     1001      127     3102 2024-04-16 07:04:28.000000 lakeapi2sql-0.8.1/lakeapi2sql/bulk_insert.py
+-rw-r--r--   0     1001      127        0 2024-04-16 07:04:28.000000 lakeapi2sql-0.8.1/py.typed
+-rw-r--r--   0     1001      127    21457 2024-04-16 07:04:28.000000 lakeapi2sql-0.8.1/src/arrow_convert.rs
+-rw-r--r--   0     1001      127     6809 2024-04-16 07:04:28.000000 lakeapi2sql-0.8.1/src/bulk_insert.rs
+-rw-r--r--   0     1001      127     1519 2024-04-16 07:04:28.000000 lakeapi2sql-0.8.1/src/connect.rs
+-rw-r--r--   0     1001      127     5190 2024-04-16 07:04:28.000000 lakeapi2sql-0.8.1/src/lib.rs
+-rw-r--r--   0     1001      127        0 2024-04-16 07:04:28.000000 lakeapi2sql-0.8.1/test/__init__.py
+-rw-r--r--   0     1001      127     1649 2024-04-16 07:04:28.000000 lakeapi2sql-0.8.1/test/test_insert.py
+-rw-r--r--   0     1001      127     1663 2024-04-16 07:04:28.000000 lakeapi2sql-0.8.1/test/test_insert_reader.py
+-rw-r--r--   0     1001      127    69760 2024-04-16 07:04:36.000000 lakeapi2sql-0.8.1/Cargo.lock
+-rw-r--r--   0     1001      127      693 2024-04-16 07:04:28.000000 lakeapi2sql-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0     1852 1970-01-01 00:00:00.000000 lakeapi2sql-0.8.1/PKG-INFO
```

### Comparing `lakeapi2sql-0.8.0/Cargo.toml` & `lakeapi2sql-0.8.1/Cargo.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "lake2sql"
-version = "0.7.6"
+version = "0.8.1"
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "lake2sql"
 crate-type = ["lib", "cdylib"]
```

### Comparing `lakeapi2sql-0.8.0/.github/workflows/CI.yml` & `lakeapi2sql-0.8.1/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `lakeapi2sql-0.8.0/.gitignore` & `lakeapi2sql-0.8.1/.gitignore`

 * *Files identical despite different names*

### Comparing `lakeapi2sql-0.8.0/LICENSE` & `lakeapi2sql-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `lakeapi2sql-0.8.0/README.md` & `lakeapi2sql-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `lakeapi2sql-0.8.0/lakeapi2sql/bulk_insert.py` & `lakeapi2sql-0.8.1/lakeapi2sql/bulk_insert.py`

 * *Files identical despite different names*

### Comparing `lakeapi2sql-0.8.0/src/arrow_convert.rs` & `lakeapi2sql-0.8.1/src/arrow_convert.rs`

 * *Files 1% similar despite different names*

```diff
@@ -147,18 +147,15 @@
                     token_rows[rowindex].push(ColumnData::String(match val {
                         Some(vs) => Some(Cow::from(vs)),
                         None => None,
                     }));
                     rowindex += 1;
                 }
             }
-            arrow::datatypes::DataType::Timestamp(
-                arrow::datatypes::TimeUnit::Millisecond,
-                None,
-            ) => {
+            arrow::datatypes::DataType::Timestamp(arrow::datatypes::TimeUnit::Millisecond, _) => {
                 let ba = col
                     .as_any()
                     .downcast_ref::<TimestampMillisecondArray>()
                     .unwrap();
 
                 let mut rowindex = 0;
                 for val in ba.iter() {
@@ -172,18 +169,15 @@
                             }
                         }
                         None => ColumnData::DateTime2(None),
                     });
                     rowindex += 1;
                 }
             }
-            arrow::datatypes::DataType::Timestamp(
-                arrow::datatypes::TimeUnit::Microsecond,
-                None,
-            ) => {
+            arrow::datatypes::DataType::Timestamp(arrow::datatypes::TimeUnit::Microsecond, _) => {
                 let ba = col
                     .as_any()
                     .downcast_ref::<TimestampMicrosecondArray>()
                     .unwrap();
 
                 let mut rowindex = 0;
                 for val in ba.iter() {
```

### Comparing `lakeapi2sql-0.8.0/src/bulk_insert.rs` & `lakeapi2sql-0.8.1/src/bulk_insert.rs`

 * *Files identical despite different names*

### Comparing `lakeapi2sql-0.8.0/src/connect.rs` & `lakeapi2sql-0.8.1/src/connect.rs`

 * *Files identical despite different names*

### Comparing `lakeapi2sql-0.8.0/src/lib.rs` & `lakeapi2sql-0.8.1/src/lib.rs`

 * *Files identical despite different names*

### Comparing `lakeapi2sql-0.8.0/test/test_insert.py` & `lakeapi2sql-0.8.1/test/test_insert.py`

 * *Files identical despite different names*

### Comparing `lakeapi2sql-0.8.0/test/test_insert_reader.py` & `lakeapi2sql-0.8.1/test/test_insert_reader.py`

 * *Files identical despite different names*

### Comparing `lakeapi2sql-0.8.0/Cargo.lock` & `lakeapi2sql-0.8.1/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -15,42 +15,42 @@
 name = "adler"
 version = "1.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f26201604c87b1e01bd3d98f8d5d9a8fcbb815e8cedb41ffccbeb4bf593a35fe"
 
 [[package]]
 name = "ahash"
-version = "0.7.7"
+version = "0.7.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5a824f2aa7e75a0c98c5a504fceb80649e9c35265d44525b5f94de4771a395cd"
+checksum = "891477e0c6a8957309ee5c45a6368af3ae14bb510732d2684ffa19af310920f9"
 dependencies = [
- "getrandom 0.2.11",
+ "getrandom 0.2.14",
  "once_cell",
  "version_check",
 ]
 
 [[package]]
 name = "ahash"
-version = "0.8.6"
+version = "0.8.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "91429305e9f0a25f6205c5b8e0d2db09e0708a7a6df0f42212bb56c32c8ac97a"
+checksum = "e89da841a80418a9b391ebaea17f5c112ffaaa96f621d2c285b5174da76b9011"
 dependencies = [
  "cfg-if",
  "const-random",
- "getrandom 0.2.11",
+ "getrandom 0.2.14",
  "once_cell",
  "version_check",
  "zerocopy",
 ]
 
 [[package]]
 name = "aho-corasick"
-version = "1.1.2"
+version = "1.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b2969dcb958b36655471fc61f7e416fa76033bdd4bfed0678d8fee1e2d07a1f0"
+checksum = "8e60d3430d3a69478ad0993f19238d2df97c507009a52b3c10addcd7f6bcb916"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "android-tzdata"
 version = "0.1.1"
@@ -64,31 +64,31 @@
 checksum = "819e7219dbd41043ac279b19830f2efc897156490d7fd6ea916720117ee66311"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "arc-swap"
-version = "1.6.0"
+version = "1.7.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bddcadddf5e9015d310179a59bb28c4d4b9920ad0f11e8e14dbadf654890c9a6"
+checksum = "69f7f8c3906b62b754cd5326047894316021dcfe5a194c8ea52bdd94934a3457"
 
 [[package]]
 name = "arrayvec"
 version = "0.7.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "96d30a06541fbafbc7f82ed10c06164cfbd2c401138f6addd8404629c4b16711"
 
 [[package]]
 name = "arrow"
 version = "48.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a8919668503a4f2d8b6da96fa7c16e93046bfb3412ffcfa1e5dc7d2e3adcb378"
 dependencies = [
- "ahash 0.8.6",
+ "ahash 0.8.11",
  "arrow-arith",
  "arrow-array",
  "arrow-buffer",
  "arrow-cast",
  "arrow-csv",
  "arrow-data",
  "arrow-ipc",
@@ -118,21 +118,21 @@
 
 [[package]]
 name = "arrow-array"
 version = "48.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d6eaf89041fa5937940ae390294ece29e1db584f46d995608d6e5fe65a2e0e9b"
 dependencies = [
- "ahash 0.8.6",
+ "ahash 0.8.11",
  "arrow-buffer",
  "arrow-data",
  "arrow-schema",
  "chrono",
  "half",
- "hashbrown 0.14.2",
+ "hashbrown 0.14.3",
  "num",
 ]
 
 [[package]]
 name = "arrow-buffer"
 version = "48.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
@@ -244,39 +244,39 @@
 
 [[package]]
 name = "arrow-row"
 version = "48.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a5d664318bc05f930559fc088888f0f7174d3c5bc888c0f4f9ae8f23aa398ba3"
 dependencies = [
- "ahash 0.8.6",
+ "ahash 0.8.11",
  "arrow-array",
  "arrow-buffer",
  "arrow-data",
  "arrow-schema",
  "half",
- "hashbrown 0.14.2",
+ "hashbrown 0.14.3",
 ]
 
 [[package]]
 name = "arrow-schema"
 version = "48.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "aaf4d737bba93da59f16129bec21e087aed0be84ff840e74146d4703879436cb"
 dependencies = [
- "bitflags 2.4.1",
+ "bitflags 2.5.0",
 ]
 
 [[package]]
 name = "arrow-select"
 version = "48.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "374c4c3b812ecc2118727b892252a4a4308f87a8aca1dbf09f3ce4bc578e668a"
 dependencies = [
- "ahash 0.8.6",
+ "ahash 0.8.11",
  "arrow-array",
  "arrow-buffer",
  "arrow-data",
  "arrow-schema",
  "num",
 ]
 
@@ -306,21 +306,21 @@
  "native-tls",
  "thiserror",
  "url",
 ]
 
 [[package]]
 name = "async-trait"
-version = "0.1.74"
+version = "0.1.80"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a66537f1bb974b254c98ed142ff995236e81b9d0fe4db0575f46612cb15eb0f9"
+checksum = "c6fa2087f2753a7da8cc1c0dbfcf89579dd57458e36769de5ac750b4671737ca"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.39",
+ "syn 2.0.59",
 ]
 
 [[package]]
 name = "asynchronous-codec"
 version = "0.6.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4057f2c32adbb2fc158e22fb38433c8e9bbf76b75a4732c7c0cbaf695fb65568"
@@ -330,50 +330,50 @@
  "futures-util",
  "memchr",
  "pin-project-lite",
 ]
 
 [[package]]
 name = "autocfg"
-version = "1.1.0"
+version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
+checksum = "f1fdabc7756949593fe60f30ec81974b613357de856987752631dea1e3394c80"
 
 [[package]]
 name = "backtrace"
-version = "0.3.69"
+version = "0.3.71"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2089b7e3f35b9dd2d0ed921ead4f6d318c27680d4a5bd167b3ee120edb105837"
+checksum = "26b05800d2e817c8b3b4b54abd461726265fa9789ae34330622f2db9ee696f9d"
 dependencies = [
  "addr2line",
  "cc",
  "cfg-if",
  "libc",
  "miniz_oxide",
  "object",
  "rustc-demangle",
 ]
 
 [[package]]
 name = "base64"
-version = "0.21.5"
+version = "0.21.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "35636a1494ede3b646cc98f74f8e62c773a38a659ebc777a2cf26b9b74171df9"
+checksum = "9d297deb1925b89f2ccc13d7635fa0714f12c87adce1c75356b39ca9b7178567"
 
 [[package]]
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
 name = "bitflags"
-version = "2.4.1"
+version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "327762f6e5a765692301e5bb513e0d9fef63be86bbc14528052b1cd3e6f03e07"
+checksum = "cf4b9d6a944f767f8e5e0db018570623c85f3d925ac718db4e06d0187adb21c1"
 
 [[package]]
 name = "bitvec"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1bc2832c24239b0141d5674bb9174f9d68a8b5b3f2753311927c172ca46f7e9c"
 dependencies = [
@@ -381,81 +381,81 @@
  "radium",
  "tap",
  "wyz",
 ]
 
 [[package]]
 name = "borsh"
-version = "1.2.0"
+version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bf617fabf5cdbdc92f774bfe5062d870f228b80056d41180797abf48bed4056e"
+checksum = "0901fc8eb0aca4c83be0106d6f2db17d86a08dfc2c25f0e84464bf381158add6"
 dependencies = [
  "borsh-derive",
  "cfg_aliases",
 ]
 
 [[package]]
 name = "borsh-derive"
-version = "1.2.0"
+version = "1.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f404657a7ea7b5249e36808dff544bc88a28f26e0ac40009f674b7a009d14be3"
+checksum = "51670c3aa053938b0ee3bd67c3817e471e626151131b934038e83c5bf8de48f5"
 dependencies = [
  "once_cell",
  "proc-macro-crate",
  "proc-macro2",
  "quote",
- "syn 2.0.39",
+ "syn 2.0.59",
  "syn_derive",
 ]
 
 [[package]]
 name = "bumpalo"
-version = "3.14.0"
+version = "3.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7f30e7476521f6f8af1a1c4c0b8cc94f0bee37d91763d0ca2665f299b6cd8aec"
+checksum = "79296716171880943b8470b5f8d03aa55eb2e645a4874bdbb28adb49162e012c"
 
 [[package]]
 name = "bytecheck"
-version = "0.6.11"
+version = "0.6.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8b6372023ac861f6e6dc89c8344a8f398fb42aaba2b5dbc649ca0c0e9dbcb627"
+checksum = "23cdc57ce23ac53c931e88a43d06d070a6fd142f2617be5855eb75efc9beb1c2"
 dependencies = [
  "bytecheck_derive",
  "ptr_meta",
  "simdutf8",
 ]
 
 [[package]]
 name = "bytecheck_derive"
-version = "0.6.11"
+version = "0.6.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a7ec4c6f261935ad534c0c22dbef2201b45918860eb1c574b972bd213a76af61"
+checksum = "3db406d29fbcd95542e92559bed4d8ad92636d1ca8b3b72ede10b4bcc010e659"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "byteorder"
 version = "1.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1fd0f2584146f6f2ef48085050886acf353beff7305ebd1ae69500e27c67f64b"
 
 [[package]]
 name = "bytes"
-version = "1.5.0"
+version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a2bd12c1caf447e69cd4528f47f94d203fd2582878ecb9e9465484c4148a8223"
+checksum = "514de17de45fdb8dc022b1a7975556c53c86f9f0aa5f534b98977b171857c2c9"
 
 [[package]]
 name = "cc"
-version = "1.0.83"
+version = "1.0.94"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f1174fb0b6ec23863f8b971027804a42614e347eafb0a95bf0b12cdae21fc4d0"
+checksum = "17f6e324229dc011159fcc089755d1e2e216a90d43a7dea6853ca740b84f35e7"
 dependencies = [
  "jobserver",
  "libc",
 ]
 
 [[package]]
 name = "cfg-if"
@@ -467,65 +467,65 @@
 name = "cfg_aliases"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fd16c4719339c4530435d38e511904438d07cce7950afa3718a84ac36c10e89e"
 
 [[package]]
 name = "chrono"
-version = "0.4.31"
+version = "0.4.38"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7f2c685bad3eb3d45a01354cedb7d5faa66194d1d58ba6e267a8de788f79db38"
+checksum = "a21f936df1771bf62b77f047b726c4625ff2e8aa607c01ec06e5a05bd8463401"
 dependencies = [
  "android-tzdata",
  "iana-time-zone",
  "num-traits",
- "windows-targets",
+ "windows-targets 0.52.5",
 ]
 
 [[package]]
 name = "connection-string"
 version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "510ca239cf13b7f8d16a2b48f263de7b4f8c566f0af58d901031473c76afb1e3"
 
 [[package]]
 name = "const-random"
-version = "0.1.17"
+version = "0.1.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5aaf16c9c2c612020bcfd042e170f6e32de9b9d75adb5277cdbbd2e2c8c8299a"
+checksum = "87e00182fe74b066627d63b85fd550ac2998d4b0bd86bfed477a0ae4c7c71359"
 dependencies = [
  "const-random-macro",
 ]
 
 [[package]]
 name = "const-random-macro"
 version = "0.1.16"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f9d839f2a20b0aee515dc581a6172f2321f96cab76c1a38a4c584a194955390e"
 dependencies = [
- "getrandom 0.2.11",
+ "getrandom 0.2.14",
  "once_cell",
  "tiny-keccak",
 ]
 
 [[package]]
 name = "core-foundation"
-version = "0.9.3"
+version = "0.9.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "194a7a9e6de53fa55116934067c844d9d749312f75c6f6d0980e8c252f8c2146"
+checksum = "91e195e091a93c46f7102ec7818a2aa394e1e1771c3ab4825963fa03e45afb8f"
 dependencies = [
  "core-foundation-sys",
  "libc",
 ]
 
 [[package]]
 name = "core-foundation-sys"
-version = "0.8.4"
+version = "0.8.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e496a50fda8aacccc86d7529e2c1e0892dbd0f898a6b5645b5561b89c3210efa"
+checksum = "06ea2b9bc92be3c2baa9334a323ebca2d6f074ff852cd1d7b11064035cd3868f"
 
 [[package]]
 name = "crunchy"
 version = "0.2.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7a81dae078cea95a014a339291cec439d2f232ebe854a9d672b796c6afafa9b7"
 
@@ -548,71 +548,71 @@
 checksum = "5efa2b3d7902f4b634a20cae3c9c4e6209dc4779feb6863329607560143efa70"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "deranged"
-version = "0.3.9"
+version = "0.3.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0f32d04922c60427da6f9fef14d042d9edddef64cb9d4ce0d64d0685fbeb1fd3"
+checksum = "b42b6fa04a440b495c8b04d0e71b707c585f83cb9cb28cf8cd0d976c315e31b4"
 dependencies = [
  "powerfmt",
 ]
 
 [[package]]
 name = "encoding_rs"
-version = "0.8.33"
+version = "0.8.34"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7268b386296a025e474d5140678f75d6de9493ae55a5d709eeb9dd08149945e1"
+checksum = "b45de904aa0b010bce2ab45264d0631681847fa7b6f2eaa7dab7619943bc4f59"
 dependencies = [
  "cfg-if",
 ]
 
 [[package]]
 name = "enumflags2"
-version = "0.7.8"
+version = "0.7.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5998b4f30320c9d93aed72f63af821bfdac50465b75428fce77b48ec482c3939"
+checksum = "3278c9d5fb675e0a51dabcf4c0d355f692b064171535ba72361be1528a9d8e8d"
 dependencies = [
  "enumflags2_derive",
 ]
 
 [[package]]
 name = "enumflags2_derive"
-version = "0.7.8"
+version = "0.7.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f95e2801cd355d4a1a3e3953ce6ee5ae9603a5c833455343a8bfe3f44d418246"
+checksum = "5c785274071b1b420972453b306eeca06acf4633829db4223b58a2a8c5953bc4"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.39",
+ "syn 2.0.59",
 ]
 
 [[package]]
 name = "equivalent"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5443807d6dff69373d433ab9ef5378ad8df50ca6298caf15de6e52e24aaf54d5"
 
 [[package]]
 name = "errno"
-version = "0.3.7"
+version = "0.3.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f258a7194e7f7c2a7837a8913aeab7fd8c383457034fa20ce4dd3dcb813e8eb8"
+checksum = "a258e46cdc063eb8519c00b9fc845fc47bcfca4130e2f08e88665ceda8474245"
 dependencies = [
  "libc",
- "windows-sys",
+ "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "fastrand"
-version = "2.0.1"
+version = "2.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "25cbce373ec4653f1a01a31e8a5e5ec0c622dc27ff9c4e6606eefef5cbbed4a5"
+checksum = "658bd65b1cf4c852a3cc96f18a8ce7b5640f6b703f905c7d74532294c2a63984"
 
 [[package]]
 name = "flatbuffers"
 version = "23.5.26"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4dac53e22462d78c16d64a1cd22371b54cc3fe94aa15e7886a2fa6e5d1ab8640"
 dependencies = [
@@ -639,103 +639,103 @@
 name = "foreign-types-shared"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "00b0228411908ca8685dba7fc2cdd70ec9990a6e753e89b6ac91a84c40fbaf4b"
 
 [[package]]
 name = "form_urlencoded"
-version = "1.2.0"
+version = "1.2.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a62bc1cf6f830c2ec14a513a9fb124d0a213a629668a4186f329db21fe045652"
+checksum = "e13624c2627564efccf4934284bdd98cbaa14e79b0b5a141218e507b3a823456"
 dependencies = [
  "percent-encoding",
 ]
 
 [[package]]
 name = "funty"
 version = "2.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e6d5a32815ae3f33302d95fdcb2ce17862f8c65363dcfd29360480ba1001fc9c"
 
 [[package]]
 name = "futures"
-version = "0.3.29"
+version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "da0290714b38af9b4a7b094b8a37086d1b4e61f2df9122c3cad2577669145335"
+checksum = "645c6916888f6cb6350d2550b80fb63e734897a8498abe35cfb732b6487804b0"
 dependencies = [
  "futures-channel",
  "futures-core",
  "futures-executor",
  "futures-io",
  "futures-sink",
  "futures-task",
  "futures-util",
 ]
 
 [[package]]
 name = "futures-channel"
-version = "0.3.29"
+version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ff4dd66668b557604244583e3e1e1eada8c5c2e96a6d0d6653ede395b78bbacb"
+checksum = "eac8f7d7865dcb88bd4373ab671c8cf4508703796caa2b1985a9ca867b3fcb78"
 dependencies = [
  "futures-core",
  "futures-sink",
 ]
 
 [[package]]
 name = "futures-core"
-version = "0.3.29"
+version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "eb1d22c66e66d9d72e1758f0bd7d4fd0bee04cad842ee34587d68c07e45d088c"
+checksum = "dfc6580bb841c5a68e9ef15c77ccc837b40a7504914d52e47b8b0e9bbda25a1d"
 
 [[package]]
 name = "futures-executor"
-version = "0.3.29"
+version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0f4fb8693db0cf099eadcca0efe2a5a22e4550f98ed16aba6c48700da29597bc"
+checksum = "a576fc72ae164fca6b9db127eaa9a9dda0d61316034f33a0a0d4eda41f02b01d"
 dependencies = [
  "futures-core",
  "futures-task",
  "futures-util",
 ]
 
 [[package]]
 name = "futures-io"
-version = "0.3.29"
+version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8bf34a163b5c4c52d0478a4d757da8fb65cabef42ba90515efee0f6f9fa45aaa"
+checksum = "a44623e20b9681a318efdd71c299b6b222ed6f231972bfe2f224ebad6311f0c1"
 
 [[package]]
 name = "futures-macro"
-version = "0.3.29"
+version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "53b153fd91e4b0147f4aced87be237c98248656bb01050b96bf3ee89220a8ddb"
+checksum = "87750cf4b7a4c0625b1529e4c543c2182106e4dedc60a2a6455e00d212c489ac"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.39",
+ "syn 2.0.59",
 ]
 
 [[package]]
 name = "futures-sink"
-version = "0.3.29"
+version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e36d3378ee38c2a36ad710c5d30c2911d752cb941c00c72dbabfb786a7970817"
+checksum = "9fb8e00e87438d937621c1c6269e53f536c14d3fbd6a042bb24879e57d474fb5"
 
 [[package]]
 name = "futures-task"
-version = "0.3.29"
+version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "efd193069b0ddadc69c46389b740bbccdd97203899b48d09c5f7969591d6bae2"
+checksum = "38d84fa142264698cdce1a9f9172cf383a0c82de1bddcf3092901442c4097004"
 
 [[package]]
 name = "futures-util"
-version = "0.3.29"
+version = "0.3.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a19526d624e703a3179b3d322efec918b6246ea0fa51d41124525f00f1cc8104"
+checksum = "3d6401deb83407ab3da39eba7e33987a73c3df0c82b4bb5813ee871c19c41d48"
 dependencies = [
  "futures-channel",
  "futures-core",
  "futures-io",
  "futures-macro",
  "futures-sink",
  "futures-task",
@@ -754,34 +754,34 @@
  "cfg-if",
  "libc",
  "wasi 0.9.0+wasi-snapshot-preview1",
 ]
 
 [[package]]
 name = "getrandom"
-version = "0.2.11"
+version = "0.2.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fe9006bed769170c11f845cf00c7c1e9092aeb3f268e007c3e760ac68008070f"
+checksum = "94b22e06ecb0110981051723910cbf0b5f5e09a2062dd7663334ee79a9d1286c"
 dependencies = [
  "cfg-if",
  "libc",
  "wasi 0.11.0+wasi-snapshot-preview1",
 ]
 
 [[package]]
 name = "gimli"
-version = "0.28.0"
+version = "0.28.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "6fb8d784f27acf97159b40fc4db5ecd8aa23b9ad5ef69cdd136d3bc80665f0c0"
+checksum = "4271d37baee1b8c7e4b708028c57d816cf9d2434acb33a549475f78c181f6253"
 
 [[package]]
 name = "h2"
-version = "0.3.22"
+version = "0.3.26"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4d6250322ef6e60f93f9a2162799302cd6f68f79f6e5d85c8c16f14d1d958178"
+checksum = "81fe527a889e1532da5c525686d96d4c2e74cdd345badf8dfef9f6b39dd5f5e8"
 dependencies = [
  "bytes",
  "fnv",
  "futures-core",
  "futures-sink",
  "futures-util",
  "http",
@@ -790,66 +790,66 @@
  "tokio",
  "tokio-util",
  "tracing",
 ]
 
 [[package]]
 name = "half"
-version = "2.3.1"
+version = "2.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bc52e53916c08643f1b56ec082790d1e86a32e58dc5268f897f313fbae7b4872"
+checksum = "6dd08c532ae367adf81c312a4580bc67f1d0fe8bc9c460520283f4c0ff277888"
 dependencies = [
  "cfg-if",
  "crunchy",
  "num-traits",
 ]
 
 [[package]]
 name = "hashbrown"
 version = "0.12.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8a9ee70c43aaf417c914396645a0fa852624801b24ebb7ae78fe8272889ac888"
 dependencies = [
- "ahash 0.7.7",
+ "ahash 0.7.8",
 ]
 
 [[package]]
 name = "hashbrown"
-version = "0.14.2"
+version = "0.14.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f93e7192158dbcda357bdec5fb5788eebf8bbac027f3f33e719d29135ae84156"
+checksum = "290f1a1d9242c78d09ce40a5e87e7554ee637af1351968159f4952f028f75604"
 
 [[package]]
 name = "heck"
 version = "0.4.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "95505c38b4572b2d910cecb0281560f54b440a19336cbbcb27bf6ce6adc6f5a8"
 
 [[package]]
 name = "hermit-abi"
-version = "0.3.3"
+version = "0.3.9"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d77f7ec81a6d05a3abb01ab6eb7590f6083d08449fe5a1c8b1e620283546ccb7"
+checksum = "d231dfb89cfffdbc30e7fc41579ed6066ad03abda9e567ccafae602b97ec5024"
 
 [[package]]
 name = "http"
-version = "0.2.11"
+version = "0.2.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8947b1a6fad4393052c7ba1f4cd97bed3e953a95c79c92ad9b051a04611d9fbb"
+checksum = "601cbb57e577e2f5ef5be8e7b83f0f63994f25aa94d673e54a92d5c516d101f1"
 dependencies = [
  "bytes",
  "fnv",
  "itoa",
 ]
 
 [[package]]
 name = "http-body"
-version = "0.4.5"
+version = "0.4.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d5f38f16d184e36f2408a55281cd658ecbd3ca05cce6d6510a176eca393e26d1"
+checksum = "7ceab25649e9960c0311ea418d17bee82c0dcec1bd053b5f9a66e265a693bed2"
 dependencies = [
  "bytes",
  "http",
  "pin-project-lite",
 ]
 
 [[package]]
@@ -862,30 +862,30 @@
 name = "httpdate"
 version = "1.0.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "df3b46402a9d5adb4c86a0cf463f42e19994e3ee891101b1841f30a545cb49a9"
 
 [[package]]
 name = "hyper"
-version = "0.14.27"
+version = "0.14.28"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ffb1cfd654a8219eaef89881fdb3bb3b1cdc5fa75ded05d6933b2b382e395468"
+checksum = "bf96e135eb83a2a8ddf766e426a841d8ddd7449d5f00d34ea02b41d2f19eef80"
 dependencies = [
  "bytes",
  "futures-channel",
  "futures-core",
  "futures-util",
  "h2",
  "http",
  "http-body",
  "httparse",
  "httpdate",
  "itoa",
  "pin-project-lite",
- "socket2 0.4.10",
+ "socket2",
  "tokio",
  "tower-service",
  "tracing",
  "want",
 ]
 
 [[package]]
@@ -913,17 +913,17 @@
  "native-tls",
  "tokio",
  "tokio-native-tls",
 ]
 
 [[package]]
 name = "iana-time-zone"
-version = "0.1.58"
+version = "0.1.60"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8326b86b6cff230b97d0d312a6c40a60726df3332e721f72a1b035f451663b20"
+checksum = "e7ffbb5a1b541ea2561f8c41c087286cc091e21e556a4f09a8f6cbf17b69b141"
 dependencies = [
  "android_system_properties",
  "core-foundation-sys",
  "iana-time-zone-haiku",
  "js-sys",
  "wasm-bindgen",
  "windows-core",
@@ -936,71 +936,71 @@
 checksum = "f31827a206f56af32e590ba56d5d2d085f558508192593743f16b2306495269f"
 dependencies = [
  "cc",
 ]
 
 [[package]]
 name = "idna"
-version = "0.4.0"
+version = "0.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7d20d6b07bfbc108882d88ed8e37d39636dcc260e15e30c45e6ba089610b917c"
+checksum = "634d9b1461af396cad843f47fdba5597a4f9e6ddd4bfb6ff5d85028c25cb12f6"
 dependencies = [
  "unicode-bidi",
  "unicode-normalization",
 ]
 
 [[package]]
 name = "indexmap"
-version = "2.1.0"
+version = "2.2.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d530e1a18b1cb4c484e6e34556a0d948706958449fca0cab753d649f2bce3d1f"
+checksum = "168fb715dda47215e360912c096649d23d58bf392ac62f73919e831745e40f26"
 dependencies = [
  "equivalent",
- "hashbrown 0.14.2",
+ "hashbrown 0.14.3",
 ]
 
 [[package]]
 name = "indoc"
-version = "2.0.4"
+version = "2.0.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1e186cfbae8084e513daff4240b4797e342f988cecda4fb6c939150f96315fd8"
+checksum = "b248f5224d1d606005e02c97f5aa4e88eeb230488bcc03bc9ca4d7991399f2b5"
 
 [[package]]
 name = "ipnet"
 version = "2.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8f518f335dce6725a761382244631d86cf0ccb2863413590b31338feb467f9c3"
 
 [[package]]
 name = "itoa"
-version = "1.0.9"
+version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "af150ab688ff2122fcef229be89cb50dd66af9e01a4ff320cc137eecc9bacc38"
+checksum = "49f1f14873335454500d59611f1cf4a4b0f786f9ac11f4312a78e4cf2566695b"
 
 [[package]]
 name = "jobserver"
-version = "0.1.27"
+version = "0.1.30"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8c37f63953c4c63420ed5fd3d6d398c719489b9f872b9fa683262f8edd363c7d"
+checksum = "685a7d121ee3f65ae4fddd72b25a04bb36b6af81bc0828f7d5434c0fe60fa3a2"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "js-sys"
-version = "0.3.65"
+version = "0.3.69"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "54c0c35952f67de54bb584e9fd912b3023117cbafc0a77d8f3dee1fb5f572fe8"
+checksum = "29c15563dc2726973df627357ce0c9ddddbea194836909d655df6a75d2cf296d"
 dependencies = [
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "lake2sql"
-version = "0.7.6"
+version = "0.8.1"
 dependencies = [
  "arrow",
  "futures",
  "log",
  "pyo3",
  "pyo3-asyncio",
  "pyo3-log",
@@ -1080,100 +1080,100 @@
 dependencies = [
  "lexical-util",
  "static_assertions",
 ]
 
 [[package]]
 name = "libc"
-version = "0.2.150"
+version = "0.2.153"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "89d92a4743f9a61002fae18374ed11e7973f530cb3a3255fb354818118b2203c"
+checksum = "9c198f91728a82281a64e1f4f9eeb25d82cb32a5de251c6bd1b5154d63a8e7bd"
 
 [[package]]
 name = "libm"
 version = "0.2.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4ec2a862134d2a7d32d7983ddcdd1c4923530833c9f2ea1a44fc5fa473989058"
 
 [[package]]
 name = "linux-raw-sys"
-version = "0.4.11"
+version = "0.4.13"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "969488b55f8ac402214f3f5fd243ebb7206cf82de60d3172994707a4bcc2b829"
+checksum = "01cda141df6706de531b6c46c3a33ecca755538219bd484262fa09410c13539c"
 
 [[package]]
 name = "lock_api"
 version = "0.4.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3c168f8615b12bc01f9c17e2eb0cc07dcae1940121185446edc3744920e8ef45"
 dependencies = [
  "autocfg",
  "scopeguard",
 ]
 
 [[package]]
 name = "log"
-version = "0.4.20"
+version = "0.4.21"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b5e6163cb8c49088c2c36f57875e58ccd8c87c7427f7fbd50ea6710b2f3f2e8f"
+checksum = "90ed8c1e510134f979dbc4f070f87d4313098b704861a105fe34231c70a3901c"
 
 [[package]]
 name = "lz4_flex"
-version = "0.11.1"
+version = "0.11.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3ea9b256699eda7b0387ffbc776dd625e28bde3918446381781245b7a50349d8"
+checksum = "75761162ae2b0e580d7e7c390558127e5f01b4194debd6221fd8c207fc80e3f5"
 dependencies = [
  "twox-hash",
 ]
 
 [[package]]
 name = "md5"
 version = "0.6.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7e6bcd6433cff03a4bfc3d9834d504467db1f1cf6d0ea765d37d330249ed629d"
 
 [[package]]
 name = "memchr"
-version = "2.6.4"
+version = "2.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f665ee40bc4a3c5590afb1e9677db74a508659dfd71e126420da8274909a0167"
+checksum = "6c8640c5d730cb13ebd907d8d04b52f55ac9a2eec55b440c8892f40d56c76c1d"
 
 [[package]]
 name = "memoffset"
-version = "0.9.0"
+version = "0.9.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5a634b1c61a95585bd15607c6ab0c4e5b226e695ff2800ba0cdccddf208c406c"
+checksum = "488016bfae457b036d996092f6cb448677611ce4449e970ceaf42695203f218a"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "mime"
 version = "0.3.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6877bb514081ee2a7ff5ef9de3281f14a4dd4bceac4c09388074a6b5df8a139a"
 
 [[package]]
 name = "miniz_oxide"
-version = "0.7.1"
+version = "0.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e7810e0be55b428ada41041c41f32c9f1a42817901b4ccf45fa3d4b6561e74c7"
+checksum = "9d811f3e15f28568be3407c8e7fdb6514c1cda3cb30683f15b6a1a1dc4ea14a7"
 dependencies = [
  "adler",
 ]
 
 [[package]]
 name = "mio"
-version = "0.8.9"
+version = "0.8.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3dce281c5e46beae905d4de1870d8b1509a9142b62eedf18b443b011ca8343d0"
+checksum = "a4a650543ca06a924e8b371db273b2756685faae30f8487da1b56505a8f78b0c"
 dependencies = [
  "libc",
  "wasi 0.11.0+wasi-snapshot-preview1",
- "windows-sys",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "native-tls"
 version = "0.2.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "07226173c32f2926027b63cce4bcd8076c3552846cbe7925f3aaffeac0a3b92e"
@@ -1188,17 +1188,17 @@
  "security-framework",
  "security-framework-sys",
  "tempfile",
 ]
 
 [[package]]
 name = "num"
-version = "0.4.1"
+version = "0.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b05180d69e3da0e530ba2a1dae5110317e49e3b7f3d41be227dc5f92e49ee7af"
+checksum = "3135b08af27d103b0a51f2ae0f8632117b7b185ccf931445affa8df530576a41"
 dependencies = [
  "num-bigint",
  "num-complex",
  "num-integer",
  "num-iter",
  "num-rational",
  "num-traits",
@@ -1213,36 +1213,41 @@
  "autocfg",
  "num-integer",
  "num-traits",
 ]
 
 [[package]]
 name = "num-complex"
-version = "0.4.4"
+version = "0.4.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1ba157ca0885411de85d6ca030ba7e2a83a28636056c7c699b07c8b6f7383214"
+checksum = "23c6602fda94a57c990fe0df199a035d83576b496aa29f4e634a8ac6004e68a6"
 dependencies = [
  "num-traits",
 ]
 
 [[package]]
+name = "num-conv"
+version = "0.1.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "51d515d32fb182ee37cda2ccdcb92950d6a3c2893aa280e540671c2cd0f3b1d9"
+
+[[package]]
 name = "num-integer"
-version = "0.1.45"
+version = "0.1.46"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "225d3389fb3509a24c93f5c29eb6bde2586b98d9f016636dff58d7c6f7569cd9"
+checksum = "7969661fd2958a5cb096e56c8e1ad0444ac2bbcd0061bd28660485a44879858f"
 dependencies = [
- "autocfg",
  "num-traits",
 ]
 
 [[package]]
 name = "num-iter"
-version = "0.1.43"
+version = "0.1.44"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7d03e6c028c5dc5cac6e2dec0efda81fc887605bb3d884578bb6d6bf7514e252"
+checksum = "d869c01cc0c455284163fd0092f1f93835385ccab5a98a0dcc497b2f8bf055a9"
 dependencies = [
  "autocfg",
  "num-integer",
  "num-traits",
 ]
 
 [[package]]
@@ -1255,17 +1260,17 @@
  "num-bigint",
  "num-integer",
  "num-traits",
 ]
 
 [[package]]
 name = "num-traits"
-version = "0.2.17"
+version = "0.2.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "39e3200413f237f41ab11ad6d161bc7239c84dcb631773ccd7de3dfe4b5c267c"
+checksum = "da0df0e5185db44f69b44f26786fe401b6c293d1907744beaa7fa62b2e5a517a"
 dependencies = [
  "autocfg",
  "libm",
 ]
 
 [[package]]
 name = "num_cpus"
@@ -1275,34 +1280,34 @@
 dependencies = [
  "hermit-abi",
  "libc",
 ]
 
 [[package]]
 name = "object"
-version = "0.32.1"
+version = "0.32.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9cf5f9dd3933bd50a9e1f149ec995f39ae2c496d31fd772c1fd45ebc27e902b0"
+checksum = "a6a622008b6e321afc04970976f62ee297fdbaa6f95318ca343e3eebb9648441"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "once_cell"
-version = "1.18.0"
+version = "1.19.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dd8b5dd2ae5ed71462c540258bedcb51965123ad7e7ccf4b9a8cafaa4a63576d"
+checksum = "3fdb12b2476b595f9358c5161aa467c2438859caa136dec86c26fdd2efe17b92"
 
 [[package]]
 name = "openssl"
-version = "0.10.59"
+version = "0.10.64"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7a257ad03cd8fb16ad4172fedf8094451e1af1c4b70097636ef2eac9a5f0cc33"
+checksum = "95a0481286a310808298130d22dd1fef0fa571e05a8f44ec801801e84b216b1f"
 dependencies = [
- "bitflags 2.4.1",
+ "bitflags 2.5.0",
  "cfg-if",
  "foreign-types",
  "libc",
  "once_cell",
  "openssl-macros",
  "openssl-sys",
 ]
@@ -1311,28 +1316,28 @@
 name = "openssl-macros"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a948666b637a0f465e8564c73e89d4dde00d72d4d473cc972f390fc3dcee7d9c"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.39",
+ "syn 2.0.59",
 ]
 
 [[package]]
 name = "openssl-probe"
 version = "0.1.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ff011a302c396a5197692431fc1948019154afc178baf7d8e37367442a4601cf"
 
 [[package]]
 name = "openssl-sys"
-version = "0.9.95"
+version = "0.9.102"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "40a4130519a360279579c2053038317e40eff64d13fd3f004f9e1b72b8a6aaf9"
+checksum = "c597637d56fbc83893a35eb0dd04b2b8e7a50c91e64e9493e398b5df4fb45fa2"
 dependencies = [
  "cc",
  "libc",
  "pkg-config",
  "vcpkg",
 ]
 
@@ -1352,40 +1357,46 @@
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "4c42a9226546d68acdd9c0a280d17ce19bfe27a46bf68784e4066115788d008e"
 dependencies = [
  "cfg-if",
  "libc",
  "redox_syscall",
  "smallvec",
- "windows-targets",
+ "windows-targets 0.48.5",
 ]
 
 [[package]]
 name = "percent-encoding"
-version = "2.3.0"
+version = "2.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9b2a4787296e9989611394c33f193f676704af1686e70b8f8033ab5ba9a35a94"
+checksum = "e3148f5046208a5d56bcfc03053e3ca6334e51da8dfb19b6cdc8b306fae3283e"
 
 [[package]]
 name = "pin-project-lite"
-version = "0.2.13"
+version = "0.2.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8afb450f006bf6385ca15ef45d71d2288452bc3683ce2e2cacc0d18e4be60b58"
+checksum = "bda66fc9667c18cb2758a2ac84d1167245054bcf85d5d1aaa6923f45801bdd02"
 
 [[package]]
 name = "pin-utils"
 version = "0.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8b870d8c151b6f2fb93e84a13146138f05d02ed11c7e7c54f8826aaaf7c9f184"
 
 [[package]]
 name = "pkg-config"
-version = "0.3.27"
+version = "0.3.30"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "d231b230927b5e4ad203db57bbcbee2802f6bce620b1e4a9024a07d94e2907ec"
+
+[[package]]
+name = "portable-atomic"
+version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "26072860ba924cbfa98ea39c8c19b4dd6a4a25423dbdf219c1eca91aa0cf6964"
+checksum = "7170ef9988bc169ba16dd36a7fa041e5c4cbeb6a35b76d4c03daded371eae7c0"
 
 [[package]]
 name = "powerfmt"
 version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "439ee305def115ba05938db6eb1644ff94165c5ab5e9420d1c1bcedbba909391"
 
@@ -1399,17 +1410,17 @@
 name = "pretty-hex"
 version = "0.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c6fa0831dd7cc608c38a5e323422a0077678fa5744aa2be4ad91c4ece8eec8d5"
 
 [[package]]
 name = "proc-macro-crate"
-version = "2.0.0"
+version = "3.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7e8366a6159044a37876a2b9817124296703c586a5c92e2c53751fa06d8d43e8"
+checksum = "6d37c51ca738a55da99dc0c4a34860fd675453b8b36209178c2249bb13651284"
 dependencies = [
  "toml_edit",
 ]
 
 [[package]]
 name = "proc-macro-error"
 version = "1.0.4"
@@ -1431,17 +1442,17 @@
  "proc-macro2",
  "quote",
  "version_check",
 ]
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.69"
+version = "1.0.80"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "134c189feb4956b20f6f547d2cf727d4c0fe06722b20a0eec87ed445a97f92da"
+checksum = "a56dea16b0a29e94408b9aa5e2940a4eedbd128a1ba20e8f7ae60fd3d465af0e"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "ptr_meta"
 version = "0.1.4"
@@ -1460,23 +1471,24 @@
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.20.0"
+version = "0.20.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "04e8453b658fe480c3e70c8ed4e3d3ec33eb74988bd186561b0cc66b85c3bc4b"
+checksum = "53bdbb96d49157e65d45cc287af5f32ffadd5f4761438b527b055fb0d4bb8233"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
  "memoffset",
  "parking_lot",
+ "portable-atomic",
  "pyo3-build-config",
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
@@ -1502,27 +1514,27 @@
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.20.0"
+version = "0.20.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a96fe70b176a89cff78f2fa7b3c930081e163d5379b4dcdf993e3ae29ca662e5"
+checksum = "deaa5745de3f5231ce10517a1f5dd97d53e5a2fd77aa6b5842292085831d48d7"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.20.0"
+version = "0.20.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "214929900fd25e6604661ed9cf349727c8920d47deff196c4e28165a6ef2a96b"
+checksum = "62b42531d03e08d4ef1f6e85a2ed422eb678b8cd62b762e53891c05faf0d4afa"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-log"
@@ -1533,41 +1545,42 @@
  "arc-swap",
  "log",
  "pyo3",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.20.0"
+version = "0.20.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dac53072f717aa1bfa4db832b39de8c875b7c7af4f4a6fe93cdbf9264cf8383b"
+checksum = "7305c720fa01b8055ec95e484a6eca7a83c841267f0dd5280f0c8b8551d2c158"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
- "syn 2.0.39",
+ "syn 2.0.59",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.20.0"
+version = "0.20.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7774b5a8282bd4f25f803b1f0d945120be959a36c72e08e7cd031c792fdfd424"
+checksum = "7c7e9b68bb9c3149c5b0cade5d07f953d6d125eb4337723c4ccdb665f1f96185"
 dependencies = [
  "heck",
  "proc-macro2",
+ "pyo3-build-config",
  "quote",
- "syn 2.0.39",
+ "syn 2.0.59",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.33"
+version = "1.0.36"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5267fca4496028628a95160fc423a33e8b2e6af8a5302579e322e4b520293cae"
+checksum = "0fa76aaf39101c457836aec0ce2316dbdc3ab723cdda1c6bd4e6ad4208acaca7"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "radium"
 version = "0.7.0"
@@ -1629,15 +1642,15 @@
 
 [[package]]
 name = "rand_core"
 version = "0.6.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ec0be4795e2f6a28069bec0b5ff3e2ac9bafc99e6a9a7dc3547996c5c816922c"
 dependencies = [
- "getrandom 0.2.11",
+ "getrandom 0.2.14",
 ]
 
 [[package]]
 name = "rand_hc"
 version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ca3129af7b92a17112d59ad498c6f81eaf463253766b90396d39ea7a39d6613c"
@@ -1652,55 +1665,55 @@
 checksum = "4722d768eff46b75989dd134e5c353f0d6296e5aaa3132e776cbdb56be7731aa"
 dependencies = [
  "bitflags 1.3.2",
 ]
 
 [[package]]
 name = "regex"
-version = "1.10.2"
+version = "1.10.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "380b951a9c5e80ddfd6136919eef32310721aa4aacd4889a8d39124b026ab343"
+checksum = "c117dbdfde9c8308975b6a18d71f3f385c89461f7b3fb054288ecf2a2058ba4c"
 dependencies = [
  "aho-corasick",
  "memchr",
  "regex-automata",
  "regex-syntax",
 ]
 
 [[package]]
 name = "regex-automata"
-version = "0.4.3"
+version = "0.4.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5f804c7828047e88b2d32e2d7fe5a105da8ee3264f01902f796c8e067dc2483f"
+checksum = "86b83b8b9847f9bf95ef68afb0b8e6cdb80f498442f5179a29fad448fcc1eaea"
 dependencies = [
  "aho-corasick",
  "memchr",
  "regex-syntax",
 ]
 
 [[package]]
 name = "regex-syntax"
-version = "0.8.2"
+version = "0.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c08c74e62047bb2de4ff487b251e4a92e24f48745648451635cec7d591162d9f"
+checksum = "adad44e29e4c806119491a7f06f03de4d1af22c3a680dd47f1e6e179439d1f56"
 
 [[package]]
 name = "rend"
-version = "0.4.1"
+version = "0.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "a2571463863a6bd50c32f94402933f03457a3fbaf697a707c5be741e459f08fd"
+checksum = "71fe3824f5629716b1589be05dacd749f6aa084c87e00e016714a8cdfccc997c"
 dependencies = [
  "bytecheck",
 ]
 
 [[package]]
 name = "reqwest"
-version = "0.11.22"
+version = "0.11.27"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "046cd98826c46c2ac8ddecae268eb5c2e58628688a5fc7a2643704a73faba95b"
+checksum = "dd67538700a17451e7cba03ac727fb961abb7607553461627b97de0b89cf4a62"
 dependencies = [
  "base64",
  "bytes",
  "encoding_rs",
  "futures-core",
  "futures-util",
  "h2",
@@ -1719,14 +1732,15 @@
  "pin-project-lite",
  "rustls",
  "rustls-native-certs",
  "rustls-pemfile",
  "serde",
  "serde_json",
  "serde_urlencoded",
+ "sync_wrapper",
  "system-configuration",
  "tokio",
  "tokio-native-tls",
  "tokio-rustls",
  "tokio-util",
  "tower-service",
  "url",
@@ -1735,59 +1749,61 @@
  "wasm-streams",
  "web-sys",
  "winreg",
 ]
 
 [[package]]
 name = "ring"
-version = "0.17.5"
+version = "0.17.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fb0205304757e5d899b9c2e448b867ffd03ae7f988002e47cd24954391394d0b"
+checksum = "c17fa4cb658e3583423e915b9f3acc01cceaee1860e33d59ebae66adc3a2dc0d"
 dependencies = [
  "cc",
- "getrandom 0.2.11",
+ "cfg-if",
+ "getrandom 0.2.14",
  "libc",
  "spin",
  "untrusted",
- "windows-sys",
+ "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "rkyv"
-version = "0.7.42"
+version = "0.7.44"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0200c8230b013893c0b2d6213d6ec64ed2b9be2e0e016682b7224ff82cff5c58"
+checksum = "5cba464629b3394fc4dbc6f940ff8f5b4ff5c7aef40f29166fd4ad12acbc99c0"
 dependencies = [
  "bitvec",
  "bytecheck",
+ "bytes",
  "hashbrown 0.12.3",
  "ptr_meta",
  "rend",
  "rkyv_derive",
  "seahash",
  "tinyvec",
  "uuid",
 ]
 
 [[package]]
 name = "rkyv_derive"
-version = "0.7.42"
+version = "0.7.44"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b2e06b915b5c230a17d7a736d1e2e63ee753c256a8614ef3f5147b13a4f5541d"
+checksum = "a7dddfff8de25e6f62b9d64e6e432bf1c6736c57d20323e15ee10435fbda7c65"
 dependencies = [
  "proc-macro2",
  "quote",
  "syn 1.0.109",
 ]
 
 [[package]]
 name = "rust_decimal"
-version = "1.33.1"
+version = "1.35.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "06676aec5ccb8fc1da723cc8c0f9a46549f21ebb8753d3915c6c41db1e7f1dc4"
+checksum = "1790d1c4c0ca81211399e0e0af16333276f375209e71a37b67698a373db5b47a"
 dependencies = [
  "arrayvec",
  "borsh",
  "bytes",
  "num-traits",
  "rand 0.8.5",
  "rkyv",
@@ -1808,30 +1824,30 @@
 checksum = "bfa0f585226d2e68097d4f95d113b15b83a82e819ab25717ec0590d9584ef366"
 dependencies = [
  "semver",
 ]
 
 [[package]]
 name = "rustix"
-version = "0.38.25"
+version = "0.38.32"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dc99bc2d4f1fed22595588a013687477aedf3cdcfb26558c559edb67b4d9b22e"
+checksum = "65e04861e65f21776e67888bfbea442b3642beaa0138fdb1dd7a84a52dffdb89"
 dependencies = [
- "bitflags 2.4.1",
+ "bitflags 2.5.0",
  "errno",
  "libc",
  "linux-raw-sys",
- "windows-sys",
+ "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "rustls"
-version = "0.21.9"
+version = "0.21.10"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "629648aced5775d558af50b2b4c7b02983a04b312126d45eeead26e7caa498b9"
+checksum = "f9d5a6813c0759e4609cd494e8e725babae6a2ca7b62a5536a13daaec6fcb7ba"
 dependencies = [
  "log",
  "ring",
  "rustls-webpki",
  "sct",
 ]
 
@@ -1864,25 +1880,25 @@
 dependencies = [
  "ring",
  "untrusted",
 ]
 
 [[package]]
 name = "ryu"
-version = "1.0.15"
+version = "1.0.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1ad4cc8da4ef723ed60bced201181d83791ad433213d8c24efffda1eec85d741"
+checksum = "e86697c916019a8588c99b5fac3cead74ec0b4b819707a682fd4d23fa0ce1ba1"
 
 [[package]]
 name = "schannel"
-version = "0.1.22"
+version = "0.1.23"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0c3733bf4cf7ea0880754e19cb5a462007c4a8c1914bff372ccc95b464f1df88"
+checksum = "fbc91545643bcf3a0bbb6569265615222618bdf33ce4ffbbd13c4bbd4c093534"
 dependencies = [
- "windows-sys",
+ "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "scopeguard"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "94143f37725109f92c262ed2cf5e59bce7498c01bcc1502d7b9afe439a4e9f49"
@@ -1901,66 +1917,66 @@
 name = "seahash"
 version = "4.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1c107b6f4780854c8b126e228ea8869f4d7b71260f962fefb57b996b8959ba6b"
 
 [[package]]
 name = "security-framework"
-version = "2.9.2"
+version = "2.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "05b64fb303737d99b81884b2c63433e9ae28abebe5eb5045dcdd175dc2ecf4de"
+checksum = "770452e37cad93e0a50d5abc3990d2bc351c36d0328f86cefec2f2fb206eaef6"
 dependencies = [
  "bitflags 1.3.2",
  "core-foundation",
  "core-foundation-sys",
  "libc",
  "security-framework-sys",
 ]
 
 [[package]]
 name = "security-framework-sys"
-version = "2.9.1"
+version = "2.10.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e932934257d3b408ed8f30db49d85ea163bfe74961f017f405b025af298f0c7a"
+checksum = "41f3cc463c0ef97e11c3461a9d3787412d30e8e7eb907c79180c4a57bf7c04ef"
 dependencies = [
  "core-foundation-sys",
  "libc",
 ]
 
 [[package]]
 name = "semver"
-version = "1.0.20"
+version = "1.0.22"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "836fa6a3e1e547f9a2c4040802ec865b5d85f4014efe00555d7090a3dcaa1090"
+checksum = "92d43fe69e652f3df9bdc2b85b2854a0825b86e4fb76bc44d945137d053639ca"
 
 [[package]]
 name = "serde"
-version = "1.0.193"
+version = "1.0.197"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "25dd9975e68d0cb5aa1120c288333fc98731bd1dd12f561e468ea4728c042b89"
+checksum = "3fb1c873e1b9b056a4dc4c0c198b24c3ffa059243875552b2bd0933b1aee4ce2"
 dependencies = [
  "serde_derive",
 ]
 
 [[package]]
 name = "serde_derive"
-version = "1.0.193"
+version = "1.0.197"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "43576ca501357b9b071ac53cdc7da8ef0cbd9493d8df094cd821777ea6e894d3"
+checksum = "7eb0b34b42edc17f6b7cac84a52a1c5f0e1bb2227e997ca9011ea3dd34e8610b"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.39",
+ "syn 2.0.59",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.108"
+version = "1.0.116"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3d1c7e3eac408d115102c4c24ad393e0821bb3a5df4d506a80f85f7a742a526b"
+checksum = "3e17db7126d17feb94eb3fad46bf1a96b034e8aacbc2e775fe81505f8b0b2813"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
@@ -1988,36 +2004,26 @@
 checksum = "8f92a496fb766b417c996b9c5e57daf2f7ad3b0bebe1ccfca4856390e3d3bb67"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "smallvec"
-version = "1.11.2"
+version = "1.13.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "4dccd0940a2dcdf68d092b8cbab7dc0ad8fa938bf95787e1b916b0e3d0e8e970"
+checksum = "3c5e1a9a646d36c3599cd173a41282daf47c44583ad367b8e6837255952e5c67"
 
 [[package]]
 name = "socket2"
-version = "0.4.10"
+version = "0.5.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9f7916fc008ca5542385b89a3d3ce689953c143e9304a9bf8beec1de48994c0d"
+checksum = "05ffd9c0a93b7543e062e759284fcf5f5e3b098501104bfbdde4d404db792871"
 dependencies = [
  "libc",
- "winapi",
-]
-
-[[package]]
-name = "socket2"
-version = "0.5.5"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7b5fac59a5cb5dd637972e5fca70daf0523c9067fcdc4842f053dae04a18f8e9"
-dependencies = [
- "libc",
- "windows-sys",
+ "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "spin"
 version = "0.9.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6980e8d7511241f8acf4aebddbb1ff938df5eebe98691418c4468d0b72a96a67"
@@ -2037,17 +2043,17 @@
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.39"
+version = "2.0.59"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "23e78b90f2fcf45d3e842032ce32e3f2d1545ba6636271dcbf24fa306d87be7a"
+checksum = "4a6531ffc7b071655e4ce2e04bd464c4830bb585a61cabb96cf808f05172615a"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
@@ -2055,18 +2061,24 @@
 version = "0.1.8"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1329189c02ff984e9736652b1631330da25eaa6bc639089ed4915d25446cbe7b"
 dependencies = [
  "proc-macro-error",
  "proc-macro2",
  "quote",
- "syn 2.0.39",
+ "syn 2.0.59",
 ]
 
 [[package]]
+name = "sync_wrapper"
+version = "0.1.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "2047c6ded9c721764247e62cd3b03c09ffc529b2ba5b10ec482ae507a4a70160"
+
+[[package]]
 name = "system-configuration"
 version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ba3a3adc5c275d719af8cb4272ea1c4a6d668a777f37e115f6d11ddbc1c8e0e7"
 dependencies = [
  "bitflags 1.3.2",
  "core-foundation",
@@ -2087,60 +2099,59 @@
 name = "tap"
 version = "1.0.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "55937e1799185b12863d447f42597ed69d9928686b8d88a1df17376a097d8369"
 
 [[package]]
 name = "target-lexicon"
-version = "0.12.12"
+version = "0.12.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "14c39fd04924ca3a864207c66fc2cd7d22d7c016007f9ce846cbb9326331930a"
+checksum = "e1fc403891a21bcfb7c37834ba66a547a8f402146eba7265b5a6d88059c9ff2f"
 
 [[package]]
 name = "tempfile"
-version = "3.8.1"
+version = "3.10.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7ef1adac450ad7f4b3c28589471ade84f25f731a7a0fe30d71dfa9f60fd808e5"
+checksum = "85b77fafb263dd9d05cbeac119526425676db3784113aa9295c88498cbf8bff1"
 dependencies = [
  "cfg-if",
  "fastrand",
- "redox_syscall",
  "rustix",
- "windows-sys",
+ "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "thiserror"
-version = "1.0.50"
+version = "1.0.58"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f9a7210f5c9a7156bb50aa36aed4c95afb51df0df00713949448cf9e97d382d2"
+checksum = "03468839009160513471e86a034bb2c5c0e4baae3b43f79ffc55c4a5427b3297"
 dependencies = [
  "thiserror-impl",
 ]
 
 [[package]]
 name = "thiserror-impl"
-version = "1.0.50"
+version = "1.0.58"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "266b2e40bc00e5a6c09c3584011e08b06f123c00362c92b975ba9843aaaa14b8"
+checksum = "c61f3ba182994efc43764a46c018c347bc492c79f024e705f46567b418f6d4f7"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.39",
+ "syn 2.0.59",
 ]
 
 [[package]]
 name = "tiberius"
 version = "0.12.2"
 source = "git+https://github.com/aersam/tiberius.git?branch=bulk#8cee1fe5d765358ca568c96423766ae3b582b9e8"
 dependencies = [
  "async-native-tls",
  "async-trait",
  "asynchronous-codec",
- "bitflags 2.4.1",
+ "bitflags 2.5.0",
  "byteorder",
  "bytes",
  "connection-string",
  "encoding_rs",
  "enumflags2",
  "futures-util",
  "num-traits",
@@ -2158,19 +2169,20 @@
  "tracing",
  "uuid",
  "winauth",
 ]
 
 [[package]]
 name = "time"
-version = "0.3.30"
+version = "0.3.36"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c4a34ab300f2dee6e562c10a046fc05e358b29f9bf92277f30c3c8d82275f6f5"
+checksum = "5dfd88e563464686c916c7e46e623e520ddc6d79fa6641390f2e3fa86e83e885"
 dependencies = [
  "deranged",
+ "num-conv",
  "powerfmt",
  "serde",
  "time-core",
 ]
 
 [[package]]
 name = "time-core"
@@ -2200,38 +2212,38 @@
 name = "tinyvec_macros"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "1f3ccbac311fea05f86f61904b462b55fb3df8837a366dfc601a0161d0532f20"
 
 [[package]]
 name = "tokio"
-version = "1.34.0"
+version = "1.37.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d0c014766411e834f7af5b8f4cf46257aab4036ca95e9d2c144a10f59ad6f5b9"
+checksum = "1adbebffeca75fcfd058afa480fb6c0b81e165a0323f9c9d39c9697e37c46787"
 dependencies = [
  "backtrace",
  "bytes",
  "libc",
  "mio",
  "num_cpus",
  "pin-project-lite",
- "socket2 0.5.5",
+ "socket2",
  "tokio-macros",
- "windows-sys",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "tokio-macros"
 version = "2.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5b8a1e28f2deaa14e508979454cb3a223b10b938b45af148bc0986de36f1923b"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.39",
+ "syn 2.0.59",
 ]
 
 [[package]]
 name = "tokio-native-tls"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bbae76ab933c85776efabc971569dd6119c580d8f5d448769dec1764bf796ef2"
@@ -2269,17 +2281,17 @@
 name = "toml_datetime"
 version = "0.6.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3550f4e9685620ac18a50ed434eb3aec30db8ba93b0287467bca5826ea25baf1"
 
 [[package]]
 name = "toml_edit"
-version = "0.20.7"
+version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "70f427fce4d84c72b5b732388bf4a9f4531b53f74e2887e3ecb2481f68f66d81"
+checksum = "6a8534fd7f78b5405e860340ad6575217ce99f38d4d5c8f2442cb5ecb50090e1"
 dependencies = [
  "indexmap",
  "toml_datetime",
  "winnow",
 ]
 
 [[package]]
@@ -2304,59 +2316,59 @@
 name = "tracing-attributes"
 version = "0.1.27"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "34704c8d6ebcbc939824180af020566b01a7c01f80641264eba0999f6c2b6be7"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.39",
+ "syn 2.0.59",
 ]
 
 [[package]]
 name = "tracing-core"
 version = "0.1.32"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c06d3da6113f116aaee68e4d601191614c9053067f9ab7f6edbcb161237daa54"
 dependencies = [
  "once_cell",
 ]
 
 [[package]]
 name = "try-lock"
-version = "0.2.4"
+version = "0.2.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "3528ecfd12c466c6f163363caf2d02a71161dd5e1cc6ae7b34207ea2d42d81ed"
+checksum = "e421abadd41a4225275504ea4d6566923418b7f05506fbc9c0fe86ba7396114b"
 
 [[package]]
 name = "twox-hash"
 version = "1.6.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "97fee6b57c6a41524a810daee9286c02d7752c4253064d0b05472833a438f675"
 dependencies = [
  "cfg-if",
  "static_assertions",
 ]
 
 [[package]]
 name = "unicode-bidi"
-version = "0.3.13"
+version = "0.3.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "92888ba5573ff080736b3648696b70cafad7d250551175acbaa4e0385b3e1460"
+checksum = "08f95100a766bf4f8f28f90d77e0a5461bbdb219042e7679bebe79004fed8d75"
 
 [[package]]
 name = "unicode-ident"
 version = "1.0.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3354b9ac3fae1ff6755cb6db53683adb661634f67557942dea4facebec0fee4b"
 
 [[package]]
 name = "unicode-normalization"
-version = "0.1.22"
+version = "0.1.23"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5c5713f0fc4b5db668a2ac63cdb7bb4469d8c9fed047b1d0292cc7b0ce2ba921"
+checksum = "a56d1686db2308d901306f92a263857ef59ea39678a5458e7cb17f01415101f5"
 dependencies = [
  "tinyvec",
 ]
 
 [[package]]
 name = "unindent"
 version = "0.2.3"
@@ -2367,28 +2379,28 @@
 name = "untrusted"
 version = "0.9.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8ecb6da28b8a351d773b68d5825ac39017e680750f980f3a1a85cd8dd28a47c1"
 
 [[package]]
 name = "url"
-version = "2.4.1"
+version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "143b538f18257fac9cad154828a57c6bf5157e1aa604d4816b5995bf6de87ae5"
+checksum = "31e6302e3bb753d46e83516cae55ae196fc0c309407cf11ab35cc51a4c2a4633"
 dependencies = [
  "form_urlencoded",
  "idna",
  "percent-encoding",
 ]
 
 [[package]]
 name = "uuid"
-version = "1.6.1"
+version = "1.8.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5e395fcf16a7a3d8127ec99782007af141946b4795001f876d54fb0d55978560"
+checksum = "a183cf7feeba97b4dd1c0d46788634f6221d87fa961b305bed08c851829efcc0"
 
 [[package]]
 name = "vcpkg"
 version = "0.2.15"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "accd4ea62f7bb7a82fe23066fb0957d48ef677f6eeb8215f372f52e48bb32426"
 
@@ -2417,96 +2429,96 @@
 name = "wasi"
 version = "0.11.0+wasi-snapshot-preview1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c8d87e72b64a3b4db28d11ce29237c246188f4f51057d65a7eab63b7987e423"
 
 [[package]]
 name = "wasm-bindgen"
-version = "0.2.88"
+version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7daec296f25a1bae309c0cd5c29c4b260e510e6d813c286b19eaadf409d40fce"
+checksum = "4be2531df63900aeb2bca0daaaddec08491ee64ceecbee5076636a3b026795a8"
 dependencies = [
  "cfg-if",
  "wasm-bindgen-macro",
 ]
 
 [[package]]
 name = "wasm-bindgen-backend"
-version = "0.2.88"
+version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e397f4664c0e4e428e8313a469aaa58310d302159845980fd23b0f22a847f217"
+checksum = "614d787b966d3989fa7bb98a654e369c762374fd3213d212cfc0251257e747da"
 dependencies = [
  "bumpalo",
  "log",
  "once_cell",
  "proc-macro2",
  "quote",
- "syn 2.0.39",
+ "syn 2.0.59",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-futures"
-version = "0.4.38"
+version = "0.4.42"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9afec9963e3d0994cac82455b2b3502b81a7f40f9a0d32181f7528d9f4b43e02"
+checksum = "76bc14366121efc8dbb487ab05bcc9d346b3b5ec0eaa76e46594cabbe51762c0"
 dependencies = [
  "cfg-if",
  "js-sys",
  "wasm-bindgen",
  "web-sys",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro"
-version = "0.2.88"
+version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5961017b3b08ad5f3fe39f1e79877f8ee7c23c5e5fd5eb80de95abc41f1f16b2"
+checksum = "a1f8823de937b71b9460c0c34e25f3da88250760bec0ebac694b49997550d726"
 dependencies = [
  "quote",
  "wasm-bindgen-macro-support",
 ]
 
 [[package]]
 name = "wasm-bindgen-macro-support"
-version = "0.2.88"
+version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c5353b8dab669f5e10f5bd76df26a9360c748f054f862ff5f3f8aae0c7fb3907"
+checksum = "e94f17b526d0a461a191c78ea52bbce64071ed5c04c9ffe424dcb38f74171bb7"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.39",
+ "syn 2.0.59",
  "wasm-bindgen-backend",
  "wasm-bindgen-shared",
 ]
 
 [[package]]
 name = "wasm-bindgen-shared"
-version = "0.2.88"
+version = "0.2.92"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "0d046c5d029ba91a1ed14da14dca44b68bf2f124cfbaf741c54151fdb3e0750b"
+checksum = "af190c94f2773fdb3729c55b007a722abb5384da03bc0986df4c289bf5567e96"
 
 [[package]]
 name = "wasm-streams"
-version = "0.3.0"
+version = "0.4.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b4609d447824375f43e1ffbc051b50ad8f4b3ae8219680c94452ea05eb240ac7"
+checksum = "b65dc4c90b63b118468cf747d8bf3566c1913ef60be765b5730ead9e0a3ba129"
 dependencies = [
  "futures-util",
  "js-sys",
  "wasm-bindgen",
  "wasm-bindgen-futures",
  "web-sys",
 ]
 
 [[package]]
 name = "web-sys"
-version = "0.3.65"
+version = "0.3.69"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5db499c5f66323272151db0e666cd34f78617522fb0c1604d31a27c50c206a85"
+checksum = "77afa9a11836342370f4817622a2f0f418b134426d91a82dfb48f532d2ec13ef"
 dependencies = [
  "js-sys",
  "wasm-bindgen",
 ]
 
 [[package]]
 name = "winapi"
@@ -2541,155 +2553,228 @@
  "md5",
  "rand 0.7.3",
  "winapi",
 ]
 
 [[package]]
 name = "windows-core"
-version = "0.51.1"
+version = "0.52.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f1f8cf84f35d2db49a46868f947758c7a1138116f7fac3bc844f43ade1292e64"
+checksum = "33ab640c8d7e35bf8ba19b884ba838ceb4fba93a4e8c65a9059d08afcfc683d9"
 dependencies = [
- "windows-targets",
+ "windows-targets 0.52.5",
 ]
 
 [[package]]
 name = "windows-sys"
 version = "0.48.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "677d2418bec65e3338edb076e806bc1ec15693c5d0104683f2efe857f61056a9"
 dependencies = [
- "windows-targets",
+ "windows-targets 0.48.5",
+]
+
+[[package]]
+name = "windows-sys"
+version = "0.52.0"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "282be5f36a8ce781fad8c8ae18fa3f9beff57ec1b52cb3de0789201425d9a33d"
+dependencies = [
+ "windows-targets 0.52.5",
 ]
 
 [[package]]
 name = "windows-targets"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9a2fa6e2155d7247be68c096456083145c183cbbbc2764150dda45a87197940c"
 dependencies = [
- "windows_aarch64_gnullvm",
- "windows_aarch64_msvc",
- "windows_i686_gnu",
- "windows_i686_msvc",
- "windows_x86_64_gnu",
- "windows_x86_64_gnullvm",
- "windows_x86_64_msvc",
+ "windows_aarch64_gnullvm 0.48.5",
+ "windows_aarch64_msvc 0.48.5",
+ "windows_i686_gnu 0.48.5",
+ "windows_i686_msvc 0.48.5",
+ "windows_x86_64_gnu 0.48.5",
+ "windows_x86_64_gnullvm 0.48.5",
+ "windows_x86_64_msvc 0.48.5",
+]
+
+[[package]]
+name = "windows-targets"
+version = "0.52.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "6f0713a46559409d202e70e28227288446bf7841d3211583a4b53e3f6d96e7eb"
+dependencies = [
+ "windows_aarch64_gnullvm 0.52.5",
+ "windows_aarch64_msvc 0.52.5",
+ "windows_i686_gnu 0.52.5",
+ "windows_i686_gnullvm",
+ "windows_i686_msvc 0.52.5",
+ "windows_x86_64_gnu 0.52.5",
+ "windows_x86_64_gnullvm 0.52.5",
+ "windows_x86_64_msvc 0.52.5",
 ]
 
 [[package]]
 name = "windows_aarch64_gnullvm"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "2b38e32f0abccf9987a4e3079dfb67dcd799fb61361e53e2882c3cbaf0d905d8"
 
 [[package]]
+name = "windows_aarch64_gnullvm"
+version = "0.52.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "7088eed71e8b8dda258ecc8bac5fb1153c5cffaf2578fc8ff5d61e23578d3263"
+
+[[package]]
 name = "windows_aarch64_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dc35310971f3b2dbbf3f0690a219f40e2d9afcf64f9ab7cc1be722937c26b4bc"
 
 [[package]]
+name = "windows_aarch64_msvc"
+version = "0.52.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9985fd1504e250c615ca5f281c3f7a6da76213ebd5ccc9561496568a2752afb6"
+
+[[package]]
 name = "windows_i686_gnu"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a75915e7def60c94dcef72200b9a8e58e5091744960da64ec734a6c6e9b3743e"
 
 [[package]]
+name = "windows_i686_gnu"
+version = "0.52.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "88ba073cf16d5372720ec942a8ccbf61626074c6d4dd2e745299726ce8b89670"
+
+[[package]]
+name = "windows_i686_gnullvm"
+version = "0.52.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "87f4261229030a858f36b459e748ae97545d6f1ec60e5e0d6a3d32e0dc232ee9"
+
+[[package]]
 name = "windows_i686_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8f55c233f70c4b27f66c523580f78f1004e8b5a8b659e05a4eb49d4166cca406"
 
 [[package]]
+name = "windows_i686_msvc"
+version = "0.52.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "db3c2bf3d13d5b658be73463284eaf12830ac9a26a90c717b7f771dfe97487bf"
+
+[[package]]
 name = "windows_x86_64_gnu"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "53d40abd2583d23e4718fddf1ebec84dbff8381c07cae67ff7768bbf19c6718e"
 
 [[package]]
+name = "windows_x86_64_gnu"
+version = "0.52.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "4e4246f76bdeff09eb48875a0fd3e2af6aada79d409d33011886d3e1581517d9"
+
+[[package]]
 name = "windows_x86_64_gnullvm"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0b7b52767868a23d5bab768e390dc5f5c55825b6d30b86c844ff2dc7414044cc"
 
 [[package]]
+name = "windows_x86_64_gnullvm"
+version = "0.52.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "852298e482cd67c356ddd9570386e2862b5673c85bd5f88df9ab6802b334c596"
+
+[[package]]
 name = "windows_x86_64_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ed94fce61571a4006852b7389a063ab983c02eb1bb37b47f8272ce92d06d9538"
 
 [[package]]
+name = "windows_x86_64_msvc"
+version = "0.52.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "bec47e5bfd1bff0eeaf6d8b485cc1074891a197ab4225d504cb7a1ab88b02bf0"
+
+[[package]]
 name = "winnow"
-version = "0.5.19"
+version = "0.5.40"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "829846f3e3db426d4cee4510841b71a8e58aa2a76b1132579487ae430ccd9c7b"
+checksum = "f593a95398737aeed53e489c785df13f3618e41dbcd6718c6addbf1395aa6876"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "winreg"
 version = "0.50.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "524e57b2c537c0f9b1e69f1965311ec12182b4122e45035b1508cd24d2adadb1"
 dependencies = [
  "cfg-if",
- "windows-sys",
+ "windows-sys 0.48.0",
 ]
 
 [[package]]
 name = "wyz"
 version = "0.5.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "05f360fc0b24296329c78fda852a1e9ae82de9cf7b27dae4b7f62f118f77b9ed"
 dependencies = [
  "tap",
 ]
 
 [[package]]
 name = "zerocopy"
-version = "0.7.26"
+version = "0.7.32"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e97e415490559a91254a2979b4829267a57d2fcd741a98eee8b722fb57289aa0"
+checksum = "74d4d3961e53fa4c9a25a8637fc2bfaf2595b3d3ae34875568a5cf64787716be"
 dependencies = [
  "zerocopy-derive",
 ]
 
 [[package]]
 name = "zerocopy-derive"
-version = "0.7.26"
+version = "0.7.32"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "dd7e48ccf166952882ca8bd778a43502c64f33bf94c12ebe2a7f08e5a0f6689f"
+checksum = "9ce1b18ccd8e73a9321186f97e46f9f04b778851177567b1975109d26a08d2a6"
 dependencies = [
  "proc-macro2",
  "quote",
- "syn 2.0.39",
+ "syn 2.0.59",
 ]
 
 [[package]]
 name = "zstd"
-version = "0.13.0"
+version = "0.13.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bffb3309596d527cfcba7dfc6ed6052f1d39dfbd7c867aa2e865e4a449c10110"
+checksum = "2d789b1514203a1120ad2429eae43a7bd32b90976a7bb8a05f7ec02fa88cc23a"
 dependencies = [
  "zstd-safe",
 ]
 
 [[package]]
 name = "zstd-safe"
-version = "7.0.0"
+version = "7.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "43747c7422e2924c11144d5229878b98180ef8b06cca4ab5af37afc8a8d8ea3e"
+checksum = "1cd99b45c6bc03a018c8b8a86025678c87e55526064e38f9df301989dce7ec0a"
 dependencies = [
  "zstd-sys",
 ]
 
 [[package]]
 name = "zstd-sys"
-version = "2.0.9+zstd.1.5.5"
+version = "2.0.10+zstd.1.5.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9e16efa8a874a0481a574084d34cc26fdb3b99627480f785888deb6386506656"
+checksum = "c253a4914af5bafc8fa8c86ee400827e83cf6ec01195ec1f1ed8441bf00d65aa"
 dependencies = [
  "cc",
  "pkg-config",
 ]
```

### Comparing `lakeapi2sql-0.8.0/pyproject.toml` & `lakeapi2sql-0.8.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["maturin>=1.1,<2.0"]
 build-backend = "maturin"
 
 [project]
 name = "lakeapi2sql"
 requires-python = ">=3.10"
-version = "0.8.0"
+version = "0.8.1"
 classifiers = [
     "Programming Language :: Rust",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
 ]
 
 dependencies = ["pyarrow >= 8.0.0"]
```

### Comparing `lakeapi2sql-0.8.0/PKG-INFO` & `lakeapi2sql-0.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-Metadata-Version: 2.1
+Metadata-Version: 2.3
 Name: lakeapi2sql
-Version: 0.8.0
+Version: 0.8.1
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Dist: pyarrow >=8.0.0
 Requires-Dist: azure-identity >=1.12.0 ; extra == 'azure'
 Provides-Extra: azure
 License-File: LICENSE
```

