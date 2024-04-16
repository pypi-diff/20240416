# Comparing `tmp/pyreqwest_impersonate-0.1.3.tar.gz` & `tmp/pyreqwest_impersonate-0.2.0.tar.gz`

## Comparing `pyreqwest_impersonate-0.1.3.tar` & `pyreqwest_impersonate-0.2.0.tar`

### file list

```diff
@@ -1,9 +1,16 @@
--rw-r--r--   0        0        0      904 1970-01-01 00:00:00.000000 pyreqwest_impersonate-0.1.3/Cargo.toml
--rw-r--r--   0     1001      127     5415 2024-04-14 14:21:37.000000 pyreqwest_impersonate-0.1.3/.github/workflows/CI.yml
--rw-r--r--   0     1001      127      686 2024-04-14 14:21:37.000000 pyreqwest_impersonate-0.1.3/.gitignore
--rw-r--r--   0     1001      127     5578 2024-04-14 14:21:37.000000 pyreqwest_impersonate-0.1.3/README.md
--rw-r--r--   0     1001      127    17152 2024-04-14 14:21:37.000000 pyreqwest_impersonate-0.1.3/src/lib.rs
--rw-r--r--   0     1001      127     3203 2024-04-14 14:21:37.000000 pyreqwest_impersonate-0.1.3/tests/test_client.py
--rw-r--r--   0     1001      127    46966 2024-04-14 14:21:37.000000 pyreqwest_impersonate-0.1.3/Cargo.lock
--rw-r--r--   0     1001      127     1067 2024-04-14 14:21:37.000000 pyreqwest_impersonate-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     6580 1970-01-01 00:00:00.000000 pyreqwest_impersonate-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      972 1970-01-01 00:00:00.000000 pyreqwest_impersonate-0.2.0/Cargo.toml
+-rw-r--r--   0     1001      127     5412 2024-04-16 14:52:28.000000 pyreqwest_impersonate-0.2.0/.github/workflows/CI.yml
+-rw-r--r--   0     1001      127      686 2024-04-16 14:52:28.000000 pyreqwest_impersonate-0.2.0/.gitignore
+-rw-r--r--   0     1001      127     7516 2024-04-16 14:52:28.000000 pyreqwest_impersonate-0.2.0/README.md
+-rw-r--r--   0     1001      127      248 2024-04-16 14:52:28.000000 pyreqwest_impersonate-0.2.0/benchmark/1_threads.csv
+-rw-r--r--   0     1001      127      249 2024-04-16 14:52:28.000000 pyreqwest_impersonate-0.2.0/benchmark/4_threads.csv
+-rw-r--r--   0     1001      127      343 2024-04-16 14:52:28.000000 pyreqwest_impersonate-0.2.0/benchmark/README.md
+-rw-r--r--   0     1001      127     3072 2024-04-16 14:52:28.000000 pyreqwest_impersonate-0.2.0/benchmark/benchmark.py
+-rw-r--r--   0     1001      127       83 2024-04-16 14:52:28.000000 pyreqwest_impersonate-0.2.0/benchmark/requirements.txt
+-rw-r--r--   0     1001      127      799 2024-04-16 14:52:28.000000 pyreqwest_impersonate-0.2.0/benchmark/server.py
+-rw-r--r--   0     1001      127    17347 2024-04-16 14:52:28.000000 pyreqwest_impersonate-0.2.0/src/lib.rs
+-rw-r--r--   0     1001      127     6559 2024-04-16 14:52:28.000000 pyreqwest_impersonate-0.2.0/src/response.rs
+-rw-r--r--   0     1001      127     3203 2024-04-16 14:52:28.000000 pyreqwest_impersonate-0.2.0/tests/test_client.py
+-rw-r--r--   0     1001      127    47243 2024-04-16 14:52:28.000000 pyreqwest_impersonate-0.2.0/Cargo.lock
+-rw-r--r--   0     1001      127     1261 2024-04-16 14:52:28.000000 pyreqwest_impersonate-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     8638 1970-01-01 00:00:00.000000 pyreqwest_impersonate-0.2.0/PKG-INFO
```

### Comparing `pyreqwest_impersonate-0.1.3/Cargo.toml` & `pyreqwest_impersonate-0.2.0/Cargo.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "pyreqwest_impersonate"
-version = "0.1.3"
+version = "0.2.0"
 edition = "2021"
 description = "HTTP client that can impersonate web browsers, mimicking their headers and `TLS/JA3/JA4/HTTP2` fingerprints"
 authors = ["deedy5"]
 
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
@@ -14,21 +14,25 @@
 [dependencies]
 pyo3 = { version = "0.21", features = ["extension-module"] }
 reqwest-impersonate = { version = "0.11", default-features = false, features = [
     "cookies",
     "blocking",
     "boring-tls",
     "impersonate",
+    "json",
     "trust-dns",  # async resolver instead of a default threadpool using `getaddrinfo`
     "multipart",  # to send a multipart/form-data body
     "socks",
     "gzip",
     "brotli",
     "deflate",
 ] }
+encoding_rs = "0.8"
+pythonize = "0.21"
+serde_json = "1"
 
 [profile.release]
 codegen-units = 1
 lto = "fat"
 opt-level = 3
 panic = "abort"
 strip = "symbols"
```

### Comparing `pyreqwest_impersonate-0.1.3/.github/workflows/CI.yml` & `pyreqwest_impersonate-0.2.0/.github/workflows/CI.yml`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 #
 name: CI
 
 on:
   push:
     branches:
       - main
-      - master
+      - '*'
     tags:
       - '*'
   pull_request:
   workflow_dispatch:
 
 permissions:
   contents: read
```

### Comparing `pyreqwest_impersonate-0.1.3/.gitignore` & `pyreqwest_impersonate-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pyreqwest_impersonate-0.1.3/src/lib.rs` & `pyreqwest_impersonate-0.2.0/src/lib.rs`

 * *Files 3% similar despite different names*

```diff
@@ -1,31 +1,21 @@
+use std::collections::HashMap;
+use std::str::FromStr;
+use std::time::Duration;
+
 use pyo3::exceptions;
 use pyo3::prelude::*;
 use reqwest_impersonate::blocking::multipart;
 use reqwest_impersonate::header::{HeaderMap, HeaderName, HeaderValue};
 use reqwest_impersonate::impersonate::Impersonate;
 use reqwest_impersonate::redirect::Policy;
 use reqwest_impersonate::Method;
-use std::collections::HashMap;
-use std::str::FromStr;
-use std::time::Duration;
 
-#[pyclass]
-struct Response {
-    #[pyo3(get)]
-    cookies: HashMap<String, String>,
-    #[pyo3(get)]
-    headers: HashMap<String, String>,
-    #[pyo3(get)]
-    status_code: u16,
-    #[pyo3(get)]
-    text: String,
-    #[pyo3(get)]
-    url: String,
-}
+mod response;
+use response::Response;
 
 #[pyclass]
 /// A blocking HTTP client that can impersonate web browsers.
 struct Client {
     client: reqwest_impersonate::blocking::Client,
     auth: Option<(String, Option<String>)>,
     auth_bearer: Option<String>,
@@ -204,126 +194,119 @@
         content: Option<Vec<u8>>,
         data: Option<HashMap<String, String>>,
         files: Option<HashMap<String, String>>,
         auth: Option<(String, Option<String>)>,
         auth_bearer: Option<String>,
         timeout: Option<f64>,
     ) -> PyResult<Response> {
-        let is_post_put_patch = method == "POST" || method == "PUT" || method == "PATCH";
-
-        // Method
-        let method = match method {
-            "GET" => Ok(Method::GET),
-            "POST" => Ok(Method::POST),
-            "HEAD" => Ok(Method::HEAD),
-            "OPTIONS" => Ok(Method::OPTIONS),
-            "PUT" => Ok(Method::PUT),
-            "PATCH" => Ok(Method::PATCH),
-            "DELETE" => Ok(Method::DELETE),
-            &_ => Err(PyErr::new::<exceptions::PyException, _>(
-                "Unrecognized HTTP method",
-            )),
-        };
-        let method = method?;
-
-        // Create request builder
-        let mut request_builder = self.client.request(method, url);
-
-        // Params (use the provided `params` if available; otherwise, fall back to `self.params`)
-        let params_to_use = params.or(self.params.clone()).unwrap_or_default();
-        if !params_to_use.is_empty() {
-            request_builder = request_builder.query(&params_to_use);
-        }
+        Python::with_gil(|py| {
+            // Release the gil
+            py.allow_threads(|| {
+                // Check if method is POST || PUT || PATCH
+                let is_post_put_patch = method == "POST" || method == "PUT" || method == "PATCH";
+
+                // Method
+                let method = match method {
+                    "GET" => Ok(Method::GET),
+                    "POST" => Ok(Method::POST),
+                    "HEAD" => Ok(Method::HEAD),
+                    "OPTIONS" => Ok(Method::OPTIONS),
+                    "PUT" => Ok(Method::PUT),
+                    "PATCH" => Ok(Method::PATCH),
+                    "DELETE" => Ok(Method::DELETE),
+                    &_ => Err(PyErr::new::<exceptions::PyException, _>(
+                        "Unrecognized HTTP method",
+                    )),
+                };
+                let method = method?;
+
+                // Create request builder
+                let mut request_builder = self.client.request(method, url);
+
+                // Params (use the provided `params` if available; otherwise, fall back to `self.params`)
+                let params_to_use = params.or(self.params.clone()).unwrap_or_default();
+                if !params_to_use.is_empty() {
+                    request_builder = request_builder.query(&params_to_use);
+                }
 
-        // Headers
-        if let Some(headers) = headers {
-            let mut headers_new = HeaderMap::new();
-            for (key, value) in headers {
-                headers_new.insert(
-                    HeaderName::from_bytes(key.as_bytes()).map_err(|_| {
-                        PyErr::new::<exceptions::PyValueError, _>("Invalid header name")
-                    })?,
-                    HeaderValue::from_str(&value).map_err(|_| {
-                        PyErr::new::<exceptions::PyValueError, _>("Invalid header value")
-                    })?,
-                );
-            }
-            request_builder = request_builder.headers(headers_new);
-        }
+                // Headers
+                if let Some(headers) = headers {
+                    let mut headers_new = HeaderMap::new();
+                    for (key, value) in headers {
+                        headers_new.insert(
+                            HeaderName::from_bytes(key.as_bytes()).map_err(|_| {
+                                PyErr::new::<exceptions::PyValueError, _>("Invalid header name")
+                            })?,
+                            HeaderValue::from_str(&value).map_err(|_| {
+                                PyErr::new::<exceptions::PyValueError, _>("Invalid header value")
+                            })?,
+                        );
+                    }
+                    request_builder = request_builder.headers(headers_new);
+                }
 
-        // Only if method POST || PUT || PATCH
-        if is_post_put_patch {
-            // Content
-            if let Some(content) = content {
-                request_builder = request_builder.body(content);
-            }
-            // Data
-            if let Some(data) = data {
-                request_builder = request_builder.form(&data);
-            }
-            // Files
-            if let Some(files) = files {
-                let mut form = multipart::Form::new();
-                for (field, path) in files {
-                    form = form.file(field, path)?;
+                // Only if method POST || PUT || PATCH
+                if is_post_put_patch {
+                    // Content
+                    if let Some(content) = content {
+                        request_builder = request_builder.body(content);
+                    }
+                    // Data
+                    if let Some(data) = data {
+                        request_builder = request_builder.form(&data);
+                    }
+                    // Files
+                    if let Some(files) = files {
+                        let mut form = multipart::Form::new();
+                        for (field, path) in files {
+                            form = form.file(field, path)?;
+                        }
+                        request_builder = request_builder.multipart(form);
+                    }
                 }
-                request_builder = request_builder.multipart(form);
-            }
-        }
 
-        // Auth
-        match (auth, auth_bearer, &self.auth, &self.auth_bearer) {
-            (Some((username, password)), None, _, _) => {
-                request_builder = request_builder.basic_auth(username, password.as_deref());
-            }
-            (None, Some(token), _, _) => {
-                request_builder = request_builder.bearer_auth(token);
-            }
-            (None, None, Some((username, password)), None) => {
-                request_builder = request_builder.basic_auth(username, password.as_deref());
-            }
-            (None, None, None, Some(token)) => {
-                request_builder = request_builder.bearer_auth(token);
-            }
-            (Some(_), Some(_), None, None) | (None, None, Some(_), Some(_)) => {
-                return Err(PyErr::new::<exceptions::PyValueError, _>(
-                    "Cannot provide both auth and auth_bearer",
-                ));
-            }
-            _ => {} // No authentication provided
-        }
+                // Auth
+                match (auth, auth_bearer, &self.auth, &self.auth_bearer) {
+                    (Some((username, password)), None, _, _) => {
+                        request_builder = request_builder.basic_auth(username, password.as_deref());
+                    }
+                    (None, Some(token), _, _) => {
+                        request_builder = request_builder.bearer_auth(token);
+                    }
+                    (None, None, Some((username, password)), None) => {
+                        request_builder = request_builder.basic_auth(username, password.as_deref());
+                    }
+                    (None, None, None, Some(token)) => {
+                        request_builder = request_builder.bearer_auth(token);
+                    }
+                    (Some(_), Some(_), None, None) | (None, None, Some(_), Some(_)) => {
+                        return Err(PyErr::new::<exceptions::PyValueError, _>(
+                            "Cannot provide both auth and auth_bearer",
+                        ));
+                    }
+                    _ => {} // No authentication provided
+                }
 
-        // Timeout
-        if let Some(seconds) = timeout {
-            request_builder = request_builder.timeout(Duration::from_secs_f64(seconds));
-        }
+                // Timeout
+                if let Some(seconds) = timeout {
+                    request_builder = request_builder.timeout(Duration::from_secs_f64(seconds));
+                }
 
-        // Send request
-        let resp = request_builder.send().map_err(|e| {
-            PyErr::new::<exceptions::PyException, _>(format!("Error in request: {}", e))
-        })?;
-        let cookies: HashMap<String, String> = resp
-            .cookies()
-            .map(|cookie| (cookie.name().to_string(), cookie.value().to_string()))
-            .collect();
-        let headers = resp
-            .headers()
-            .iter()
-            .map(|(k, v)| (k.as_str().to_string(), v.to_str().unwrap_or("").to_string()))
-            .collect();
-        let status_code = resp.status().as_u16();
-        let url = resp.url().to_string();
-        let text = resp.text().unwrap_or_else(|_| String::new());
-
-        Ok(Response {
-            cookies,
-            headers,
-            status_code,
-            text,
-            url,
+                // Send request
+                let resp = request_builder.send().map_err(|e| {
+                    PyErr::new::<exceptions::PyException, _>(format!("Error in request: {}", e))
+                })?;
+
+                Ok(Response {
+                    resp,
+                    encoding: "utf-8".to_string(),
+                    _content_as_vec: None,
+                    _text: None,
+                })
+            })
         })
     }
 
     fn get(
         &self,
         url: &str,
         params: Option<HashMap<String, String>>,
```

### Comparing `pyreqwest_impersonate-0.1.3/tests/test_client.py` & `pyreqwest_impersonate-0.2.0/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `pyreqwest_impersonate-0.1.3/Cargo.lock` & `pyreqwest_impersonate-0.2.0/Cargo.lock`

 * *Files 0% similar despite different names*

```diff
@@ -707,15 +707,15 @@
 [[package]]
 name = "libloading"
 version = "0.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0c2a198fb6b0eada2a8df47933734e6d35d350665a33a3593d7164fa52c75c19"
 dependencies = [
  "cfg-if",
- "windows-targets 0.48.5",
+ "windows-targets 0.52.4",
 ]
 
 [[package]]
 name = "linked-hash-map"
 version = "0.5.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0717cef1bc8b636c6e1c1bbdefc09e6322da8a9321966e8928ef80d20f7f770f"
@@ -1003,18 +1003,31 @@
  "pyo3-build-config",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "pyreqwest_impersonate"
-version = "0.1.3"
+version = "0.2.0"
 dependencies = [
+ "encoding_rs",
  "pyo3",
+ "pythonize",
  "reqwest-impersonate",
+ "serde_json",
+]
+
+[[package]]
+name = "pythonize"
+version = "0.21.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "9d0664248812c38cc55a4ed07f88e4df516ce82604b93b1ffdc041aa77a6cb3c"
+dependencies = [
+ "pyo3",
+ "serde",
 ]
 
 [[package]]
 name = "quick-error"
 version = "1.2.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "a1d01941d82fa2ab50be1e79e6714289dd7cde78eba4c074bc5a4374f650dfe0"
```

### Comparing `pyreqwest_impersonate-0.1.3/pyproject.toml` & `pyreqwest_impersonate-0.2.0/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -22,9 +22,23 @@
     "Programming Language :: Python :: 3.12",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: PyPy",
     "Topic :: Internet :: WWW/HTTP",
     "Topic :: Software Development :: Libraries :: Python Modules",
 ]
 dynamic = ["version"]
+
+dependencies = []
+
+[project.optional-dependencies]
+dev = [
+    "pytest>=8.1.1",
+    "pytest-retry>=1.6.2",
+]
+
 [tool.maturin]
 features = ["pyo3/extension-module"]
+
+[tool.pytest.ini_options]
+retries = 3
+retry_delay = 0.5
+cumulative_timing = false
```

### Comparing `pyreqwest_impersonate-0.1.3/PKG-INFO` & `pyreqwest_impersonate-0.2.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,40 +1,54 @@
 Metadata-Version: 2.3
 Name: pyreqwest_impersonate
-Version: 0.1.3
+Version: 0.2.0
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Internet :: WWW/HTTP
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
+Requires-Dist: pytest >=8.1.1 ; extra == 'dev'
+Requires-Dist: pytest-retry >=1.6.2 ; extra == 'dev'
+Provides-Extra: dev
 Summary: HTTP client that can impersonate web browsers, mimicking their headers and `TLS/JA3/JA4/HTTP2` fingerprints
 Keywords: python,request,impersonate
 Author: deedy5
 License: MIT License
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
 
 ![Python >= 3.8](https://img.shields.io/badge/python->=3.8-red.svg) [![](https://badgen.net/github/release/deedy5/pyreqwest-impersonate)](https://github.com/deedy5/pyreqwest-impersonate/releases) [![](https://badge.fury.io/py/pyreqwest_impersonate.svg)](https://pypi.org/project/pyreqwest_impersonate) [![Downloads](https://static.pepy.tech/badge/pyreqwest_impersonate/week)](https://pepy.tech/project/pyreqwest_impersonate) [![CI](https://github.com/deedy5/pyreqwest-impersonate/actions/workflows/CI.yml/badge.svg?branch=main)](https://github.com/deedy5/pyreqwest-impersonate/actions/workflows/CI.yml)
 # Pyreqwest_impersonate
 
-HTTP client that can impersonate web browsers, mimicking their headers and `TLS/JA3/JA4/HTTP2` fingerprints.</br>
-Binding to the Rust `reqwest_impersonate` library.
+The fastest python HTTP client that can impersonate web browsers by mimicking their headers and `TLS/JA3/JA4/HTTP2` fingerprints.</br>
+Binding to the Rust `reqwest_impersonate` library.</br>
+🏁 Check the benchmarks for more details.
+
 
 Provides precompiled wheels:
 - [x] Linux:  `amd64`, `aarch64`.
 - [x] Windows: `amd64`.
 - [x] MacOS:  `amd64`, `aarch64`.
 
+## Table of Contents
+
+- [Installation](#installation)
+- [Usage](#usage)
+ - [I. Client](#i-client)
+ - [II. AsyncClient](#ii-asyncclient)
+ - [III. Response Object](#iii-response-object)
+
+
 ## Installation
 
 ```python
 pip install -U pyreqwest_impersonate
 ```
 
 ## Usage
@@ -63,15 +77,15 @@
         max_redirects (int, optional): Maximum redirects to follow. Default 20. Applies if `follow_redirects` is True.
         verify (bool, optional): Verify SSL certificates. Default is True.
         http1 (bool, optional): Use only HTTP/1.1. Default is None.
         http2 (bool, optional): Use only HTTP/2. Default is None.
     """
 ```
 
-### Client Methods
+#### Client Methods
 
 The `Client` class provides a set of methods for making HTTP requests: `get`, `head`, `options`, `delete`, `post`, `put`, `patch`, each of which internally utilizes the `request()` method for execution. The parameters for these methods closely resemble those in `httpx`.
 ```python
 get(url, *, params=None, headers=None, auth=None, auth_bearer=None, timeout=None)
 
 Performs a GET request to the specified URL.
 
@@ -94,33 +108,64 @@
 - data (Optional[Dict[str, str]]): The form data to send in the request body. Default is None.
 - files (Optional[Dict[str, str]]): A map of file fields to file paths to be sent as multipart/form-data. Default is None.
 - auth (Optional[Tuple[str, Optional[str]]]): A tuple containing the username and an optional password for basic authentication. Default is None.
 - auth_bearer (Optional[str]): A string representing the bearer token for bearer token authentication. Default is None.
 - timeout (Optional[float]): The timeout for the request in seconds. Default is 30.
 ```
 
-#### Examples:
+#### Example
 
-_Client.get()_
 ```python
 from pyreqwest_impersonate import Client
 
 client = Client(impersonate="chrome_123")
+
+# get request
 resp = client.get("https://tls.peet.ws/api/all")
-print(resp.text)
-print(resp.status_code)
-print(resp.url)
-print(resp.headers)
-print(resp.cookies)
-```
-_Client.post()_
-```python
-from pyreqwest_impersonate import Client
+print(resp.json())
 
+# post request
 data = {"key1": "value1", "key2": "value2"}
 auth = ("user", "password")
-resp = Client().post(url="https://httpbin.org/anything", data=data, auth=auth)
+resp = client.post(url="https://httpbin.org/anything", data=data, auth=auth)
 print(resp.text)
 ```
 ### II. AsyncClient
 
 TODO
+
+### III. Response Object
+
+#### Key Features
+
+- `High Performance`: The attributes of the `Response` object are executed in Rust, which is known for its high performance. This ensures that operations like accessing headers, decoding text, or parsing JSON are very fast.
+- `Lazy Execution`: All attributes of the `Response` object are executed lazily. This means that the actual computation or data retrieval happens only when you access the attribute, not when the `Response` object is created. This approach optimizes performance by avoiding unnecessary computations.
+- `Automatic Character Encoding Detection`: The `Response` object intelligently detects the character encoding of the response body from the "Content-Type" header. If the encoding is not specified, it defaults to "UTF-8".
+
+#### Response attributes and methods
+
+- `cookies`: Fetches the cookies from the response as a dictionary.
+- `headers`: Retrieves the headers from the response as a dictionary.
+- `status_code`: Gets the status code of the response as an integer.
+- `url`: Returns the URL of the response as a string.
+- `content`: Provides the content of the response as bytes.
+- `text`: Decodes the response body into text, automatically detecting the character encoding.
+- `json()`: Parses the response body as JSON, converting it into a Python object for easy manipulation.
+
+#### Example
+
+```python
+from pyreqwest_impersonate import Client
+
+client = Client()
+
+response = client.get("https://example.com")
+
+print(response.status_code)  # Access the status code
+print(response.url)  # Access the URL
+print(response.headers)  # Access headers
+print(response.cookies)  # Access cookies
+print(response.content)  # Get the content as bytes
+print(response.text)  # Decode the content as text
+print(response.json())  # Parse the content as JSON
+```
+
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

