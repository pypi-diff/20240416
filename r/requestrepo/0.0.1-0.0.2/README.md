# Comparing `tmp/requestrepo-0.0.1.tar.gz` & `tmp/requestrepo-0.0.2.tar.gz`

## Comparing `requestrepo-0.0.1.tar` & `requestrepo-0.0.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 requestrepo-0.0.1/requirements.txt
--rw-r--r--   0        0        0     4814 2020-02-02 00:00:00.000000 requestrepo-0.0.1/src/requestrepo/__init__.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 requestrepo-0.0.1/.gitignore
--rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 requestrepo-0.0.1/LICENSE
--rw-r--r--   0        0        0     1274 2020-02-02 00:00:00.000000 requestrepo-0.0.1/README.md
--rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 requestrepo-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1804 2020-02-02 00:00:00.000000 requestrepo-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 requestrepo-0.0.2/requirements.txt
+-rw-r--r--   0        0        0     4814 2020-02-02 00:00:00.000000 requestrepo-0.0.2/src/requestrepo/__init__.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 requestrepo-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1064 2020-02-02 00:00:00.000000 requestrepo-0.0.2/LICENSE
+-rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 requestrepo-0.0.2/README.md
+-rw-r--r--   0        0        0      580 2020-02-02 00:00:00.000000 requestrepo-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2221 2020-02-02 00:00:00.000000 requestrepo-0.0.2/PKG-INFO
```

### Comparing `requestrepo-0.0.1/src/requestrepo/__init__.py` & `requestrepo-0.0.2/src/requestrepo/__init__.py`

 * *Files identical despite different names*

### Comparing `requestrepo-0.0.1/.gitignore` & `requestrepo-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `requestrepo-0.0.1/LICENSE` & `requestrepo-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `requestrepo-0.0.1/README.md` & `requestrepo-0.0.2/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,61 +1,82 @@
-## requestrepo Python client
+# requestrepo Python client
 
 Python bindings to automate requestrepo.com
 
-**Installation**
+## Installation
 
 ```bash
 pip install requestrepo
 ```
 
-**Basic Usage**
+## Basic Usage
 
-1. **Instantiate the `Requestrepo` class:**
+**Instantiate the `Requestrepo` class:**
 
 ```python
 from requestrepo import Requestrepo  # Requestrepo, RequestRepo and requestrepo are accepted imports
 
-client = Requestrepo() # if token is not provided via the constructor or REQUESTREPO_TOKEN environment variable, a new one will be generated and printed to stderr
+client = Requestrepo() # new token printed to console
 client = Requestrepo("your-token-here")
 ```
 
-or
+or via environment variables:
 
 ```bash
 REQUESTREPO_TOKEN=token python your_script.py
 ```
 
-**Examples**
+## Examples
 
 **Example 1: Async request retrieval via `on_request`**
 
 ```python
 from requestrepo import Requestrepo
 
 def on_request(request_data: dict):
    print("New Request Received:", request_data)
 
 client = Requestrepo(token="your-token-here")
 
+print(client.subdomain) # abcd1234
+print(client.domain) # abcd1234.requestrepo.com
+
 client.await_requests()
 ```
 
 **Example 2: Synchronous request retrieval**
 
 ```python
 from requestrepo import Requestrepo
 
 client = Requestrepo(token="your_api_token")
 
+print(client.subdomain) # abcd1234
+print(client.domain) # abcd1234.requestrepo.com
+
 # Get the latest request (blocks until one is received)
 new_request = client.get_request()
 print("Latest Request:", new_request)
 ```
 
-**Contributing**
+**Example 3: Retrieve old requests**
+
+You can iterate over all requests that are stored on the server:
+
+```python
+from requestrepo import Requestrepo
+
+client = Requestrepo(token="your_api_token")
+
+for request in client.get_old_requests():
+    print("Request:", request)
+
+client.delete_all_requests() # clear all requests on the server
+```
+
+## Contributing
 
 Contributions are welcome! Please submit a pull request or open an issue if you have any ideas or suggestions.
 
-**License**
+## License
 
 MIT
```

### Comparing `requestrepo-0.0.1/pyproject.toml` & `requestrepo-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "requestrepo"
-version = "0.0.1"
+version = "0.0.2"
 authors = [{ name = "Dragos Albastroiu", email = "adragos@protonmail.com" }]
 description = "Python bindings to automate requestrepo.com"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
   "Programming Language :: Python :: 3",
   "License :: OSI Approved :: MIT License",
```

### Comparing `requestrepo-0.0.1/PKG-INFO` & `requestrepo-0.0.2/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,75 +1,96 @@
 Metadata-Version: 2.3
 Name: requestrepo
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python bindings to automate requestrepo.com
 Project-URL: Homepage, https://github.com/adrgs/requestrepo-lib
 Project-URL: Issues, https://github.com/adrgs/requestrepo-lib/issues
 Author-email: Dragos Albastroiu <adragos@protonmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
-## requestrepo Python client
+# requestrepo Python client
 
 Python bindings to automate requestrepo.com
 
-**Installation**
+## Installation
 
 ```bash
 pip install requestrepo
 ```
 
-**Basic Usage**
+## Basic Usage
 
-1. **Instantiate the `Requestrepo` class:**
+**Instantiate the `Requestrepo` class:**
 
 ```python
 from requestrepo import Requestrepo  # Requestrepo, RequestRepo and requestrepo are accepted imports
 
-client = Requestrepo() # if token is not provided via the constructor or REQUESTREPO_TOKEN environment variable, a new one will be generated and printed to stderr
+client = Requestrepo() # new token printed to console
 client = Requestrepo("your-token-here")
 ```
 
-or
+or via environment variables:
 
 ```bash
 REQUESTREPO_TOKEN=token python your_script.py
 ```
 
-**Examples**
+## Examples
 
 **Example 1: Async request retrieval via `on_request`**
 
 ```python
 from requestrepo import Requestrepo
 
 def on_request(request_data: dict):
    print("New Request Received:", request_data)
 
 client = Requestrepo(token="your-token-here")
 
+print(client.subdomain) # abcd1234
+print(client.domain) # abcd1234.requestrepo.com
+
 client.await_requests()
 ```
 
 **Example 2: Synchronous request retrieval**
 
 ```python
 from requestrepo import Requestrepo
 
 client = Requestrepo(token="your_api_token")
 
+print(client.subdomain) # abcd1234
+print(client.domain) # abcd1234.requestrepo.com
+
 # Get the latest request (blocks until one is received)
 new_request = client.get_request()
 print("Latest Request:", new_request)
 ```
 
-**Contributing**
+**Example 3: Retrieve old requests**
+
+You can iterate over all requests that are stored on the server:
+
+```python
+from requestrepo import Requestrepo
+
+client = Requestrepo(token="your_api_token")
+
+for request in client.get_old_requests():
+    print("Request:", request)
+
+client.delete_all_requests() # clear all requests on the server
+```
+
+## Contributing
 
 Contributions are welcome! Please submit a pull request or open an issue if you have any ideas or suggestions.
 
-**License**
+## License
 
 MIT
```

