# Comparing `tmp/servicing-0.0.3.tar.gz` & `tmp/servicing-0.0.4.tar.gz`

## Comparing `servicing-0.0.3.tar` & `servicing-0.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0      531 1970-01-01 00:00:00.000000 servicing-0.0.3/Cargo.toml
--rw-r--r--   0     1001      127     3958 2024-04-15 16:45:33.000000 servicing-0.0.3/.github/workflows/cicd.yml
--rw-r--r--   0     1001      127      686 2024-04-15 16:45:33.000000 servicing-0.0.3/.gitignore
--rw-r--r--   0     1001      127      165 2024-04-15 16:45:33.000000 servicing-0.0.3/.vimspector.json
--rw-r--r--   0     1001      127      693 2024-04-15 16:45:33.000000 servicing-0.0.3/README.md
--rw-r--r--   0     1001      127      271 2024-04-15 16:45:33.000000 servicing-0.0.3/build.rs
--rw-r--r--   0     1001      127     2475 2024-04-15 16:45:33.000000 servicing-0.0.3/servicing.pyi
--rw-r--r--   0     1001      127    12113 2024-04-15 16:45:33.000000 servicing-0.0.3/src/dispatcher/mod.rs
--rw-r--r--   0     1001      127     1455 2024-04-15 16:45:33.000000 servicing-0.0.3/src/error/mod.rs
--rw-r--r--   0     1001      127     5533 2024-04-15 16:45:33.000000 servicing-0.0.3/src/helper/mod.rs
--rw-r--r--   0     1001      127      637 2024-04-15 16:45:33.000000 servicing-0.0.3/src/lib.rs
--rw-r--r--   0     1001      127     2596 2024-04-15 16:45:33.000000 servicing-0.0.3/src/models/mod.rs
--rw-r--r--   0     1001      127      302 2024-04-15 16:45:33.000000 servicing-0.0.3/template/service.yaml
--rw-r--r--   0     1001      127    41593 2024-04-15 16:45:38.000000 servicing-0.0.3/Cargo.lock
--rw-r--r--   0     1001      127      390 2024-04-15 16:45:33.000000 servicing-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     1022 1970-01-01 00:00:00.000000 servicing-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0      531 1970-01-01 00:00:00.000000 servicing-0.0.4/Cargo.toml
+-rw-r--r--   0     1001      127     3958 2024-04-15 23:24:02.000000 servicing-0.0.4/.github/workflows/cicd.yml
+-rw-r--r--   0     1001      127      686 2024-04-15 23:24:02.000000 servicing-0.0.4/.gitignore
+-rw-r--r--   0     1001      127      165 2024-04-15 23:24:02.000000 servicing-0.0.4/.vimspector.json
+-rw-r--r--   0     1001      127      693 2024-04-15 23:24:02.000000 servicing-0.0.4/README.md
+-rw-r--r--   0     1001      127      271 2024-04-15 23:24:02.000000 servicing-0.0.4/build.rs
+-rw-r--r--   0     1001      127     2761 2024-04-15 23:24:02.000000 servicing-0.0.4/servicing.pyi
+-rw-r--r--   0     1001      127    12688 2024-04-15 23:24:02.000000 servicing-0.0.4/src/dispatcher/mod.rs
+-rw-r--r--   0     1001      127     1455 2024-04-15 23:24:02.000000 servicing-0.0.4/src/error/mod.rs
+-rw-r--r--   0     1001      127     5533 2024-04-15 23:24:02.000000 servicing-0.0.4/src/helper/mod.rs
+-rw-r--r--   0     1001      127      637 2024-04-15 23:24:02.000000 servicing-0.0.4/src/lib.rs
+-rw-r--r--   0     1001      127     3361 2024-04-15 23:24:02.000000 servicing-0.0.4/src/models/mod.rs
+-rw-r--r--   0     1001      127      302 2024-04-15 23:24:02.000000 servicing-0.0.4/template/service.yaml
+-rw-r--r--   0     1001      127    41832 2024-04-15 23:24:02.000000 servicing-0.0.4/Cargo.lock
+-rw-r--r--   0     1001      127      390 2024-04-15 23:24:02.000000 servicing-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     1022 1970-01-01 00:00:00.000000 servicing-0.0.4/PKG-INFO
```

### Comparing `servicing-0.0.3/Cargo.toml` & `servicing-0.0.4/Cargo.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "servicing"
-version = "0.0.3"
+version = "0.0.4"
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "servicing"
 crate-type = ["cdylib"]
```

### Comparing `servicing-0.0.3/.github/workflows/cicd.yml` & `servicing-0.0.4/.github/workflows/cicd.yml`

 * *Files identical despite different names*

### Comparing `servicing-0.0.3/.gitignore` & `servicing-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `servicing-0.0.3/README.md` & `servicing-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `servicing-0.0.3/servicing.pyi` & `servicing-0.0.4/servicing.pyi`

 * *Files 6% similar despite different names*

```diff
@@ -6,16 +6,20 @@
     UserProvidedConfig is a class that represents the service configuration
 
     :param port: the port on which the service should running
     :param replicas: the number of replicas of the service
     :param cloud: the cloud on which the service should running
     """
 
-    def __init__(self, port: int,
-                 replicas: int, cloud: str) -> None: ...
+    def __init__(self, port: Optional[int] = None,
+                 replicas: Optional[int] = None,
+                 cloud: Optional[str] = None,
+                 workdir: Optional[str] = None,
+                 setup: Optional[str] = None,
+                 run: Optional[str] = None) -> None: ...
 
 
 class Dispatcher:
     """
     Dispatcher is a class that represents the service dispatcher, which is
     responsible for housing all the Servicing functionality
     """
@@ -57,32 +61,33 @@
         Get the status of a service
 
         :param name: the name of the service
         :param pretty: whether to return the status in a pretty format
         :return: the status of the service in string format
         """
 
-    def save(self) -> None:
+    def save(self, location: Optional[str] = None) -> None:
         """
         Save the dispatcher's cache
+
+        :param location: the location of the cache, defaults to home directory
         """
 
     def save_as_b64(self) -> str:
         """
         Save the dispatcher's cache as a base64 string
 
         :return: the base64 string of the cache
         """
 
     def load(self, location: Optional[str] = None) -> None:
         """
         Load the dispatcher's cache
 
-        :param location: the location of the cache
-        :return: the status of the service in string format
+        :param location: the location of the cache, defaults to home directory
         """
 
     def load_as_b64(self, b64: str) -> None:
         """
         Load the dispatcher's cache from a base64 string
 
         :param b64: the base64 string of the cache
```

### Comparing `servicing-0.0.3/src/dispatcher/mod.rs` & `servicing-0.0.4/src/dispatcher/mod.rs`

 * *Files 3% similar despite different names*

```diff
@@ -265,20 +265,31 @@
                 Some(false) => serde_json::to_string(service)?,
                 None => serde_json::to_string(service)?,
             });
         }
         Err(ServicingError::ServiceNotFound(name))
     }
 
-    pub fn save(&self) -> Result<(), ServicingError> {
+    pub fn save(&self, location: Option<PathBuf>) -> Result<(), ServicingError> {
         let bin = bincode::serialize(&*self.service.lock()?)?;
 
         helper::write_to_file_binary(
             &helper::create_file(
-                &helper::create_directory(".servicing", true)?,
+                &{
+                    if let Some(location) = location {
+                        helper::create_directory(
+                            location
+                                .to_str()
+                                .ok_or(ServicingError::General("Location is None".to_string()))?,
+                            false,
+                        )?
+                    } else {
+                        helper::create_directory(".servicing", true)?
+                    }
+                },
                 "services.bin",
             )?,
             &bin,
         )?;
 
         Ok(())
     }
@@ -336,22 +347,25 @@
     #[test]
     fn test_dispatcher() {
         let mut dis = super::Dispatcher::new().unwrap();
 
         dis.add_service(
             "testing".to_string(),
             Some(UserProvidedConfig {
-                port: 1234,
-                replicas: 5,
-                cloud: "aws".to_string(),
+                port: Some(1234),
+                replicas: Some(5),
+                cloud: Some("aws".to_string()),
+                workdir: None,
+                setup: None,
+                run: None,
             }),
         )
         .unwrap();
 
-        dis.save().unwrap();
+        dis.save(None).unwrap();
 
         // check what has been added
         {
             let services = dis.service.lock().unwrap();
             let service = services.get("testing").unwrap();
             assert_eq!(service.template.resources.ports, 1234);
             assert_eq!(service.template.service.replicas, 5);
```

### Comparing `servicing-0.0.3/src/error/mod.rs` & `servicing-0.0.4/src/error/mod.rs`

 * *Files identical despite different names*

### Comparing `servicing-0.0.3/src/helper/mod.rs` & `servicing-0.0.4/src/helper/mod.rs`

 * *Files identical despite different names*

### Comparing `servicing-0.0.3/src/lib.rs` & `servicing-0.0.4/src/lib.rs`

 * *Files identical despite different names*

### Comparing `servicing-0.0.3/src/models/mod.rs` & `servicing-0.0.4/src/models/mod.rs`

 * *Files 22% similar despite different names*

```diff
@@ -1,26 +1,39 @@
 use pyo3::{pyclass, pymethods};
 use serde::{Deserialize, Serialize};
 
 #[pyclass]
 #[derive(Clone, Serialize, Deserialize, Debug)]
 pub struct UserProvidedConfig {
-    pub port: u16,
-    pub replicas: u16,
-    pub cloud: String,
+    pub port: Option<u16>,
+    pub replicas: Option<u16>,
+    pub cloud: Option<String>,
+    pub workdir: Option<String>,
+    pub setup: Option<String>,
+    pub run: Option<String>,
 }
 
 #[pymethods]
 impl UserProvidedConfig {
     #[new]
-    pub fn new(port: u16, replicas: u16, cloud: String) -> Self {
+    pub fn new(
+        port: Option<u16>,
+        replicas: Option<u16>,
+        cloud: Option<String>,
+        workdir: Option<String>,
+        setup: Option<String>,
+        run: Option<String>,
+    ) -> Self {
         UserProvidedConfig {
             port,
             replicas,
             cloud,
+            workdir,
+            setup,
+            run,
         }
     }
 }
 
 #[derive(Serialize, Deserialize, Debug)]
 pub struct Configuration {
     pub service: Service,
@@ -28,17 +41,32 @@
     pub workdir: String,
     pub setup: String,
     pub run: String,
 }
 
 impl Configuration {
     pub fn update(&mut self, config: &UserProvidedConfig) {
-        self.service.replicas = config.replicas;
-        self.resources.ports = config.port;
-        self.resources.cloud = config.cloud.clone();
+        if let Some(port) = config.port {
+            self.resources.ports = port;
+        }
+        if let Some(replicas) = config.replicas {
+            self.service.replicas = replicas;
+        }
+        if let Some(cloud) = &config.cloud {
+            self.resources.cloud = cloud.clone();
+        }
+        if let Some(workdir) = &config.workdir {
+            self.workdir = workdir.clone();
+        }
+        if let Some(setup) = &config.setup {
+            self.setup = setup.clone();
+        }
+        if let Some(run) = &config.run {
+            self.run = run.clone();
+        }
     }
 
     #[allow(dead_code)]
     pub fn test_config() -> Configuration {
         test_config()
     }
 }
```

### Comparing `servicing-0.0.3/Cargo.lock` & `servicing-0.0.4/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -93,20 +93,14 @@
  "miniz_oxide",
  "object",
  "rustc-demangle",
 ]
 
 [[package]]
 name = "base64"
-version = "0.21.7"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "9d297deb1925b89f2ccc13d7635fa0714f12c87adce1c75356b39ca9b7178567"
-
-[[package]]
-name = "base64"
 version = "0.22.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9475866fec1451be56a3c2400fd081ff546538961565ccb5b7142cbd22bc7a51"
 
 [[package]]
 name = "bincode"
 version = "1.3.3"
@@ -126,29 +120,29 @@
 name = "bitflags"
 version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "cf4b9d6a944f767f8e5e0db018570623c85f3d925ac718db4e06d0187adb21c1"
 
 [[package]]
 name = "bumpalo"
-version = "3.15.4"
+version = "3.16.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7ff69b9dd49fd426c69a0db9fc04dd934cdb6645ff000864d98f7e2af8830eaa"
+checksum = "79296716171880943b8470b5f8d03aa55eb2e645a4874bdbb28adb49162e012c"
 
 [[package]]
 name = "bytes"
 version = "1.6.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "514de17de45fdb8dc022b1a7975556c53c86f9f0aa5f534b98977b171857c2c9"
 
 [[package]]
 name = "cc"
-version = "1.0.90"
+version = "1.0.94"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "8cd6604a82acf3039f1144f54b8eb34e91ffba622051189e71b781822d5ee1f5"
+checksum = "17f6e324229dc011159fcc089755d1e2e216a90d43a7dea6853ca740b84f35e7"
 
 [[package]]
 name = "cfg-if"
 version = "1.0.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "baf1de4339761588bc0619e3cbc0120ee582ebb74b53b4efbf79117bd2da40fd"
 
@@ -193,17 +187,17 @@
  "option-ext",
  "redox_users",
  "windows-sys 0.48.0",
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
 name = "env_filter"
 version = "0.1.0"
@@ -316,17 +310,17 @@
  "futures-task",
  "pin-project-lite",
  "pin-utils",
 ]
 
 [[package]]
 name = "getrandom"
-version = "0.2.12"
+version = "0.2.14"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "190092ea657667030ac6a35e305e62fc4dd69fd98ac98631e5d3a2b1575a12b5"
+checksum = "94b22e06ecb0110981051723910cbf0b5f5e09a2062dd7663334ee79a9d1286c"
 dependencies = [
  "cfg-if",
  "libc",
  "wasi",
 ]
 
 [[package]]
@@ -416,17 +410,17 @@
 name = "humantime"
 version = "2.1.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9a3a5bfb195931eeb336b2a7b4d761daec841b97f947d34394601737a7bba5e4"
 
 [[package]]
 name = "hyper"
-version = "1.2.0"
+version = "1.3.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "186548d73ac615b32a73aafe38fb4f56c0d340e110e5a200bcadbaf2e199263a"
+checksum = "9f24ce812868d86d19daa79bf3bf9175bc44ea323391147a5e3abde2a283871b"
 dependencies = [
  "bytes",
  "futures-channel",
  "futures-util",
  "h2",
  "http",
  "http-body",
@@ -770,17 +764,17 @@
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
 version = "0.21.1"
@@ -842,17 +836,17 @@
  "pyo3-build-config",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.35"
+version = "1.0.36"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "291ec9ab5efd934aaf503a6466c5d5251535d108ee747472c3977cc5acc868ef"
+checksum = "0fa76aaf39101c457836aec0ce2316dbdc3ab723cdda1c6bd4e6ad4208acaca7"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "redox_syscall"
 version = "0.4.1"
@@ -900,19 +894,19 @@
 name = "regex-syntax"
 version = "0.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "adad44e29e4c806119491a7f06f03de4d1af22c3a680dd47f1e6e179439d1f56"
 
 [[package]]
 name = "reqwest"
-version = "0.12.2"
+version = "0.12.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "2d66674f2b6fb864665eea7a3c1ac4e3dfacd2fda83cf6f935a612e01b0e3338"
+checksum = "3e6cc1e89e689536eb5aeede61520e874df5a4707df811cd5da4aa5fbb2aae19"
 dependencies = [
- "base64 0.21.7",
+ "base64",
  "bytes",
  "encoding_rs",
  "futures-core",
  "futures-util",
  "h2",
  "http",
  "http-body",
@@ -961,22 +955,29 @@
  "libc",
  "linux-raw-sys",
  "windows-sys 0.52.0",
 ]
 
 [[package]]
 name = "rustls-pemfile"
-version = "1.0.4"
+version = "2.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1c74cae0a4cf6ccbbf5f359f08efdf8ee7e1dc532573bf0db71968cb56b1448c"
+checksum = "29993a25686778eb88d4189742cd713c9bce943bc54251a33509dc63cbacf73d"
 dependencies = [
- "base64 0.21.7",
+ "base64",
+ "rustls-pki-types",
 ]
 
 [[package]]
+name = "rustls-pki-types"
+version = "1.4.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "ecd36cc4259e3e4514335c4a138c6b43171a8d61d8f5c9348f9fc7529416f247"
+
+[[package]]
 name = "ryu"
 version = "1.0.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e86697c916019a8588c99b5fac3cead74ec0b4b819707a682fd4d23fa0ce1ba1"
 
 [[package]]
 name = "schannel"
@@ -1070,17 +1071,17 @@
  "ryu",
  "serde",
  "unsafe-libyaml",
 ]
 
 [[package]]
 name = "servicing"
-version = "0.0.3"
+version = "0.0.4"
 dependencies = [
- "base64 0.22.0",
+ "base64",
  "bincode",
  "dirs",
  "env_logger",
  "log",
  "pyo3",
  "regex",
  "reqwest",
@@ -1123,17 +1124,17 @@
 dependencies = [
  "libc",
  "windows-sys 0.52.0",
 ]
 
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
@@ -1482,15 +1483,15 @@
 
 [[package]]
 name = "windows-sys"
 version = "0.52.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "282be5f36a8ce781fad8c8ae18fa3f9beff57ec1b52cb3de0789201425d9a33d"
 dependencies = [
- "windows-targets 0.52.4",
+ "windows-targets 0.52.5",
 ]
 
 [[package]]
 name = "windows-targets"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9a2fa6e2155d7247be68c096456083145c183cbbbc2764150dda45a87197940c"
@@ -1502,113 +1503,120 @@
  "windows_x86_64_gnu 0.48.5",
  "windows_x86_64_gnullvm 0.48.5",
  "windows_x86_64_msvc 0.48.5",
 ]
 
 [[package]]
 name = "windows-targets"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7dd37b7e5ab9018759f893a1952c9420d060016fc19a472b4bb20d1bdd694d1b"
+checksum = "6f0713a46559409d202e70e28227288446bf7841d3211583a4b53e3f6d96e7eb"
 dependencies = [
- "windows_aarch64_gnullvm 0.52.4",
- "windows_aarch64_msvc 0.52.4",
- "windows_i686_gnu 0.52.4",
- "windows_i686_msvc 0.52.4",
- "windows_x86_64_gnu 0.52.4",
- "windows_x86_64_gnullvm 0.52.4",
- "windows_x86_64_msvc 0.52.4",
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
 name = "windows_aarch64_gnullvm"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "bcf46cf4c365c6f2d1cc93ce535f2c8b244591df96ceee75d8e83deb70a9cac9"
+checksum = "7088eed71e8b8dda258ecc8bac5fb1153c5cffaf2578fc8ff5d61e23578d3263"
 
 [[package]]
 name = "windows_aarch64_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "dc35310971f3b2dbbf3f0690a219f40e2d9afcf64f9ab7cc1be722937c26b4bc"
 
 [[package]]
 name = "windows_aarch64_msvc"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "da9f259dd3bcf6990b55bffd094c4f7235817ba4ceebde8e6d11cd0c5633b675"
+checksum = "9985fd1504e250c615ca5f281c3f7a6da76213ebd5ccc9561496568a2752afb6"
 
 [[package]]
 name = "windows_i686_gnu"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a75915e7def60c94dcef72200b9a8e58e5091744960da64ec734a6c6e9b3743e"
 
 [[package]]
 name = "windows_i686_gnu"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b474d8268f99e0995f25b9f095bc7434632601028cf86590aea5c8a5cb7801d3"
+checksum = "88ba073cf16d5372720ec942a8ccbf61626074c6d4dd2e745299726ce8b89670"
+
+[[package]]
+name = "windows_i686_gnullvm"
+version = "0.52.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "87f4261229030a858f36b459e748ae97545d6f1ec60e5e0d6a3d32e0dc232ee9"
 
 [[package]]
 name = "windows_i686_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "8f55c233f70c4b27f66c523580f78f1004e8b5a8b659e05a4eb49d4166cca406"
 
 [[package]]
 name = "windows_i686_msvc"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1515e9a29e5bed743cb4415a9ecf5dfca648ce85ee42e15873c3cd8610ff8e02"
+checksum = "db3c2bf3d13d5b658be73463284eaf12830ac9a26a90c717b7f771dfe97487bf"
 
 [[package]]
 name = "windows_x86_64_gnu"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "53d40abd2583d23e4718fddf1ebec84dbff8381c07cae67ff7768bbf19c6718e"
 
 [[package]]
 name = "windows_x86_64_gnu"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5eee091590e89cc02ad514ffe3ead9eb6b660aedca2183455434b93546371a03"
+checksum = "4e4246f76bdeff09eb48875a0fd3e2af6aada79d409d33011886d3e1581517d9"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0b7b52767868a23d5bab768e390dc5f5c55825b6d30b86c844ff2dc7414044cc"
 
 [[package]]
 name = "windows_x86_64_gnullvm"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "77ca79f2451b49fa9e2af39f0747fe999fcda4f5e241b2898624dca97a1f2177"
+checksum = "852298e482cd67c356ddd9570386e2862b5673c85bd5f88df9ab6802b334c596"
 
 [[package]]
 name = "windows_x86_64_msvc"
 version = "0.48.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ed94fce61571a4006852b7389a063ab983c02eb1bb37b47f8272ce92d06d9538"
 
 [[package]]
 name = "windows_x86_64_msvc"
-version = "0.52.4"
+version = "0.52.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "32b752e52a2da0ddfbdbcc6fceadfeede4c939ed16d13e648833a61dfb611ed8"
+checksum = "bec47e5bfd1bff0eeaf6d8b485cc1074891a197ab4225d504cb7a1ab88b02bf0"
 
 [[package]]
 name = "winreg"
-version = "0.50.0"
+version = "0.52.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "524e57b2c537c0f9b1e69f1965311ec12182b4122e45035b1508cd24d2adadb1"
+checksum = "a277a57398d4bfa075df44f501a17cfdf8542d224f0d36095a2adc7aee4ef0a5"
 dependencies = [
  "cfg-if",
  "windows-sys 0.48.0",
 ]
```

### Comparing `servicing-0.0.3/PKG-INFO` & `servicing-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: servicing
-Version: 0.0.3
+Version: 0.0.4
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
 ### SERVICING: a small binary aimed at service configuration and cluster deployment for OPENAD
```

