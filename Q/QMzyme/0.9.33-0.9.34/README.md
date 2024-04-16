# Comparing `tmp/QMzyme-0.9.33.tar.gz` & `tmp/QMzyme-0.9.34.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "QMzyme-0.9.33.tar", last modified: Wed Feb 14 17:29:44 2024, max compression
+gzip compressed data, was "QMzyme-0.9.34.tar", last modified: Wed Feb 14 17:47:59 2024, max compression
```

## Comparing `QMzyme-0.9.33.tar` & `QMzyme-0.9.34.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 hrk      (77984) NIST\647DIV (36682)        0 2024-02-14 17:29:44.687579 QMzyme-0.9.33/
--rw-r--r--   0 hrk      (77984) NIST\647DIV (36682)     3555 2024-02-13 22:03:02.000000 QMzyme-0.9.33/CODE_OF_CONDUCT.md
--rw-r--r--   0 hrk      (77984) NIST\647DIV (36682)     1068 2023-09-08 22:06:04.000000 QMzyme-0.9.33/LICENSE
--rw-r--r--   0 hrk      (77984) NIST\647DIV (36682)       70 2023-09-08 22:06:04.000000 QMzyme-0.9.33/MANIFEST.in
--rw-r--r--   0 hrk      (77984) NIST\647DIV (36682)     9637 2024-02-14 17:29:44.687452 QMzyme-0.9.33/PKG-INFO
-drwxr-xr-x   0 hrk      (77984) NIST\647DIV (36682)        0 2024-02-14 17:29:44.685346 QMzyme-0.9.33/QMzyme/
--rw-r--r--   0 hrk      (77984) NIST\647DIV (36682)      106 2023-11-07 19:49:13.000000 QMzyme-0.9.33/QMzyme/QM_region_analysis.py
--rw-r--r--   0 hrk      (77984) NIST\647DIV (36682)      154 2024-02-12 22:16:56.000000 QMzyme-0.9.33/QMzyme/__init__.py
--rw-r--r--   0 hrk      (77984) NIST\647DIV (36682)       23 2024-02-14 17:29:44.000000 QMzyme-0.9.33/QMzyme/_version.py
--rw-r--r--   0 hrk      (77984) NIST\647DIV (36682)     2334 2024-02-13 21:18:03.000000 QMzyme-0.9.33/QMzyme/aqme_wrapper.py
-drwxr-xr-x   0 hrk      (77984) NIST\647DIV (36682)        0 2024-02-14 17:29:44.686504 QMzyme-0.9.33/QMzyme/data/
--rw-r--r--   0 hrk      (77984) NIST\647DIV (36682)        0 2024-02-13 22:21:05.000000 QMzyme-0.9.33/QMzyme/data/__init__.py
--rw-r--r--   0 hrk      (77984) NIST\647DIV (36682)    32658 2024-02-14 17:27:34.000000 QMzyme-0.9.33/QMzyme/generate.py
--rw-r--r--   0 hrk      (77984) NIST\647DIV (36682)     2081 2024-02-12 23:35:16.000000 QMzyme-0.9.33/QMzyme/mdanalysis_wrapper.py
--rw-r--r--   0 hrk      (77984) NIST\647DIV (36682)    34988 2023-10-03 21:24:25.000000 QMzyme-0.9.33/QMzyme/old_generate.py
--rw-r--r--   0 hrk      (77984) NIST\647DIV (36682)     6081 2023-10-06 22:28:21.000000 QMzyme-0.9.33/QMzyme/protein_parser.py
--rw-r--r--   0 hrk      (77984) NIST\647DIV (36682)       61 2023-09-08 22:06:04.000000 QMzyme-0.9.33/QMzyme/py.typed
--rw-r--r--   0 hrk      (77984) NIST\647DIV (36682)     6669 2024-02-06 03:12:34.000000 QMzyme-0.9.33/QMzyme/rdkit_wrapper.py
--rw-r--r--   0 hrk      (77984) NIST\647DIV (36682)    20788 2024-02-14 17:28:53.000000 QMzyme-0.9.33/QMzyme/utils.py
-drwxr-xr-x   0 hrk      (77984) NIST\647DIV (36682)        0 2024-02-14 17:29:44.687075 QMzyme-0.9.33/QMzyme.egg-info/
--rw-r--r--   0 hrk      (77984) NIST\647DIV (36682)     9637 2024-02-14 17:29:44.000000 QMzyme-0.9.33/QMzyme.egg-info/PKG-INFO
--rw-r--r--   0 hrk      (77984) NIST\647DIV (36682)      556 2024-02-14 17:29:44.000000 QMzyme-0.9.33/QMzyme.egg-info/SOURCES.txt
--rw-r--r--   0 hrk      (77984) NIST\647DIV (36682)        1 2024-02-14 17:29:44.000000 QMzyme-0.9.33/QMzyme.egg-info/dependency_links.txt
--rw-r--r--   0 hrk      (77984) NIST\647DIV (36682)        1 2023-09-08 22:06:04.000000 QMzyme-0.9.33/QMzyme.egg-info/not-zip-safe
--rw-r--r--   0 hrk      (77984) NIST\647DIV (36682)       55 2024-02-14 17:29:44.000000 QMzyme-0.9.33/QMzyme.egg-info/requires.txt
--rw-r--r--   0 hrk      (77984) NIST\647DIV (36682)       13 2024-02-14 17:29:44.000000 QMzyme-0.9.33/QMzyme.egg-info/top_level.txt
--rw-r--r--   0 hrk      (77984) NIST\647DIV (36682)     9124 2024-02-13 17:32:45.000000 QMzyme-0.9.33/README.md
--rw-r--r--   0 hrk      (77984) NIST\647DIV (36682)     3047 2024-02-13 21:41:33.000000 QMzyme-0.9.33/pyproject.toml
--rw-r--r--   0 hrk      (77984) NIST\647DIV (36682)      262 2024-02-14 17:29:44.687857 QMzyme-0.9.33/setup.cfg
-drwxr-xr-x   0 hrk      (77984) NIST\647DIV (36682)        0 2024-02-14 17:29:44.686829 QMzyme-0.9.33/tests/
--rw-r--r--   0 hrk      (77984) NIST\647DIV (36682)      113 2023-09-08 22:06:04.000000 QMzyme-0.9.33/tests/__init__.py
--rw-r--r--   0 hrk      (77984) NIST\647DIV (36682)     3707 2024-02-13 20:46:42.000000 QMzyme-0.9.33/tests/test_QMzyme.py
+drwxr-xr-x   0 hrk      (77984) NIST\647DIV (36682)        0 2024-02-14 17:47:59.214424 QMzyme-0.9.34/
+-rw-r--r--   0 hrk      (77984) NIST\647DIV (36682)     3555 2024-02-13 22:03:02.000000 QMzyme-0.9.34/CODE_OF_CONDUCT.md
+-rw-r--r--   0 hrk      (77984) NIST\647DIV (36682)     1068 2023-09-08 22:06:04.000000 QMzyme-0.9.34/LICENSE
+-rw-r--r--   0 hrk      (77984) NIST\647DIV (36682)       70 2023-09-08 22:06:04.000000 QMzyme-0.9.34/MANIFEST.in
+-rw-r--r--   0 hrk      (77984) NIST\647DIV (36682)     9637 2024-02-14 17:47:59.214253 QMzyme-0.9.34/PKG-INFO
+drwxr-xr-x   0 hrk      (77984) NIST\647DIV (36682)        0 2024-02-14 17:47:59.211001 QMzyme-0.9.34/QMzyme/
+-rw-r--r--   0 hrk      (77984) NIST\647DIV (36682)      106 2023-11-07 19:49:13.000000 QMzyme-0.9.34/QMzyme/QM_region_analysis.py
+-rw-r--r--   0 hrk      (77984) NIST\647DIV (36682)      154 2024-02-12 22:16:56.000000 QMzyme-0.9.34/QMzyme/__init__.py
+-rw-r--r--   0 hrk      (77984) NIST\647DIV (36682)       23 2024-02-14 17:47:59.000000 QMzyme-0.9.34/QMzyme/_version.py
+-rw-r--r--   0 hrk      (77984) NIST\647DIV (36682)     2334 2024-02-13 21:18:03.000000 QMzyme-0.9.34/QMzyme/aqme_wrapper.py
+drwxr-xr-x   0 hrk      (77984) NIST\647DIV (36682)        0 2024-02-14 17:47:59.212954 QMzyme-0.9.34/QMzyme/data/
+-rw-r--r--   0 hrk      (77984) NIST\647DIV (36682)        0 2024-02-13 22:21:05.000000 QMzyme-0.9.34/QMzyme/data/__init__.py
+-rw-r--r--   0 hrk      (77984) NIST\647DIV (36682)    32658 2024-02-14 17:27:34.000000 QMzyme-0.9.34/QMzyme/generate.py
+-rw-r--r--   0 hrk      (77984) NIST\647DIV (36682)     2081 2024-02-12 23:35:16.000000 QMzyme-0.9.34/QMzyme/mdanalysis_wrapper.py
+-rw-r--r--   0 hrk      (77984) NIST\647DIV (36682)    34988 2023-10-03 21:24:25.000000 QMzyme-0.9.34/QMzyme/old_generate.py
+-rw-r--r--   0 hrk      (77984) NIST\647DIV (36682)     6081 2023-10-06 22:28:21.000000 QMzyme-0.9.34/QMzyme/protein_parser.py
+-rw-r--r--   0 hrk      (77984) NIST\647DIV (36682)       61 2023-09-08 22:06:04.000000 QMzyme-0.9.34/QMzyme/py.typed
+-rw-r--r--   0 hrk      (77984) NIST\647DIV (36682)     6669 2024-02-06 03:12:34.000000 QMzyme-0.9.34/QMzyme/rdkit_wrapper.py
+-rw-r--r--   0 hrk      (77984) NIST\647DIV (36682)    20820 2024-02-14 17:43:19.000000 QMzyme-0.9.34/QMzyme/utils.py
+drwxr-xr-x   0 hrk      (77984) NIST\647DIV (36682)        0 2024-02-14 17:47:59.213723 QMzyme-0.9.34/QMzyme.egg-info/
+-rw-r--r--   0 hrk      (77984) NIST\647DIV (36682)     9637 2024-02-14 17:47:59.000000 QMzyme-0.9.34/QMzyme.egg-info/PKG-INFO
+-rw-r--r--   0 hrk      (77984) NIST\647DIV (36682)      556 2024-02-14 17:47:59.000000 QMzyme-0.9.34/QMzyme.egg-info/SOURCES.txt
+-rw-r--r--   0 hrk      (77984) NIST\647DIV (36682)        1 2024-02-14 17:47:59.000000 QMzyme-0.9.34/QMzyme.egg-info/dependency_links.txt
+-rw-r--r--   0 hrk      (77984) NIST\647DIV (36682)        1 2023-09-08 22:06:04.000000 QMzyme-0.9.34/QMzyme.egg-info/not-zip-safe
+-rw-r--r--   0 hrk      (77984) NIST\647DIV (36682)       55 2024-02-14 17:47:59.000000 QMzyme-0.9.34/QMzyme.egg-info/requires.txt
+-rw-r--r--   0 hrk      (77984) NIST\647DIV (36682)       13 2024-02-14 17:47:59.000000 QMzyme-0.9.34/QMzyme.egg-info/top_level.txt
+-rw-r--r--   0 hrk      (77984) NIST\647DIV (36682)     9124 2024-02-13 17:32:45.000000 QMzyme-0.9.34/README.md
+-rw-r--r--   0 hrk      (77984) NIST\647DIV (36682)     3047 2024-02-13 21:41:33.000000 QMzyme-0.9.34/pyproject.toml
+-rw-r--r--   0 hrk      (77984) NIST\647DIV (36682)      262 2024-02-14 17:47:59.214765 QMzyme-0.9.34/setup.cfg
+drwxr-xr-x   0 hrk      (77984) NIST\647DIV (36682)        0 2024-02-14 17:47:59.213396 QMzyme-0.9.34/tests/
+-rw-r--r--   0 hrk      (77984) NIST\647DIV (36682)      113 2023-09-08 22:06:04.000000 QMzyme-0.9.34/tests/__init__.py
+-rw-r--r--   0 hrk      (77984) NIST\647DIV (36682)     3707 2024-02-13 20:46:42.000000 QMzyme-0.9.34/tests/test_QMzyme.py
```

### Comparing `QMzyme-0.9.33/CODE_OF_CONDUCT.md` & `QMzyme-0.9.34/CODE_OF_CONDUCT.md`

 * *Files identical despite different names*

### Comparing `QMzyme-0.9.33/LICENSE` & `QMzyme-0.9.34/LICENSE`

 * *Files identical despite different names*

### Comparing `QMzyme-0.9.33/PKG-INFO` & `QMzyme-0.9.34/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QMzyme
-Version: 0.9.33
+Version: 0.9.34
 Summary: QM-based enzyme model generation and validation.
 Author-email: Heidi Klem <heidi.klem@nist.gov>
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.0
 Description-Content-Type: text/markdown
```

### Comparing `QMzyme-0.9.33/QMzyme/aqme_wrapper.py` & `QMzyme-0.9.34/QMzyme/aqme_wrapper.py`

 * *Files identical despite different names*

### Comparing `QMzyme-0.9.33/QMzyme/generate.py` & `QMzyme-0.9.34/QMzyme/generate.py`

 * *Files identical despite different names*

### Comparing `QMzyme-0.9.33/QMzyme/mdanalysis_wrapper.py` & `QMzyme-0.9.34/QMzyme/mdanalysis_wrapper.py`

 * *Files identical despite different names*

### Comparing `QMzyme-0.9.33/QMzyme/old_generate.py` & `QMzyme-0.9.34/QMzyme/old_generate.py`

 * *Files identical despite different names*

### Comparing `QMzyme-0.9.33/QMzyme/protein_parser.py` & `QMzyme-0.9.34/QMzyme/protein_parser.py`

 * *Files identical despite different names*

### Comparing `QMzyme-0.9.33/QMzyme/rdkit_wrapper.py` & `QMzyme-0.9.34/QMzyme/rdkit_wrapper.py`

 * *Files identical despite different names*

### Comparing `QMzyme-0.9.33/QMzyme/utils.py` & `QMzyme-0.9.34/QMzyme/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -153,15 +153,15 @@
             non_protein_residues['Number'].append(number)
         if 'HETNAM' in line:
             non_protein_chemical_name[line[11:14]]=line[15:].split('  ')[0]
 
     residues_reordered=False
     if clean==True:
         for i,line in enumerate(data):
-            if pdb_info('record_type',line) in ['ATOM','HETATM']:
+            if pdb_info('record_type',line).strip() in ['ATOM','HETATM']:
                 atom_type = pdb_info('atom_name',line)
                 res_num = pdb_info('res_number',line)
                 res_name = pdb_info('res_name',line)
                 if res_num != res_num_previous:
                     if res_name not in solvent_list:
                         residue_count += 1
                         if int(res_num.split()[0]) != residue_count:
@@ -304,15 +304,15 @@
             raise FileNotFoundError("test file {} not found.".format(file))
     else:
         if data is None:
             raise Exception("Must define either file or lines from a pdb file.")
 
     pdb_data = {'res_name_sequence':[],'atom_sequence':[],'number_of_atoms':0,'atom_coords':[],'res_num_sequence':[]}
     for line in data:
-        if pdb_info('record_type',line) in ['ATOM','HETATM']:
+        if pdb_info('record_type',line).strip() in ['ATOM','HETATM']:
             pdb_data['res_name_sequence'].append(pdb_info('res_name',line))
             pdb_data['res_num_sequence'].append(pdb_info('res_number',line))
             pdb_data['number_of_atoms'] += 1
             pdb_data['atom_sequence'].append(pdb_info('atom_name',line))
             pdb_data['atom_coords'].append((pdb_info('x',line),
                                           pdb_info('y',line),
                                           pdb_info('z',line)))
@@ -364,16 +364,16 @@
     coords = []
     if type(file) is str:
         data = get_outlines(file)
     else:
         data = file
     count = 0
     for i, line in enumerate(data):
-        if pdb_info('record_type',line) in ['ATOM','HETATM']:
-            coords.append([float(pdb_info(coord, line) for coord in ['x', 'y', 'z'])])
+        if pdb_info('record_type',line).strip() in ['ATOM','HETATM']:
+            coords.append([float(pdb_info(coord, line)) for coord in ['x', 'y', 'z']])
             #coords.append([float(line.split()[x+6]) for x in range(3)])
     return np.array(coords)
 
 def coords_from_gout(file):
     coords = []
     data = get_outlines(file)
     done = False
@@ -506,15 +506,15 @@
             else:
                 f.write(line)
 
 def get_atoms(file):
     atoms = []
     with open(file, 'r') as f:
         for line in f.readlines():
-            if pdb_info('record_type',line) in ['ATOM','HETATM']:
+            if pdb_info('record_type',line).strip() in ['ATOM','HETATM']:
                 atoms.append(pdb_info('element_symbol',line).strip())
     return atoms
 
 def res_charges(residues):
         charge=0 
         if type(residues) is dict:
             for i,res in enumerate(residues):
```

### Comparing `QMzyme-0.9.33/QMzyme.egg-info/PKG-INFO` & `QMzyme-0.9.34/QMzyme.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: QMzyme
-Version: 0.9.33
+Version: 0.9.34
 Summary: QM-based enzyme model generation and validation.
 Author-email: Heidi Klem <heidi.klem@nist.gov>
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.0
 Description-Content-Type: text/markdown
```

### Comparing `QMzyme-0.9.33/QMzyme.egg-info/SOURCES.txt` & `QMzyme-0.9.34/QMzyme.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `QMzyme-0.9.33/README.md` & `QMzyme-0.9.34/README.md`

 * *Files identical despite different names*

### Comparing `QMzyme-0.9.33/pyproject.toml` & `QMzyme-0.9.34/pyproject.toml`

 * *Files identical despite different names*

### Comparing `QMzyme-0.9.33/tests/test_QMzyme.py` & `QMzyme-0.9.34/tests/test_QMzyme.py`

 * *Files identical despite different names*

