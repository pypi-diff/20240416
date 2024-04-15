# Comparing `tmp/masscube-0.0.6.tar.gz` & `tmp/masscube-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "masscube-0.0.6.tar", last modified: Fri Apr  5 03:19:58 2024, max compression
+gzip compressed data, was "masscube-0.0.7.tar", last modified: Mon Apr 15 23:29:23 2024, max compression
```

## Comparing `masscube-0.0.6.tar` & `masscube-0.0.7.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 jiemoniu   (501) staff       (20)        0 2024-04-05 03:19:58.356791 masscube-0.0.6/
--rw-r--r--   0 jiemoniu   (501) staff       (20)     1064 2023-12-15 01:08:30.000000 masscube-0.0.6/LICENSE
--rw-r--r--   0 jiemoniu   (501) staff       (20)     2597 2024-04-05 03:19:58.356612 masscube-0.0.6/PKG-INFO
--rw-r--r--   0 jiemoniu   (501) staff       (20)     1820 2024-03-21 20:30:54.000000 masscube-0.0.6/README.md
--rw-r--r--   0 jiemoniu   (501) staff       (20)      959 2024-04-05 00:44:14.000000 masscube-0.0.6/pyproject.toml
--rw-r--r--   0 jiemoniu   (501) staff       (20)       38 2024-04-05 03:19:58.356829 masscube-0.0.6/setup.cfg
-drwxr-xr-x   0 jiemoniu   (501) staff       (20)        0 2024-04-05 03:19:58.349487 masscube-0.0.6/src/
-drwxr-xr-x   0 jiemoniu   (501) staff       (20)        0 2024-04-05 03:19:58.355561 masscube-0.0.6/src/masscube/
--rw-r--r--   0 jiemoniu   (501) staff       (20)      124 2024-03-20 21:39:26.000000 masscube-0.0.6/src/masscube/__init__.py
--rw-r--r--   0 jiemoniu   (501) staff       (20)    19558 2024-04-03 22:03:37.000000 masscube-0.0.6/src/masscube/alignment.py
--rw-r--r--   0 jiemoniu   (501) staff       (20)    15266 2024-04-02 00:57:05.000000 masscube-0.0.6/src/masscube/annotation.py
--rw-r--r--   0 jiemoniu   (501) staff       (20)     2062 2024-04-03 22:01:18.000000 masscube-0.0.6/src/masscube/feature_evaluation.py
--rw-r--r--   0 jiemoniu   (501) staff       (20)     8772 2024-04-03 20:16:56.000000 masscube-0.0.6/src/masscube/feature_grouping.py
--rw-r--r--   0 jiemoniu   (501) staff       (20)      973 2024-03-07 23:40:12.000000 masscube-0.0.6/src/masscube/feature_table_utils.py
--rw-r--r--   0 jiemoniu   (501) staff       (20)     7337 2024-03-01 00:56:56.000000 masscube-0.0.6/src/masscube/network.py
--rw-r--r--   0 jiemoniu   (501) staff       (20)     3477 2024-03-22 03:35:49.000000 masscube-0.0.6/src/masscube/normalization.py
--rw-r--r--   0 jiemoniu   (501) staff       (20)    10243 2024-04-03 00:15:40.000000 masscube-0.0.6/src/masscube/params.py
--rw-r--r--   0 jiemoniu   (501) staff       (20)    10680 2024-04-03 22:03:45.000000 masscube-0.0.6/src/masscube/peak_detect.py
--rw-r--r--   0 jiemoniu   (501) staff       (20)    29428 2024-04-05 02:13:47.000000 masscube-0.0.6/src/masscube/raw_data_utils.py
--rw-r--r--   0 jiemoniu   (501) staff       (20)     5504 2024-03-22 22:35:24.000000 masscube-0.0.6/src/masscube/stats.py
--rw-r--r--   0 jiemoniu   (501) staff       (20)     2783 2024-03-20 18:39:36.000000 masscube-0.0.6/src/masscube/utils_functions.py
--rw-r--r--   0 jiemoniu   (501) staff       (20)    12618 2024-04-03 23:13:18.000000 masscube-0.0.6/src/masscube/visualization.py
--rw-r--r--   0 jiemoniu   (501) staff       (20)     5717 2024-04-03 23:10:04.000000 masscube-0.0.6/src/masscube/workflows.py
-drwxr-xr-x   0 jiemoniu   (501) staff       (20)        0 2024-04-05 03:19:58.356409 masscube-0.0.6/src/masscube.egg-info/
--rw-r--r--   0 jiemoniu   (501) staff       (20)     2597 2024-04-05 03:19:58.000000 masscube-0.0.6/src/masscube.egg-info/PKG-INFO
--rw-r--r--   0 jiemoniu   (501) staff       (20)      678 2024-04-05 03:19:58.000000 masscube-0.0.6/src/masscube.egg-info/SOURCES.txt
--rw-r--r--   0 jiemoniu   (501) staff       (20)        1 2024-04-05 03:19:58.000000 masscube-0.0.6/src/masscube.egg-info/dependency_links.txt
--rw-r--r--   0 jiemoniu   (501) staff       (20)      138 2024-04-05 03:19:58.000000 masscube-0.0.6/src/masscube.egg-info/entry_points.txt
--rw-r--r--   0 jiemoniu   (501) staff       (20)      129 2024-04-05 03:19:58.000000 masscube-0.0.6/src/masscube.egg-info/requires.txt
--rw-r--r--   0 jiemoniu   (501) staff       (20)        9 2024-04-05 03:19:58.000000 masscube-0.0.6/src/masscube.egg-info/top_level.txt
+drwxr-xr-x   0 jiemoniu   (501) staff       (20)        0 2024-04-15 23:29:23.525569 masscube-0.0.7/
+-rw-r--r--   0 jiemoniu   (501) staff       (20)     1064 2023-12-15 01:08:30.000000 masscube-0.0.7/LICENSE
+-rw-r--r--   0 jiemoniu   (501) staff       (20)     2597 2024-04-15 23:29:23.525417 masscube-0.0.7/PKG-INFO
+-rw-r--r--   0 jiemoniu   (501) staff       (20)     1820 2024-03-21 20:30:54.000000 masscube-0.0.7/README.md
+-rw-r--r--   0 jiemoniu   (501) staff       (20)      962 2024-04-15 23:29:15.000000 masscube-0.0.7/pyproject.toml
+-rw-r--r--   0 jiemoniu   (501) staff       (20)       38 2024-04-15 23:29:23.525616 masscube-0.0.7/setup.cfg
+drwxr-xr-x   0 jiemoniu   (501) staff       (20)        0 2024-04-15 23:29:23.519690 masscube-0.0.7/src/
+drwxr-xr-x   0 jiemoniu   (501) staff       (20)        0 2024-04-15 23:29:23.524490 masscube-0.0.7/src/masscube/
+-rw-r--r--   0 jiemoniu   (501) staff       (20)      124 2024-03-20 21:39:26.000000 masscube-0.0.7/src/masscube/__init__.py
+-rw-r--r--   0 jiemoniu   (501) staff       (20)    17035 2024-04-12 00:19:22.000000 masscube-0.0.7/src/masscube/alignment.py
+-rw-r--r--   0 jiemoniu   (501) staff       (20)    15266 2024-04-02 00:57:05.000000 masscube-0.0.7/src/masscube/annotation.py
+-rw-r--r--   0 jiemoniu   (501) staff       (20)     2062 2024-04-11 23:20:27.000000 masscube-0.0.7/src/masscube/feature_evaluation.py
+-rw-r--r--   0 jiemoniu   (501) staff       (20)     8772 2024-04-03 20:16:56.000000 masscube-0.0.7/src/masscube/feature_grouping.py
+-rw-r--r--   0 jiemoniu   (501) staff       (20)      973 2024-03-07 23:40:12.000000 masscube-0.0.7/src/masscube/feature_table_utils.py
+-rw-r--r--   0 jiemoniu   (501) staff       (20)     7337 2024-03-01 00:56:56.000000 masscube-0.0.7/src/masscube/network.py
+-rw-r--r--   0 jiemoniu   (501) staff       (20)     3477 2024-03-22 03:35:49.000000 masscube-0.0.7/src/masscube/normalization.py
+-rw-r--r--   0 jiemoniu   (501) staff       (20)    10243 2024-04-03 00:15:40.000000 masscube-0.0.7/src/masscube/params.py
+-rw-r--r--   0 jiemoniu   (501) staff       (20)    10750 2024-04-12 17:33:27.000000 masscube-0.0.7/src/masscube/peak_detect.py
+-rw-r--r--   0 jiemoniu   (501) staff       (20)    29438 2024-04-11 20:41:17.000000 masscube-0.0.7/src/masscube/raw_data_utils.py
+-rw-r--r--   0 jiemoniu   (501) staff       (20)     5479 2024-04-11 22:19:50.000000 masscube-0.0.7/src/masscube/stats.py
+-rw-r--r--   0 jiemoniu   (501) staff       (20)     2783 2024-03-20 18:39:36.000000 masscube-0.0.7/src/masscube/utils_functions.py
+-rw-r--r--   0 jiemoniu   (501) staff       (20)    12646 2024-04-12 00:24:57.000000 masscube-0.0.7/src/masscube/visualization.py
+-rw-r--r--   0 jiemoniu   (501) staff       (20)    10842 2024-04-15 22:58:59.000000 masscube-0.0.7/src/masscube/workflows.py
+drwxr-xr-x   0 jiemoniu   (501) staff       (20)        0 2024-04-15 23:29:23.525237 masscube-0.0.7/src/masscube.egg-info/
+-rw-r--r--   0 jiemoniu   (501) staff       (20)     2597 2024-04-15 23:29:23.000000 masscube-0.0.7/src/masscube.egg-info/PKG-INFO
+-rw-r--r--   0 jiemoniu   (501) staff       (20)      678 2024-04-15 23:29:23.000000 masscube-0.0.7/src/masscube.egg-info/SOURCES.txt
+-rw-r--r--   0 jiemoniu   (501) staff       (20)        1 2024-04-15 23:29:23.000000 masscube-0.0.7/src/masscube.egg-info/dependency_links.txt
+-rw-r--r--   0 jiemoniu   (501) staff       (20)      141 2024-04-15 23:29:23.000000 masscube-0.0.7/src/masscube.egg-info/entry_points.txt
+-rw-r--r--   0 jiemoniu   (501) staff       (20)      129 2024-04-15 23:29:23.000000 masscube-0.0.7/src/masscube.egg-info/requires.txt
+-rw-r--r--   0 jiemoniu   (501) staff       (20)        9 2024-04-15 23:29:23.000000 masscube-0.0.7/src/masscube.egg-info/top_level.txt
```

### Comparing `masscube-0.0.6/LICENSE` & `masscube-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `masscube-0.0.6/PKG-INFO` & `masscube-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: masscube
-Version: 0.0.6
+Version: 0.0.7
 Summary: Accurate and fast data processing for metabolomics
 Author-email: Huaxu Yu <yhxchem@outlook.com>
 Maintainer-email: Huaxu Yu <yhxchem@outlook.com>
 Project-URL: Homepage, https://github.com/huaxuyu/masscube
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `masscube-0.0.6/README.md` & `masscube-0.0.7/README.md`

 * *Files identical despite different names*

### Comparing `masscube-0.0.6/pyproject.toml` & `masscube-0.0.7/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "masscube"
-version = "0.0.6"
+version = "0.0.7"
 authors = [
   { name="Huaxu Yu", email="yhxchem@outlook.com" },
 ]
 maintainers = [
   { name="Huaxu Yu", email="yhxchem@outlook.com" },
 ]
 description = "Accurate and fast data processing for metabolomics"
@@ -30,11 +30,11 @@
     "ms_entropy>=1.1.1",
     "networkx",
     "scikit-learn"
 ]
 
 [project.scripts]
 untargeted-metabolomics = "masscube:untargeted_metabolomics_workflow"
-build-sample-table = "masscube:generate_sample_table"
+generate-sample-table = "masscube:generate_sample_table"
 
 [project.urls]
 "Homepage" = "https://github.com/huaxuyu/masscube"
```

### Comparing `masscube-0.0.6/src/masscube/alignment.py` & `masscube-0.0.7/src/masscube/alignment.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,37 +25,37 @@
 
     Returns
     ----------------------------------------------------------
     feature_table: DataFrame
         The aligned feature table.
     """
 
-    # STEP 1: get names of individual files (.csv)
-    csv_file_names = parameters.sample_names
-    csv_file_names = [f + ".csv" for f in csv_file_names]
-    csv_file_names = [os.path.join(path, name) for name in csv_file_names]
+    # STEP 1: get names of individual files (.txt)
+    txt_file_names = parameters.sample_names
+    txt_file_names = [f + ".txt" for f in txt_file_names]
+    txt_file_names = [os.path.join(path, name) for name in txt_file_names]
 
     # STEP 2: initiate aligned features
     feature_table = _init_feature_table(sample_names=parameters.sample_names)
 
     mz_tol = parameters.align_mz_tol
     rt_tol = parameters.align_rt_tol
     # STEP 3: read individual feature tables and align features
     last_file_feature_idx = 0
     int_seq = np.zeros(len(feature_table))
     problematic_files = []
     for i, file_name in enumerate(tqdm(parameters.sample_names)):
 
         # check if the file exists
-        if not os.path.exists(csv_file_names[i]):
+        if not os.path.exists(txt_file_names[i]):
             problematic_files.append(file_name)
             continue
         
         # read feature table
-        current_table = pd.read_csv(csv_file_names[i], low_memory=False)
+        current_table = pd.read_csv(txt_file_names[i], low_memory=False, sep="\t")
         current_table = current_table[current_table["MS2"].notna()|(current_table["peak_height"] > parameters.int_tol*3)]
         # sort current table by peak height from high to low
         current_table = current_table.sort_values(by="peak_height", ascending=False)
         current_table.index = range(len(current_table))
         new_feature_idx = []
 
         mz_seq = np.array(feature_table["m/z"], dtype=float)
@@ -313,17 +313,15 @@
         self.peak_area_seq.append(row["peak_area"])
         self.top_average_seq.append(row["top_average"])
         self.ms2_seq.append(row["MS2"])
 
         if row["peak_height"] > self.highest_roi_intensity:
             self.highest_roi_intensity = row["peak_height"]
             self.highest_roi = row
-            
 
-    
     def choose_best_ms2(self):
         """
         A function to choose the best MS2 for the feature. 
         The best MS2 is the one with the highest summed intensity.
         """
 
         total_ints = []
@@ -356,85 +354,14 @@
         self.is_isotope = self.highest_roi.is_isotope
         self.isotope_mz_seq = self.highest_roi.isotope_mz_seq
         self.isotope_int_seq = self.highest_roi.isotope_int_seq
         self.is_in_source_fragment = self.highest_roi.is_in_source_fragment
         self.adduct_type = self.highest_roi.adduct_type
 
 
-# def summarize_aligned_features(feature_list):
-#     """
-#     A function to summarize the aligned features.
-
-#     Parameters
-#     ----------------------------------------------------------
-#     feature_list: list
-#         A list of aligned features.   
-#     """
-
-#     for i, f in enumerate(feature_list):
-#         f.sum_feature(i)
-
-
-# def output_aligned_features(feature_list, file_names, path, int_values="peak_height"):
-#     """
-#     A function to output the aligned features.
-
-#     Parameters
-#     ----------------------------------------------------------
-#     feature_list: list
-#         A list of aligned features.
-#     output_path: str
-#         The path to the output file.
-#     """
-
-#     result = []
-
-#     for idx, f in enumerate(feature_list):
-        
-#         iso_dist = ""
-#         for i in range(len(f.isotope_mz_seq)):
-#             iso_dist += str(np.round(f.isotope_mz_seq[i], decimals=4)) + ";" + str(np.round(f.isotope_int_seq[i], decimals=0)) + "|"
-#         iso_dist = iso_dist[:-1]
-
-#         ms2 = ""
-#         if f.best_ms2 is not None:
-#             for i in range(len(f.best_ms2.peaks)):
-#                 ms2 += str(np.round(f.best_ms2.peaks[i, 0], decimals=4)) + ";" + str(np.round(f.best_ms2.peaks[i, 1], decimals=0)) + "|"
-#             ms2 = ms2[:-1]
-
-#         if int_values.lower()=="peak_area":
-#             int_seq = f.peak_area_seq
-#         elif int_values.lower()=="peak_height":
-#             int_seq = f.peak_height_seq
-#         elif int_values.lower()=="top_average":
-#             int_seq = f.top_average_seq
-
-#         temp = [idx+1, f.mz, f.rt, ms2, f.charge_state, f.is_isotope, iso_dist,
-#                 f.is_in_source_fragment, f.adduct_type, f.annotation, f.annotation_mode,
-#                 f.similarity, f.matched_peak_number, f.smiles, f.inchikey]
-                
-#         temp.extend(int_seq)
-
-#         result.append(temp)
-
-#     # convert result to a pandas dataframe
-#     columns = ["id", "mz", "rt", "ms2", "charge_state", "is_isotope", "isotope_dist",
-#                 "in_source_fragment", "adduct_type", "annotation", "annotation mode", 
-#                 "similarity_score", "matched_peak_number", "smiles", "inchikey"]
-
-#     file_names_output = [name.split("/")[-1].split(".")[0] for name in file_names]
-
-#     columns.extend(file_names_output)
-#     df = pd.DataFrame(result, columns=columns)
-    
-#     # save the dataframe to csv file
-#     path = path + "aligned_feature_table.csv"
-#     df.to_csv(path, index=False)
-
-
 # generate an empty feature table with 100000 rows
 def _init_feature_table(rows=5000, sample_names=[]):
     tmp = pd.DataFrame(
         columns=["ID", "m/z", "RT", "adduct", "is_isotope", "is_in_source_fragment", "Gaussian_similarity", "noise_level", "charge", "isotopes", "MS2", 
                 "matched_MS2", "search_mode", "annotation", "formula", "similarity", "matched_peak_number", "SMILES", "InChIKey", 
                 "fill_percentage", "alignment_reference"] + sample_names,
         index=range(rows)
```

### Comparing `masscube-0.0.6/src/masscube/annotation.py` & `masscube-0.0.7/src/masscube/annotation.py`

 * *Files identical despite different names*

### Comparing `masscube-0.0.6/src/masscube/feature_evaluation.py` & `masscube-0.0.7/src/masscube/feature_evaluation.py`

 * *Files identical despite different names*

### Comparing `masscube-0.0.6/src/masscube/feature_grouping.py` & `masscube-0.0.7/src/masscube/feature_grouping.py`

 * *Files identical despite different names*

### Comparing `masscube-0.0.6/src/masscube/feature_table_utils.py` & `masscube-0.0.7/src/masscube/feature_table_utils.py`

 * *Files identical despite different names*

### Comparing `masscube-0.0.6/src/masscube/network.py` & `masscube-0.0.7/src/masscube/network.py`

 * *Files identical despite different names*

### Comparing `masscube-0.0.6/src/masscube/normalization.py` & `masscube-0.0.7/src/masscube/normalization.py`

 * *Files identical despite different names*

### Comparing `masscube-0.0.6/src/masscube/params.py` & `masscube-0.0.7/src/masscube/params.py`

 * *Files identical despite different names*

### Comparing `masscube-0.0.6/src/masscube/peak_detect.py` & `masscube-0.0.7/src/masscube/peak_detect.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,14 +74,16 @@
         # Create new rois for the rest
         for i in range(len(s.int_seq)):
             if i not in visited_idx:
                 # Add a zero before the new roi
                 roi = Roi(scan_idx=last_ms1_idx, rt=last_rt, mz=s.mz_seq[i], intensity=0)
                 roi.extend_roi(scan_idx=ms1_idx, rt=s.rt, mz=s.mz_seq[i], intensity=s.int_seq[i])
                 rois.append(roi)
+        
+        rois.sort(key=lambda x: x.int_seq[-1], reverse=True)
         last_ms1_idx = ms1_idx
         last_rt = s.rt
            
     # Move all rois to final_rois
     for roi in rois:
         final_rois.append(roi)
 
@@ -92,15 +94,15 @@
     """
     Function to cut an ROI by providing the start and end positions.
     """
 
     r.int_seq = np.array(r.int_seq)
     r.noise_level = calculate_noise_level(r.int_seq)
 
-    if r.noise_level > 0.4 or len(r.int_seq) < 10 or r.peak_height < 3*int_tol:
+    if r.noise_level > 0.5 or len(r.int_seq) < 10 or r.peak_height < 3*int_tol:
         return [r]
 
     ss = gaussian_filter1d(r.int_seq, sigma=1)
     peaks, _ = find_peaks(ss, prominence=np.max(ss)*0.01, distance=5)
 
     peaks = peaks[r.int_seq[peaks] > 2*int_tol]
```

### Comparing `masscube-0.0.6/src/masscube/raw_data_utils.py` & `masscube-0.0.7/src/masscube/raw_data_utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -373,16 +373,16 @@
         # save the dataframe to csv file
         if user_defined_output_path:
             path = user_defined_output_path
         else:
             path = os.path.join(self.params.single_file_dir)
             if not os.path.exists(path):
                 os.makedirs(path)
-            path = os.path.join(self.params.single_file_dir, self.file_name + ".csv")
-        df.to_csv(path, index=False)
+            path = os.path.join(self.params.single_file_dir, self.file_name + ".txt")
+        df.to_csv(path, index=False, sep="\t")
     
 
     def get_eic_data(self, target_mz, target_rt=None, mz_tol=0.005, rt_tol=0.3, rt_range=None):
         """
         To get the EIC data of a target m/z.
 
         Parameters
```

### Comparing `masscube-0.0.6/src/masscube/stats.py` & `masscube-0.0.7/src/masscube/stats.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # A module for statistical analysis
 
 # imports
-from scipy.stats import ttest_ind, false_discovery_control, f_oneway
+from scipy.stats import ttest_ind, f_oneway
 import numpy as np
 import os
 
 def statistical_analysis(feature_table, params, before_norm=False):
     """
     1. Univariate analysis (t-test and p-value adjustment for two groups; ANOVA and p-value adjustment for multiple groups)
     2. Multivariate analysis (PCA)
```

### Comparing `masscube-0.0.6/src/masscube/utils_functions.py` & `masscube-0.0.7/src/masscube/utils_functions.py`

 * *Files identical despite different names*

### Comparing `masscube-0.0.6/src/masscube/visualization.py` & `masscube-0.0.7/src/masscube/visualization.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 import matplotlib.pyplot as plt
 import matplotlib.colors as mcolors
 import random
 import numpy as np
 import os
 import re
+from tqdm import tqdm
 
 from .annotation import _extract_peaks_from_string
 
 def plot_bpcs(data_list=None, output=None, autocolor=False):
     """
     A function to plot the base peak chromatograms (overlapped) of a list of data.
     
@@ -221,15 +222,15 @@
 
     if output_dir is None and params is not None:
         output_dir = params.ms2_matching_dir
     elif output_dir is None and params is None:
         print("Please provide the output directory for MS2 matching plots.")
         return None
 
-    for i in range(len(ms2)):
+    for i in tqdm(range(len(ms2))):
         peaks1 = _extract_peaks_from_string(ms2[i])
         peaks2 = _extract_peaks_from_string(matched_ms2[i])
 
         # replace all the special characters to "_"
         a = re.sub(r"[^a-zA-Z0-9]", "_", annotations[i])
         a = re.sub(r"[^a-zA-Z0-9]+", "_", a)
         a = "ID" + "_" + str(id[i]) + "_" + a
```

### Comparing `masscube-0.0.6/src/masscube.egg-info/PKG-INFO` & `masscube-0.0.7/src/masscube.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: masscube
-Version: 0.0.6
+Version: 0.0.7
 Summary: Accurate and fast data processing for metabolomics
 Author-email: Huaxu Yu <yhxchem@outlook.com>
 Maintainer-email: Huaxu Yu <yhxchem@outlook.com>
 Project-URL: Homepage, https://github.com/huaxuyu/masscube
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `masscube-0.0.6/src/masscube.egg-info/SOURCES.txt` & `masscube-0.0.7/src/masscube.egg-info/SOURCES.txt`

 * *Files identical despite different names*

