# Comparing `tmp/qandle-0.0.4.tar.gz` & `tmp/qandle-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qandle-0.0.4.tar", max compression
+gzip compressed data, was "qandle-0.0.5.tar", max compression
```

## Comparing `qandle-0.0.4.tar` & `qandle-0.0.5.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0     1093 2024-03-30 18:49:42.545657 qandle-0.0.4/LICENSE
--rw-r--r--   0        0        0     1135 2024-03-31 18:29:44.605494 qandle-0.0.4/pyproject.toml
--rw-r--r--   0        0        0     1261 2024-03-31 11:31:53.551883 qandle-0.0.4/README.md
--rw-r--r--   0        0        0      811 2024-03-14 10:47:47.000000 qandle-0.0.4/src/qandle/__init__.py
--rw-r--r--   0        0        0      165 2024-02-21 11:31:40.000000 qandle-0.0.4/src/qandle/ansaetze/__init__.py
--rw-r--r--   0        0        0      542 2024-03-11 16:28:49.000000 qandle-0.0.4/src/qandle/ansaetze/ansatz.py
--rw-r--r--   0        0        0     3104 2024-03-14 10:47:47.000000 qandle-0.0.4/src/qandle/ansaetze/specialunitary.py
--rw-r--r--   0        0        0     3712 2024-03-14 10:47:47.000000 qandle-0.0.4/src/qandle/ansaetze/stronglyentangling.py
--rw-r--r--   0        0        0     3515 2024-03-14 10:47:47.000000 qandle-0.0.4/src/qandle/ansaetze/twolocal.py
--rw-r--r--   0        0        0     3699 2024-03-11 16:28:49.000000 qandle-0.0.4/src/qandle/config.py
--rw-r--r--   0        0        0     2430 2024-03-11 16:28:49.000000 qandle-0.0.4/src/qandle/convolution.py
--rw-r--r--   0        0        0     5283 2024-03-11 16:28:49.000000 qandle-0.0.4/src/qandle/drawer.py
--rw-r--r--   0        0        0     4143 2024-03-19 14:44:34.000000 qandle-0.0.4/src/qandle/embeddings.py
--rw-r--r--   0        0        0      248 2024-03-11 16:28:49.000000 qandle-0.0.4/src/qandle/errors.py
--rw-r--r--   0        0        0     3957 2024-03-19 14:56:38.000000 qandle-0.0.4/src/qandle/measurements.py
--rw-r--r--   0        0        0    16116 2024-03-14 10:47:47.000000 qandle-0.0.4/src/qandle/operators.py
--rw-r--r--   0        0        0     1614 2024-03-19 11:24:27.000000 qandle-0.0.4/src/qandle/qasm.py
--rw-r--r--   0        0        0    10804 2024-03-19 11:54:11.000000 qandle-0.0.4/src/qandle/qcircuit.py
--rw-r--r--   0        0        0      195 2024-03-31 16:46:23.306355 qandle-0.0.4/src/qandle/requirements.txt
--rw-r--r--   0        0        0      107 2024-02-21 11:31:40.000000 qandle-0.0.4/src/qandle/splitter/__init__.py
--rw-r--r--   0        0        0     2199 2024-03-11 16:28:49.000000 qandle-0.0.4/src/qandle/splitter/grouping.py
--rw-r--r--   0        0        0     6173 2024-03-28 19:34:23.000000 qandle-0.0.4/src/qandle/splitter/main.py
--rw-r--r--   0        0        0        0 2023-11-12 15:37:29.000000 qandle-0.0.4/src/qandle/test/__init__.py
--rw-r--r--   0        0        0      326 2024-03-14 10:47:47.000000 qandle-0.0.4/src/qandle/test/check_qasm.py
--rw-r--r--   0        0        0     3293 2024-03-14 10:47:47.000000 qandle-0.0.4/src/qandle/test/test_ansaetze.py
--rw-r--r--   0        0        0     1352 2024-02-21 11:31:40.000000 qandle-0.0.4/src/qandle/test/test_convolution.py
--rw-r--r--   0        0        0     4524 2024-02-21 11:31:40.000000 qandle-0.0.4/src/qandle/test/test_embeddings.py
--rw-r--r--   0        0        0     1860 2024-03-11 17:19:06.000000 qandle-0.0.4/src/qandle/test/test_measurements.py
--rw-r--r--   0        0        0     6530 2024-03-14 10:47:47.000000 qandle-0.0.4/src/qandle/test/test_operators.py
--rw-r--r--   0        0        0     2593 2024-03-14 10:47:47.000000 qandle-0.0.4/src/qandle/test/test_splitter.py
--rw-r--r--   0        0        0     2750 2024-03-11 16:28:49.000000 qandle-0.0.4/src/qandle/utils.py
--rw-r--r--   0        0        0     2484 1970-01-01 00:00:00.000000 qandle-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0     1093 2024-03-30 18:49:42.545657 qandle-0.0.5/LICENSE
+-rw-r--r--   0        0        0     1135 2024-04-16 14:11:16.277187 qandle-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0     1854 2024-04-16 14:09:46.711412 qandle-0.0.5/README.md
+-rw-r--r--   0        0        0      811 2024-03-14 10:47:47.000000 qandle-0.0.5/src/qandle/__init__.py
+-rw-r--r--   0        0        0      165 2024-02-21 11:31:40.000000 qandle-0.0.5/src/qandle/ansaetze/__init__.py
+-rw-r--r--   0        0        0      542 2024-03-11 16:28:49.000000 qandle-0.0.5/src/qandle/ansaetze/ansatz.py
+-rw-r--r--   0        0        0     3104 2024-03-14 10:47:47.000000 qandle-0.0.5/src/qandle/ansaetze/specialunitary.py
+-rw-r--r--   0        0        0     3712 2024-03-14 10:47:47.000000 qandle-0.0.5/src/qandle/ansaetze/stronglyentangling.py
+-rw-r--r--   0        0        0     3515 2024-03-14 10:47:47.000000 qandle-0.0.5/src/qandle/ansaetze/twolocal.py
+-rw-r--r--   0        0        0     3699 2024-03-11 16:28:49.000000 qandle-0.0.5/src/qandle/config.py
+-rw-r--r--   0        0        0     2430 2024-03-11 16:28:49.000000 qandle-0.0.5/src/qandle/convolution.py
+-rw-r--r--   0        0        0     5283 2024-03-11 16:28:49.000000 qandle-0.0.5/src/qandle/drawer.py
+-rw-r--r--   0        0        0     4143 2024-03-19 14:44:34.000000 qandle-0.0.5/src/qandle/embeddings.py
+-rw-r--r--   0        0        0      248 2024-03-11 16:28:49.000000 qandle-0.0.5/src/qandle/errors.py
+-rw-r--r--   0        0        0     3957 2024-03-19 14:56:38.000000 qandle-0.0.5/src/qandle/measurements.py
+-rw-r--r--   0        0        0    16116 2024-03-14 10:47:47.000000 qandle-0.0.5/src/qandle/operators.py
+-rw-r--r--   0        0        0     1614 2024-03-19 11:24:27.000000 qandle-0.0.5/src/qandle/qasm.py
+-rw-r--r--   0        0        0    10804 2024-03-19 11:54:11.000000 qandle-0.0.5/src/qandle/qcircuit.py
+-rw-r--r--   0        0        0      195 2024-03-31 16:46:23.306355 qandle-0.0.5/src/qandle/requirements.txt
+-rw-r--r--   0        0        0      107 2024-02-21 11:31:40.000000 qandle-0.0.5/src/qandle/splitter/__init__.py
+-rw-r--r--   0        0        0     2199 2024-03-11 16:28:49.000000 qandle-0.0.5/src/qandle/splitter/grouping.py
+-rw-r--r--   0        0        0     6173 2024-03-28 19:34:23.000000 qandle-0.0.5/src/qandle/splitter/main.py
+-rw-r--r--   0        0        0        0 2023-11-12 15:37:29.000000 qandle-0.0.5/src/qandle/test/__init__.py
+-rw-r--r--   0        0        0      326 2024-03-14 10:47:47.000000 qandle-0.0.5/src/qandle/test/check_qasm.py
+-rw-r--r--   0        0        0     3293 2024-03-14 10:47:47.000000 qandle-0.0.5/src/qandle/test/test_ansaetze.py
+-rw-r--r--   0        0        0     1352 2024-02-21 11:31:40.000000 qandle-0.0.5/src/qandle/test/test_convolution.py
+-rw-r--r--   0        0        0     4524 2024-02-21 11:31:40.000000 qandle-0.0.5/src/qandle/test/test_embeddings.py
+-rw-r--r--   0        0        0     1860 2024-03-11 17:19:06.000000 qandle-0.0.5/src/qandle/test/test_measurements.py
+-rw-r--r--   0        0        0     6530 2024-03-14 10:47:47.000000 qandle-0.0.5/src/qandle/test/test_operators.py
+-rw-r--r--   0        0        0     2593 2024-03-14 10:47:47.000000 qandle-0.0.5/src/qandle/test/test_splitter.py
+-rw-r--r--   0        0        0     2750 2024-03-11 16:28:49.000000 qandle-0.0.5/src/qandle/utils.py
+-rw-r--r--   0        0        0     3077 1970-01-01 00:00:00.000000 qandle-0.0.5/PKG-INFO
```

### Comparing `qandle-0.0.4/LICENSE` & `qandle-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `qandle-0.0.4/pyproject.toml` & `qandle-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "qandle"
-version = "0.0.4"
+version = "0.0.5"
 description = "QANDLE is a fast and simple quantum state-vector simulator for hybrid machine learning using the PyTorch library."
 authors = ["Gerhard Stenzel <gerhard.stenzel@ifi.lmu.de>"]
 license = "MIT"
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
```

### Comparing `qandle-0.0.4/README.md` & `qandle-0.0.5/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # QANDLE
 **QANDLE** is a fast and simple quantum state-vector simulator for hybrid machine learning using the PyTorch library.
-Documentation and examples can be found in the [QANDLE documentation](https://gstenzel.github.io/qandle/).
+Documentation and examples can be found in the [QANDLE documentation](https://gstenzel.github.io/qandle/), the code resides on [GitHub](https://github.com/gstenzel/qandle).
+The paper can be found on [arXiv](https://arxiv.org/abs/2404.09213).
 
 ## Installation
 ```bash
 pip install qandle
 ```
 
 ## Usage
@@ -37,7 +38,19 @@
 # Run the circuit
 circuit(input_state, data_reuploading=data_reuploading)
 ```	
 
 ## License
 This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
 
+## Citation
+If you use QANDLE in your research, please cite the following paper:
+```bbl
+@misc{qandle2024,
+      title={Qandle: Accelerating State Vector Simulation Using Gate-Matrix Caching and Circuit Splitting}, 
+      author={Gerhard Stenzel and Sebastian Zielinski and Michael Kölle and Philipp Altmann and Jonas Nüßlein and Thomas Gabor},
+      year={2024},
+      eprint={2404.09213},
+      archivePrefix={arXiv},
+      primaryClass={quant-ph}
+}
+```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `qandle-0.0.4/src/qandle/__init__.py` & `qandle-0.0.5/src/qandle/__init__.py`

 * *Files identical despite different names*

### Comparing `qandle-0.0.4/src/qandle/ansaetze/ansatz.py` & `qandle-0.0.5/src/qandle/ansaetze/ansatz.py`

 * *Files identical despite different names*

### Comparing `qandle-0.0.4/src/qandle/ansaetze/specialunitary.py` & `qandle-0.0.5/src/qandle/ansaetze/specialunitary.py`

 * *Files identical despite different names*

### Comparing `qandle-0.0.4/src/qandle/ansaetze/stronglyentangling.py` & `qandle-0.0.5/src/qandle/ansaetze/stronglyentangling.py`

 * *Files identical despite different names*

### Comparing `qandle-0.0.4/src/qandle/ansaetze/twolocal.py` & `qandle-0.0.5/src/qandle/ansaetze/twolocal.py`

 * *Files identical despite different names*

### Comparing `qandle-0.0.4/src/qandle/config.py` & `qandle-0.0.5/src/qandle/config.py`

 * *Files identical despite different names*

### Comparing `qandle-0.0.4/src/qandle/convolution.py` & `qandle-0.0.5/src/qandle/convolution.py`

 * *Files identical despite different names*

### Comparing `qandle-0.0.4/src/qandle/drawer.py` & `qandle-0.0.5/src/qandle/drawer.py`

 * *Files identical despite different names*

### Comparing `qandle-0.0.4/src/qandle/embeddings.py` & `qandle-0.0.5/src/qandle/embeddings.py`

 * *Files identical despite different names*

### Comparing `qandle-0.0.4/src/qandle/measurements.py` & `qandle-0.0.5/src/qandle/measurements.py`

 * *Files identical despite different names*

### Comparing `qandle-0.0.4/src/qandle/operators.py` & `qandle-0.0.5/src/qandle/operators.py`

 * *Files identical despite different names*

### Comparing `qandle-0.0.4/src/qandle/qasm.py` & `qandle-0.0.5/src/qandle/qasm.py`

 * *Files identical despite different names*

### Comparing `qandle-0.0.4/src/qandle/qcircuit.py` & `qandle-0.0.5/src/qandle/qcircuit.py`

 * *Files identical despite different names*

### Comparing `qandle-0.0.4/src/qandle/splitter/grouping.py` & `qandle-0.0.5/src/qandle/splitter/grouping.py`

 * *Files identical despite different names*

### Comparing `qandle-0.0.4/src/qandle/splitter/main.py` & `qandle-0.0.5/src/qandle/splitter/main.py`

 * *Files identical despite different names*

### Comparing `qandle-0.0.4/src/qandle/test/test_ansaetze.py` & `qandle-0.0.5/src/qandle/test/test_ansaetze.py`

 * *Files identical despite different names*

### Comparing `qandle-0.0.4/src/qandle/test/test_convolution.py` & `qandle-0.0.5/src/qandle/test/test_convolution.py`

 * *Files identical despite different names*

### Comparing `qandle-0.0.4/src/qandle/test/test_embeddings.py` & `qandle-0.0.5/src/qandle/test/test_embeddings.py`

 * *Files identical despite different names*

### Comparing `qandle-0.0.4/src/qandle/test/test_measurements.py` & `qandle-0.0.5/src/qandle/test/test_measurements.py`

 * *Files identical despite different names*

### Comparing `qandle-0.0.4/src/qandle/test/test_operators.py` & `qandle-0.0.5/src/qandle/test/test_operators.py`

 * *Files identical despite different names*

### Comparing `qandle-0.0.4/src/qandle/test/test_splitter.py` & `qandle-0.0.5/src/qandle/test/test_splitter.py`

 * *Files identical despite different names*

### Comparing `qandle-0.0.4/src/qandle/utils.py` & `qandle-0.0.5/src/qandle/utils.py`

 * *Files identical despite different names*

### Comparing `qandle-0.0.4/PKG-INFO` & `qandle-0.0.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qandle
-Version: 0.0.4
+Version: 0.0.5
 Summary: QANDLE is a fast and simple quantum state-vector simulator for hybrid machine learning using the PyTorch library.
 License: MIT
 Author: Gerhard Stenzel
 Author-email: gerhard.stenzel@ifi.lmu.de
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: GPU :: NVIDIA CUDA
@@ -25,15 +25,16 @@
 Requires-Dist: torch (>=2.0,<3.0)
 Project-URL: documentation, https://gstenzel.github.io/qandle/
 Project-URL: repository, https://github.com/gstenzel/qandle/
 Description-Content-Type: text/markdown
 
 # QANDLE
 **QANDLE** is a fast and simple quantum state-vector simulator for hybrid machine learning using the PyTorch library.
-Documentation and examples can be found in the [QANDLE documentation](https://gstenzel.github.io/qandle/).
+Documentation and examples can be found in the [QANDLE documentation](https://gstenzel.github.io/qandle/), the code resides on [GitHub](https://github.com/gstenzel/qandle).
+The paper can be found on [arXiv](https://arxiv.org/abs/2404.09213).
 
 ## Installation
 ```bash
 pip install qandle
 ```
 
 ## Usage
@@ -66,8 +67,20 @@
 # Run the circuit
 circuit(input_state, data_reuploading=data_reuploading)
 ```	
 
 ## License
 This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.
 
+## Citation
+If you use QANDLE in your research, please cite the following paper:
+```bbl
+@misc{qandle2024,
+      title={Qandle: Accelerating State Vector Simulation Using Gate-Matrix Caching and Circuit Splitting}, 
+      author={Gerhard Stenzel and Sebastian Zielinski and Michael Kölle and Philipp Altmann and Jonas Nüßlein and Thomas Gabor},
+      year={2024},
+      eprint={2404.09213},
+      archivePrefix={arXiv},
+      primaryClass={quant-ph}
+}
+```
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

