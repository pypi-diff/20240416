# Comparing `tmp/QDsim-1.0.0.tar.gz` & `tmp/qdsim-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "QDsim-1.0.0.tar", last modified: Tue Apr  2 15:35:55 2024, max compression
+gzip compressed data, was "qdsim-1.0.1.tar", last modified: Tue Apr 16 12:53:40 2024, max compression
```

## Comparing `QDsim-1.0.0.tar` & `qdsim-1.0.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 valentinagualt (2043739619) DASTUD\Domain Users (1653728465)        0 2024-04-02 15:35:55.722385 QDsim-1.0.0/
--rw-rw-r--   0 valentinagualt (2043739619) DASTUD\Domain Users (1653728465)     1076 2024-03-26 09:26:22.000000 QDsim-1.0.0/LICENSE
--rw-r--r--   0 valentinagualt (2043739619) DASTUD\Domain Users (1653728465)     4808 2024-04-02 15:35:55.722190 QDsim-1.0.0/PKG-INFO
-drwxr-xr-x   0 valentinagualt (2043739619) DASTUD\Domain Users (1653728465)        0 2024-04-02 15:35:55.721966 QDsim-1.0.0/QDsim.egg-info/
--rw-r--r--   0 valentinagualt (2043739619) DASTUD\Domain Users (1653728465)     4808 2024-04-02 15:35:55.000000 QDsim-1.0.0/QDsim.egg-info/PKG-INFO
--rw-r--r--   0 valentinagualt (2043739619) DASTUD\Domain Users (1653728465)      324 2024-04-02 15:35:55.000000 QDsim-1.0.0/QDsim.egg-info/SOURCES.txt
--rw-r--r--   0 valentinagualt (2043739619) DASTUD\Domain Users (1653728465)        1 2024-04-02 15:35:55.000000 QDsim-1.0.0/QDsim.egg-info/dependency_links.txt
--rw-r--r--   0 valentinagualt (2043739619) DASTUD\Domain Users (1653728465)        6 2024-04-02 15:35:55.000000 QDsim-1.0.0/QDsim.egg-info/top_level.txt
--rw-r--r--   0 valentinagualt (2043739619) DASTUD\Domain Users (1653728465)     4131 2024-04-02 15:10:19.000000 QDsim-1.0.0/README.md
--rw-r--r--   0 valentinagualt (2043739619) DASTUD\Domain Users (1653728465)      788 2024-04-02 15:27:37.000000 QDsim-1.0.0/pyproject.toml
-drwxr-xr-x   0 valentinagualt (2043739619) DASTUD\Domain Users (1653728465)        0 2024-04-02 15:35:55.721571 QDsim-1.0.0/qdsim/
--rw-r--r--   0 valentinagualt (2043739619) DASTUD\Domain Users (1653728465)    16953 2024-03-26 10:53:41.000000 QDsim-1.0.0/qdsim/_CapacitanceQDArray.py
--rw-r--r--   0 valentinagualt (2043739619) DASTUD\Domain Users (1653728465)    44284 2024-03-27 13:02:57.000000 QDsim-1.0.0/qdsim/_QuantumDotDevice.py
--rw-r--r--   0 valentinagualt (2043739619) DASTUD\Domain Users (1653728465)    45674 2024-04-02 14:44:04.000000 QDsim-1.0.0/qdsim/_QuantumDotSimulator.py
--rw-r--r--   0 valentinagualt (2043739619) DASTUD\Domain Users (1653728465)      246 2024-03-26 10:58:30.000000 QDsim-1.0.0/qdsim/__init__.py
--rw-r--r--   0 valentinagualt (2043739619) DASTUD\Domain Users (1653728465)     2473 2023-10-18 14:16:51.000000 QDsim-1.0.0/qdsim/_auxiliaryfunctions.py
--rw-r--r--   0 valentinagualt (2043739619) DASTUD\Domain Users (1653728465)     4104 2023-10-23 09:01:22.000000 QDsim-1.0.0/qdsim/_noisefunctions.py
--rw-r--r--   0 valentinagualt (2043739619) DASTUD\Domain Users (1653728465)     6104 2024-04-02 14:08:04.000000 QDsim-1.0.0/qdsim/_plotCSD.py
--rw-r--r--   0 valentinagualt (2043739619) DASTUD\Domain Users (1653728465)       38 2024-04-02 15:35:55.722440 QDsim-1.0.0/setup.cfg
+drwxr-xr-x   0 valentinagualt (2043739619) 1653728465        0 2024-04-16 12:53:40.735328 qdsim-1.0.1/
+-rw-rw-r--   0 valentinagualt (2043739619) 1653728465     1076 2024-03-26 09:26:22.000000 qdsim-1.0.1/LICENSE
+-rw-r--r--   0 valentinagualt (2043739619) 1653728465     4959 2024-04-16 12:53:40.735137 qdsim-1.0.1/PKG-INFO
+drwxr-xr-x   0 valentinagualt (2043739619) 1653728465        0 2024-04-16 12:53:40.734929 qdsim-1.0.1/QDsim.egg-info/
+-rw-r--r--   0 valentinagualt (2043739619) 1653728465     4959 2024-04-16 12:53:40.000000 qdsim-1.0.1/QDsim.egg-info/PKG-INFO
+-rw-r--r--   0 valentinagualt (2043739619) 1653728465      324 2024-04-16 12:53:40.000000 qdsim-1.0.1/QDsim.egg-info/SOURCES.txt
+-rw-r--r--   0 valentinagualt (2043739619) 1653728465        1 2024-04-16 12:53:40.000000 qdsim-1.0.1/QDsim.egg-info/dependency_links.txt
+-rw-r--r--   0 valentinagualt (2043739619) 1653728465        6 2024-04-16 12:53:40.000000 qdsim-1.0.1/QDsim.egg-info/top_level.txt
+-rw-r--r--   0 valentinagualt (2043739619) 1653728465     4282 2024-04-02 15:43:06.000000 qdsim-1.0.1/README.md
+-rw-r--r--   0 valentinagualt (2043739619) 1653728465      788 2024-04-16 12:43:11.000000 qdsim-1.0.1/pyproject.toml
+drwxr-xr-x   0 valentinagualt (2043739619) 1653728465        0 2024-04-16 12:53:40.734656 qdsim-1.0.1/qdsim/
+-rw-r--r--   0 valentinagualt (2043739619) 1653728465    16953 2024-03-26 10:53:41.000000 qdsim-1.0.1/qdsim/_CapacitanceQDArray.py
+-rw-r--r--   0 valentinagualt (2043739619) 1653728465    44284 2024-03-27 13:02:57.000000 qdsim-1.0.1/qdsim/_QuantumDotDevice.py
+-rw-r--r--   0 valentinagualt (2043739619) 1653728465    47171 2024-04-12 08:10:40.000000 qdsim-1.0.1/qdsim/_QuantumDotSimulator.py
+-rw-r--r--   0 valentinagualt (2043739619) 1653728465      306 2024-04-16 12:35:25.000000 qdsim-1.0.1/qdsim/__init__.py
+-rw-r--r--   0 valentinagualt (2043739619) 1653728465     2473 2023-10-18 14:16:51.000000 qdsim-1.0.1/qdsim/_auxiliaryfunctions.py
+-rw-r--r--   0 valentinagualt (2043739619) 1653728465     4104 2023-10-23 09:01:22.000000 qdsim-1.0.1/qdsim/_noisefunctions.py
+-rw-r--r--   0 valentinagualt (2043739619) 1653728465     6104 2024-04-02 14:08:04.000000 qdsim-1.0.1/qdsim/_plotCSD.py
+-rw-r--r--   0 valentinagualt (2043739619) 1653728465       38 2024-04-16 12:53:40.735380 qdsim-1.0.1/setup.cfg
```

### Comparing `QDsim-1.0.0/LICENSE` & `qdsim-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `QDsim-1.0.0/PKG-INFO` & `qdsim-1.0.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QDsim
-Version: 1.0.0
+Version: 1.0.1
 Summary: QDsim is an user-friendly tool that quickly simulates charge stability diagrams for large quantum dot devices (even 100+ dots).
 Author: Charles Renshaw-Whitman, Vinicius F. Hernandes, Eliška Greplová
 Author-email: Valentina Gualtieri <v.gualtieri@tudelft.nl>
 Project-URL: Homepage, https://gitlab.com/QMAI/papers/qdsim/
 Project-URL: Issues, https://gitlab.com/QMAI/papers/qdsim/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -73,14 +73,17 @@
     scanning_gate_indexes=[0, 1])
 
 # Step 3: Plot the charge stability diagram
 qdsimulator.plot_charge_stability_diagrams()
 ```
 <img style="float: right;" src="results/figures/DQD_current.png">
 
+## Contributing
+We welcome contributors and collaborators.
+The person wanting to contribute can start by opening an issue and they will hear from us. 
 
 ## Authors and acknowledgment
 Here is a list of authors who have contributed to this project:
 - [Valentina Gualtieri](https://github.com/vgualtieri)
 - Charles Renshaw-Whitman
 - [Vinicius F. Hernandes](https://gitlab.com/vfhernandes)
 - [Eliška Greplová](https://github.com/greplova)
```

### Comparing `QDsim-1.0.0/QDsim.egg-info/PKG-INFO` & `qdsim-1.0.1/QDsim.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QDsim
-Version: 1.0.0
+Version: 1.0.1
 Summary: QDsim is an user-friendly tool that quickly simulates charge stability diagrams for large quantum dot devices (even 100+ dots).
 Author: Charles Renshaw-Whitman, Vinicius F. Hernandes, Eliška Greplová
 Author-email: Valentina Gualtieri <v.gualtieri@tudelft.nl>
 Project-URL: Homepage, https://gitlab.com/QMAI/papers/qdsim/
 Project-URL: Issues, https://gitlab.com/QMAI/papers/qdsim/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
@@ -73,14 +73,17 @@
     scanning_gate_indexes=[0, 1])
 
 # Step 3: Plot the charge stability diagram
 qdsimulator.plot_charge_stability_diagrams()
 ```
 <img style="float: right;" src="results/figures/DQD_current.png">
 
+## Contributing
+We welcome contributors and collaborators.
+The person wanting to contribute can start by opening an issue and they will hear from us. 
 
 ## Authors and acknowledgment
 Here is a list of authors who have contributed to this project:
 - [Valentina Gualtieri](https://github.com/vgualtieri)
 - Charles Renshaw-Whitman
 - [Vinicius F. Hernandes](https://gitlab.com/vfhernandes)
 - [Eliška Greplová](https://github.com/greplova)
```

### Comparing `QDsim-1.0.0/README.md` & `qdsim-1.0.1/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -58,14 +58,17 @@
     scanning_gate_indexes=[0, 1])
 
 # Step 3: Plot the charge stability diagram
 qdsimulator.plot_charge_stability_diagrams()
 ```
 <img style="float: right;" src="results/figures/DQD_current.png">
 
+## Contributing
+We welcome contributors and collaborators.
+The person wanting to contribute can start by opening an issue and they will hear from us. 
 
 ## Authors and acknowledgment
 Here is a list of authors who have contributed to this project:
 - [Valentina Gualtieri](https://github.com/vgualtieri)
 - Charles Renshaw-Whitman
 - [Vinicius F. Hernandes](https://gitlab.com/vfhernandes)
 - [Eliška Greplová](https://github.com/greplova)
```

### Comparing `QDsim-1.0.0/pyproject.toml` & `qdsim-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "QDsim"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
   { name = "Valentina Gualtieri", email = "v.gualtieri@tudelft.nl" },
   { name = "Charles Renshaw-Whitman" },
   { name = "Vinicius F. Hernandes" },
   { name = "Eliška Greplová"},
 ]
 description = "QDsim is an user-friendly tool that quickly simulates charge stability diagrams for large quantum dot devices (even 100+ dots)."
```

### Comparing `QDsim-1.0.0/qdsim/_CapacitanceQDArray.py` & `qdsim-1.0.1/qdsim/_CapacitanceQDArray.py`

 * *Files identical despite different names*

### Comparing `QDsim-1.0.0/qdsim/_QuantumDotDevice.py` & `qdsim-1.0.1/qdsim/_QuantumDotDevice.py`

 * *Files identical despite different names*

### Comparing `QDsim-1.0.0/qdsim/_QuantumDotSimulator.py` & `qdsim-1.0.1/qdsim/_QuantumDotSimulator.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 import tqdm
 from ._plotCSD import *  # for plotting
 import matplotlib.pyplot as plt
 from ._auxiliaryfunctions import *
 import copy
 import json
 import os
+from datetime import datetime
+
 from itertools import combinations
 
 
 class QDSimulator:
     """
     Class for simulating the charge stability diagram of a quantum dot array, in the constant interaction model.
 
@@ -821,14 +823,52 @@
             if isinstance(attr_value, np.ndarray):
                 attr_value = attr_value.tolist()
 
             attribute_dict[attr_name] = attr_value
 
         return attribute_dict
 
+    def save(self, path_to_root=None):
+        """
+        Saves all the information of the device and the simulation in a structured way.
+        Useful for creating datasets.
+
+
+        Args:
+            path_to_root (str, optional): The path to the root directory where a 'dataset' folder will be created and
+            filled with one folder per simulation. If None, the current working directory is used. Defaults to None.
+
+        Returns:
+            None
+
+        """
+        if path_to_root is None:
+            path_to_root = os.getcwd()
+
+        # Create the directory if it does not exist
+        if not os.path.exists(path_to_root):
+            os.makedirs(f"{path_to_root}/dataset")
+
+        # Create a directory for the simulation in the dataset folder
+        timestamp = datetime.now().strftime('%Y-%m-%d_%H-%M-%S')
+        simulation_folder = f"{path_to_root}/dataset/simulation_{timestamp}"
+        os.makedirs(simulation_folder)
+
+        # Save the QDDevice and QDSimulator information in a JSON file (but not the simulated results)
+        self.save_to_json(self, f"{simulation_folder}/simulation_info_{timestamp}.json")
+
+        npy_folder = f"{simulation_folder}/npy_files"
+        os.makedirs(npy_folder)
+
+        # Save the simulated results in .npy files
+        self.save_results_to_npy(f"{npy_folder}/voltage_occupation_data.npy", f"{npy_folder}/sensing_data.npy",
+                                    f"{npy_folder}/current_data.npy")
+
+
+
 
 ########################################################################################################################
 # Auxiliary functions, not part of the class
 
 
 def generate_linspace_arrays(v_ranges, n_points):
     """
```

### Comparing `QDsim-1.0.0/qdsim/_auxiliaryfunctions.py` & `qdsim-1.0.1/qdsim/_auxiliaryfunctions.py`

 * *Files identical despite different names*

### Comparing `QDsim-1.0.0/qdsim/_noisefunctions.py` & `qdsim-1.0.1/qdsim/_noisefunctions.py`

 * *Files identical despite different names*

### Comparing `QDsim-1.0.0/qdsim/_plotCSD.py` & `qdsim-1.0.1/qdsim/_plotCSD.py`

 * *Files identical despite different names*

