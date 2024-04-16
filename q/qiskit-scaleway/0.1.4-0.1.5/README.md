# Comparing `tmp/qiskit_scaleway-0.1.4.tar.gz` & `tmp/qiskit_scaleway-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qiskit_scaleway-0.1.4.tar", last modified: Thu Apr 11 09:28:53 2024, max compression
+gzip compressed data, was "qiskit_scaleway-0.1.5.tar", last modified: Tue Apr 16 12:39:04 2024, max compression
```

## Comparing `qiskit_scaleway-0.1.4.tar` & `qiskit_scaleway-0.1.5.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxrwxr-x   0 valentin  (1000) valentin  (1000)        0 2024-04-11 09:28:53.771495 qiskit_scaleway-0.1.4/
--rw-rw-r--   0 valentin  (1000) valentin  (1000)    11357 2024-02-29 13:51:39.000000 qiskit_scaleway-0.1.4/LICENSE
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     1525 2024-04-11 09:28:53.771495 qiskit_scaleway-0.1.4/PKG-INFO
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     1330 2024-04-10 08:10:14.000000 qiskit_scaleway-0.1.4/README.md
-drwxrwxr-x   0 valentin  (1000) valentin  (1000)        0 2024-04-11 09:28:53.771495 qiskit_scaleway-0.1.4/qiskit_scaleway/
--rw-rw-r--   0 valentin  (1000) valentin  (1000)       39 2024-04-03 12:51:52.000000 qiskit_scaleway-0.1.4/qiskit_scaleway/__init__.py
-drwxrwxr-x   0 valentin  (1000) valentin  (1000)        0 2024-04-11 09:28:53.771495 qiskit_scaleway-0.1.4/qiskit_scaleway/backends/
--rw-rw-r--   0 valentin  (1000) valentin  (1000)      178 2024-04-10 08:10:14.000000 qiskit_scaleway-0.1.4/qiskit_scaleway/backends/__init__.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     4951 2024-04-10 08:10:14.000000 qiskit_scaleway-0.1.4/qiskit_scaleway/backends/aer_backend.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     3504 2024-04-10 09:37:46.000000 qiskit_scaleway-0.1.4/qiskit_scaleway/backends/aer_job.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     2877 2024-04-10 08:10:14.000000 qiskit_scaleway-0.1.4/qiskit_scaleway/backends/qsim_backend.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     9781 2024-04-10 09:26:04.000000 qiskit_scaleway-0.1.4/qiskit_scaleway/backends/qsim_job.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     1892 2024-04-10 08:10:14.000000 qiskit_scaleway-0.1.4/qiskit_scaleway/backends/scaleway_backend.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     2041 2024-04-10 09:26:04.000000 qiskit_scaleway-0.1.4/qiskit_scaleway/backends/scaleway_job.py
-drwxrwxr-x   0 valentin  (1000) valentin  (1000)        0 2024-04-11 09:28:53.771495 qiskit_scaleway-0.1.4/qiskit_scaleway/primitives/
--rw-rw-r--   0 valentin  (1000) valentin  (1000)       70 2024-04-10 08:10:14.000000 qiskit_scaleway-0.1.4/qiskit_scaleway/primitives/__init__.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)      740 2024-04-10 08:10:14.000000 qiskit_scaleway-0.1.4/qiskit_scaleway/primitives/aer_estimator.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)      568 2024-04-10 08:10:14.000000 qiskit_scaleway-0.1.4/qiskit_scaleway/primitives/aer_sampler.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     2532 2024-04-10 08:10:14.000000 qiskit_scaleway-0.1.4/qiskit_scaleway/provider.py
-drwxrwxr-x   0 valentin  (1000) valentin  (1000)        0 2024-04-11 09:28:53.771495 qiskit_scaleway-0.1.4/qiskit_scaleway/utils/
--rw-rw-r--   0 valentin  (1000) valentin  (1000)       31 2024-04-03 12:51:52.000000 qiskit_scaleway-0.1.4/qiskit_scaleway/utils/__init__.py
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     4057 2024-04-03 12:51:52.000000 qiskit_scaleway-0.1.4/qiskit_scaleway/utils/client.py
-drwxrwxr-x   0 valentin  (1000) valentin  (1000)        0 2024-04-11 09:28:53.771495 qiskit_scaleway-0.1.4/qiskit_scaleway.egg-info/
--rw-rw-r--   0 valentin  (1000) valentin  (1000)     1525 2024-04-11 09:28:53.000000 qiskit_scaleway-0.1.4/qiskit_scaleway.egg-info/PKG-INFO
--rw-rw-r--   0 valentin  (1000) valentin  (1000)      744 2024-04-11 09:28:53.000000 qiskit_scaleway-0.1.4/qiskit_scaleway.egg-info/SOURCES.txt
--rw-rw-r--   0 valentin  (1000) valentin  (1000)        1 2024-04-11 09:28:53.000000 qiskit_scaleway-0.1.4/qiskit_scaleway.egg-info/dependency_links.txt
--rw-rw-r--   0 valentin  (1000) valentin  (1000)      127 2024-04-11 09:28:53.000000 qiskit_scaleway-0.1.4/qiskit_scaleway.egg-info/requires.txt
--rw-rw-r--   0 valentin  (1000) valentin  (1000)       16 2024-04-11 09:28:53.000000 qiskit_scaleway-0.1.4/qiskit_scaleway.egg-info/top_level.txt
--rw-rw-r--   0 valentin  (1000) valentin  (1000)       38 2024-04-11 09:28:53.771495 qiskit_scaleway-0.1.4/setup.cfg
--rw-rw-r--   0 valentin  (1000) valentin  (1000)      514 2024-04-10 09:25:44.000000 qiskit_scaleway-0.1.4/setup.py
+drwxrwxr-x   0 valentin  (1000) valentin  (1000)        0 2024-04-16 12:39:04.186541 qiskit_scaleway-0.1.5/
+-rw-rw-r--   0 valentin  (1000) valentin  (1000)    11357 2024-02-29 13:51:39.000000 qiskit_scaleway-0.1.5/LICENSE
+-rw-rw-r--   0 valentin  (1000) valentin  (1000)     2178 2024-04-16 12:39:04.186541 qiskit_scaleway-0.1.5/PKG-INFO
+-rw-rw-r--   0 valentin  (1000) valentin  (1000)     1983 2024-04-16 12:36:19.000000 qiskit_scaleway-0.1.5/README.md
+drwxrwxr-x   0 valentin  (1000) valentin  (1000)        0 2024-04-16 12:39:04.182541 qiskit_scaleway-0.1.5/qiskit_scaleway/
+-rw-rw-r--   0 valentin  (1000) valentin  (1000)       39 2024-04-03 12:51:52.000000 qiskit_scaleway-0.1.5/qiskit_scaleway/__init__.py
+drwxrwxr-x   0 valentin  (1000) valentin  (1000)        0 2024-04-16 12:39:04.186541 qiskit_scaleway-0.1.5/qiskit_scaleway/backends/
+-rw-rw-r--   0 valentin  (1000) valentin  (1000)      178 2024-04-10 08:10:14.000000 qiskit_scaleway-0.1.5/qiskit_scaleway/backends/__init__.py
+-rw-rw-r--   0 valentin  (1000) valentin  (1000)     5083 2024-04-16 12:36:19.000000 qiskit_scaleway-0.1.5/qiskit_scaleway/backends/aer_backend.py
+-rw-rw-r--   0 valentin  (1000) valentin  (1000)     3504 2024-04-10 09:37:46.000000 qiskit_scaleway-0.1.5/qiskit_scaleway/backends/aer_job.py
+-rw-rw-r--   0 valentin  (1000) valentin  (1000)     3010 2024-04-16 12:36:19.000000 qiskit_scaleway-0.1.5/qiskit_scaleway/backends/qsim_backend.py
+-rw-rw-r--   0 valentin  (1000) valentin  (1000)     9781 2024-04-10 09:26:04.000000 qiskit_scaleway-0.1.5/qiskit_scaleway/backends/qsim_job.py
+-rw-rw-r--   0 valentin  (1000) valentin  (1000)     1892 2024-04-10 08:10:14.000000 qiskit_scaleway-0.1.5/qiskit_scaleway/backends/scaleway_backend.py
+-rw-rw-r--   0 valentin  (1000) valentin  (1000)     2041 2024-04-10 09:26:04.000000 qiskit_scaleway-0.1.5/qiskit_scaleway/backends/scaleway_job.py
+drwxrwxr-x   0 valentin  (1000) valentin  (1000)        0 2024-04-16 12:39:04.186541 qiskit_scaleway-0.1.5/qiskit_scaleway/primitives/
+-rw-rw-r--   0 valentin  (1000) valentin  (1000)       70 2024-04-10 08:10:14.000000 qiskit_scaleway-0.1.5/qiskit_scaleway/primitives/__init__.py
+-rw-rw-r--   0 valentin  (1000) valentin  (1000)      740 2024-04-10 08:10:14.000000 qiskit_scaleway-0.1.5/qiskit_scaleway/primitives/aer_estimator.py
+-rw-rw-r--   0 valentin  (1000) valentin  (1000)      568 2024-04-10 08:10:14.000000 qiskit_scaleway-0.1.5/qiskit_scaleway/primitives/aer_sampler.py
+-rw-rw-r--   0 valentin  (1000) valentin  (1000)     2532 2024-04-10 08:10:14.000000 qiskit_scaleway-0.1.5/qiskit_scaleway/provider.py
+drwxrwxr-x   0 valentin  (1000) valentin  (1000)        0 2024-04-16 12:39:04.186541 qiskit_scaleway-0.1.5/qiskit_scaleway/utils/
+-rw-rw-r--   0 valentin  (1000) valentin  (1000)       31 2024-04-03 12:51:52.000000 qiskit_scaleway-0.1.5/qiskit_scaleway/utils/__init__.py
+-rw-rw-r--   0 valentin  (1000) valentin  (1000)     3957 2024-04-16 12:36:19.000000 qiskit_scaleway-0.1.5/qiskit_scaleway/utils/client.py
+drwxrwxr-x   0 valentin  (1000) valentin  (1000)        0 2024-04-16 12:39:04.186541 qiskit_scaleway-0.1.5/qiskit_scaleway.egg-info/
+-rw-rw-r--   0 valentin  (1000) valentin  (1000)     2178 2024-04-16 12:39:04.000000 qiskit_scaleway-0.1.5/qiskit_scaleway.egg-info/PKG-INFO
+-rw-rw-r--   0 valentin  (1000) valentin  (1000)      744 2024-04-16 12:39:04.000000 qiskit_scaleway-0.1.5/qiskit_scaleway.egg-info/SOURCES.txt
+-rw-rw-r--   0 valentin  (1000) valentin  (1000)        1 2024-04-16 12:39:04.000000 qiskit_scaleway-0.1.5/qiskit_scaleway.egg-info/dependency_links.txt
+-rw-rw-r--   0 valentin  (1000) valentin  (1000)      127 2024-04-16 12:39:04.000000 qiskit_scaleway-0.1.5/qiskit_scaleway.egg-info/requires.txt
+-rw-rw-r--   0 valentin  (1000) valentin  (1000)       16 2024-04-16 12:39:04.000000 qiskit_scaleway-0.1.5/qiskit_scaleway.egg-info/top_level.txt
+-rw-rw-r--   0 valentin  (1000) valentin  (1000)       38 2024-04-16 12:39:04.186541 qiskit_scaleway-0.1.5/setup.cfg
+-rw-rw-r--   0 valentin  (1000) valentin  (1000)      514 2024-04-16 12:37:52.000000 qiskit_scaleway-0.1.5/setup.py
```

### Comparing `qiskit_scaleway-0.1.4/LICENSE` & `qiskit_scaleway-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `qiskit_scaleway-0.1.4/PKG-INFO` & `qiskit_scaleway-0.1.5/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,24 @@
-Metadata-Version: 2.1
-Name: qiskit_scaleway
-Version: 0.1.4
-Summary: UNKNOWN
-Home-page: UNKNOWN
-License: UNKNOWN
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Scaleway provider for Qiskit
 
 **Qiskit Scaleway** is a Python package to run quantum circuits on [Scaleway](https://www.scaleway.com/en/) infrastructure, providing access to [Aer](https://github.com/Qiskit/qiskit-aer) and [Qsim](https://github.com/quantumlib/qsim) simulators on powerful hardware (CPU and GPU).
 
+To run circuits over [Quandela](https://www.quandela.com/) backends provided by Scaleway, you must use [Perceval SDK](https://perceval.quandela.net/) through the [Scaleway provider](https://perceval.quandela.net/docs/providers.html).
+
 More info on the [Quantum service web page](https://labs.scaleway.com/en/qaas/).
 
 ## Installation
 
-We encourage installing Scaleway provider via the pip tool (a python package manager):
+We encourage installing Scaleway provider via the pip tool (a Python package manager):
 
 ```bash
 pip install qiskit-scaleway
 ```
 
-## Usage
+## Getting started
 ```python
 from qiskit import QuantumCircuit
 from qiskit_scaleway import ScalewayProvider
 
 provider = ScalewayProvider(
     project_id="<your-scaleway-project-id>",
     secret_key="<your-scaleway-secret-key>",
@@ -40,22 +32,24 @@
 qc.h(0)
 qc.cx(0, 1)
 qc.cx(0, 2)
 qc.cx(0, 3)
 qc.measure_all()
 
 # Create and send a job to a new QPU's session (or on an existing one)
-result = backend.run(qc, shots=1000).result()
+result = backend.run(qc, method="statevector", shots=1000).result()
 
 if result.success:
     print(result.get_counts())
 else:
     print(result.to_dict()["error"])
 
 ```
 
-## Contribute
-TODO
+## Development
+This repository is at its early stage and is still in active development. If you are looking for a way to contribute please read [CONTRIBUTING.md](CONTRIBUTING.md).
 
-## Licence
-[License Apache 2.0](LICENCE)
+## Reach us
+We love feedback. Feel free to reach us on [Scaleway Slack community](https://slack.scaleway.com/), we are waiting for you on [#opensource](https://scaleway-community.slack.com/app_redirect?channel=opensource)..
 
+## Licence
+[License Apache 2.0](LICENCE)
```

### Comparing `qiskit_scaleway-0.1.4/qiskit_scaleway/backends/aer_backend.py` & `qiskit_scaleway-0.1.5/qiskit_scaleway/backends/aer_backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,14 +46,17 @@
         )
         self._target.num_qubits = num_qubits
 
         # Set option validators
         self.options.set_validator("shots", (1, 10000000))
         self.options.set_validator("memory", bool)
 
+    def __repr__(self) -> str:
+        return f"<AerBackend(name={self.name},num_qubits={self.num_qubits},platform_id={self.id})>"
+
     @property
     def target(self):
         return self._target
 
     @property
     def num_qubits(self) -> int:
         return self._target.num_qubits
```

### Comparing `qiskit_scaleway-0.1.4/qiskit_scaleway/backends/aer_job.py` & `qiskit_scaleway-0.1.5/qiskit_scaleway/backends/aer_job.py`

 * *Files identical despite different names*

### Comparing `qiskit_scaleway-0.1.4/qiskit_scaleway/backends/qsim_backend.py` & `qiskit_scaleway-0.1.5/qiskit_scaleway/backends/qsim_backend.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,17 @@
         self._options = self._default_options()
 
         # Set option validators
         self.options.set_validator("shots", (1, 10000000))
 
         self._max_qubits = num_qubits
 
+    def __repr__(self) -> str:
+        return f"<QsimBackend(name={self.name},num_qubits={self.num_qubits},platform_id={self.id})>"
+
     @property
     def target(self):
         return None
 
     @property
     def num_qubits(self) -> int:
         return self._max_qubits
```

### Comparing `qiskit_scaleway-0.1.4/qiskit_scaleway/backends/qsim_job.py` & `qiskit_scaleway-0.1.5/qiskit_scaleway/backends/qsim_job.py`

 * *Files identical despite different names*

### Comparing `qiskit_scaleway-0.1.4/qiskit_scaleway/backends/scaleway_backend.py` & `qiskit_scaleway-0.1.5/qiskit_scaleway/backends/scaleway_backend.py`

 * *Files identical despite different names*

### Comparing `qiskit_scaleway-0.1.4/qiskit_scaleway/backends/scaleway_job.py` & `qiskit_scaleway-0.1.5/qiskit_scaleway/backends/scaleway_job.py`

 * *Files identical despite different names*

### Comparing `qiskit_scaleway-0.1.4/qiskit_scaleway/primitives/aer_estimator.py` & `qiskit_scaleway-0.1.5/qiskit_scaleway/primitives/aer_estimator.py`

 * *Files identical despite different names*

### Comparing `qiskit_scaleway-0.1.4/qiskit_scaleway/primitives/aer_sampler.py` & `qiskit_scaleway-0.1.5/qiskit_scaleway/primitives/aer_sampler.py`

 * *Files identical despite different names*

### Comparing `qiskit_scaleway-0.1.4/qiskit_scaleway/provider.py` & `qiskit_scaleway-0.1.5/qiskit_scaleway/provider.py`

 * *Files identical despite different names*

### Comparing `qiskit_scaleway-0.1.4/qiskit_scaleway/utils/client.py` & `qiskit_scaleway-0.1.5/qiskit_scaleway/utils/client.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 import httpx
 
 
 _ENDPOINT_PLATFORM = "/platforms"
 _ENDPOINT_SESSION = "/sessions"
 _ENDPOINT_JOB = "/jobs"
-_PROVIDER_NAME = "scaleway"
 
 
 class QaaSClient:
     def __init__(self, project_id: str, token: str, url: str) -> None:
         self.__token = token
         self.__url = url
         self.__project_id = project_id
@@ -21,22 +20,19 @@
 
     def _api_headers(self) -> dict:
         return {"X-Auth-Token": self.__token}
 
     def _build_endpoint(self, endpoint: str) -> str:
         return f"{self.__url}{endpoint}"
 
-    def list_platforms(self, name: str = "") -> dict:
-        http_client = self._http_client()
-        endpoint = (
-            f"{self._build_endpoint(_ENDPOINT_PLATFORM)}?providerName={_PROVIDER_NAME}"
-        )
+    def list_platforms(self, name: str) -> dict:
+        assert name is not None
 
-        if name:
-            endpoint += f"&name={name}"
+        http_client = self._http_client()
+        endpoint = f"{self._build_endpoint(_ENDPOINT_PLATFORM)}?name={name}"
 
         resp = http_client.get(endpoint)
         resp.raise_for_status()
 
         return resp.json()
 
     def create_session(
```

### Comparing `qiskit_scaleway-0.1.4/qiskit_scaleway.egg-info/PKG-INFO` & `qiskit_scaleway-0.1.5/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,34 @@
 Metadata-Version: 2.1
-Name: qiskit-scaleway
-Version: 0.1.4
+Name: qiskit_scaleway
+Version: 0.1.5
 Summary: UNKNOWN
 Home-page: UNKNOWN
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Scaleway provider for Qiskit
 
 **Qiskit Scaleway** is a Python package to run quantum circuits on [Scaleway](https://www.scaleway.com/en/) infrastructure, providing access to [Aer](https://github.com/Qiskit/qiskit-aer) and [Qsim](https://github.com/quantumlib/qsim) simulators on powerful hardware (CPU and GPU).
 
+To run circuits over [Quandela](https://www.quandela.com/) backends provided by Scaleway, you must use [Perceval SDK](https://perceval.quandela.net/) through the [Scaleway provider](https://perceval.quandela.net/docs/providers.html).
+
 More info on the [Quantum service web page](https://labs.scaleway.com/en/qaas/).
 
 ## Installation
 
-We encourage installing Scaleway provider via the pip tool (a python package manager):
+We encourage installing Scaleway provider via the pip tool (a Python package manager):
 
 ```bash
 pip install qiskit-scaleway
 ```
 
-## Usage
+## Getting started
 ```python
 from qiskit import QuantumCircuit
 from qiskit_scaleway import ScalewayProvider
 
 provider = ScalewayProvider(
     project_id="<your-scaleway-project-id>",
     secret_key="<your-scaleway-secret-key>",
@@ -40,22 +42,25 @@
 qc.h(0)
 qc.cx(0, 1)
 qc.cx(0, 2)
 qc.cx(0, 3)
 qc.measure_all()
 
 # Create and send a job to a new QPU's session (or on an existing one)
-result = backend.run(qc, shots=1000).result()
+result = backend.run(qc, method="statevector", shots=1000).result()
 
 if result.success:
     print(result.get_counts())
 else:
     print(result.to_dict()["error"])
 
 ```
 
-## Contribute
-TODO
+## Development
+This repository is at its early stage and is still in active development. If you are looking for a way to contribute please read [CONTRIBUTING.md](CONTRIBUTING.md).
+
+## Reach us
+We love feedback. Feel free to reach us on [Scaleway Slack community](https://slack.scaleway.com/), we are waiting for you on [#opensource](https://scaleway-community.slack.com/app_redirect?channel=opensource)..
 
 ## Licence
 [License Apache 2.0](LICENCE)
```

### Comparing `qiskit_scaleway-0.1.4/qiskit_scaleway.egg-info/SOURCES.txt` & `qiskit_scaleway-0.1.5/qiskit_scaleway.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qiskit_scaleway-0.1.4/setup.py` & `qiskit_scaleway-0.1.5/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as f:
     description = f.read()
 
 setup(
     name="qiskit_scaleway",
-    version="0.1.4",
+    version="0.1.5",
     packages=find_packages(),
     install_requires=[
         "qiskit==1.0.2",
         "qiskit-aer==0.14.0.1",
         "randomname==0.2.1",
         "httpx==0.27.0",
         "dataclasses-json==0.6.4",
```

