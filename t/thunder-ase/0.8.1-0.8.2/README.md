# Comparing `tmp/thunder-ase-0.8.1.tar.gz` & `tmp/thunder_ase-0.8.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "thunder-ase-0.8.1.tar", last modified: Fri Mar 29 02:33:04 2024, max compression
+gzip compressed data, was "thunder_ase-0.8.2.tar", last modified: Tue Apr 16 11:34:11 2024, max compression
```

## Comparing `thunder-ase-0.8.1.tar` & `thunder_ase-0.8.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 02:33:04.243111 thunder-ase-0.8.1/
--rw-r--r--   0 runner    (1001) docker     (127)     8689 2024-03-29 02:33:04.243111 thunder-ase-0.8.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8345 2024-03-29 02:32:55.000000 thunder-ase-0.8.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      722 2024-03-29 02:32:55.000000 thunder-ase-0.8.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-29 02:33:04.243111 thunder-ase-0.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-29 02:32:55.000000 thunder-ase-0.8.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 02:33:04.243111 thunder-ase-0.8.1/thunder_ase/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-29 02:32:55.000000 thunder-ase-0.8.1/thunder_ase/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    33543 2024-03-29 02:32:55.000000 thunder-ase-0.8.1/thunder_ase/fireball.py
--rw-r--r--   0 runner    (1001) docker     (127)     6726 2024-03-29 02:32:55.000000 thunder-ase-0.8.1/thunder_ase/optimize.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 02:33:04.243111 thunder-ase-0.8.1/thunder_ase/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-03-29 02:32:55.000000 thunder-ase-0.8.1/thunder_ase/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10921 2024-03-29 02:32:55.000000 thunder-ase-0.8.1/thunder_ase/utils/basis_set.py
--rw-r--r--   0 runner    (1001) docker     (127)     5041 2024-03-29 02:32:55.000000 thunder-ase-0.8.1/thunder_ase/utils/mwfn.py
--rw-r--r--   0 runner    (1001) docker     (127)     2694 2024-03-29 02:32:55.000000 thunder-ase-0.8.1/thunder_ase/utils/shell_dict.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-29 02:33:04.243111 thunder-ase-0.8.1/thunder_ase.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8689 2024-03-29 02:33:04.000000 thunder-ase-0.8.1/thunder_ase.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      402 2024-03-29 02:33:04.000000 thunder-ase-0.8.1/thunder_ase.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-29 02:33:04.000000 thunder-ase-0.8.1/thunder_ase.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       65 2024-03-29 02:33:04.000000 thunder-ase-0.8.1/thunder_ase.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-03-29 02:33:04.000000 thunder-ase-0.8.1/thunder_ase.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:34:11.506564 thunder_ase-0.8.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     8687 2024-04-16 11:34:11.506564 thunder_ase-0.8.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8343 2024-04-16 11:34:06.000000 thunder_ase-0.8.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      722 2024-04-16 11:34:06.000000 thunder_ase-0.8.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 11:34:11.506564 thunder_ase-0.8.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 11:34:06.000000 thunder_ase-0.8.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:34:11.502565 thunder_ase-0.8.2/thunder_ase/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 11:34:06.000000 thunder_ase-0.8.2/thunder_ase/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    33664 2024-04-16 11:34:06.000000 thunder_ase-0.8.2/thunder_ase/fireball.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6726 2024-04-16 11:34:06.000000 thunder_ase-0.8.2/thunder_ase/optimize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:34:11.506564 thunder_ase-0.8.2/thunder_ase/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1967 2024-04-16 11:34:06.000000 thunder_ase-0.8.2/thunder_ase/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10921 2024-04-16 11:34:06.000000 thunder_ase-0.8.2/thunder_ase/utils/basis_set.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5041 2024-04-16 11:34:06.000000 thunder_ase-0.8.2/thunder_ase/utils/mwfn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2694 2024-04-16 11:34:06.000000 thunder_ase-0.8.2/thunder_ase/utils/shell_dict.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:34:11.506564 thunder_ase-0.8.2/thunder_ase.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     8687 2024-04-16 11:34:11.000000 thunder_ase-0.8.2/thunder_ase.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      402 2024-04-16 11:34:11.000000 thunder_ase-0.8.2/thunder_ase.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 11:34:11.000000 thunder_ase-0.8.2/thunder_ase.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       65 2024-04-16 11:34:11.000000 thunder_ase-0.8.2/thunder_ase.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-16 11:34:11.000000 thunder_ase-0.8.2/thunder_ase.egg-info/top_level.txt
```

### Comparing `thunder-ase-0.8.1/PKG-INFO` & `thunder_ase-0.8.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thunder-ase
-Version: 0.8.1
+Version: 0.8.2
 Summary: ASE calculator interface for FIREBALL code
 Author-email: PJ Ren <openrpj@gmail.com>
 Project-URL: Homepage, https://github.com/thunder-dft/thunder-ase
 Project-URL: Bug Tracker, https://github.com/thunder-dft/thunder-ase/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -64,16 +64,16 @@
 
 print("The energy for optimized structure is {:.3f} eV.".format(atoms.get_potential_energy()))
 ```
 
 #### Grimme's DFT-D3 and DFT-D4 combination
 
 See 
-* [DFDT-D3 example](examples/6_Benzene_DFT-D3/Benzene_DFT-D3.ipynb)  
-* [DFDT-D4 example](examples/6_Benzene_DFT-D4/Benzene_DFT-D4.ipynb).
+* [DFT-D3 example](examples/6_Benzene_DFT-D3/Benzene_DFT-D3.ipynb)  
+* [DFT-D4 example](examples/6_Benzene_DFT-D4/Benzene_DFT-D4.ipynb).
 
 More info: 
 * [DFT-D3 manual](https://www.chemiebn.uni-bonn.de/pctc/mulliken-center/software/dft-d3/get-the-current-version-of-dft-d3)
 * [DFT-D3 in ASE](https://wiki.fysik.dtu.dk/ase/ase/calculators/dftd3.html)
 * [DFT-D4 with ASE support](https://dftd4.readthedocs.io/en/latest/reference/ase.html)
```

### Comparing `thunder-ase-0.8.1/README.md` & `thunder_ase-0.8.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -51,16 +51,16 @@
 
 print("The energy for optimized structure is {:.3f} eV.".format(atoms.get_potential_energy()))
 ```
 
 #### Grimme's DFT-D3 and DFT-D4 combination
 
 See 
-* [DFDT-D3 example](examples/6_Benzene_DFT-D3/Benzene_DFT-D3.ipynb)  
-* [DFDT-D4 example](examples/6_Benzene_DFT-D4/Benzene_DFT-D4.ipynb).
+* [DFT-D3 example](examples/6_Benzene_DFT-D3/Benzene_DFT-D3.ipynb)  
+* [DFT-D4 example](examples/6_Benzene_DFT-D4/Benzene_DFT-D4.ipynb).
 
 More info: 
 * [DFT-D3 manual](https://www.chemiebn.uni-bonn.de/pctc/mulliken-center/software/dft-d3/get-the-current-version-of-dft-d3)
 * [DFT-D3 in ASE](https://wiki.fysik.dtu.dk/ase/ase/calculators/dftd3.html)
 * [DFT-D4 with ASE support](https://dftd4.readthedocs.io/en/latest/reference/ase.html)
```

### Comparing `thunder-ase-0.8.1/pyproject.toml` & `thunder_ase-0.8.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "thunder-ase"
-version = "0.8.1"
+version = "0.8.2"
 authors = [
   { name="PJ Ren", email="openrpj@gmail.com" },
 ]
 description = "ASE calculator interface for FIREBALL code"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `thunder-ase-0.8.1/thunder_ase/fireball.py` & `thunder_ase-0.8.2/thunder_ase/fireball.py`

 * *Files 0% similar despite different names*

```diff
@@ -744,15 +744,19 @@
             raise ImportError(method)
 
         if atoms is None:
             atoms = self.atoms
 
         atoms.calc = self
 
-        dyn = Optimizer(atoms, trajectory='minimize.traj', logfile='minimize.log', **kwargs)
+        if 'trajectory' not in kwargs:
+            kwargs['trajectory'] = 'minimize.traj'
+        if 'logfile' not in kwargs:
+            kwargs['logfile'] = 'minimize.log'
+        dyn = Optimizer(atoms, **kwargs)
         dyn.converged = MethodType(rms_converged, dyn)  # use rms as convergence criteria instead of fmax
         self.dynamics(dyn, fmax=fmax)
 
 
 class MultiFireball:
     name = 'multi_fireball'
```

### Comparing `thunder-ase-0.8.1/thunder_ase/optimize.py` & `thunder_ase-0.8.2/thunder_ase/optimize.py`

 * *Files identical despite different names*

### Comparing `thunder-ase-0.8.1/thunder_ase/utils/__init__.py` & `thunder_ase-0.8.2/thunder_ase/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `thunder-ase-0.8.1/thunder_ase/utils/basis_set.py` & `thunder_ase-0.8.2/thunder_ase/utils/basis_set.py`

 * *Files identical despite different names*

### Comparing `thunder-ase-0.8.1/thunder_ase/utils/mwfn.py` & `thunder_ase-0.8.2/thunder_ase/utils/mwfn.py`

 * *Files identical despite different names*

### Comparing `thunder-ase-0.8.1/thunder_ase/utils/shell_dict.py` & `thunder_ase-0.8.2/thunder_ase/utils/shell_dict.py`

 * *Files identical despite different names*

### Comparing `thunder-ase-0.8.1/thunder_ase.egg-info/PKG-INFO` & `thunder_ase-0.8.2/thunder_ase.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: thunder-ase
-Version: 0.8.1
+Version: 0.8.2
 Summary: ASE calculator interface for FIREBALL code
 Author-email: PJ Ren <openrpj@gmail.com>
 Project-URL: Homepage, https://github.com/thunder-dft/thunder-ase
 Project-URL: Bug Tracker, https://github.com/thunder-dft/thunder-ase/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -64,16 +64,16 @@
 
 print("The energy for optimized structure is {:.3f} eV.".format(atoms.get_potential_energy()))
 ```
 
 #### Grimme's DFT-D3 and DFT-D4 combination
 
 See 
-* [DFDT-D3 example](examples/6_Benzene_DFT-D3/Benzene_DFT-D3.ipynb)  
-* [DFDT-D4 example](examples/6_Benzene_DFT-D4/Benzene_DFT-D4.ipynb).
+* [DFT-D3 example](examples/6_Benzene_DFT-D3/Benzene_DFT-D3.ipynb)  
+* [DFT-D4 example](examples/6_Benzene_DFT-D4/Benzene_DFT-D4.ipynb).
 
 More info: 
 * [DFT-D3 manual](https://www.chemiebn.uni-bonn.de/pctc/mulliken-center/software/dft-d3/get-the-current-version-of-dft-d3)
 * [DFT-D3 in ASE](https://wiki.fysik.dtu.dk/ase/ase/calculators/dftd3.html)
 * [DFT-D4 with ASE support](https://dftd4.readthedocs.io/en/latest/reference/ase.html)
```

