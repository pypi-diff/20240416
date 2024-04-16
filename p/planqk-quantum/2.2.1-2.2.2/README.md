# Comparing `tmp/planqk-quantum-2.2.1.tar.gz` & `tmp/planqk-quantum-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "planqk-quantum-2.2.1.tar", last modified: Wed Apr 10 13:51:38 2024, max compression
+gzip compressed data, was "planqk-quantum-2.2.2.tar", last modified: Mon Apr 15 17:47:47 2024, max compression
```

## Comparing `planqk-quantum-2.2.1.tar` & `planqk-quantum-2.2.2.tar`

### file list

```diff
@@ -1,58 +1,56 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:51:38.176738 planqk-quantum-2.2.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-10 13:51:27.000000 planqk-quantum-2.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     3721 2024-04-10 13:51:38.176738 planqk-quantum-2.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-04-10 13:51:27.000000 planqk-quantum-2.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:51:38.168738 planqk-quantum-2.2.1/planqk/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 13:51:27.000000 planqk-quantum-2.2.1/planqk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-10 13:51:27.000000 planqk-quantum-2.2.1/planqk/context.py
--rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-04-10 13:51:27.000000 planqk-quantum-2.2.1/planqk/credentials.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:51:38.168738 planqk-quantum-2.2.1/planqk/dwave/
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-10 13:51:27.000000 planqk-quantum-2.2.1/planqk/dwave/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2406 2024-04-10 13:51:27.000000 planqk-quantum-2.2.1/planqk/dwave/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-04-10 13:51:27.000000 planqk-quantum-2.2.1/planqk/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:51:38.172738 planqk-quantum-2.2.1/planqk/qiskit/
--rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-10 13:51:27.000000 planqk-quantum-2.2.1/planqk/qiskit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9514 2024-04-10 13:51:27.000000 planqk-quantum-2.2.1/planqk/qiskit/backend.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:51:38.172738 planqk-quantum-2.2.1/planqk/qiskit/client/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 13:51:27.000000 planqk-quantum-2.2.1/planqk/qiskit/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5135 2024-04-10 13:51:27.000000 planqk-quantum-2.2.1/planqk/qiskit/client/backend_dtos.py
--rw-r--r--   0 runner    (1001) docker     (127)     6097 2024-04-10 13:51:27.000000 planqk-quantum-2.2.1/planqk/qiskit/client/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-10 13:51:27.000000 planqk-quantum-2.2.1/planqk/qiskit/client/dto_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-04-10 13:51:27.000000 planqk-quantum-2.2.1/planqk/qiskit/client/job_dtos.py
--rw-r--r--   0 runner    (1001) docker     (127)     4415 2024-04-10 13:51:27.000000 planqk-quantum-2.2.1/planqk/qiskit/job.py
--rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-04-10 13:51:27.000000 planqk-quantum-2.2.1/planqk/qiskit/options.py
--rw-r--r--   0 runner    (1001) docker     (127)     5191 2024-04-10 13:51:27.000000 planqk-quantum-2.2.1/planqk/qiskit/planqk_runtime_job.py
--rw-r--r--   0 runner    (1001) docker     (127)     5002 2024-04-10 13:51:27.000000 planqk-quantum-2.2.1/planqk/qiskit/provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:51:38.172738 planqk-quantum-2.2.1/planqk/qiskit/providers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 13:51:27.000000 planqk-quantum-2.2.1/planqk/qiskit/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1800 2024-04-10 13:51:27.000000 planqk-quantum-2.2.1/planqk/qiskit/providers/adapter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:51:38.172738 planqk-quantum-2.2.1/planqk/qiskit/providers/aws/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 13:51:27.000000 planqk-quantum-2.2.1/planqk/qiskit/providers/aws/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      271 2024-04-10 13:51:27.000000 planqk-quantum-2.2.1/planqk/qiskit/providers/aws/aws_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     1450 2024-04-10 13:51:27.000000 planqk-quantum-2.2.1/planqk/qiskit/providers/aws_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-04-10 13:51:27.000000 planqk-quantum-2.2.1/planqk/qiskit/providers/aws_converters.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:51:38.172738 planqk-quantum-2.2.1/planqk/qiskit/providers/azure/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 13:51:27.000000 planqk-quantum-2.2.1/planqk/qiskit/providers/azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      313 2024-04-10 13:51:27.000000 planqk-quantum-2.2.1/planqk/qiskit/providers/azure/ionq_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)      649 2024-04-10 13:51:27.000000 planqk-quantum-2.2.1/planqk/qiskit/providers/azure_adapter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:51:38.172738 planqk-quantum-2.2.1/planqk/qiskit/providers/ibm/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 13:51:27.000000 planqk-quantum-2.2.1/planqk/qiskit/providers/ibm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1896 2024-04-10 13:51:27.000000 planqk-quantum-2.2.1/planqk/qiskit/providers/ibm/ibm_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)     3701 2024-04-10 13:51:27.000000 planqk-quantum-2.2.1/planqk/qiskit/providers/ibm/ibm_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)     3606 2024-04-10 13:51:27.000000 planqk-quantum-2.2.1/planqk/qiskit/providers/job_input_converter.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:51:38.176738 planqk-quantum-2.2.1/planqk/qiskit/providers/qryd/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-10 13:51:27.000000 planqk-quantum-2.2.1/planqk/qiskit/providers/qryd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5082 2024-04-10 13:51:27.000000 planqk-quantum-2.2.1/planqk/qiskit/providers/qryd/pcp_gate.py
--rw-r--r--   0 runner    (1001) docker     (127)     5434 2024-04-10 13:51:27.000000 planqk-quantum-2.2.1/planqk/qiskit/providers/qryd/pcz_gate.py
--rw-r--r--   0 runner    (1001) docker     (127)     1848 2024-04-10 13:51:27.000000 planqk-quantum-2.2.1/planqk/qiskit/providers/qryd/qryd_adapter.py
--rw-r--r--   0 runner    (1001) docker     (127)      638 2024-04-10 13:51:27.000000 planqk-quantum-2.2.1/planqk/qiskit/providers/qryd/qryd_backend.py
--rw-r--r--   0 runner    (1001) docker     (127)    14088 2024-04-10 13:51:27.000000 planqk-quantum-2.2.1/planqk/qiskit/providers/qryd/qryd_converters.py
--rw-r--r--   0 runner    (1001) docker     (127)     7936 2024-04-10 13:51:27.000000 planqk-quantum-2.2.1/planqk/qiskit/runtime_provider.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 13:51:38.176738 planqk-quantum-2.2.1/planqk_quantum.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3721 2024-04-10 13:51:38.000000 planqk-quantum-2.2.1/planqk_quantum.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1504 2024-04-10 13:51:38.000000 planqk-quantum-2.2.1/planqk_quantum.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 13:51:38.000000 planqk-quantum-2.2.1/planqk_quantum.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-10 13:51:38.000000 planqk-quantum-2.2.1/planqk_quantum.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-10 13:51:38.000000 planqk-quantum-2.2.1/planqk_quantum.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 13:51:38.176738 planqk-quantum-2.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-10 13:51:27.000000 planqk-quantum-2.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:47:47.360958 planqk-quantum-2.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-15 17:47:38.000000 planqk-quantum-2.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     3721 2024-04-15 17:47:47.356958 planqk-quantum-2.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3259 2024-04-15 17:47:38.000000 planqk-quantum-2.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:47:47.352958 planqk-quantum-2.2.2/planqk/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 17:47:38.000000 planqk-quantum-2.2.2/planqk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1178 2024-04-15 17:47:38.000000 planqk-quantum-2.2.2/planqk/context.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-04-15 17:47:38.000000 planqk-quantum-2.2.2/planqk/credentials.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:47:47.352958 planqk-quantum-2.2.2/planqk/dwave/
+-rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-15 17:47:38.000000 planqk-quantum-2.2.2/planqk/dwave/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2406 2024-04-15 17:47:38.000000 planqk-quantum-2.2.2/planqk/dwave/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1231 2024-04-15 17:47:38.000000 planqk-quantum-2.2.2/planqk/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:47:47.352958 planqk-quantum-2.2.2/planqk/qiskit/
+-rw-r--r--   0 runner    (1001) docker     (127)      106 2024-04-15 17:47:38.000000 planqk-quantum-2.2.2/planqk/qiskit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10026 2024-04-15 17:47:38.000000 planqk-quantum-2.2.2/planqk/qiskit/backend.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:47:47.356958 planqk-quantum-2.2.2/planqk/qiskit/client/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 17:47:38.000000 planqk-quantum-2.2.2/planqk/qiskit/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5135 2024-04-15 17:47:38.000000 planqk-quantum-2.2.2/planqk/qiskit/client/backend_dtos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6097 2024-04-15 17:47:38.000000 planqk-quantum-2.2.2/planqk/qiskit/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      162 2024-04-15 17:47:38.000000 planqk-quantum-2.2.2/planqk/qiskit/client/dto_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1773 2024-04-15 17:47:38.000000 planqk-quantum-2.2.2/planqk/qiskit/client/job_dtos.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4415 2024-04-15 17:47:38.000000 planqk-quantum-2.2.2/planqk/qiskit/job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1359 2024-04-15 17:47:38.000000 planqk-quantum-2.2.2/planqk/qiskit/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5191 2024-04-15 17:47:38.000000 planqk-quantum-2.2.2/planqk/qiskit/planqk_runtime_job.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5247 2024-04-15 17:47:38.000000 planqk-quantum-2.2.2/planqk/qiskit/provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:47:47.356958 planqk-quantum-2.2.2/planqk/qiskit/providers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 17:47:38.000000 planqk-quantum-2.2.2/planqk/qiskit/providers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:47:47.356958 planqk-quantum-2.2.2/planqk/qiskit/providers/aws/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 17:47:38.000000 planqk-quantum-2.2.2/planqk/qiskit/providers/aws/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1548 2024-04-15 17:47:38.000000 planqk-quantum-2.2.2/planqk/qiskit/providers/aws/aws_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1569 2024-04-15 17:47:38.000000 planqk-quantum-2.2.2/planqk/qiskit/providers/aws_converters.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:47:47.356958 planqk-quantum-2.2.2/planqk/qiskit/providers/azure/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 17:47:38.000000 planqk-quantum-2.2.2/planqk/qiskit/providers/azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      498 2024-04-15 17:47:38.000000 planqk-quantum-2.2.2/planqk/qiskit/providers/azure/azure_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)      345 2024-04-15 17:47:38.000000 planqk-quantum-2.2.2/planqk/qiskit/providers/azure/ionq_backend.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:47:47.356958 planqk-quantum-2.2.2/planqk/qiskit/providers/ibm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 17:47:38.000000 planqk-quantum-2.2.2/planqk/qiskit/providers/ibm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2470 2024-04-15 17:47:38.000000 planqk-quantum-2.2.2/planqk/qiskit/providers/ibm/ibm_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3116 2024-04-15 17:47:38.000000 planqk-quantum-2.2.2/planqk/qiskit/providers/ibm/ibm_provider_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)      190 2024-04-15 17:47:38.000000 planqk-quantum-2.2.2/planqk/qiskit/providers/ibm/ibm_runtime_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3606 2024-04-15 17:47:38.000000 planqk-quantum-2.2.2/planqk/qiskit/providers/job_input_converter.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:47:47.356958 planqk-quantum-2.2.2/planqk/qiskit/providers/qryd/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 17:47:38.000000 planqk-quantum-2.2.2/planqk/qiskit/providers/qryd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5082 2024-04-15 17:47:38.000000 planqk-quantum-2.2.2/planqk/qiskit/providers/qryd/pcp_gate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5434 2024-04-15 17:47:38.000000 planqk-quantum-2.2.2/planqk/qiskit/providers/qryd/pcz_gate.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2297 2024-04-15 17:47:38.000000 planqk-quantum-2.2.2/planqk/qiskit/providers/qryd/qryd_backend.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14088 2024-04-15 17:47:38.000000 planqk-quantum-2.2.2/planqk/qiskit/providers/qryd/qryd_converters.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8397 2024-04-15 17:47:38.000000 planqk-quantum-2.2.2/planqk/qiskit/runtime_provider.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 17:47:47.356958 planqk-quantum-2.2.2/planqk_quantum.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3721 2024-04-15 17:47:47.000000 planqk-quantum-2.2.2/planqk_quantum.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1451 2024-04-15 17:47:47.000000 planqk-quantum-2.2.2/planqk_quantum.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 17:47:47.000000 planqk-quantum-2.2.2/planqk_quantum.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-15 17:47:47.000000 planqk-quantum-2.2.2/planqk_quantum.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-15 17:47:47.000000 planqk-quantum-2.2.2/planqk_quantum.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 17:47:47.360958 planqk-quantum-2.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-15 17:47:38.000000 planqk-quantum-2.2.2/setup.py
```

### Comparing `planqk-quantum-2.2.1/LICENSE` & `planqk-quantum-2.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `planqk-quantum-2.2.1/PKG-INFO` & `planqk-quantum-2.2.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: planqk-quantum
-Version: 2.2.1
+Version: 2.2.2
 Summary: Python SDK for the PlanQK Platform
 Home-page: https://github.com/planqk/planqk-quantum
 Author: Anaqor AG
 Author-email: info@anaqor.io
 License: apache-2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `planqk-quantum-2.2.1/README.md` & `planqk-quantum-2.2.2/README.md`

 * *Files identical despite different names*

### Comparing `planqk-quantum-2.2.1/planqk/context.py` & `planqk-quantum-2.2.2/planqk/context.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-2.2.1/planqk/credentials.py` & `planqk-quantum-2.2.2/planqk/credentials.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-2.2.1/planqk/dwave/provider.py` & `planqk-quantum-2.2.2/planqk/dwave/provider.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-2.2.1/planqk/exceptions.py` & `planqk-quantum-2.2.2/planqk/exceptions.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-2.2.1/planqk/qiskit/backend.py` & `planqk-quantum-2.2.2/planqk/qiskit/backend.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import datetime
-from abc import ABC
+from abc import ABC, abstractmethod
 from copy import copy
+from typing import Optional
 
+from qiskit.circuit import Instruction as QiskitInstruction, Delay, Parameter
 from qiskit.circuit import Measure
 from qiskit.providers import BackendV2, Provider
 from qiskit.providers.models import QasmBackendConfiguration, GateConfig
 from qiskit.transpiler import Target
 
-from .client.backend_dtos import ConfigurationDto, TYPE, BackendDto, ConnectivityDto, PROVIDER
+from .client.backend_dtos import ConfigurationDto, TYPE, BackendDto, PROVIDER
 from .client.job_dtos import JobDto
 from .job import PlanqkJob
 from .options import OptionsV2
-from .providers.adapter import ProviderAdapterFactory
 
 
 class PlanqkBackend(BackendV2, ABC):
 
     def __init__(  # pylint: disable=too-many-arguments
             self,
             backend_info: BackendDto,
@@ -50,40 +51,69 @@
                            name=name,
                            description=description,
                            online_date=online_date,
                            backend_version=backend_version,
                            **fields,
                            )
         self._backend_info = backend_info
+        self._is_simulator = self.backend_info.type == TYPE.SIMULATOR
         self._target = self._planqk_backend_to_target()
         self._configuration = self._planqk_backend_dto_to_configuration()
         self._instance = None
 
+    @property
+    def backend_info(self):
+        return self._backend_info
+
+    @property
+    def is_simulator(self):
+        return self._is_simulator
+
+    @abstractmethod
+    def to_gate(self, name: str):
+        pass
+
+    @abstractmethod
+    def get_single_qubit_gate_properties(self):
+        pass
+
+    @abstractmethod
+    def get_multi_qubit_gate_properties(self):
+        pass
+
+    non_gate_instr_mapping = {
+        "delay": Delay(Parameter("t")),
+        "measure": Measure(),
+    }
+
+    def to_non_gate_instruction(self, name: str) -> Optional[QiskitInstruction]:
+        instr = self.non_gate_instr_mapping.get(name, None)
+        if instr is not None:
+            instr.has_single_gate_props = True
+            return instr
+        return None
+
     def _planqk_backend_to_target(self) -> Target:
         """Converts properties of a PlanQK actual into Qiskit Target object.
 
         Returns:
             target for Qiskit actual
         """
         # building target
-        configuration: ConfigurationDto = self._backend_info.configuration
+
+        configuration: ConfigurationDto = self.backend_info.configuration
         qubit_count: int = configuration.qubit_count
         target = Target(description=f"Target for PlanQK actual {self.name}", num_qubits=qubit_count)
 
-        is_simulator = self._backend_info.type == TYPE.SIMULATOR
-        qubits = configuration.qubits
-        connectivity: ConnectivityDto = self._backend_info.configuration.connectivity
-
-        adapter = ProviderAdapterFactory.get_adapter(self._backend_info.provider)
-
-        single_qubit_props = adapter.single_qubit_gate_props(qubits, is_simulator)
-        multi_qubit_props = adapter.multi_qubit_gate_props(qubits, connectivity, is_simulator)
+        single_qubit_props = self.get_single_qubit_gate_properties()
+        multi_qubit_props = self.get_multi_qubit_gate_properties()
         gates_names = {gate.name.lower() for gate in configuration.gates}
+
         for gate in gates_names:
-            gate = adapter.to_gate(gate, is_simulator)
+            gate = self.to_gate(gate)
 
             if gate is None:
                 continue
 
             if gate.num_qubits == 1:
                 target.add_instruction(instruction=gate, properties=single_qubit_props)
             elif gate.num_qubits > 1:
@@ -92,49 +122,49 @@
                 # For gates without qubit number qargs can not be determined
                 target.add_instruction(instruction=gate, properties={None: None})
 
         target.add_instruction(Measure(), single_qubit_props)
 
         non_gate_instructions = set(configuration.instructions).difference(gates_names).difference({'measure'})
         for non_gate_instruction_name in non_gate_instructions:
-            instruction = adapter.to_non_gate_instruction(non_gate_instruction_name, is_simulator)
+            instruction = self.to_non_gate_instruction(non_gate_instruction_name)
             if instruction is not None:
                 if instruction.has_single_gate_props:
                     target.add_instruction(instruction, single_qubit_props)
                 else:
                     target.add_instruction(instruction=instruction, name=non_gate_instruction_name)
 
         return target
 
     def _planqk_backend_dto_to_configuration(self) -> QasmBackendConfiguration:
         basis_gates = [self._get_gate_config_from_target(basis_gate.name)
-                       for basis_gate in self._backend_info.configuration.gates if basis_gate.native_gate
+                       for basis_gate in self.backend_info.configuration.gates if basis_gate.native_gate
                        and self._get_gate_config_from_target(basis_gate.name) is not None]
         gates = [self._get_gate_config_from_target(gate.name)
-                 for gate in self._backend_info.configuration.gates if not gate.native_gate
+                 for gate in self.backend_info.configuration.gates if not gate.native_gate
                  and self._get_gate_config_from_target(gate.name) is not None]
 
         return QasmBackendConfiguration(
             backend_name=self.name,
             backend_version=self.backend_version,
-            n_qubits=self._backend_info.configuration.qubit_count,
+            n_qubits=self.backend_info.configuration.qubit_count,
             basis_gates=basis_gates,
             gates=gates,
             local=False,
-            simulator=self._backend_info.type == TYPE.SIMULATOR,
+            simulator=self.backend_info.type == TYPE.SIMULATOR,
             conditional=False,
             open_pulse=False,
-            memory=self._backend_info.configuration.memory_result_supported,
-            max_shots=self._backend_info.configuration.shots_range.max,
+            memory=self.backend_info.configuration.memory_result_supported,
+            max_shots=self.backend_info.configuration.shots_range.max,
             coupling_map=self.coupling_map,
             supported_instructions=self._target.instructions,
-            max_experiments=self._backend_info.configuration.shots_range.max,  # Only one circuit is supported per job
-            description=self._backend_info.documentation.description,
-            min_shots=self._backend_info.configuration.shots_range.min,
-            online_date=self._backend_info.updated_at  # TODO replace with online date
+            max_experiments=self.backend_info.configuration.shots_range.max,  # Only one circuit is supported per job
+            description=self.backend_info.documentation.description,
+            min_shots=self.backend_info.configuration.shots_range.min,
+            online_date=self.backend_info.updated_at  # TODO replace with online date
         )
 
     def _get_gate_config_from_target(self, name) -> GateConfig:
         operations = [operation for operation in self._target.operations
                       if isinstance(operation.name, str)  # Filters out the IBM conditional instructions having no name
                       and operation.name.casefold() == name.casefold()]
         if len(operations) == 1:
@@ -151,19 +181,19 @@
 
     @property
     def max_circuits(self):
         return None
 
     @property
     def min_shots(self):
-        return self._backend_info.configuration.shots_range.min
+        return self.backend_info.configuration.shots_range.min
 
     @property
     def max_shots(self):
-        return self._backend_info.configuration.shots_range.max
+        return self.backend_info.configuration.shots_range.max
 
     @classmethod
     def _default_options(cls):
         return OptionsV2()
 
     def run(self, circuit, **kwargs) -> PlanqkJob:
         """Run a circuit on the backend as job.
@@ -179,30 +209,30 @@
         if isinstance(circuit, (list, tuple)):
             if len(circuit) > 1:
                 raise ValueError("Multi-experiment jobs are not supported")
             circuit = circuit[0]
 
         # PennyLane-Qiskit Plugin identifies the result based on the circuit name which must be "circ0"
         circuit.name = "circ0"
-        shots = kwargs.get('shots', self._backend_info.configuration.shots_range.min)
+        shots = kwargs.get('shots', self.backend_info.configuration.shots_range.min)
 
         # add kwargs, if defined as options, to a copy of the options
         options = copy(self.options)
         if kwargs:
             for field in kwargs:
                 if field in options.data:
                     options[field] = kwargs[field]
 
-        supported_input_formats = self._backend_info.configuration.supported_input_formats
+        supported_input_formats = self.backend_info.configuration.supported_input_formats
 
         backend_input = convert_to_backend_input(supported_input_formats, circuit, self, options)
-        input_params = convert_to_backend_params(self._backend_info.provider, circuit, options)
+        input_params = convert_to_backend_params(self.backend_info.provider, circuit, options)
 
-        job_request = JobDto(backend_id=self._backend_info.id,
-                             provider=self._backend_info.provider.name,
+        job_request = JobDto(backend_id=self.backend_info.id,
+                             provider=self.backend_info.provider.name,
                              input_format=backend_input[0],
                              input=backend_input[1],
                              shots=shots,
                              input_params=input_params)
 
         return PlanqkJob(backend=self, job_details=job_request)
 
@@ -224,8 +254,8 @@
             QasmBackendConfiguration: the configuration for the actual.
         """
         return self._configuration
 
     @property
     def backend_provider(self) -> PROVIDER:
         """Return the provider offering the quantum backend resource."""
-        return self._backend_info.provider
+        return self.backend_info.provider
```

### Comparing `planqk-quantum-2.2.1/planqk/qiskit/client/backend_dtos.py` & `planqk-quantum-2.2.2/planqk/qiskit/client/backend_dtos.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-2.2.1/planqk/qiskit/client/client.py` & `planqk-quantum-2.2.2/planqk/qiskit/client/client.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-2.2.1/planqk/qiskit/client/job_dtos.py` & `planqk-quantum-2.2.2/planqk/qiskit/client/job_dtos.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-2.2.1/planqk/qiskit/job.py` & `planqk-quantum-2.2.2/planqk/qiskit/job.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-2.2.1/planqk/qiskit/options.py` & `planqk-quantum-2.2.2/planqk/qiskit/options.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-2.2.1/planqk/qiskit/planqk_runtime_job.py` & `planqk-quantum-2.2.2/planqk/qiskit/planqk_runtime_job.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-2.2.1/planqk/qiskit/provider.py` & `planqk-quantum-2.2.2/planqk/qiskit/provider.py`

 * *Files 4% similar despite different names*

```diff
@@ -89,28 +89,32 @@
             'online_date': backend_dto.updated_at,
             'backend_version': "2",
         }
 
         # add additional parameters to the backend init params
         backend_init_params.update(**kwargs)
 
+        return self._get_backend_object(backend_dto, backend_init_params)
+
+    def _get_backend_object(self, backend_dto, backend_init_params):
         if backend_dto.provider == PROVIDER.AWS:
             from planqk.qiskit.providers.aws.aws_backend import PlanqkAwsBackend
             return PlanqkAwsBackend(**backend_init_params)
         if backend_dto.provider == PROVIDER.AZURE:
             from planqk.qiskit.providers.azure.ionq_backend import PlanqkAzureIonqBackend
             return PlanqkAzureIonqBackend(**backend_init_params)
         elif backend_dto.provider == PROVIDER.QRYD:
             from planqk.qiskit.providers.qryd.qryd_backend import PlanqkQrydBackend
             return PlanqkQrydBackend(**backend_init_params)
         elif backend_dto.provider in {PROVIDER.IBM, PROVIDER.IBM_CLOUD}:
-            from planqk.qiskit.providers.ibm.ibm_backend import PlanqkIbmBackend
-            return PlanqkIbmBackend(**backend_init_params)
+            from planqk.qiskit.providers.ibm.ibm_provider_backend import PlanqkIbmProviderBackend
+            return PlanqkIbmProviderBackend(**backend_init_params)
         else:
-            return PlanqkBackend(**backend_init_params)
+            return QiskitBackendNotFoundError(
+                f"Backends of provider '{backend_dto.provider}' are not supported.")
 
     def retrieve_job(self, backend: PlanqkBackend, job_id: str):
         """
         Retrieve a job from the backend.
 
         Args:
             backend (PlanqkBackend): the backend that run the job.
```

### Comparing `planqk-quantum-2.2.1/planqk/qiskit/providers/aws_adapter.py` & `planqk-quantum-2.2.2/planqk/qiskit/providers/aws/aws_backend.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,32 +1,40 @@
-from typing import Optional, List
+from typing import Optional
 
 from qiskit.circuit import Gate
 from qiskit_braket_provider.providers.adapter import _GATE_NAME_TO_QISKIT_GATE
 
-import planqk.qiskit.providers.adapter as adapter
-from planqk.qiskit.client.backend_dtos import QubitDto, ConnectivityDto
+from planqk.qiskit import PlanqkBackend
+from planqk.qiskit.options import OptionsV2
 
 
-class AwsAdapter(adapter.ProviderAdapter):
-    """Adapter for AWS Braket backend."""
+class PlanqkAwsBackend(PlanqkBackend):
 
-    def to_gate(self, name: str, is_simulator: bool = False) -> Optional[Gate]:
+    def __init__(self, **kwargs):
+        super().__init__(**kwargs)
+
+    @classmethod
+    def _default_options(cls):
+        return OptionsV2()
+
+    def to_gate(self, name: str) -> Optional[Gate]:
         name = name.lower()
         gate = _GATE_NAME_TO_QISKIT_GATE.get(name, None)
         # Braket quantum backends only support 1 and 2 qubit gates
-        return gate if (gate and gate.num_qubits < 3) or is_simulator else None
+        return gate if (gate and gate.num_qubits < 3) or self.is_simulator else None
 
-    def single_qubit_gate_props(self, qubits: List[QubitDto], is_simulator: bool = False):
-        if is_simulator:
+    def get_single_qubit_gate_properties(self) -> dict:
+        if self.is_simulator:
             return {None: None}
-        return {(int(qubit.id),): None for qubit in qubits}
+        return {(int(qubit.id),): None for qubit in self.backend_info.configuration.qubits}
 
-    def multi_qubit_gate_props(self, qubits: List[QubitDto], connectivity: ConnectivityDto, is_simulator: bool = False):
-        if is_simulator:
+    def get_multi_qubit_gate_properties(self) -> dict:
+        qubits = self.backend_info.configuration.qubits
+        connectivity = self.backend_info.configuration.connectivity
+        if self.is_simulator:
             return {None: None}
         if connectivity.fully_connected:
             return {(int(qubit1.id), int(qubit2.id)): None for qubit1 in qubits for qubit2 in qubits
                     if qubit1.id != qubit2.id}
         else:
             return {(int(qubit), int(connected_qubit)): None
                     for qubit, connections in connectivity.graph.items()
```

### Comparing `planqk-quantum-2.2.1/planqk/qiskit/providers/aws_converters.py` & `planqk-quantum-2.2.2/planqk/qiskit/providers/aws_converters.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-2.2.1/planqk/qiskit/providers/ibm/ibm_adapter.py` & `planqk-quantum-2.2.2/planqk/qiskit/providers/ibm/ibm_backend.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,15 +1,17 @@
-from typing import Optional, List
+from typing import Optional
 
-from qiskit.circuit import Gate, IfElseOp, WhileLoopOp, ForLoopOp, SwitchCaseOp, Instruction
+from qiskit.circuit import Gate
+from qiskit.circuit import IfElseOp, WhileLoopOp, ForLoopOp, SwitchCaseOp, Instruction
 from qiskit.circuit import Parameter, Reset
 from qiskit.circuit.library import IGate, SXGate, XGate, CXGate, RZGate, ECRGate, CZGate
+from qiskit.qobj.utils import MeasLevel, MeasReturnType
 
-from planqk.qiskit.client.backend_dtos import QubitDto, ConnectivityDto
-from planqk.qiskit.providers.adapter import ProviderAdapter
+from planqk.qiskit import PlanqkBackend
+from planqk.qiskit.options import OptionsV2
 
 ibm_name_mapping = {
     "id": IGate(),
     "sx": SXGate(),
     "x": XGate(),
     "cx": CXGate(),
     "rz": RZGate(Parameter("λ")),
@@ -22,29 +24,50 @@
     "if_else": IfElseOp,
     "while_loop": WhileLoopOp,
     "for_loop": ForLoopOp,
     "switch_case": SwitchCaseOp,
 }
 
 
-class IbmAdapter(ProviderAdapter):
+class PlanqkIbmBackend(PlanqkBackend):
 
-    def to_gate(self, name: str, is_simulator: bool = False) -> Optional[Gate]:
-        name = name.lower()
+    def __init__(self, **kwargs):
+        PlanqkBackend.__init__(self, **kwargs)
+
+    def _default_options(self):
+        return OptionsV2(
+            shots=4000,
+            memory=False,
+            meas_level=MeasLevel.CLASSIFIED,
+            meas_return=MeasReturnType.AVERAGE,
+            memory_slots=None,
+            memory_slot_size=100,
+            rep_time=None,
+            rep_delay=None,
+            init_qubits=True,
+            use_measure_esp=None,
+            # Simulator only
+            noise_model=None,
+            seed_simulator=None,
+        )
 
+    def to_gate(self, name: str) -> Optional[Gate]:
+        name = name.lower()
         return ibm_name_mapping.get(name, None) or Gate(name, 0, [])
 
-    def to_non_gate_instruction(self, name: str, is_simulator: bool = False) -> Optional[Instruction]:
+    def get_single_qubit_gate_properties(self) -> dict:
+        qubits = self.backend_info.configuration.qubits
+        return {None: None} if self.is_simulator else {(int(qubit.id),): None for qubit in qubits}
+
+    def get_multi_qubit_gate_properties(self) -> dict:
+        connectivity = self.backend_info.configuration.connectivity
+        return {None: None} if self.is_simulator else {(int(qubit), int(connected_qubit)): None
+                                                       for qubit, connections in connectivity.graph.items()
+                                                       for connected_qubit in connections}
+
+    def to_non_gate_instruction(self, name: str) -> Optional[Instruction]:
         if name in qiskit_control_flow_mapping:
             instr = qiskit_control_flow_mapping[name]
             instr.has_single_gate_props = False
             return instr
 
-        return super().to_non_gate_instruction(name, is_simulator)
-
-    def single_qubit_gate_props(self, qubits: List[QubitDto], is_simulator: bool = False):
-        return {None: None} if is_simulator else {(int(qubit.id),): None for qubit in qubits}
-
-    def multi_qubit_gate_props(self, qubits: List[QubitDto], connectivity: ConnectivityDto, is_simulator: bool = False):
-        return {None: None} if is_simulator else {(int(qubit), int(connected_qubit)): None
-                                                  for qubit, connections in connectivity.graph.items()
-                                                  for connected_qubit in connections}
+        return super().to_non_gate_instruction(name)
```

### Comparing `planqk-quantum-2.2.1/planqk/qiskit/providers/ibm/ibm_backend.py` & `planqk-quantum-2.2.2/planqk/qiskit/providers/ibm/ibm_provider_backend.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,64 +1,46 @@
 import json
-from typing import Dict, Optional, List
+from typing import Dict
+from typing import Optional, List
 
 from qiskit import QuantumCircuit
-from qiskit.providers import Options
 from qiskit.providers.models import BackendStatus
-from qiskit.qobj.utils import MeasLevel, MeasReturnType
 from qiskit_ibm_provider import IBMBackend
 from qiskit_ibm_provider.job import IBMCircuitJob
 from qiskit_ibm_provider.utils import RuntimeEncoder
 
-from planqk.qiskit import PlanqkBackend, PlanqkJob
+from planqk.qiskit import PlanqkJob
 from planqk.qiskit.client.backend_dtos import STATUS
 from planqk.qiskit.client.client import _PlanqkClient
 from planqk.qiskit.client.job_dtos import JobDto, INPUT_FORMAT, RuntimeJobParamsDto
-from planqk.qiskit.options import OptionsV2
 from planqk.qiskit.planqk_runtime_job import PlanqkRuntimeJob
+from planqk.qiskit.providers.ibm.ibm_backend import PlanqkIbmBackend
 
 
-def _encode_circuit_base64(circuit: QuantumCircuit, backend: PlanqkBackend, options: Options):
+def _encode_circuit_base64(circuit: QuantumCircuit):
     # Transforms circuit to base64 encoded byte stream
     input_json_str = json.dumps(circuit, cls=RuntimeEncoder)
     # Transform back to json but with the base64 encoded byte stream
     return json.loads(input_json_str)
 
 
-class PlanqkIbmBackend(PlanqkBackend):
+class PlanqkIbmProviderBackend(PlanqkIbmBackend):
 
     def __init__(self, **kwargs):
-        PlanqkBackend.__init__(self, **kwargs)
+        PlanqkIbmBackend.__init__(self, **kwargs)
         self.ibm_backend = IBMBackend(configuration=self.configuration(), provider=None, api_client=None)
         self.ibm_backend._runtime_run = self._submit_job
         self.ibm_backend.status = self.status
 
-    def _default_options(self):
-        return OptionsV2(
-            shots=4000,
-            memory=False,
-            meas_level=MeasLevel.CLASSIFIED,
-            meas_return=MeasReturnType.AVERAGE,
-            memory_slots=None,
-            memory_slot_size=100,
-            rep_time=None,
-            rep_delay=None,
-            init_qubits=True,
-            use_measure_esp=None,
-            # Simulator only
-            noise_model=None,
-            seed_simulator=None,
-        )
-
     def run(self, circuit, **kwargs) -> PlanqkRuntimeJob:
         return IBMBackend.run(self.ibm_backend, circuit, **kwargs)
 
     def status(self):
-        operational = self._backend_info.status == STATUS.ONLINE
-        status_msg = "active" if operational else self._backend_info.status.name.lower()
+        operational = self.backend_info.status == STATUS.ONLINE
+        status_msg = "active" if operational else self.backend_info.status.name.lower()
         pending_jobs = 0  # TODO set pending jobs
 
         return BackendStatus.from_dict({'backend_name': self.name,
                                         'backend_version': self.backend_version,
                                         'operational': operational,
                                         'status_msg': status_msg,
                                         'pending_jobs': pending_jobs})
@@ -75,16 +57,16 @@
         hgp_name = 'ibm-q/open/main'
 
         runtime_job_params = RuntimeJobParamsDto(
             program_id=program_id,
             hgp=hgp_name
         )
 
-        job_request = JobDto(backend_id=self._backend_info.id,
-                             provider=self._backend_info.provider.name,
+        job_request = JobDto(backend_id=self.backend_info.id,
+                             provider=self.backend_info.provider.name,
                              input_format=INPUT_FORMAT.QISKIT,
                              input=encoded_input,
                              shots=inputs.get('shots'),
                              input_params=runtime_job_params.dict())
 
         return PlanqkRuntimeJob(backend=self, job_details=job_request)
```

### Comparing `planqk-quantum-2.2.1/planqk/qiskit/providers/job_input_converter.py` & `planqk-quantum-2.2.2/planqk/qiskit/providers/job_input_converter.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-2.2.1/planqk/qiskit/providers/qryd/pcp_gate.py` & `planqk-quantum-2.2.2/planqk/qiskit/providers/qryd/pcp_gate.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-2.2.1/planqk/qiskit/providers/qryd/pcz_gate.py` & `planqk-quantum-2.2.2/planqk/qiskit/providers/qryd/pcz_gate.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-2.2.1/planqk/qiskit/providers/qryd/qryd_converters.py` & `planqk-quantum-2.2.2/planqk/qiskit/providers/qryd/qryd_converters.py`

 * *Files identical despite different names*

### Comparing `planqk-quantum-2.2.1/planqk/qiskit/runtime_provider.py` & `planqk-quantum-2.2.2/planqk/qiskit/runtime_provider.py`

 * *Files 7% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         # Mock close_session method of API client as it is called by the session object after a program has run
         self._api_client = type('Mock_API_Client', (), {'close_session': lambda self: None})
 
     def backend(
             self,
             name: str = None,
             instance: Optional[str] = None,
-    ) -> str:
+    ):
         """Return a single backend matching the specified filtering.
 
         Args:
             name: Name of the backend.
             instance: This is only supported for ``ibm_quantum`` runtime and is in the
                 hub/group/project format. If an instance is not given, among the providers
                 with access to the backend, a premium provider will be priotized.
@@ -54,14 +54,22 @@
         backend = self.get_backend(name=name)
         if backend.backend_provider not in {PROVIDER.IBM, PROVIDER.IBM_CLOUD, PROVIDER.TSYSTEMS}:
             raise QiskitBackendNotFoundError(
                 f"Backend '{name}' is not from IBM. Qiskit Runtime only supports IBM backends.")
 
         return backend
 
+    def _get_backend_object(self, backend_dto, backend_init_params):
+        if backend_dto.provider in {PROVIDER.IBM, PROVIDER.IBM_CLOUD, PROVIDER.TSYSTEMS}:
+            from planqk.qiskit.providers.ibm.ibm_runtime_backend import PlanqkIbmRuntimeBackend
+            return PlanqkIbmRuntimeBackend(**backend_init_params)
+        else:
+            return QiskitBackendNotFoundError(
+                f"Backends of provider '{backend_dto.provider}' are not supported.")
+
     def run(self,
             program_id: str,
             inputs: Dict,
             options: Optional[Union[RuntimeOptions, Dict]] = None,
             callback: Optional[Callable] = None,
             result_decoder: Optional[Union[Type[ResultDecoder], Sequence[Type[ResultDecoder]]]] = None,
             session_id: Optional[str] = None,
```

### Comparing `planqk-quantum-2.2.1/planqk_quantum.egg-info/PKG-INFO` & `planqk-quantum-2.2.2/planqk_quantum.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: planqk-quantum
-Version: 2.2.1
+Version: 2.2.2
 Summary: Python SDK for the PlanQK Platform
 Home-page: https://github.com/planqk/planqk-quantum
 Author: Anaqor AG
 Author-email: info@anaqor.io
 License: apache-2.0
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `planqk-quantum-2.2.1/planqk_quantum.egg-info/SOURCES.txt` & `planqk-quantum-2.2.2/planqk_quantum.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -16,30 +16,28 @@
 planqk/qiskit/runtime_provider.py
 planqk/qiskit/client/__init__.py
 planqk/qiskit/client/backend_dtos.py
 planqk/qiskit/client/client.py
 planqk/qiskit/client/dto_utils.py
 planqk/qiskit/client/job_dtos.py
 planqk/qiskit/providers/__init__.py
-planqk/qiskit/providers/adapter.py
-planqk/qiskit/providers/aws_adapter.py
 planqk/qiskit/providers/aws_converters.py
-planqk/qiskit/providers/azure_adapter.py
 planqk/qiskit/providers/job_input_converter.py
 planqk/qiskit/providers/aws/__init__.py
 planqk/qiskit/providers/aws/aws_backend.py
 planqk/qiskit/providers/azure/__init__.py
+planqk/qiskit/providers/azure/azure_backend.py
 planqk/qiskit/providers/azure/ionq_backend.py
 planqk/qiskit/providers/ibm/__init__.py
-planqk/qiskit/providers/ibm/ibm_adapter.py
 planqk/qiskit/providers/ibm/ibm_backend.py
+planqk/qiskit/providers/ibm/ibm_provider_backend.py
+planqk/qiskit/providers/ibm/ibm_runtime_backend.py
 planqk/qiskit/providers/qryd/__init__.py
 planqk/qiskit/providers/qryd/pcp_gate.py
 planqk/qiskit/providers/qryd/pcz_gate.py
-planqk/qiskit/providers/qryd/qryd_adapter.py
 planqk/qiskit/providers/qryd/qryd_backend.py
 planqk/qiskit/providers/qryd/qryd_converters.py
 planqk_quantum.egg-info/PKG-INFO
 planqk_quantum.egg-info/SOURCES.txt
 planqk_quantum.egg-info/dependency_links.txt
 planqk_quantum.egg-info/requires.txt
 planqk_quantum.egg-info/top_level.txt
```

### Comparing `planqk-quantum-2.2.1/setup.py` & `planqk-quantum-2.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 with open('./requirements.txt', 'r') as fh:
     requirements = fh.readlines()
 
 setup(
     name='planqk-quantum',
-    version="2.2.1",
+    version="2.2.2",
     author='Anaqor AG',
     author_email='info@anaqor.io',
     url='https://github.com/planqk/planqk-quantum',
     description='Python SDK for the PlanQK Platform',
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_namespace_packages(include=['planqk', 'planqk.*']),
```

