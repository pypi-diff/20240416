# Comparing `tmp/pennylane-kq-0.0.5.tar.gz` & `tmp/pennylane_kq-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pennylane-kq-0.0.5.tar", last modified: Thu Dec 21 01:58:36 2023, max compression
+gzip compressed data, was "pennylane_kq-0.0.6.tar", last modified: Tue Apr 16 06:30:57 2024, max compression
```

## Comparing `pennylane-kq-0.0.5.tar` & `pennylane_kq-0.0.6.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 ino        (501) staff       (20)        0 2023-12-21 01:58:36.840197 pennylane-kq-0.0.5/
--rw-r--r--   0 ino        (501) staff       (20)     1335 2023-08-22 08:26:43.000000 pennylane-kq-0.0.5/LICENSE
--rw-r--r--   0 ino        (501) staff       (20)     1616 2023-12-21 01:58:36.840077 pennylane-kq-0.0.5/PKG-INFO
--rw-r--r--   0 ino        (501) staff       (20)     1304 2023-12-21 01:57:51.000000 pennylane-kq-0.0.5/README.md
-drwxr-xr-x   0 ino        (501) staff       (20)        0 2023-12-21 01:58:36.839009 pennylane-kq-0.0.5/pennylane_kq/
--rw-r--r--   0 ino        (501) staff       (20)      293 2023-12-21 00:35:30.000000 pennylane-kq-0.0.5/pennylane_kq/__init__.py
--rw-r--r--   0 ino        (501) staff       (20)       97 2023-12-21 01:58:22.000000 pennylane-kq-0.0.5/pennylane_kq/_version.py
--rw-r--r--   0 ino        (501) staff       (20)     3414 2023-12-21 00:40:33.000000 pennylane-kq-0.0.5/pennylane_kq/kq_emulator.py
--rw-r--r--   0 ino        (501) staff       (20)     3442 2023-12-21 00:36:04.000000 pennylane-kq-0.0.5/pennylane_kq/kq_emulator_aws.py
--rw-r--r--   0 ino        (501) staff       (20)     3414 2023-12-21 00:40:27.000000 pennylane-kq-0.0.5/pennylane_kq/kq_hardware.py
--rw-r--r--   0 ino        (501) staff       (20)     2164 2023-12-12 04:40:40.000000 pennylane-kq-0.0.5/pennylane_kq/kq_local_emulator.py
-drwxr-xr-x   0 ino        (501) staff       (20)        0 2023-12-21 01:58:36.839901 pennylane-kq-0.0.5/pennylane_kq.egg-info/
--rw-r--r--   0 ino        (501) staff       (20)     1616 2023-12-21 01:58:36.000000 pennylane-kq-0.0.5/pennylane_kq.egg-info/PKG-INFO
--rw-r--r--   0 ino        (501) staff       (20)      451 2023-12-21 01:58:36.000000 pennylane-kq-0.0.5/pennylane_kq.egg-info/SOURCES.txt
--rw-r--r--   0 ino        (501) staff       (20)        1 2023-12-21 01:58:36.000000 pennylane-kq-0.0.5/pennylane_kq.egg-info/dependency_links.txt
--rw-r--r--   0 ino        (501) staff       (20)      230 2023-12-21 01:58:36.000000 pennylane-kq-0.0.5/pennylane_kq.egg-info/entry_points.txt
--rw-r--r--   0 ino        (501) staff       (20)        1 2023-11-13 13:51:28.000000 pennylane-kq-0.0.5/pennylane_kq.egg-info/not-zip-safe
--rw-r--r--   0 ino        (501) staff       (20)       22 2023-12-21 01:58:36.000000 pennylane-kq-0.0.5/pennylane_kq.egg-info/requires.txt
--rw-r--r--   0 ino        (501) staff       (20)       13 2023-12-21 01:58:36.000000 pennylane-kq-0.0.5/pennylane_kq.egg-info/top_level.txt
--rw-r--r--   0 ino        (501) staff       (20)       38 2023-12-21 01:58:36.840232 pennylane-kq-0.0.5/setup.cfg
--rw-r--r--   0 ino        (501) staff       (20)     1113 2023-12-21 01:55:43.000000 pennylane-kq-0.0.5/setup.py
+drwxr-xr-x   0 ino        (501) staff       (20)        0 2024-04-16 06:30:57.782693 pennylane_kq-0.0.6/
+-rw-r--r--   0 ino        (501) staff       (20)     1335 2023-08-22 08:26:43.000000 pennylane_kq-0.0.6/LICENSE
+-rw-r--r--   0 ino        (501) staff       (20)     1668 2024-04-16 06:30:57.782483 pennylane_kq-0.0.6/PKG-INFO
+-rw-r--r--   0 ino        (501) staff       (20)     1304 2023-12-21 01:57:51.000000 pennylane_kq-0.0.6/README.md
+drwxr-xr-x   0 ino        (501) staff       (20)        0 2024-04-16 06:30:57.780784 pennylane_kq-0.0.6/pennylane_kq/
+-rw-r--r--   0 ino        (501) staff       (20)      293 2023-12-21 00:35:30.000000 pennylane_kq-0.0.6/pennylane_kq/__init__.py
+-rw-r--r--   0 ino        (501) staff       (20)       97 2024-04-16 06:29:12.000000 pennylane_kq-0.0.6/pennylane_kq/_version.py
+-rw-r--r--   0 ino        (501) staff       (20)     3439 2024-04-16 06:26:52.000000 pennylane_kq-0.0.6/pennylane_kq/kq_emulator.py
+-rw-r--r--   0 ino        (501) staff       (20)     3479 2023-12-27 04:57:04.000000 pennylane_kq-0.0.6/pennylane_kq/kq_emulator_aws.py
+-rw-r--r--   0 ino        (501) staff       (20)     3451 2023-12-27 04:56:48.000000 pennylane_kq-0.0.6/pennylane_kq/kq_hardware.py
+-rw-r--r--   0 ino        (501) staff       (20)     2435 2024-01-15 04:53:37.000000 pennylane_kq-0.0.6/pennylane_kq/kq_local_emulator.py
+drwxr-xr-x   0 ino        (501) staff       (20)        0 2024-04-16 06:30:57.782247 pennylane_kq-0.0.6/pennylane_kq.egg-info/
+-rw-r--r--   0 ino        (501) staff       (20)     1668 2024-04-16 06:30:57.000000 pennylane_kq-0.0.6/pennylane_kq.egg-info/PKG-INFO
+-rw-r--r--   0 ino        (501) staff       (20)      451 2024-04-16 06:30:57.000000 pennylane_kq-0.0.6/pennylane_kq.egg-info/SOURCES.txt
+-rw-r--r--   0 ino        (501) staff       (20)        1 2024-04-16 06:30:57.000000 pennylane_kq-0.0.6/pennylane_kq.egg-info/dependency_links.txt
+-rw-r--r--   0 ino        (501) staff       (20)      230 2024-04-16 06:30:57.000000 pennylane_kq-0.0.6/pennylane_kq.egg-info/entry_points.txt
+-rw-r--r--   0 ino        (501) staff       (20)        1 2023-11-13 13:51:28.000000 pennylane_kq-0.0.6/pennylane_kq.egg-info/not-zip-safe
+-rw-r--r--   0 ino        (501) staff       (20)       22 2024-04-16 06:30:57.000000 pennylane_kq-0.0.6/pennylane_kq.egg-info/requires.txt
+-rw-r--r--   0 ino        (501) staff       (20)       13 2024-04-16 06:30:57.000000 pennylane_kq-0.0.6/pennylane_kq.egg-info/top_level.txt
+-rw-r--r--   0 ino        (501) staff       (20)       38 2024-04-16 06:30:57.782742 pennylane_kq-0.0.6/setup.cfg
+-rw-r--r--   0 ino        (501) staff       (20)     1113 2023-12-21 01:55:43.000000 pennylane_kq-0.0.6/setup.py
```

### Comparing `pennylane-kq-0.0.5/LICENSE` & `pennylane_kq-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pennylane-kq-0.0.5/PKG-INFO` & `pennylane_kq-0.0.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 Metadata-Version: 2.1
 Name: pennylane-kq
-Version: 0.0.5
+Version: 0.0.6
 Summary: A Pennylane plugin for KQ Cloud System
 Home-page: https://www.github.com/inojeon/pennylane-kq
 Author: Inho Jeon
 Author-email: inojeon@kisti.re.kr
 License: BSD-2
 Provides: pennylane_kq
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pennylane>=0.31
+Requires-Dist: numpy
 
 # PennyLane Korea Quantum Plugin
 
 The PennyLane-KQ plugin integrates the KQ quantum computing library.
 
 [PennyLane](https://pennylane.readthedocs.io) is a cross-platform Python library for quantum machine learning, automatic differentiation, and optimization of hybrid quantum-classical computations.
```

### Comparing `pennylane-kq-0.0.5/README.md` & `pennylane_kq-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `pennylane-kq-0.0.5/pennylane_kq/kq_emulator.py` & `pennylane_kq-0.0.6/pennylane_kq/kq_emulator.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,29 +15,29 @@
     short_name = "kq.emulator"
     pennylane_requires = ">=0.16.0"
     version = "0.0.1"
     author = "Inho Jeon"
     accessToken = None
     resourceId = "f8284e6e-d97e-4afc-a015-39d382273a99"
 
-    operations = {"PauliX", "RX", "CNOT", "RY", "RZ"}
+    operations = {"PauliX", "RX", "CNOT", "RY", "RZ", "Hadamard"}
     observables = {"PauliZ", "PauliX", "PauliY"}
 
     def __init__(self, wires=4, shots=1024, accessKeyId=None, secretAccessKey=None):
         super().__init__(wires=wires, shots=shots)
         self.accessKeyId = accessKeyId
         self.secretAccessKey = secretAccessKey
         # self.hardware_options = hardware_options or "kqEmulator"
 
     def apply(self, operations, **kwargs):
         self.run(self._circuit)
 
     def _get_token(self):
         print("get KQ Cloud Token")
-        api_url = f"http://150.183.154.20:31001/oauth/token"
+        api_url = f"http://150.183.154.20/oauth/token"
         headers = {"Content-Type": "application/x-www-form-urlencoded"}
         data = {
             "grant_type": "apikey",
             "accessKeyId": self.accessKeyId,
             "secretAccessKey": self.secretAccessKey,
         }
         requestData = requests.post(api_url, data=data, headers=headers)
@@ -48,22 +48,22 @@
         else:
             raise DeviceError(
                 f"/oauth/token error. req code : {requestData.status_code}"
             )
 
     def _job_submit(self, circuits):
         print("job submit")
-        URL = "http://150.183.154.20:31001/v2/jobs"
+        URL = "http://150.183.154.20/v2/jobs"
         headers = {
             "Content-Type": "application/json",
             "Authorization": f"Bearer {self.accessToken}",
         }
         data = {
             "resource": {"id": self.resourceId},
-            "code": circuits[0].to_openqasm(),
+            "code": circuits[0].to_openqasm(wires=sorted(circuits[0].wires)),
             "shot": self.shots,
             "name": "test job",
             "type": "QASM",
         }
         res = requests.post(URL, data=json.dumps(data), headers=headers)
 
         if res.status_code == 201:
@@ -72,15 +72,15 @@
             raise DeviceError(f"Job sumbit error. req code : {res.status_code}")
 
     def _check_job_status(self, jobId):
         timeout = 6000
         timeout_start = time.time()
 
         while time.time() < timeout_start + timeout:
-            URL = f"http://150.183.154.20:31001/v2/jobs/{jobId}"
+            URL = f"http://150.183.154.20/v2/jobs/{jobId}"
             headers = {"Authorization": f"Bearer {self.accessToken}"}
             res = requests.get(URL, headers=headers)
             status = res.json().get("status")
             print(f"job status check: {status}")
 
             if status == "COMPLETED":
                 return res.json().get("result")
```

### Comparing `pennylane-kq-0.0.5/pennylane_kq/kq_emulator_aws.py` & `pennylane_kq-0.0.6/pennylane_kq/kq_emulator_aws.py`

 * *Files 3% similar despite different names*

```diff
@@ -55,15 +55,15 @@
         URL = "http://3.39.145.223:31001/v2/jobs"
         headers = {
             "Content-Type": "application/json",
             "Authorization": f"Bearer {self.accessToken}",
         }
         data = {
             "resource": {"id": "aae7709c-e335-4420-b231-6f8c88aa85be"},
-            "code": circuits[0].to_openqasm(),
+            "input_file": circuits[0].to_openqasm(wires=sorted(circuits[0].wires)),
             "shot": self.shots,
             "name": "test job",
             "type": "QASM",
         }
         res = requests.post(URL, data=json.dumps(data), headers=headers)
 
         if res.status_code == 201:
```

### Comparing `pennylane-kq-0.0.5/pennylane_kq/kq_hardware.py` & `pennylane_kq-0.0.6/pennylane_kq/kq_hardware.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,15 @@
         URL = "http://150.183.154.20:31001/v2/jobs"
         headers = {
             "Content-Type": "application/json",
             "Authorization": f"Bearer {self.accessToken}",
         }
         data = {
             "resource": {"id": self.resourceId},
-            "code": circuits[0].to_openqasm(),
+            "input_file": circuits[0].to_openqasm(wires=sorted(circuits[0].wires)),
             "shot": self.shots,
             "name": "test job",
             "type": "QASM",
         }
         res = requests.post(URL, data=json.dumps(data), headers=headers)
 
         if res.status_code == 201:
```

### Comparing `pennylane-kq-0.0.5/pennylane_kq/kq_local_emulator.py` & `pennylane_kq-0.0.6/pennylane_kq/kq_local_emulator.py`

 * *Files 9% similar despite different names*

```diff
@@ -15,29 +15,31 @@
 
     name = "Korea Quantum Local Emulator"
     short_name = "kq.local_emulator"
     pennylane_requires = ">=0.16.0"
     version = "0.0.1"
     author = "Inho Jeon"
 
-    operations = {"PauliX", "RX", "CNOT", "RY", "RZ"}
+    operations = {"PauliX", "RX", "CNOT", "RY", "RZ", "Hadamard"}
     observables = {"PauliZ", "PauliX", "PauliY"}
 
     def __init__(self, wires=4, shots=1024):
         super().__init__(wires=wires, shots=shots)
 
     def apply(self, operations, **kwargs):
         print("apply")
         # self.run(self._circuit)
 
     def _job_submit(self, circuits):
+        # print(circuits[0].wires)
+        # print(circuits[0].to_openqasm(wires=sorted(circuits[0].wires)))
         URL = "http://localhost:8000/job/"
         headers = {"Content-Type": "application/json"}
         data = {
-            "input_file": circuits[0].to_openqasm(),
+            "input_file": circuits[0].to_openqasm(wires=sorted(circuits[0].wires)),
             "shot": self.shots,
             "type": "qasm",
         }
         res = requests.post(URL, data=json.dumps(data), headers=headers)
 
         if res.status_code == 201:
             return res.json().get("jobUUID")
@@ -59,11 +61,15 @@
                 res = requests.get(URL)
                 return res.json()
 
     def batch_execute(
         self, circuits
     ):  # pragma: no cover, pylint:disable=arguments-differ
         # print(self.accessKeyId, self.secretAccessKey)
-        jobUUID = self._job_submit(circuits)
-        result = self._check_job_status(jobUUID)
 
-        return [result["results"][0]["data"]["counts"]]
+        # jobUUID = self._job_submit(circuits)
+        # result = self._check_job_status(jobUUID)
+
+        # return [result["results"][0]["data"]["counts"]]
+
+        print(circuits[0].to_openqasm(wires=sorted(circuits[0].wires)))
+        return {"-1": "00", "1": "32"}
```

### Comparing `pennylane-kq-0.0.5/pennylane_kq.egg-info/PKG-INFO` & `pennylane_kq-0.0.6/pennylane_kq.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 Metadata-Version: 2.1
 Name: pennylane-kq
-Version: 0.0.5
+Version: 0.0.6
 Summary: A Pennylane plugin for KQ Cloud System
 Home-page: https://www.github.com/inojeon/pennylane-kq
 Author: Inho Jeon
 Author-email: inojeon@kisti.re.kr
 License: BSD-2
 Provides: pennylane_kq
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: pennylane>=0.31
+Requires-Dist: numpy
 
 # PennyLane Korea Quantum Plugin
 
 The PennyLane-KQ plugin integrates the KQ quantum computing library.
 
 [PennyLane](https://pennylane.readthedocs.io) is a cross-platform Python library for quantum machine learning, automatic differentiation, and optimization of hybrid quantum-classical computations.
```

### Comparing `pennylane-kq-0.0.5/setup.py` & `pennylane_kq-0.0.6/setup.py`

 * *Files identical despite different names*

