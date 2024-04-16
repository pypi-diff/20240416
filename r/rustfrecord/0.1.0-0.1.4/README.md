# Comparing `tmp/rustfrecord-0.1.0.tar.gz` & `tmp/rustfrecord-0.1.4.tar.gz`

## Comparing `rustfrecord-0.1.0.tar` & `rustfrecord-0.1.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      818 1970-01-01 00:00:00.000000 rustfrecord-0.1.0/Cargo.toml
--rw-r--r--   0     1001      127     1341 2024-04-16 12:05:31.000000 rustfrecord-0.1.0/.devcontainer/devcontainer.json
--rw-r--r--   0     1001      127     5102 2024-04-16 12:05:31.000000 rustfrecord-0.1.0/.github/workflows/CI.yml
--rw-r--r--   0     1001      127       85 2024-04-16 12:05:31.000000 rustfrecord-0.1.0/.gitignore
--rw-r--r--   0     1001      127      166 2024-04-16 12:05:31.000000 rustfrecord-0.1.0/.vscode/settings.json
--rw-r--r--   0     1001      127      230 2024-04-16 12:05:31.000000 rustfrecord-0.1.0/README.md
--rw-r--r--   0     1001      127      634 2024-04-16 12:05:31.000000 rustfrecord-0.1.0/main.py
--rw-r--r--   0     1001      127     2536 2024-04-16 12:05:31.000000 rustfrecord-0.1.0/requirements-linux.txt
--rw-r--r--   0     1001      127      508 2024-04-16 12:05:31.000000 rustfrecord-0.1.0/requirements-macos.txt
--rw-r--r--   0     1001      127     1163 2024-04-16 12:05:31.000000 rustfrecord-0.1.0/src/lib.rs
--rw-r--r--   0     1001      127     1571 2024-04-16 12:05:31.000000 rustfrecord-0.1.0/src/pyo3_tch.rs
--rw-r--r--   0     1001      127     1951 2024-04-16 12:05:31.000000 rustfrecord-0.1.0/src/tfrecord_reader.rs
--rw-r--r--   0     1001      127    45986 2024-04-16 12:05:31.000000 rustfrecord-0.1.0/Cargo.lock
--rw-r--r--   0     1001      127      571 2024-04-16 12:05:31.000000 rustfrecord-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      715 1970-01-01 00:00:00.000000 rustfrecord-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      898 1970-01-01 00:00:00.000000 rustfrecord-0.1.4/Cargo.toml
+-rw-r--r--   0      502       20     1341 2024-04-11 08:51:17.000000 rustfrecord-0.1.4/.devcontainer/devcontainer.json
+-rw-r--r--   0      502       20     5102 2024-04-16 11:33:55.000000 rustfrecord-0.1.4/.github/workflows/CI.yml
+-rw-r--r--   0      502       20       85 2024-04-15 12:50:52.000000 rustfrecord-0.1.4/.gitignore
+-rw-r--r--   0      502       20      166 2024-04-15 10:44:23.000000 rustfrecord-0.1.4/.vscode/settings.json
+-rw-r--r--   0      502       20     1507 2024-04-16 13:52:52.000000 rustfrecord-0.1.4/README.md
+-rw-r--r--   0      502       20      634 2024-04-11 18:53:31.000000 rustfrecord-0.1.4/main.py
+-rw-r--r--   0      502       20     2536 2024-04-15 13:20:59.000000 rustfrecord-0.1.4/requirements-linux.txt
+-rw-r--r--   0      502       20      508 2024-04-15 13:20:18.000000 rustfrecord-0.1.4/requirements-macos.txt
+-rw-r--r--   0      502       20     1163 2024-04-15 11:11:32.000000 rustfrecord-0.1.4/src/lib.rs
+-rw-r--r--   0      502       20     1571 2024-04-11 10:57:05.000000 rustfrecord-0.1.4/src/pyo3_tch.rs
+-rw-r--r--   0      502       20     1951 2024-04-15 10:17:58.000000 rustfrecord-0.1.4/src/tfrecord_reader.rs
+-rw-r--r--   0      502       20    45986 2024-04-16 14:00:24.000000 rustfrecord-0.1.4/Cargo.lock
+-rw-r--r--   0      502       20      571 2024-04-16 07:56:44.000000 rustfrecord-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     1992 1970-01-01 00:00:00.000000 rustfrecord-0.1.4/PKG-INFO
```

### Comparing `rustfrecord-0.1.0/Cargo.toml` & `rustfrecord-0.1.4/Cargo.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 [package]
 name = "rustfrecord"
-version = "0.1.0"
+version = "0.1.4"
+description = "Rust implementation to read TFRecord files into PyTorch tensors"
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "rustfrecord"
 crate-type = ["cdylib"]
```

### Comparing `rustfrecord-0.1.0/.devcontainer/devcontainer.json` & `rustfrecord-0.1.4/.devcontainer/devcontainer.json`

 * *Files identical despite different names*

### Comparing `rustfrecord-0.1.0/.github/workflows/CI.yml` & `rustfrecord-0.1.4/.github/workflows/CI.yml`

 * *Files identical despite different names*

### Comparing `rustfrecord-0.1.0/main.py` & `rustfrecord-0.1.4/main.py`

 * *Files identical despite different names*

### Comparing `rustfrecord-0.1.0/requirements-linux.txt` & `rustfrecord-0.1.4/requirements-linux.txt`

 * *Files identical despite different names*

### Comparing `rustfrecord-0.1.0/src/lib.rs` & `rustfrecord-0.1.4/src/lib.rs`

 * *Files identical despite different names*

### Comparing `rustfrecord-0.1.0/src/pyo3_tch.rs` & `rustfrecord-0.1.4/src/pyo3_tch.rs`

 * *Files identical despite different names*

### Comparing `rustfrecord-0.1.0/src/tfrecord_reader.rs` & `rustfrecord-0.1.4/src/tfrecord_reader.rs`

 * *Files identical despite different names*

### Comparing `rustfrecord-0.1.0/Cargo.lock` & `rustfrecord-0.1.4/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -1158,15 +1158,15 @@
 name = "rustc-demangle"
 version = "0.1.23"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "d626bb9dae77e28219937af045c257c28bfd3f69333c512553507f5f9798cb76"
 
 [[package]]
 name = "rustfrecord"
-version = "0.1.0"
+version = "0.1.4"
 dependencies = [
  "anyhow",
  "flate2",
  "pyo3",
  "tch",
  "tfrecord",
  "torch-sys",
```

### Comparing `rustfrecord-0.1.0/pyproject.toml` & `rustfrecord-0.1.4/pyproject.toml`

 * *Files identical despite different names*

