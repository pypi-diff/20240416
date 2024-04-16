# Comparing `tmp/typos-1.20.8.tar.gz` & `tmp/typos-1.20.9.tar.gz`

## Comparing `typos-1.20.8.tar` & `typos-1.20.9.tar`

### file list

```diff
@@ -1,46 +1,46 @@
--rw-r--r--   0     1001      127      589 2024-04-12 21:04:15.000000 typos-1.20.8/crates/typos/Cargo.toml
--rw-r--r--   0     1001      127     2794 2024-04-12 21:04:15.000000 typos-1.20.8/crates/typos/src/check.rs
--rw-r--r--   0     1001      127     2167 2024-04-12 21:04:15.000000 typos-1.20.8/crates/typos/src/dict.rs
--rw-r--r--   0     1001      127       74 2024-04-12 21:04:15.000000 typos-1.20.8/crates/typos/src/lib.rs
--rw-r--r--   0     1001      127    46856 2024-04-12 21:04:15.000000 typos-1.20.8/crates/typos/src/tokens.rs
--rw-r--r--   0     1001      127     5770 2024-04-12 21:04:15.000000 typos-1.20.8/README.md
--rw-r--r--   0     1001      127      740 2024-04-12 21:04:15.000000 typos-1.20.8/crates/typos-dict/Cargo.toml
--rw-r--r--   0     1001      127       59 2024-04-12 21:04:15.000000 typos-1.20.8/crates/typos-dict/src/lib.rs
--rw-r--r--   0     1001      127  7269036 2024-04-12 21:04:15.000000 typos-1.20.8/crates/typos-dict/src/word_codegen.rs
--rw-r--r--   0     1001      127      671 2024-04-12 21:04:15.000000 typos-1.20.8/crates/varcon/Cargo.toml
--rw-r--r--   0     1001      127 12563224 2024-04-12 21:04:15.000000 typos-1.20.8/crates/varcon/src/codegen.rs
--rw-r--r--   0     1001      127      432 2024-04-12 21:04:15.000000 typos-1.20.8/crates/varcon/src/lib.rs
--rw-r--r--   0     1001      127      921 2024-04-12 21:04:15.000000 typos-1.20.8/crates/typos-vars/Cargo.toml
--rw-r--r--   0     1001      127      117 2024-04-12 21:04:15.000000 typos-1.20.8/crates/typos-vars/src/lib.rs
--rw-r--r--   0     1001      127  6086180 2024-04-12 21:04:15.000000 typos-1.20.8/crates/typos-vars/src/vars_codegen.rs
--rw-r--r--   0     1001      127      541 2024-04-12 21:04:15.000000 typos-1.20.8/crates/varcon-core/Cargo.toml
--rw-r--r--   0     1001      127     1488 2024-04-12 21:04:15.000000 typos-1.20.8/crates/varcon-core/src/borrowed.rs
--rw-r--r--   0     1001      127     2850 2024-04-12 21:04:15.000000 typos-1.20.8/crates/varcon-core/src/lib.rs
--rw-r--r--   0     1001      127    18974 2024-04-12 21:04:15.000000 typos-1.20.8/crates/varcon-core/src/parser.rs
--rw-r--r--   0     1001      127      646 2024-04-12 21:04:15.000000 typos-1.20.8/crates/dictgen/Cargo.toml
--rw-r--r--   0     1001      127      130 2024-04-12 21:04:15.000000 typos-1.20.8/crates/dictgen/src/lib.rs
--rw-r--r--   0     1001      127     2687 2024-04-12 21:04:15.000000 typos-1.20.8/crates/dictgen/src/map.rs
--rw-r--r--   0     1001      127     3726 2024-04-12 21:04:15.000000 typos-1.20.8/crates/dictgen/src/table.rs
--rw-r--r--   0     1001      127    10629 2024-04-12 21:04:15.000000 typos-1.20.8/crates/dictgen/src/trie.rs
--rw-r--r--   0        0        0     2853 1970-01-01 00:00:00.000000 typos-1.20.8/crates/typos-cli/Cargo.toml
--rw-r--r--   0     1001      127     3092 2024-04-12 21:04:15.000000 typos-1.20.8/crates/typos-cli/benches/check_file.rs
--rw-r--r--   0     1001      127     5640 2024-04-12 21:04:15.000000 typos-1.20.8/crates/typos-cli/benches/correct_word.rs
--rw-r--r--   0     1001      127     1724 2024-04-12 21:04:15.000000 typos-1.20.8/crates/typos-cli/benches/data.rs
--rw-r--r--   0     1001      127     3298 2024-04-12 21:04:15.000000 typos-1.20.8/crates/typos-cli/benches/tokenize.rs
--rw-r--r--   0     1001      127     8981 2024-04-12 21:04:15.000000 typos-1.20.8/crates/typos-cli/src/bin/typos-cli/args.rs
--rw-r--r--   0     1001      127    12158 2024-04-12 21:04:15.000000 typos-1.20.8/crates/typos-cli/src/bin/typos-cli/main.rs
--rw-r--r--   0     1001      127    11379 2024-04-12 21:04:15.000000 typos-1.20.8/crates/typos-cli/src/bin/typos-cli/report.rs
--rw-r--r--   0     1001      127    20949 2024-04-12 21:04:15.000000 typos-1.20.8/crates/typos-cli/src/config.rs
--rw-r--r--   0     1001      127    10420 2024-04-12 21:04:15.000000 typos-1.20.8/crates/typos-cli/src/default_types.rs
--rw-r--r--   0     1001      127    12513 2024-04-12 21:04:15.000000 typos-1.20.8/crates/typos-cli/src/dict.rs
--rw-r--r--   0     1001      127    33435 2024-04-12 21:04:15.000000 typos-1.20.8/crates/typos-cli/src/file.rs
--rw-r--r--   0     1001      127     6790 2024-04-12 21:04:15.000000 typos-1.20.8/crates/typos-cli/src/file_type.rs
--rw-r--r--   0     1001      127     3554 2024-04-12 21:04:15.000000 typos-1.20.8/crates/typos-cli/src/file_type_specifics.rs
--rw-r--r--   0     1001      127      324 2024-04-12 21:04:15.000000 typos-1.20.8/crates/typos-cli/src/lib.rs
--rw-r--r--   0     1001      127    17561 2024-04-12 21:04:15.000000 typos-1.20.8/crates/typos-cli/src/policy.rs
--rw-r--r--   0     1001      127     5551 2024-04-12 21:04:15.000000 typos-1.20.8/crates/typos-cli/src/report.rs
--rw-r--r--   0     1001      127      228 2024-04-12 21:04:15.000000 typos-1.20.8/crates/typos-cli/tests/cmd/false-positives.in/README.md
--rw-r--r--   0     1001      127    44060 2024-04-12 21:04:15.000000 typos-1.20.8/Cargo.lock
--rw-r--r--   0        0        0      459 1970-01-01 00:00:00.000000 typos-1.20.8/Cargo.toml
--rw-r--r--   0        0        0      489 1970-01-01 00:00:00.000000 typos-1.20.8/pyproject.toml
--rw-r--r--   0        0        0     6340 1970-01-01 00:00:00.000000 typos-1.20.8/PKG-INFO
+-rw-r--r--   0     1001      127      740 2024-04-16 16:58:52.000000 typos-1.20.9/crates/typos-dict/Cargo.toml
+-rw-r--r--   0     1001      127       59 2024-04-16 16:58:52.000000 typos-1.20.9/crates/typos-dict/src/lib.rs
+-rw-r--r--   0     1001      127  7269036 2024-04-16 16:58:52.000000 typos-1.20.9/crates/typos-dict/src/word_codegen.rs
+-rw-r--r--   0     1001      127     5770 2024-04-16 16:58:52.000000 typos-1.20.9/README.md
+-rw-r--r--   0     1001      127      541 2024-04-16 16:58:52.000000 typos-1.20.9/crates/varcon-core/Cargo.toml
+-rw-r--r--   0     1001      127     1488 2024-04-16 16:58:52.000000 typos-1.20.9/crates/varcon-core/src/borrowed.rs
+-rw-r--r--   0     1001      127     2850 2024-04-16 16:58:52.000000 typos-1.20.9/crates/varcon-core/src/lib.rs
+-rw-r--r--   0     1001      127    18974 2024-04-16 16:58:52.000000 typos-1.20.9/crates/varcon-core/src/parser.rs
+-rw-r--r--   0     1001      127      671 2024-04-16 16:58:52.000000 typos-1.20.9/crates/varcon/Cargo.toml
+-rw-r--r--   0     1001      127 12563224 2024-04-16 16:58:52.000000 typos-1.20.9/crates/varcon/src/codegen.rs
+-rw-r--r--   0     1001      127      432 2024-04-16 16:58:52.000000 typos-1.20.9/crates/varcon/src/lib.rs
+-rw-r--r--   0     1001      127      589 2024-04-16 16:58:52.000000 typos-1.20.9/crates/typos/Cargo.toml
+-rw-r--r--   0     1001      127     2794 2024-04-16 16:58:52.000000 typos-1.20.9/crates/typos/src/check.rs
+-rw-r--r--   0     1001      127     2167 2024-04-16 16:58:52.000000 typos-1.20.9/crates/typos/src/dict.rs
+-rw-r--r--   0     1001      127       74 2024-04-16 16:58:52.000000 typos-1.20.9/crates/typos/src/lib.rs
+-rw-r--r--   0     1001      127    46856 2024-04-16 16:58:52.000000 typos-1.20.9/crates/typos/src/tokens.rs
+-rw-r--r--   0     1001      127      921 2024-04-16 16:58:52.000000 typos-1.20.9/crates/typos-vars/Cargo.toml
+-rw-r--r--   0     1001      127      117 2024-04-16 16:58:52.000000 typos-1.20.9/crates/typos-vars/src/lib.rs
+-rw-r--r--   0     1001      127  6086180 2024-04-16 16:58:52.000000 typos-1.20.9/crates/typos-vars/src/vars_codegen.rs
+-rw-r--r--   0     1001      127      646 2024-04-16 16:58:52.000000 typos-1.20.9/crates/dictgen/Cargo.toml
+-rw-r--r--   0     1001      127      130 2024-04-16 16:58:52.000000 typos-1.20.9/crates/dictgen/src/lib.rs
+-rw-r--r--   0     1001      127     2687 2024-04-16 16:58:52.000000 typos-1.20.9/crates/dictgen/src/map.rs
+-rw-r--r--   0     1001      127     3726 2024-04-16 16:58:52.000000 typos-1.20.9/crates/dictgen/src/table.rs
+-rw-r--r--   0     1001      127    10629 2024-04-16 16:58:52.000000 typos-1.20.9/crates/dictgen/src/trie.rs
+-rw-r--r--   0        0        0     2853 1970-01-01 00:00:00.000000 typos-1.20.9/crates/typos-cli/Cargo.toml
+-rw-r--r--   0     1001      127     3092 2024-04-16 16:58:52.000000 typos-1.20.9/crates/typos-cli/benches/check_file.rs
+-rw-r--r--   0     1001      127     5640 2024-04-16 16:58:52.000000 typos-1.20.9/crates/typos-cli/benches/correct_word.rs
+-rw-r--r--   0     1001      127     1724 2024-04-16 16:58:52.000000 typos-1.20.9/crates/typos-cli/benches/data.rs
+-rw-r--r--   0     1001      127     3298 2024-04-16 16:58:52.000000 typos-1.20.9/crates/typos-cli/benches/tokenize.rs
+-rw-r--r--   0     1001      127     8981 2024-04-16 16:58:52.000000 typos-1.20.9/crates/typos-cli/src/bin/typos-cli/args.rs
+-rw-r--r--   0     1001      127    12158 2024-04-16 16:58:52.000000 typos-1.20.9/crates/typos-cli/src/bin/typos-cli/main.rs
+-rw-r--r--   0     1001      127    11379 2024-04-16 16:58:52.000000 typos-1.20.9/crates/typos-cli/src/bin/typos-cli/report.rs
+-rw-r--r--   0     1001      127    20949 2024-04-16 16:58:52.000000 typos-1.20.9/crates/typos-cli/src/config.rs
+-rw-r--r--   0     1001      127    10420 2024-04-16 16:58:52.000000 typos-1.20.9/crates/typos-cli/src/default_types.rs
+-rw-r--r--   0     1001      127    12555 2024-04-16 16:58:52.000000 typos-1.20.9/crates/typos-cli/src/dict.rs
+-rw-r--r--   0     1001      127    33435 2024-04-16 16:58:52.000000 typos-1.20.9/crates/typos-cli/src/file.rs
+-rw-r--r--   0     1001      127     6790 2024-04-16 16:58:52.000000 typos-1.20.9/crates/typos-cli/src/file_type.rs
+-rw-r--r--   0     1001      127     3554 2024-04-16 16:58:52.000000 typos-1.20.9/crates/typos-cli/src/file_type_specifics.rs
+-rw-r--r--   0     1001      127      324 2024-04-16 16:58:52.000000 typos-1.20.9/crates/typos-cli/src/lib.rs
+-rw-r--r--   0     1001      127    17561 2024-04-16 16:58:52.000000 typos-1.20.9/crates/typos-cli/src/policy.rs
+-rw-r--r--   0     1001      127     5551 2024-04-16 16:58:52.000000 typos-1.20.9/crates/typos-cli/src/report.rs
+-rw-r--r--   0     1001      127      228 2024-04-16 16:58:52.000000 typos-1.20.9/crates/typos-cli/tests/cmd/false-positives.in/README.md
+-rw-r--r--   0     1001      127    44060 2024-04-16 16:58:52.000000 typos-1.20.9/Cargo.lock
+-rw-r--r--   0        0        0      459 1970-01-01 00:00:00.000000 typos-1.20.9/Cargo.toml
+-rw-r--r--   0        0        0      489 1970-01-01 00:00:00.000000 typos-1.20.9/pyproject.toml
+-rw-r--r--   0        0        0     6340 1970-01-01 00:00:00.000000 typos-1.20.9/PKG-INFO
```

### Comparing `typos-1.20.8/crates/typos/Cargo.toml` & `typos-1.20.9/crates/typos/Cargo.toml`

 * *Files identical despite different names*

### Comparing `typos-1.20.8/crates/typos/src/check.rs` & `typos-1.20.9/crates/typos/src/check.rs`

 * *Files identical despite different names*

### Comparing `typos-1.20.8/crates/typos/src/dict.rs` & `typos-1.20.9/crates/typos/src/dict.rs`

 * *Files identical despite different names*

### Comparing `typos-1.20.8/crates/typos/src/tokens.rs` & `typos-1.20.9/crates/typos/src/tokens.rs`

 * *Files identical despite different names*

### Comparing `typos-1.20.8/README.md` & `typos-1.20.9/README.md`

 * *Files identical despite different names*

### Comparing `typos-1.20.8/crates/typos-dict/Cargo.toml` & `typos-1.20.9/crates/typos-dict/Cargo.toml`

 * *Files identical despite different names*

### Comparing `typos-1.20.8/crates/typos-dict/src/word_codegen.rs` & `typos-1.20.9/crates/typos-dict/src/word_codegen.rs`

 * *Files identical despite different names*

### Comparing `typos-1.20.8/crates/varcon/Cargo.toml` & `typos-1.20.9/crates/varcon/Cargo.toml`

 * *Files identical despite different names*

### Comparing `typos-1.20.8/crates/varcon/src/codegen.rs` & `typos-1.20.9/crates/varcon/src/codegen.rs`

 * *Files identical despite different names*

### Comparing `typos-1.20.8/crates/typos-vars/Cargo.toml` & `typos-1.20.9/crates/typos-vars/Cargo.toml`

 * *Files identical despite different names*

### Comparing `typos-1.20.8/crates/typos-vars/src/vars_codegen.rs` & `typos-1.20.9/crates/typos-vars/src/vars_codegen.rs`

 * *Files identical despite different names*

### Comparing `typos-1.20.8/crates/varcon-core/Cargo.toml` & `typos-1.20.9/crates/varcon-core/Cargo.toml`

 * *Files identical despite different names*

### Comparing `typos-1.20.8/crates/varcon-core/src/borrowed.rs` & `typos-1.20.9/crates/varcon-core/src/borrowed.rs`

 * *Files identical despite different names*

### Comparing `typos-1.20.8/crates/varcon-core/src/lib.rs` & `typos-1.20.9/crates/varcon-core/src/lib.rs`

 * *Files identical despite different names*

### Comparing `typos-1.20.8/crates/varcon-core/src/parser.rs` & `typos-1.20.9/crates/varcon-core/src/parser.rs`

 * *Files identical despite different names*

### Comparing `typos-1.20.8/crates/dictgen/Cargo.toml` & `typos-1.20.9/crates/dictgen/Cargo.toml`

 * *Files identical despite different names*

### Comparing `typos-1.20.8/crates/dictgen/src/map.rs` & `typos-1.20.9/crates/dictgen/src/map.rs`

 * *Files identical despite different names*

### Comparing `typos-1.20.8/crates/dictgen/src/table.rs` & `typos-1.20.9/crates/dictgen/src/table.rs`

 * *Files identical despite different names*

### Comparing `typos-1.20.8/crates/dictgen/src/trie.rs` & `typos-1.20.9/crates/dictgen/src/trie.rs`

 * *Files identical despite different names*

### Comparing `typos-1.20.8/crates/typos-cli/Cargo.toml` & `typos-1.20.9/crates/typos-cli/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "typos-cli"
-version = "1.20.8"
+version = "1.20.9"
 description = "Source Code Spelling Correction"
 readme = "../../README.md"
 categories = ["development-tools", "text-processing"]
 keywords = ["development", "spelling"]
 license.workspace = true
 repository.workspace = true
 edition.workspace = true
```

### Comparing `typos-1.20.8/crates/typos-cli/benches/check_file.rs` & `typos-1.20.9/crates/typos-cli/benches/check_file.rs`

 * *Files identical despite different names*

### Comparing `typos-1.20.8/crates/typos-cli/benches/correct_word.rs` & `typos-1.20.9/crates/typos-cli/benches/correct_word.rs`

 * *Files identical despite different names*

### Comparing `typos-1.20.8/crates/typos-cli/benches/data.rs` & `typos-1.20.9/crates/typos-cli/benches/data.rs`

 * *Files identical despite different names*

### Comparing `typos-1.20.8/crates/typos-cli/benches/tokenize.rs` & `typos-1.20.9/crates/typos-cli/benches/tokenize.rs`

 * *Files identical despite different names*

### Comparing `typos-1.20.8/crates/typos-cli/src/bin/typos-cli/args.rs` & `typos-1.20.9/crates/typos-cli/src/bin/typos-cli/args.rs`

 * *Files identical despite different names*

### Comparing `typos-1.20.8/crates/typos-cli/src/bin/typos-cli/main.rs` & `typos-1.20.9/crates/typos-cli/src/bin/typos-cli/main.rs`

 * *Files identical despite different names*

### Comparing `typos-1.20.8/crates/typos-cli/src/bin/typos-cli/report.rs` & `typos-1.20.9/crates/typos-cli/src/bin/typos-cli/report.rs`

 * *Files identical despite different names*

### Comparing `typos-1.20.8/crates/typos-cli/src/config.rs` & `typos-1.20.9/crates/typos-cli/src/config.rs`

 * *Files identical despite different names*

### Comparing `typos-1.20.8/crates/typos-cli/src/default_types.rs` & `typos-1.20.9/crates/typos-cli/src/default_types.rs`

 * *Files identical despite different names*

### Comparing `typos-1.20.8/crates/typos-cli/src/dict.rs` & `typos-1.20.9/crates/typos-cli/src/dict.rs`

 * *Files 1% similar despite different names*

```diff
@@ -50,14 +50,15 @@
 }
 
 #[cfg(feature = "dict")]
 impl BuiltIn {
     fn correct_ident_with_dict<'s>(&self, ident: &str) -> Option<Status<'s>> {
         match ident {
             "O_WRONLY" => Some(Status::Valid),
+            "dBA" => Some(Status::Valid),
             _ => None,
         }
     }
 
     // Not using `Status` to avoid the allocations
     fn correct_word_with_dict(
         &self,
```

### Comparing `typos-1.20.8/crates/typos-cli/src/file.rs` & `typos-1.20.9/crates/typos-cli/src/file.rs`

 * *Files identical despite different names*

### Comparing `typos-1.20.8/crates/typos-cli/src/file_type.rs` & `typos-1.20.9/crates/typos-cli/src/file_type.rs`

 * *Files identical despite different names*

### Comparing `typos-1.20.8/crates/typos-cli/src/file_type_specifics.rs` & `typos-1.20.9/crates/typos-cli/src/file_type_specifics.rs`

 * *Files identical despite different names*

### Comparing `typos-1.20.8/crates/typos-cli/src/policy.rs` & `typos-1.20.9/crates/typos-cli/src/policy.rs`

 * *Files identical despite different names*

### Comparing `typos-1.20.8/crates/typos-cli/src/report.rs` & `typos-1.20.9/crates/typos-cli/src/report.rs`

 * *Files identical despite different names*

### Comparing `typos-1.20.8/Cargo.lock` & `typos-1.20.9/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -1334,15 +1334,15 @@
  "unicode-segmentation",
  "unicode-xid",
  "winnow",
 ]
 
 [[package]]
 name = "typos-cli"
-version = "1.20.8"
+version = "1.20.9"
 dependencies = [
  "ahash",
  "anstream",
  "anstyle",
  "anyhow",
  "assert_fs",
  "bstr",
```

### Comparing `typos-1.20.8/PKG-INFO` & `typos-1.20.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: typos
-Version: 1.20.8
+Version: 1.20.9
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Summary: Source Code Spelling Correction
 Keywords: development,spelling
```

