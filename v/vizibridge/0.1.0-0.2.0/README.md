# Comparing `tmp/vizibridge-0.1.0.tar.gz` & `tmp/vizibridge-0.2.0.tar.gz`

## Comparing `vizibridge-0.1.0.tar` & `vizibridge-0.2.0.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      338 1970-01-01 00:00:00.000000 vizibridge-0.1.0/Cargo.toml
--rw-r--r--   0     1000     1000      705 2024-04-14 15:09:54.000000 vizibridge-0.1.0/.gitignore
--rw-r--r--   0     1000     1000     1695 2024-04-16 15:15:42.000000 vizibridge-0.1.0/.gitlab-ci.yml
--rw-r--r--   0     1000     1000       70 2024-04-15 20:20:32.000000 vizibridge-0.1.0/Dockerfile
--rw-r--r--   0     1000     1000     1073 2024-04-15 07:40:49.000000 vizibridge-0.1.0/LICENSE
--rw-r--r--   0     1000     1000     1236 2024-04-14 15:04:49.000000 vizibridge-0.1.0/python/vizibridge/__init__.py
--rw-r--r--   0     1000     1000       32 2024-04-10 21:12:58.000000 vizibridge-0.1.0/rust-toolchain.toml
--rw-r--r--   0     1000     1000     2747 2024-04-15 11:37:37.000000 vizibridge-0.1.0/src/lib.rs
--rw-r--r--   0     1000     1000     8453 2024-04-14 15:05:40.000000 vizibridge-0.1.0/Cargo.lock
--rw-r--r--   0     1000     1000      514 2024-04-14 16:21:57.000000 vizibridge-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      343 1970-01-01 00:00:00.000000 vizibridge-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      338 1970-01-01 00:00:00.000000 vizibridge-0.2.0/Cargo.toml
+-rw-rw-rw-   0        0        0      705 2024-04-16 20:35:12.000000 vizibridge-0.2.0/.gitignore
+-rw-rw-rw-   0        0        0     1974 2024-04-16 20:35:12.000000 vizibridge-0.2.0/.gitlab-ci.yml
+-rw-rw-rw-   0        0        0       70 2024-04-16 20:35:12.000000 vizibridge-0.2.0/Dockerfile
+-rw-rw-rw-   0        0        0     1073 2024-04-16 20:35:12.000000 vizibridge-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0     1459 2024-04-16 20:35:12.000000 vizibridge-0.2.0/python/vizibridge/__init__.py
+-rw-rw-rw-   0        0        0       32 2024-04-16 20:35:12.000000 vizibridge-0.2.0/rust-toolchain.toml
+-rw-rw-rw-   0        0        0     3018 2024-04-16 20:35:12.000000 vizibridge-0.2.0/src/lib.rs
+-rw-r--r--   0        0        0     8453 2024-04-16 20:35:15.000000 vizibridge-0.2.0/Cargo.lock
+-rw-rw-rw-   0        0        0      514 2024-04-16 20:35:12.000000 vizibridge-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      343 1970-01-01 00:00:00.000000 vizibridge-0.2.0/PKG-INFO
```

### Comparing `vizibridge-0.1.0/.gitignore` & `vizibridge-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `vizibridge-0.1.0/.gitlab-ci.yml` & `vizibridge-0.2.0/.gitlab-ci.yml`

 * *Files 8% similar despite different names*

```diff
@@ -29,14 +29,26 @@
 
   artifacts:
     paths:
         - ./target/wheels/* 
     reports:
       dotenv: generate_executables.env
 
+upload_pypi:
+  stage: release
+  tags:
+    - ci.inria.fr
+    - medium
+  image: "$CI_REGISTRY_IMAGE/vizibridge_cont"
+  rules:
+    - if: $CI_COMMIT_TAG                 # Run this job when a tag is created
+  script:
+    - export MATURIN_PYPI_TOKEN=$PYPI_TOKEN
+    - maturin publish
+
 release_job:
   stage: release
   tags:
     - ci.inria.fr
     - medium
   image: registry.gitlab.com/gitlab-org/release-cli:latest
   rules:
```

### Comparing `vizibridge-0.1.0/LICENSE` & `vizibridge-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `vizibridge-0.1.0/python/vizibridge/__init__.py` & `vizibridge-0.2.0/python/vizibridge/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,27 @@
 from vizibridge._vizibridge import DNA as rust_DNA
+import vizibridge._vizibridge as rust_types
+
 import re
 from typing import Iterator, Self
 
+__all__ = ["DNA", "Kmer"]
+
 non_CGTA = re.compile("[^ACGT]")
 
+Pykmers = [getattr(rust_types, a) for a in dir(rust_types) if a.startswith("PyKmer")]
+
+Kmer = Pykmers[0]
+for t in Pykmers[1:]:
+    Kmer |= t
+
+
 class DNA:
     __slots__ = ("data",)
+
     def __init__(self, data: rust_DNA | str):
         if isinstance(data, str):
             self.data = rust_DNA(data)
         elif isinstance(data, rust_DNA):
             self.data = data
         else:
             raise TypeError(type(data))
@@ -31,13 +43,12 @@
             return type(self)(data)
 
         raise KeyError(__key)
 
     def __repr__(self):
         return repr(self.data)
 
-
     def __len__(self):
         return len(self.data)
 
-    def enum_canonical_kmer(self, k: int):
+    def enum_canonical_kmer(self, k: int) -> Kmer:
         return getattr(self.data, f"enumerate_canonical_kmer{k}")()
```

### Comparing `vizibridge-0.1.0/src/lib.rs` & `vizibridge-0.2.0/src/lib.rs`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 use pyo3::prelude::*;
 use pyo3::types::{PyString, PyType};
 use seq_macro::seq;
 use vizitig_lib::dna::{Nucleotid, DNA};
 use vizitig_lib::iterators::CanonicalKmerIterator;
 use vizitig_lib::kmer::ShortKmer;
 
+
+/// A class wrapper around a DNA struct from vizicomp
 #[pyclass(name = "DNA")]
 pub struct PyDNA {
     pub content: DNA,
 }
 
 seq!(N in 3..=31{
 #[pymethods]
@@ -28,73 +30,83 @@
         Ok(self.content.content.clone().into_iter().map(|u| char::from(u)).collect::<String>())
     }
 
     fn __len__(&self) -> PyResult<usize>{
         Ok(self.content.content.len())
     }
 
+    /// get the Nucleotid as a char at a given index
     pub fn get_index(&self, index: usize) -> PyResult<char>{
         Ok(self.content.content[index].into())
     }
+
+    /// get a slice of the DNA
     pub fn get_slice(&self, start: usize, stop: usize) -> PyResult<Self> {
         Ok(PyDNA {
             content: DNA {
                 content: self.content.content.get(start..stop).unwrap().to_vec()
             }
         })
     }
 
     #(
+
+    /// Enumerate canonical N-kmer
     pub fn enumerate_canonical_kmer~N(&self) -> PyResult<Vec<PyKmer~N>>{
         let it : CanonicalKmerIterator<N, u64> = (&self.content).try_into().unwrap();
         Ok(it.map(|u| PyKmer~N{content: u }).collect())
     }
     )*
 
 }
 });
 
 seq!(N in 3..=31{
-#[pyclass(name="Kmer")]
+/// A Wrapper around an efficient representation of a N-kmer
+#[pyclass]
 #[derive(Clone)]
 pub struct PyKmer~N{
     content: ShortKmer<N>,
 }
 #[pymethods]
 impl PyKmer~N{
+
     #[classmethod]
     fn from_dna(_: &PyType, dna: &PyDNA) -> PyResult<Self>{
         let nucleotids : &[Nucleotid; N] = dna.content.content.first_chunk::<N>().unwrap();
         let kmer : ShortKmer<N> = nucleotids.try_into().unwrap();
-        Ok(PyKmer~N{ content: kmer })
+        Ok(Self { content: kmer })
     }
 
     fn add_left_nucleotid(&self, n: char) -> PyResult<Self>{
-        Ok(PyKmer~N{ content: self.content.append_left(n.try_into().unwrap()) })
+        Ok(Self { content: self.content.append_left(n.try_into().unwrap()) })
     }
 
-
     fn add_right_nucleotid(&self, n: char) -> PyResult<Self>{
-        Ok(PyKmer~N{ content: self.content.append(n.try_into().unwrap()) })
+        Ok(Self { content: self.content.append(n.try_into().unwrap()) })
+    }
+
+    fn __hash__(&self) -> PyResult<u64>{
+        Ok(self.content.get_data())
     }
 
     fn __repr__(&self) -> PyResult<String>{
-        return Ok(format!("{}", &self.content))
+        Ok(format!("{}", &self.content))
     }
 
     fn __str__(&self) -> PyResult<String>{
-        return Ok((&self.content).into())
+        Ok((&self.content).into())
     }
 
     fn __lt__(&self, other: Self) -> PyResult<bool> {
-        return Ok(self.content <= other.content)
+        Ok(self.content <= other.content)
     }
 
     fn __gt__(&self, other: Self) -> PyResult<bool> {
-        return Ok(self.content >= other.content)
+        Ok(self.content >= other.content)
     }
 }
 });
 
 
 seq!(N in 3..=31{
 #[pymodule]
```

### Comparing `vizibridge-0.1.0/Cargo.lock` & `vizibridge-0.2.0/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -96,17 +96,17 @@
 name = "portable-atomic"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7170ef9988bc169ba16dd36a7fa041e5c4cbeb6a35b76d4c03daded371eae7c0"
 
 [[package]]
 name = "proc-macro2"
-version = "1.0.79"
+version = "1.0.80"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e835ff2298f5721608eb1a980ecaee1aef2c132bf95ecc026a11b7bf3c01c02e"
+checksum = "a56dea16b0a29e94408b9aa5e2940a4eedbd128a1ba20e8f7ae60fd3d465af0e"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
 version = "0.20.3"
@@ -204,17 +204,17 @@
 name = "smallvec"
 version = "1.13.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3c5e1a9a646d36c3599cd173a41282daf47c44583ad367b8e6837255952e5c67"
 
 [[package]]
 name = "syn"
-version = "2.0.58"
+version = "2.0.59"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "44cfb93f38070beee36b3fef7d4f5a16f27751d94b187b666a5cc5e9b0d30687"
+checksum = "4a6531ffc7b071655e4ce2e04bd464c4830bb585a61cabb96cf808f05172615a"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
@@ -233,15 +233,15 @@
 name = "unindent"
 version = "0.2.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "c7de7d73e1754487cb58364ee906a499937a0dfabd86bcb980fa99ec8c8fa2ce"
 
 [[package]]
 name = "vizibridge"
-version = "0.1.0"
+version = "0.2.0"
 dependencies = [
  "pyo3",
  "seq-macro",
  "vizitig-lib",
 ]
 
 [[package]]
```

### Comparing `vizibridge-0.1.0/pyproject.toml` & `vizibridge-0.2.0/pyproject.toml`

 * *Files identical despite different names*

