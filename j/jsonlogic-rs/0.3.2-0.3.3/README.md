# Comparing `tmp/jsonlogic-rs-0.3.2.tar.gz` & `tmp/jsonlogic_rs-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsonlogic-rs-0.3.2.tar", last modified: Sat Jul 22 13:48:27 2023, max compression
+gzip compressed data, was "jsonlogic_rs-0.3.3.tar", last modified: Tue Apr 16 04:27:21 2024, max compression
```

## Comparing `jsonlogic-rs-0.3.2.tar` & `jsonlogic_rs-0.3.3.tar`

### file list

```diff
@@ -1,33 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 13:48:27.451334 jsonlogic-rs-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-07-22 13:47:30.000000 jsonlogic-rs-0.3.2/Cargo.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-07-22 13:47:30.000000 jsonlogic-rs-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-07-22 13:47:30.000000 jsonlogic-rs-0.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    10460 2023-07-22 13:48:27.451334 jsonlogic-rs-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9354 2023-07-22 13:47:30.000000 jsonlogic-rs-0.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 13:48:27.451334 jsonlogic-rs-0.3.2/py/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 13:48:27.451334 jsonlogic-rs-0.3.2/py/jsonlogic_rs/
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-07-22 13:47:30.000000 jsonlogic-rs-0.3.2/py/jsonlogic_rs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 13:48:27.451334 jsonlogic-rs-0.3.2/py/jsonlogic_rs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10460 2023-07-22 13:48:27.000000 jsonlogic-rs-0.3.2/py/jsonlogic_rs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-07-22 13:48:27.000000 jsonlogic-rs-0.3.2/py/jsonlogic_rs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 13:48:27.000000 jsonlogic-rs-0.3.2/py/jsonlogic_rs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-07-22 13:48:27.000000 jsonlogic-rs-0.3.2/py/jsonlogic_rs.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-07-22 13:48:27.000000 jsonlogic-rs-0.3.2/py/jsonlogic_rs.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-07-22 13:47:30.000000 jsonlogic-rs-0.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-07-22 13:48:27.451334 jsonlogic-rs-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3011 2023-07-22 13:47:30.000000 jsonlogic-rs-0.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 13:48:27.451334 jsonlogic-rs-0.3.2/src/
--rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-07-22 13:47:30.000000 jsonlogic-rs-0.3.2/src/bin.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1247 2023-07-22 13:47:30.000000 jsonlogic-rs-0.3.2/src/error.rs
--rw-r--r--   0 runner    (1001) docker     (123)      870 2023-07-22 13:47:30.000000 jsonlogic-rs-0.3.2/src/func.rs
--rw-r--r--   0 runner    (1001) docker     (123)    41847 2023-07-22 13:47:30.000000 jsonlogic-rs-0.3.2/src/js_op.rs
--rw-r--r--   0 runner    (1001) docker     (123)    48168 2023-07-22 13:47:30.000000 jsonlogic-rs-0.3.2/src/lib.rs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-07-22 13:48:27.451334 jsonlogic-rs-0.3.2/src/op/
--rw-r--r--   0 runner    (1001) docker     (123)    14230 2023-07-22 13:47:30.000000 jsonlogic-rs-0.3.2/src/op/array.rs
--rw-r--r--   0 runner    (1001) docker     (123)     8976 2023-07-22 13:47:30.000000 jsonlogic-rs-0.3.2/src/op/data.rs
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-07-22 13:47:30.000000 jsonlogic-rs-0.3.2/src/op/impure.rs
--rw-r--r--   0 runner    (1001) docker     (123)     6828 2023-07-22 13:47:30.000000 jsonlogic-rs-0.3.2/src/op/logic.rs
--rw-r--r--   0 runner    (1001) docker     (123)    17078 2023-07-22 13:47:30.000000 jsonlogic-rs-0.3.2/src/op/mod.rs
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-07-22 13:47:30.000000 jsonlogic-rs-0.3.2/src/op/numeric.rs
--rw-r--r--   0 runner    (1001) docker     (123)     5685 2023-07-22 13:47:30.000000 jsonlogic-rs-0.3.2/src/op/string.rs
--rw-r--r--   0 runner    (1001) docker     (123)     3414 2023-07-22 13:47:30.000000 jsonlogic-rs-0.3.2/src/value.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:27:21.806041 jsonlogic_rs-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1322 2024-04-16 04:26:51.000000 jsonlogic_rs-0.3.3/Cargo.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-16 04:26:51.000000 jsonlogic_rs-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-16 04:26:51.000000 jsonlogic_rs-0.3.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    10522 2024-04-16 04:27:21.806041 jsonlogic_rs-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9365 2024-04-16 04:26:51.000000 jsonlogic_rs-0.3.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:27:21.802041 jsonlogic_rs-0.3.3/py/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:27:21.802041 jsonlogic_rs-0.3.3/py/jsonlogic_rs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1163 2024-04-16 04:26:51.000000 jsonlogic_rs-0.3.3/py/jsonlogic_rs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:27:21.806041 jsonlogic_rs-0.3.3/py/jsonlogic_rs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10522 2024-04-16 04:27:21.000000 jsonlogic_rs-0.3.3/py/jsonlogic_rs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      499 2024-04-16 04:27:21.000000 jsonlogic_rs-0.3.3/py/jsonlogic_rs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 04:27:21.000000 jsonlogic_rs-0.3.3/py/jsonlogic_rs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 04:27:21.000000 jsonlogic_rs-0.3.3/py/jsonlogic_rs.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-16 04:27:21.000000 jsonlogic_rs-0.3.3/py/jsonlogic_rs.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      133 2024-04-16 04:26:51.000000 jsonlogic_rs-0.3.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-16 04:27:21.806041 jsonlogic_rs-0.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3063 2024-04-16 04:26:51.000000 jsonlogic_rs-0.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:27:21.806041 jsonlogic_rs-0.3.3/src/
+-rw-r--r--   0 runner    (1001) docker     (127)     2195 2024-04-16 04:26:51.000000 jsonlogic_rs-0.3.3/src/bin.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1247 2024-04-16 04:26:51.000000 jsonlogic_rs-0.3.3/src/error.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      870 2024-04-16 04:26:51.000000 jsonlogic_rs-0.3.3/src/func.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    41847 2024-04-16 04:26:51.000000 jsonlogic_rs-0.3.3/src/js_op.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    48168 2024-04-16 04:26:51.000000 jsonlogic_rs-0.3.3/src/lib.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:27:21.806041 jsonlogic_rs-0.3.3/src/op/
+-rw-r--r--   0 runner    (1001) docker     (127)    14230 2024-04-16 04:26:51.000000 jsonlogic_rs-0.3.3/src/op/array.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     8976 2024-04-16 04:26:51.000000 jsonlogic_rs-0.3.3/src/op/data.rs
+-rw-r--r--   0 runner    (1001) docker     (127)      423 2024-04-16 04:26:51.000000 jsonlogic_rs-0.3.3/src/op/impure.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     6828 2024-04-16 04:26:51.000000 jsonlogic_rs-0.3.3/src/op/logic.rs
+-rw-r--r--   0 runner    (1001) docker     (127)    17078 2024-04-16 04:26:51.000000 jsonlogic_rs-0.3.3/src/op/mod.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     1269 2024-04-16 04:26:51.000000 jsonlogic_rs-0.3.3/src/op/numeric.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     5685 2024-04-16 04:26:51.000000 jsonlogic_rs-0.3.3/src/op/string.rs
+-rw-r--r--   0 runner    (1001) docker     (127)     3414 2024-04-16 04:26:51.000000 jsonlogic_rs-0.3.3/src/value.rs
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 04:27:21.806041 jsonlogic_rs-0.3.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      935 2024-04-16 04:26:51.000000 jsonlogic_rs-0.3.3/tests/test_py.py
```

### Comparing `jsonlogic-rs-0.3.2/Cargo.toml` & `jsonlogic_rs-0.3.3/Cargo.toml`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 edition = "2018"
 homepage = "https://github.com/bestowinc/json-logic-rs"
 keywords = ["json", "jsonlogic", "s-expressions", "web", "logic"]
 license = "MIT"
 name = "jsonlogic-rs"
 readme = "README.md"
 repository = "https://github.com/bestowinc/json-logic-rs"
-version = "0.3.2"
+version = "0.3.3"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 
 [lib]
 # cdylib for CFFI and python integration
 # lib for regular rust stuff
 crate-type = ["cdylib", "lib"]
```

### Comparing `jsonlogic-rs-0.3.2/LICENSE` & `jsonlogic_rs-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `jsonlogic-rs-0.3.2/PKG-INFO` & `jsonlogic_rs-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsonlogic-rs
-Version: 0.3.2
+Version: 0.3.3
 Summary: JsonLogic implemented with a Rust backend
 Home-page: https://www.github.com/bestowinc/json-logic-rs
 Author: Matthew Planchard
 Author-email: msplanchard@gmail.com
 Maintainer-email: msplanchard@gmail.com
 Keywords: json,jsonlogic,s-expressions,rust
 Classifier: Development Status :: 5 - Production/Stable
@@ -17,14 +17,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Rust
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # json-logic-rs
 
 ![Continuous Integration](https://github.com/Bestowinc/json-logic-rs/workflows/Continuous%20Integration/badge.svg?branch=master)
@@ -49,15 +50,15 @@
 Being built in Rust, we are able to provide the package in a variety of
 languages. The table below describes current language support:
 
 | **Language**         | **Available Via**                                                          |
 | -------------------- | -------------------------------------------------------------------------- |
 | Rust                 | [Cargo](https://crates.io/crates/jsonlogic-rs)                             |
 | JavaScript (as WASM) | Node Package via [NPM](https://www.npmjs.com/package/@bestow/jsonlogic-rs) |
-| Python               | [PyPI](https://pypi.org/project/jsonlogic-rs/)                  |
+| Python               | [PyPI](https://pypi.org/project/jsonlogic-rs/)                             |
 
 ## Installation
 
 ### Rust
 
 To use as a Rust library, add to your `Cargo.toml`:
 
@@ -81,15 +82,15 @@
 ```
 
 Note that the package is distributed as a node package, so you'll need to use
 `browserify`, `webpack`, or similar to install for the browser.
 
 ### Python
 
-Supports Python 3.6+.
+Supports Python 3.7+.
 
 Wheels are distributed for many platforms, so you can often just run:
 
 ``` sh
 pip install jsonlogic-rs
 ```
 
@@ -226,15 +227,15 @@
 
 ## Building
 
 ### Prerequisites
 
 You must have Rust installed and `cargo` available in your `PATH`.
 
-If you would like to build or test the Python distribution, Python 3.6 or
+If you would like to build or test the Python distribution, Python 3.7 or
 newer must be available in your `PATH`. The `venv` module must be part of the
 Python distribution (looking at you, Ubuntu).
 
 If you would like to run tests for the WASM package, `node` 10 or newer must be
 available in your `PATH`.
 
 ### Rust
```

### Comparing `jsonlogic-rs-0.3.2/README.md` & `jsonlogic_rs-0.3.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 Being built in Rust, we are able to provide the package in a variety of
 languages. The table below describes current language support:
 
 | **Language**         | **Available Via**                                                          |
 | -------------------- | -------------------------------------------------------------------------- |
 | Rust                 | [Cargo](https://crates.io/crates/jsonlogic-rs)                             |
 | JavaScript (as WASM) | Node Package via [NPM](https://www.npmjs.com/package/@bestow/jsonlogic-rs) |
-| Python               | [PyPI](https://pypi.org/project/jsonlogic-rs/)                  |
+| Python               | [PyPI](https://pypi.org/project/jsonlogic-rs/)                             |
 
 ## Installation
 
 ### Rust
 
 To use as a Rust library, add to your `Cargo.toml`:
 
@@ -54,15 +54,15 @@
 ```
 
 Note that the package is distributed as a node package, so you'll need to use
 `browserify`, `webpack`, or similar to install for the browser.
 
 ### Python
 
-Supports Python 3.6+.
+Supports Python 3.7+.
 
 Wheels are distributed for many platforms, so you can often just run:
 
 ``` sh
 pip install jsonlogic-rs
 ```
 
@@ -199,15 +199,15 @@
 
 ## Building
 
 ### Prerequisites
 
 You must have Rust installed and `cargo` available in your `PATH`.
 
-If you would like to build or test the Python distribution, Python 3.6 or
+If you would like to build or test the Python distribution, Python 3.7 or
 newer must be available in your `PATH`. The `venv` module must be part of the
 Python distribution (looking at you, Ubuntu).
 
 If you would like to run tests for the WASM package, `node` 10 or newer must be
 available in your `PATH`.
 
 ### Rust
```

### Comparing `jsonlogic-rs-0.3.2/py/jsonlogic_rs/__init__.py` & `jsonlogic_rs-0.3.3/py/jsonlogic_rs/__init__.py`

 * *Files identical despite different names*

### Comparing `jsonlogic-rs-0.3.2/py/jsonlogic_rs.egg-info/PKG-INFO` & `jsonlogic_rs-0.3.3/py/jsonlogic_rs.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsonlogic-rs
-Version: 0.3.2
+Version: 0.3.3
 Summary: JsonLogic implemented with a Rust backend
 Home-page: https://www.github.com/bestowinc/json-logic-rs
 Author: Matthew Planchard
 Author-email: msplanchard@gmail.com
 Maintainer-email: msplanchard@gmail.com
 Keywords: json,jsonlogic,s-expressions,rust
 Classifier: Development Status :: 5 - Production/Stable
@@ -17,14 +17,15 @@
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Rust
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # json-logic-rs
 
 ![Continuous Integration](https://github.com/Bestowinc/json-logic-rs/workflows/Continuous%20Integration/badge.svg?branch=master)
@@ -49,15 +50,15 @@
 Being built in Rust, we are able to provide the package in a variety of
 languages. The table below describes current language support:
 
 | **Language**         | **Available Via**                                                          |
 | -------------------- | -------------------------------------------------------------------------- |
 | Rust                 | [Cargo](https://crates.io/crates/jsonlogic-rs)                             |
 | JavaScript (as WASM) | Node Package via [NPM](https://www.npmjs.com/package/@bestow/jsonlogic-rs) |
-| Python               | [PyPI](https://pypi.org/project/jsonlogic-rs/)                  |
+| Python               | [PyPI](https://pypi.org/project/jsonlogic-rs/)                             |
 
 ## Installation
 
 ### Rust
 
 To use as a Rust library, add to your `Cargo.toml`:
 
@@ -81,15 +82,15 @@
 ```
 
 Note that the package is distributed as a node package, so you'll need to use
 `browserify`, `webpack`, or similar to install for the browser.
 
 ### Python
 
-Supports Python 3.6+.
+Supports Python 3.7+.
 
 Wheels are distributed for many platforms, so you can often just run:
 
 ``` sh
 pip install jsonlogic-rs
 ```
 
@@ -226,15 +227,15 @@
 
 ## Building
 
 ### Prerequisites
 
 You must have Rust installed and `cargo` available in your `PATH`.
 
-If you would like to build or test the Python distribution, Python 3.6 or
+If you would like to build or test the Python distribution, Python 3.7 or
 newer must be available in your `PATH`. The `venv` module must be part of the
 Python distribution (looking at you, Ubuntu).
 
 If you would like to run tests for the WASM package, `node` 10 or newer must be
 available in your `PATH`.
 
 ### Rust
```

### Comparing `jsonlogic-rs-0.3.2/setup.py` & `jsonlogic_rs-0.3.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 from pathlib import Path
+from subprocess import PIPE, Popen
+
 from setuptools import setup
 from setuptools_rust import Binding, RustExtension
-from subprocess import Popen, PIPE
 
 PKG_ROOT = Path(__file__).parent
 SETUP_REQUIRES = ["setuptools-rust", "wheel", "setuptools"]
 SHORT_DESCRIPTION = "JsonLogic implemented with a Rust backend"
 URL = "https://www.github.com/bestowinc/json-logic-rs"
 AUTHOR = "Matthew Planchard"
 EMAIL = "msplanchard@gmail.com"
@@ -17,14 +18,15 @@
     print("Generating Cargo lockfile")
     proc = Popen(("cargo", "generate-lockfile"), stdout=PIPE, stderr=PIPE)
     _out, err = tuple(map(bytes.decode, proc.communicate()))
     if proc.returncode != 0:
         raise RuntimeError(f"Could not generate Cargo lockfile: {err}")
     return
 
+
 def get_version():
     generate_lockfile()
     proc = Popen(("cargo", "pkgid"), stdout=PIPE, stderr=PIPE)
     out, err = tuple(map(bytes.decode, proc.communicate()))
     if proc.returncode != 0:
         raise RuntimeError(f"Could not get Cargo package info: {err}")
     version = out.split("@")[-1]
@@ -47,28 +49,29 @@
     description=SHORT_DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     keywords=["json", "jsonlogic", "s-expressions", "rust"],
     classifiers=[
         # See https://pypi.python.org/pypi?%3Aaction=list_classifiers for all
         # available setup classifiers
-        'Development Status :: 5 - Production/Stable',
+        "Development Status :: 5 - Production/Stable",
         "Intended Audience :: Developers",
         "License :: OSI Approved :: MIT License",
         "Natural Language :: English",
         "Operating System :: POSIX :: Linux",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
         "Programming Language :: Python :: 3.11",
+        "Programming Language :: Python :: 3.12",
         "Programming Language :: Rust",
         # 'Programming Language :: Python :: Implementation :: PyPy',
     ],
     rust_extensions=[
         RustExtension(
             # Python package name before the dot, name of C extension to
             # stick inside of it after the dot.
```

### Comparing `jsonlogic-rs-0.3.2/src/bin.rs` & `jsonlogic_rs-0.3.3/src/bin.rs`

 * *Files identical despite different names*

### Comparing `jsonlogic-rs-0.3.2/src/error.rs` & `jsonlogic_rs-0.3.3/src/error.rs`

 * *Files identical despite different names*

### Comparing `jsonlogic-rs-0.3.2/src/func.rs` & `jsonlogic_rs-0.3.3/src/func.rs`

 * *Files identical despite different names*

### Comparing `jsonlogic-rs-0.3.2/src/js_op.rs` & `jsonlogic_rs-0.3.3/src/js_op.rs`

 * *Files identical despite different names*

### Comparing `jsonlogic-rs-0.3.2/src/lib.rs` & `jsonlogic_rs-0.3.3/src/lib.rs`

 * *Files identical despite different names*

### Comparing `jsonlogic-rs-0.3.2/src/op/array.rs` & `jsonlogic_rs-0.3.3/src/op/array.rs`

 * *Files identical despite different names*

### Comparing `jsonlogic-rs-0.3.2/src/op/data.rs` & `jsonlogic_rs-0.3.3/src/op/data.rs`

 * *Files identical despite different names*

### Comparing `jsonlogic-rs-0.3.2/src/op/logic.rs` & `jsonlogic_rs-0.3.3/src/op/logic.rs`

 * *Files identical despite different names*

### Comparing `jsonlogic-rs-0.3.2/src/op/mod.rs` & `jsonlogic_rs-0.3.3/src/op/mod.rs`

 * *Files identical despite different names*

### Comparing `jsonlogic-rs-0.3.2/src/op/numeric.rs` & `jsonlogic_rs-0.3.3/src/op/numeric.rs`

 * *Files identical despite different names*

### Comparing `jsonlogic-rs-0.3.2/src/op/string.rs` & `jsonlogic_rs-0.3.3/src/op/string.rs`

 * *Files identical despite different names*

### Comparing `jsonlogic-rs-0.3.2/src/value.rs` & `jsonlogic_rs-0.3.3/src/value.rs`

 * *Files identical despite different names*

