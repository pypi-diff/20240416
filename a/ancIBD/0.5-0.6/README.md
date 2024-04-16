# Comparing `tmp/ancIBD-0.5.tar.gz` & `tmp/ancIBD-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ancIBD-0.5.tar", last modified: Fri Jul 21 12:34:24 2023, max compression
+gzip compressed data, was "dist/ancIBD-0.6.tar", last modified: Tue Apr 16 13:38:50 2024, max compression
```

## Comparing `ancIBD-0.5.tar` & `ancIBD-0.6.tar`

### file list

```diff
@@ -1,46 +1,47 @@
-drwxrwsr-x   0 hr97     (174915) reich     (3060)        0 2023-07-21 12:34:24.000000 ancIBD-0.5/
--rw-rw-r--   0 hr97     (174915) reich     (3060)       20 2022-06-09 09:27:59.000000 ancIBD-0.5/MANIFEST.in
--rw-rw-r--   0 hr97     (174915) reich     (3060)      873 2023-07-21 12:34:24.000000 ancIBD-0.5/PKG-INFO
--rw-rw-r--   0 hr97     (174915) reich     (3060)      316 2023-07-21 09:48:38.000000 ancIBD-0.5/README.md
-drwxrwsr-x   0 hr97     (174915) reich     (3060)        0 2023-07-21 12:34:23.000000 ancIBD-0.5/ancIBD/
-drwxrwsr-x   0 hr97     (174915) reich     (3060)        0 2023-07-21 12:34:24.000000 ancIBD-0.5/ancIBD/.ipynb_checkpoints/
--rw-rw-r--   0 hr97     (174915) reich     (3060)    25752 2023-06-28 20:05:58.000000 ancIBD-0.5/ancIBD/.ipynb_checkpoints/cfunc-checkpoint.pyx
-drwxrwsr-x   0 hr97     (174915) reich     (3060)        0 2023-07-21 12:34:24.000000 ancIBD-0.5/ancIBD/IO/
--rw-rw-r--   0 hr97     (174915) reich     (3060)        5 2022-05-30 09:29:11.000000 ancIBD-0.5/ancIBD/IO/__init__.py
--rw-rw-r--   0 hr97     (174915) reich     (3060)     9654 2023-05-17 15:57:33.000000 ancIBD-0.5/ancIBD/IO/batch_run.py
--rw-rw-r--   0 hr97     (174915) reich     (3060)     2282 2023-05-12 10:01:20.000000 ancIBD-0.5/ancIBD/IO/h5_duplicates.py
--rw-rw-r--   0 hr97     (174915) reich     (3060)     4518 2023-05-12 10:01:19.000000 ancIBD-0.5/ancIBD/IO/h5_load.py
--rw-rw-r--   0 hr97     (174915) reich     (3060)     8621 2023-05-17 15:57:33.000000 ancIBD-0.5/ancIBD/IO/h5_modify.py
--rw-rw-r--   0 hr97     (174915) reich     (3060)     2888 2022-05-30 13:20:00.000000 ancIBD-0.5/ancIBD/IO/h5_qc.py
--rw-rw-r--   0 hr97     (174915) reich     (3060)     7793 2022-05-31 12:43:44.000000 ancIBD-0.5/ancIBD/IO/ind_ibd.py
--rw-rw-r--   0 hr97     (174915) reich     (3060)     7076 2023-06-28 14:17:47.000000 ancIBD-0.5/ancIBD/IO/prepare_h5.py
--rw-rw-r--   0 hr97     (174915) reich     (3060)        5 2022-05-27 13:36:54.000000 ancIBD-0.5/ancIBD/__init__.py
--rw-rw-r--   0 hr97     (174915) reich     (3060)     2054 2023-06-28 19:21:39.000000 ancIBD-0.5/ancIBD/ancIBD_summary.py
--rw-rw-r--   0 hr97     (174915) reich     (3060)  1241528 2023-06-28 20:23:11.000000 ancIBD-0.5/ancIBD/cfunc.c
--rw-rw-r--   0 hr97     (174915) reich     (3060)    25752 2023-06-28 20:05:58.000000 ancIBD-0.5/ancIBD/cfunc.pyx
--rw-rw-r--   0 hr97     (174915) reich     (3060)     7632 2023-06-28 19:21:39.000000 ancIBD-0.5/ancIBD/emission.py
--rw-rw-r--   0 hr97     (174915) reich     (3060)     3446 2023-06-28 19:21:39.000000 ancIBD-0.5/ancIBD/hmm.py
-drwxrwsr-x   0 hr97     (174915) reich     (3060)        0 2023-07-21 12:34:24.000000 ancIBD-0.5/ancIBD/ibd_stats/
--rw-rw-r--   0 hr97     (174915) reich     (3060)        5 2022-05-27 13:40:03.000000 ancIBD-0.5/ancIBD/ibd_stats/__init__.py
--rw-rw-r--   0 hr97     (174915) reich     (3060)     8606 2023-06-08 21:19:20.000000 ancIBD-0.5/ancIBD/ibd_stats/funcs.py
--rw-rw-r--   0 hr97     (174915) reich     (3060)    12220 2023-06-29 12:15:30.000000 ancIBD-0.5/ancIBD/loaddata.py
--rw-rw-r--   0 hr97     (174915) reich     (3060)     6149 2023-06-28 19:21:39.000000 ancIBD-0.5/ancIBD/main.py
-drwxrwsr-x   0 hr97     (174915) reich     (3060)        0 2023-07-21 12:34:24.000000 ancIBD-0.5/ancIBD/plot/
--rw-rw-r--   0 hr97     (174915) reich     (3060)        5 2022-05-27 13:37:56.000000 ancIBD-0.5/ancIBD/plot/__init__.py
--rw-rw-r--   0 hr97     (174915) reich     (3060)     2272 2023-06-08 21:19:20.000000 ancIBD-0.5/ancIBD/plot/plot_df.py
--rw-rw-r--   0 hr97     (174915) reich     (3060)    10773 2023-03-30 09:50:27.000000 ancIBD-0.5/ancIBD/plot/plot_karyotype.py
--rw-rw-r--   0 hr97     (174915) reich     (3060)     3659 2022-06-09 10:34:54.000000 ancIBD-0.5/ancIBD/plot/plot_opphomos.py
--rw-rw-r--   0 hr97     (174915) reich     (3060)     4583 2022-06-09 10:35:02.000000 ancIBD-0.5/ancIBD/plot/plot_posterior.py
--rw-rw-r--   0 hr97     (174915) reich     (3060)    10751 2023-06-28 19:21:39.000000 ancIBD-0.5/ancIBD/postprocessing.py
--rw-rw-r--   0 hr97     (174915) reich     (3060)    11875 2023-06-28 19:21:39.000000 ancIBD-0.5/ancIBD/run.py
--rw-rw-r--   0 hr97     (174915) reich     (3060)     6206 2023-06-28 19:21:39.000000 ancIBD-0.5/ancIBD/run_ancIBD.py
--rw-rw-r--   0 hr97     (174915) reich     (3060)    11808 2023-06-28 19:21:39.000000 ancIBD-0.5/ancIBD/transition.py
-drwxrwsr-x   0 hr97     (174915) reich     (3060)        0 2023-07-21 12:34:24.000000 ancIBD-0.5/ancIBD.egg-info/
--rw-rw-r--   0 hr97     (174915) reich     (3060)      873 2023-07-21 12:34:22.000000 ancIBD-0.5/ancIBD.egg-info/PKG-INFO
--rw-rw-r--   0 hr97     (174915) reich     (3060)      854 2023-07-21 12:34:23.000000 ancIBD-0.5/ancIBD.egg-info/SOURCES.txt
--rw-rw-r--   0 hr97     (174915) reich     (3060)        1 2023-07-21 12:34:22.000000 ancIBD-0.5/ancIBD.egg-info/dependency_links.txt
--rw-rw-r--   0 hr97     (174915) reich     (3060)       99 2023-07-21 12:34:22.000000 ancIBD-0.5/ancIBD.egg-info/entry_points.txt
--rw-rw-r--   0 hr97     (174915) reich     (3060)       68 2023-07-21 12:34:22.000000 ancIBD-0.5/ancIBD.egg-info/requires.txt
--rw-rw-r--   0 hr97     (174915) reich     (3060)        7 2023-07-21 12:34:22.000000 ancIBD-0.5/ancIBD.egg-info/top_level.txt
--rw-rw-r--   0 hr97     (174915) reich     (3060)       38 2023-07-21 12:34:24.000000 ancIBD-0.5/setup.cfg
--rw-rw-r--   0 hr97     (174915) reich     (3060)     1569 2023-07-21 12:33:14.000000 ancIBD-0.5/setup.py
+drwxrwsr-x   0 hr97     (174915) reich     (3060)        0 2024-04-16 13:38:50.000000 ancIBD-0.6/
+-rw-rw-r--   0 hr97     (174915) reich     (3060)       20 2022-06-09 09:27:59.000000 ancIBD-0.6/MANIFEST.in
+-rw-rw-r--   0 hr97     (174915) reich     (3060)      873 2024-04-16 13:38:50.000000 ancIBD-0.6/PKG-INFO
+-rw-rw-r--   0 hr97     (174915) reich     (3060)      316 2023-07-21 09:48:38.000000 ancIBD-0.6/README.md
+drwxrwsr-x   0 hr97     (174915) reich     (3060)        0 2024-04-16 13:38:50.000000 ancIBD-0.6/ancIBD/
+drwxrwsr-x   0 hr97     (174915) reich     (3060)        0 2024-04-16 13:38:50.000000 ancIBD-0.6/ancIBD/.ipynb_checkpoints/
+-rw-rw-r--   0 hr97     (174915) reich     (3060)    25752 2023-06-28 20:05:58.000000 ancIBD-0.6/ancIBD/.ipynb_checkpoints/cfunc-checkpoint.pyx
+drwxrwsr-x   0 hr97     (174915) reich     (3060)        0 2024-04-16 13:38:50.000000 ancIBD-0.6/ancIBD/IO/
+-rw-rw-r--   0 hr97     (174915) reich     (3060)        5 2022-05-30 09:29:11.000000 ancIBD-0.6/ancIBD/IO/__init__.py
+-rw-rw-r--   0 hr97     (174915) reich     (3060)    11084 2023-08-31 13:33:39.000000 ancIBD-0.6/ancIBD/IO/batch_run.py
+-rw-rw-r--   0 hr97     (174915) reich     (3060)     2282 2023-05-12 10:01:20.000000 ancIBD-0.6/ancIBD/IO/h5_duplicates.py
+-rw-rw-r--   0 hr97     (174915) reich     (3060)     6232 2024-03-24 22:02:32.000000 ancIBD-0.6/ancIBD/IO/h5_load.py
+-rw-rw-r--   0 hr97     (174915) reich     (3060)     8621 2023-05-17 15:57:33.000000 ancIBD-0.6/ancIBD/IO/h5_modify.py
+-rw-rw-r--   0 hr97     (174915) reich     (3060)     2888 2022-05-30 13:20:00.000000 ancIBD-0.6/ancIBD/IO/h5_qc.py
+-rw-rw-r--   0 hr97     (174915) reich     (3060)    10872 2024-03-13 13:39:48.000000 ancIBD-0.6/ancIBD/IO/ind_ibd.py
+-rw-rw-r--   0 hr97     (174915) reich     (3060)     7076 2023-06-28 14:17:47.000000 ancIBD-0.6/ancIBD/IO/prepare_h5.py
+-rw-rw-r--   0 hr97     (174915) reich     (3060)        5 2022-05-27 13:36:54.000000 ancIBD-0.6/ancIBD/__init__.py
+-rw-rw-r--   0 hr97     (174915) reich     (3060)     2529 2024-03-13 13:39:48.000000 ancIBD-0.6/ancIBD/ancIBD_summary.py
+-rw-rw-r--   0 hr97     (174915) reich     (3060)  1241528 2023-06-28 20:23:11.000000 ancIBD-0.6/ancIBD/cfunc.c
+-rw-rw-r--   0 hr97     (174915) reich     (3060)    25752 2023-06-28 20:05:58.000000 ancIBD-0.6/ancIBD/cfunc.pyx
+-rw-rw-r--   0 hr97     (174915) reich     (3060)    10195 2024-03-13 13:39:48.000000 ancIBD-0.6/ancIBD/emission.py
+-rw-rw-r--   0 hr97     (174915) reich     (3060)     3446 2023-06-28 19:21:39.000000 ancIBD-0.6/ancIBD/hmm.py
+drwxrwsr-x   0 hr97     (174915) reich     (3060)        0 2024-04-16 13:38:50.000000 ancIBD-0.6/ancIBD/ibd_stats/
+-rw-rw-r--   0 hr97     (174915) reich     (3060)        5 2022-05-27 13:40:03.000000 ancIBD-0.6/ancIBD/ibd_stats/__init__.py
+-rw-rw-r--   0 hr97     (174915) reich     (3060)     8606 2023-06-08 21:19:20.000000 ancIBD-0.6/ancIBD/ibd_stats/funcs.py
+-rw-rw-r--   0 hr97     (174915) reich     (3060)    13712 2024-03-24 18:41:00.000000 ancIBD-0.6/ancIBD/loaddata.py
+-rw-rw-r--   0 hr97     (174915) reich     (3060)     6169 2024-03-13 13:39:48.000000 ancIBD-0.6/ancIBD/main.py
+drwxrwsr-x   0 hr97     (174915) reich     (3060)        0 2024-04-16 13:38:50.000000 ancIBD-0.6/ancIBD/plot/
+-rw-rw-r--   0 hr97     (174915) reich     (3060)        5 2022-05-27 13:37:56.000000 ancIBD-0.6/ancIBD/plot/__init__.py
+-rw-rw-r--   0 hr97     (174915) reich     (3060)     2272 2023-06-08 21:19:20.000000 ancIBD-0.6/ancIBD/plot/plot_df.py
+-rw-rw-r--   0 hr97     (174915) reich     (3060)    10773 2023-03-30 09:50:27.000000 ancIBD-0.6/ancIBD/plot/plot_karyotype.py
+-rw-rw-r--   0 hr97     (174915) reich     (3060)     4095 2024-03-13 13:39:48.000000 ancIBD-0.6/ancIBD/plot/plot_opphomos.py
+-rw-rw-r--   0 hr97     (174915) reich     (3060)     7381 2024-03-24 22:02:27.000000 ancIBD-0.6/ancIBD/plot/plot_posterior.py
+-rw-rw-r--   0 hr97     (174915) reich     (3060)    16121 2024-03-13 13:39:48.000000 ancIBD-0.6/ancIBD/postprocessing.py
+-rw-rw-r--   0 hr97     (174915) reich     (3060)    25291 2024-03-24 22:22:44.000000 ancIBD-0.6/ancIBD/run.py
+-rw-rw-r--   0 hr97     (174915) reich     (3060)     7842 2024-03-13 13:39:48.000000 ancIBD-0.6/ancIBD/run_ancIBD.py
+-rw-rw-r--   0 hr97     (174915) reich     (3060)     8818 2024-03-13 13:39:48.000000 ancIBD-0.6/ancIBD/run_ancIBDX.py
+-rw-rw-r--   0 hr97     (174915) reich     (3060)    17635 2024-03-13 13:39:48.000000 ancIBD-0.6/ancIBD/transition.py
+drwxrwsr-x   0 hr97     (174915) reich     (3060)        0 2024-04-16 13:38:50.000000 ancIBD-0.6/ancIBD.egg-info/
+-rw-rw-r--   0 hr97     (174915) reich     (3060)      873 2024-04-16 13:38:49.000000 ancIBD-0.6/ancIBD.egg-info/PKG-INFO
+-rw-rw-r--   0 hr97     (174915) reich     (3060)      876 2024-04-16 13:38:50.000000 ancIBD-0.6/ancIBD.egg-info/SOURCES.txt
+-rw-rw-r--   0 hr97     (174915) reich     (3060)        1 2024-04-16 13:38:49.000000 ancIBD-0.6/ancIBD.egg-info/dependency_links.txt
+-rw-rw-r--   0 hr97     (174915) reich     (3060)      133 2024-04-16 13:38:49.000000 ancIBD-0.6/ancIBD.egg-info/entry_points.txt
+-rw-rw-r--   0 hr97     (174915) reich     (3060)       68 2024-04-16 13:38:49.000000 ancIBD-0.6/ancIBD.egg-info/requires.txt
+-rw-rw-r--   0 hr97     (174915) reich     (3060)        7 2024-04-16 13:38:49.000000 ancIBD-0.6/ancIBD.egg-info/top_level.txt
+-rw-rw-r--   0 hr97     (174915) reich     (3060)       38 2024-04-16 13:38:50.000000 ancIBD-0.6/setup.cfg
+-rw-rw-r--   0 hr97     (174915) reich     (3060)     1623 2024-04-16 13:35:18.000000 ancIBD-0.6/setup.py
```

### Comparing `ancIBD-0.5/PKG-INFO` & `ancIBD-0.6/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ancIBD
-Version: 0.5
+Version: 0.6
 Summary: Identify IBD segments between pairs of individuals in ancient human DNA data
 Home-page: https://github.com/hringbauer/ancIBD
 Author: Harald Ringbauer
 Author-email: harald_ringbauer@eva.mpg.de
 License: UNKNOWN
 Description: # ancIBD
         This Python software package screens ancient human DNA for long IBD blocks (Identity by Descent segments) shared between pairs of individuals.
```

### Comparing `ancIBD-0.5/ancIBD/.ipynb_checkpoints/cfunc-checkpoint.pyx` & `ancIBD-0.6/ancIBD/.ipynb_checkpoints/cfunc-checkpoint.pyx`

 * *Files identical despite different names*

### Comparing `ancIBD-0.5/ancIBD/IO/batch_run.py` & `ancIBD-0.6/ancIBD/IO/batch_run.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """
-Functions to prepare parameters for a batch run.
-Splits up all pairs into batches, in a standard algorithm
-@ Author: Harald Ringbauer, 2022
+Various Functions to prepare parameters for a batched run on a cluster
+Splits up individuals into batches, run all pw. batches with ancIBD, and then collect results.
+Functions here splits up input into batches, in a standardized way
+@ Author: Harald Ringbauer, 2023
 """
 
 import numpy as np
 import pandas as pd
 import os as os
 import itertools as it
 
@@ -194,20 +195,20 @@
         batches = np.column_stack(np.tril_indices(n=batches, k=0))
     res = []
     
     for b1,b2 in batches:
         folder_batch = os.path.join(folder_out, f"batch{b1}_{b2}/")
         df_ibds = join_chromosomes(folder_batch, file_out="", 
                                    chs=chs, output=output)
+        # Do Filtering here per batch to avoid giant file size
+        df_ibds = filter_ibd_df(df_ibds, min_cm=min_cm, snp_cm=snp_cm, output=output) 
         res.append(df_ibds)
     df_res = pd.concat(res)
-    df_res = filter_ibd_df(df_res, min_cm=min_cm, snp_cm=snp_cm, output=output) 
     return df_res 
 
-
 def print_runid_missing(b = 1, folder_out = "", output=False):
     """Finds and prints indices of missing output (chXX.tsv) for batchwise runs.
     Return list of missing indices. Ideal for rerunning batch scripts.
     Uses C Indexing as would be used in submission script."""
     batches = np.column_stack(np.tril_indices(n=b, k=0))
 
     ls = []
@@ -217,7 +218,39 @@
             exist = os.path.exists(folder_batch)
             if not exist:
                 if output:
                     print(f"Missing! ch: {ch} batch: {b1}-{b2}")
                 l = b * (b+1)/2 * (ch-1) + (b1+1) * b1/2 + b2 + 1 # The +1 is c indexing
                 ls.append(str(int(l)))
     return ls
+
+def find_output_missing(metapath="", folder_out="",
+                        batch_size = 400, rge = [10, 20]):
+    """Return List of all run nr.s that are missing.
+    metapath: Path to .tsv of IIDs run for IBD screening [str]
+    folder_out: Output folder [str]
+    batch_size: How many individuals have been run per batch [int]"""
+    
+    df = pd.read_csv(metapath, sep="\t")
+    k = len(df)
+
+    run_nr_missing = []
+    for i in range(rge[0], rge[1]):
+        b1, b2, ch  = get_run_lists_batch(i, k=k, batch_size=batch_size, output=False)
+        path = os.path.join(folder_out, f"batch{b1}_{b2}", f"ch{ch}.tsv")
+        there = os.path.exists(path)
+
+        if not there:
+            run_nr_missing.append(i)
+
+    print(f"Did not find output for: {len(run_nr_missing)} / {rge[1]-rge[0]} Runs")
+    if len(run_nr_missing) == 0:
+        print("Success! Everything found")
+    return run_nr_missing
+
+def get_batch_nr(n_iids, batchsize=400, n_chr=22):
+    """Get the number of jobs to submit to cluster.
+    Return n [int]"""
+    n_batch = np.ceil(n_iids/batchsize)
+    print(f"{n_iids} in batches of {batchsize}: {n_batch} Batches")
+    n = int((n_batch * (n_batch+1) * n_chr)/2)
+    print(f"Need {n} Submissions in total (0-{n-1})")
```

### Comparing `ancIBD-0.5/ancIBD/IO/h5_duplicates.py` & `ancIBD-0.6/ancIBD/IO/h5_duplicates.py`

 * *Files identical despite different names*

### Comparing `ancIBD-0.5/ancIBD/IO/h5_load.py` & `ancIBD-0.6/ancIBD/IO/h5_load.py`

 * *Files 26% similar despite different names*

```diff
@@ -34,17 +34,22 @@
 def get_coverage(f, j):
     """Get Coverage of sample j in hdf5 f"""
     ads =  f["calldata/AD"][:,j,:2]
     ads[ads<0]=0
     cov = np.mean(ads)*2
     return cov
 
-def get_markers_good(f, j, output=True, cutoff=0.99):
+def get_markers_good(f, j, output=True, cutoff=0.99, ploidy=2):
     """Get markers"""
-    m = np.max(f["calldata/GP"][:,j,:], axis=1)
+    if ploidy==2:
+        m = np.max(f["calldata/GP"][:,j,:], axis=1)
+    elif ploidy==1:
+        m = np.nanmax(f["calldata/GP"][:,j,:], axis=1)
+    else:
+        raise ValueError("ploidy should be 1 or 2.")
     idx = (m>=cutoff)
     if output:
         c1 = np.mean(idx)
         print(f"Filtering to {cutoff} GP variants: {c1:.3f}x")
     return idx
 
 ###########################
@@ -90,39 +95,50 @@
     df_ind = pd.concat(dfs)
     return df_ind
 
 #############################
 ### Extract Pairs of Markers
 
 def get_genos_pairs(f, sample1="SUC006", sample2="R26.SG", 
-                    cutoff=0.98, output=True, phased=False, exact=False):
+                    cutoff=0.98, output=True, phased=False, exact=False, ploidy=(2,2)):
     """Return Genotypes and Map of pairs at intersection with GP>cutoff.
     phased: Whether to return [lx2] phased vector or [l] vetor of #derived.
     exact: Whether IID has to be an exact match"""
     if exact:
         j1 = get_idx_iid_exact(f, sample1)
         j2 = get_idx_iid_exact(f, sample2)
         
     else:
         j1 = get_idx_iid(f, sample1)
         j2 = get_idx_iid(f, sample2)
     
-    idx1 = get_markers_good(f, j1, cutoff=cutoff, output=output)
-    idx2 = get_markers_good(f, j2, cutoff=cutoff, output=output)
+    idx1 = get_markers_good(f, j1, cutoff=cutoff, output=output, ploidy=ploidy[0])
+    idx2 = get_markers_good(f, j2, cutoff=cutoff, output=output, ploidy=ploidy[1])
     idx = (idx1 & idx2)
     snp_frac = np.mean(idx)
     if output:
         print(f"Filtering to common GP variants: {snp_frac:.3f}x")
     
     m = f["variants/MAP"][:][idx]
     
     gt1 = f["calldata/GT"][:, j1, :][idx,:]
     gt2 = f["calldata/GT"][:, j2, :][idx,:]
     if not phased:
-        gt1, gt2 = np.sum(gt1, axis=1), np.sum(gt2, axis=1)
+        if ploidy[0] == 2:
+            gt1 = np.sum(gt1, axis=1)
+        elif ploidy[0] == 1:
+            gt1 = gt1[:,0]
+        else:
+            raise ValueError("ploidy should be 1 or 2.")
+        if ploidy[1] == 2:
+            gt2 = np.sum(gt2, axis=1)
+        elif ploidy[1] == 1:
+            gt2 = gt2[:,0]
+        else:
+            raise ValueError("ploidy should be 1 or 2.")
     return gt1, gt2, m
 
 def opp_homos(g1, g2):
     """Return opposing homozygotes"""
     o1 = (g1 == 0) & (g2 == 2)
     o2 = (g1 == 2) & (g2 == 0)
     return (o1 | o2)
@@ -133,8 +149,34 @@
     """Return opposing homozygotes boolean array and map array at intersection with
     GP>cutoff."""
     load_path = f_path + str(ch) + ".h5"
     with h5py.File(load_path, "r") as f:
         g1, g2, m = get_genos_pairs(f, sample1=iid1, sample2=iid2, 
                                 cutoff=cutoff, output=output, exact=exact)
         o_homos = opp_homos(g1, g2)
-    return o_homos, m
+    return o_homos, m
+
+def get_opp_homos_X(f_path, iid1, iid2, ploidy=(2,2), cutoff=0.99, output=True, exact=False):
+    """
+    return oppo homo boolean array and map array at intersection with GP>cutoff. This function is tailored for X chromosome.
+    Be careful with the ploidy difference between males and females.
+    The ploidy argument should be a tuple of two integers, indicating the ploidy of iid1, iid2, respectively. 
+    """
+    with h5py.File(f_path, 'r') as f:
+        g1, g2, m = get_genos_pairs(f, sample1=iid1, sample2=iid2, cutoff=cutoff, output=output, exact=exact, ploidy=ploidy)
+        if ploidy[0] == 1:
+            g1 = 2*g1
+        if ploidy[1] == 1:
+            g2 = 2*g2
+        o_homos = opp_homos(g1, g2)
+    return o_homos, m
+
+
+def get_diff_gt_f(f_path, iid1, iid2, ch, cutoff=0.99, output=True, exact=False):
+    """
+    Return diff genotype boolean array and map array at intersection of maxGP > cutoff
+    """
+    load_path = f_path + str(ch) + ".h5"
+    with h5py.File(load_path, 'r') as f:
+        g1, g2, m = get_genos_pairs(f, sample1=iid1, sample2=iid2, 
+                                cutoff=cutoff, output=output, exact=exact)
+    return g1 != g2, m
```

### Comparing `ancIBD-0.5/ancIBD/IO/h5_modify.py` & `ancIBD-0.6/ancIBD/IO/h5_modify.py`

 * *Files identical despite different names*

### Comparing `ancIBD-0.5/ancIBD/IO/h5_qc.py` & `ancIBD-0.6/ancIBD/IO/h5_qc.py`

 * *Files identical despite different names*

### Comparing `ancIBD-0.5/ancIBD/IO/ind_ibd.py` & `ancIBD-0.6/ancIBD/IO/ind_ibd.py`

 * *Files 17% similar despite different names*

```diff
@@ -110,14 +110,94 @@
     ### Save if needed
     if len(savepath) > 0:
         df_res.to_csv(savepath, sep="\t", index=False)
         print(f"Saved {len(df_res)} individual IBD pairs to: {savepath}")
 
     return df_res
 
+def create_ind_ibd_df_IBD2(ibd_data = "/n/groups/reich/hringbauer/git/yamnaya/output/ibd/v43/ch_all.tsv",
+                      min_cms = [8, 12, 16, 20], snp_cm = 220, 
+                      min_cm = 6, sort_col = -1,
+                      savepath="", output=True):
+    """Create dataframe with summary statistics for each individual.
+    !!!This should only be used for ancIBD run with the IBD2 mode.!!!
+    Return this novel dataframe in hapROH format [IBD in cM]
+    ibd_data: If string, what ibd file to load. Or IBD dataframe.
+    savepath: If given: Save post-processed IBD dataframe to there.
+    min_cms: What IBD lengths to use as cutoff in analysis [cM]. Note that this filter only applies to IBD1.
+    snp_cm: Minimum Density of SNP per cM of IBD block. Note that this filter only applies to IBD1.
+    sort_col: Which min_cms col to use for sort. If <0 no sort conducted."""
+    if isinstance(ibd_data, str): 
+        df_ibd = pd.read_csv(ibd_data, sep="\t")
+    else:
+        df_ibd = ibd_data
+        
+    ### Filter. Be aggressive here for good set for  relatedness. Cutoff the slack
+    df_ibd1 = df_ibd[df_ibd['segment_type'] == 'IBD1']
+    df_ibd1 = filter_ibd_df(df_ibd1, min_cm=min_cms[0], snp_cm=snp_cm, output=output)
+    df_ibd2 = df_ibd[df_ibd['segment_type'] == 'IBD2']
+
+    ### Fish out the no IBD data
+    if len(df_ibd)==0:
+        df_res = pd.DataFrame(columns=['iid1','iid2', "max_IBD"])
+        for m_cm in min_cms:
+            df_res[f"sum_IBD>{m_cm}"] = 0
+            df_res[f"n_IBD>{m_cm}"] = 0
+    
+    else: # In case there are IBD
+        if output:
+            print('IBD1:')
+            print(df_ibd1["ch"].value_counts())
+            print('IBD2:')
+            print(df_ibd2["ch"].value_counts())
+
+        #df_ibd = df_ibd.sort_values(by = ["iid1", "iid2", "ch"]) # Sort so it is easier to split up
+        grouped1 = df_ibd1.groupby(['iid1','iid2'])
+
+        df_res = pd.DataFrame(grouped1.groups.keys())
+
+        df_res.columns = ["iid1", "iid2"]
+
+        ### Create the actual statistics
+        stats = [roh_statistics_df(df, min_cms=min_cms) for _, df in grouped1]
+        stats = np.array(stats)
+
+        df_res["max_IBD"] = stats[:, 0, 2] * 100
+
+        ### Add Values for varying cM cutoffs:
+        for j, m_cm in enumerate(min_cms):
+            df_res[f"sum_IBD>{m_cm}"] = stats[:,j, 0] * 100
+            df_res[f"n_IBD>{m_cm}"] = stats[:,j,1]
+
+        ### add IBD2 column
+        sumIBD2 = df_ibd2.groupby(['iid1','iid2'])['lengthM'].sum().reset_index()
+        print(sumIBD2)
+        stats = [100*sumIBD2[(sumIBD2["iid1"]==k[0]) & (sumIBD2["iid2"]==k[1])]['lengthM'].sum() for k in grouped1.groups.keys()]
+        print(stats)
+        df_res["sum_IBD2"] = stats
+
+        if sort_col>=0:
+            df_res = df_res.sort_values(by=f"sum_IBD>{min_cms[sort_col]}", ascending=False)  # Sort output by minimal Cutoff  
+    
+    ### Save if needed
+    if len(savepath) > 0:
+        df_res.to_csv(savepath, sep="\t", index=False)
+        print(f"Saved {len(df_res)} individual IBD pairs to: {savepath}")
+
+    return df_res
+
+
+
+
+
+
+
+
+
+
 def ind_all_ibd_df(path_ibd = "/n/groups/reich/hringbauer/git/yamnaya/output/ibd/v43/ch_all.tsv",
                    col_lengthM="lengthM", snp_cm = 220, min_cm = 5,
                    output=True, sort=True, decimals=2, col_new="ibd", savepath=""):
     """Create dataframe with all IBD for each indivdiual pair
     Return this novel dataframe in hapROH format [IBD in cM]
     path_ibd: What ibd file to load.
     snp_cm: Minimum Density of SNP per cM of IBD block.
```

### Comparing `ancIBD-0.5/ancIBD/IO/prepare_h5.py` & `ancIBD-0.6/ancIBD/IO/prepare_h5.py`

 * *Files identical despite different names*

### Comparing `ancIBD-0.5/ancIBD/ancIBD_summary.py` & `ancIBD-0.6/ancIBD/ancIBD_summary.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,38 @@
 ## a wrapper script to summarize the results of ancIBD (combine results from all 22 autosomes)
 from ancIBD.IO.ind_ibd import combine_all_chroms
-from ancIBD.IO.ind_ibd import create_ind_ibd_df
+from ancIBD.IO.ind_ibd import create_ind_ibd_df, create_ind_ibd_df_IBD2
 import argparse
 import os
 from pathlib import Path
 
 def main():
     parser = argparse.ArgumentParser(description='Run ancIBD.')
     parser.add_argument('--tsv', action="store", dest="tsv", type=str, required=True,
                         help="base path to the individual IBD files.")
     parser.add_argument('--ch', action="store", dest="ch", type=str, required=False, default='1-22', help='chromosome number, expressed in the format chrom-chrom, e.g, 1-22). The default is 1-22.')
     parser.add_argument('--bin', action="store", dest="bin", type=str, required=False, default='8,12,16,20', help='length bin over which IBD sharing summary statistics for pairs of samples will be calculated. Default is 8,12,16,20.')
     parser.add_argument('--snp_cm', action="store", dest="snp_cm", type=float, required=False, default=220, help='minimum number of SNPs per centimorgan for a segment to be considered. The default is 220 to reduce false positive rates.')
     parser.add_argument('--out', action="store", dest="out", type=str, required=False, help='output folder to store results. If not specified, the results will be stored in the current directory.')
+    parser.add_argument('--IBD2', action='store_true', dest='IBD2', default=False, help='if specified, the script will also summarize IBD2 segments. The default is False.')
     args = parser.parse_args()
 
     ch1, ch2 = args.ch.split('-')
     chs = range(int(ch1), int(ch2)+1)
     oDir = args.out
     if oDir is None:
         # set output directory to current directory
         oDir = os.getcwd()
 
     combine_all_chroms(chs=chs, folder_base=args.tsv,
                    path_save=os.path.join(oDir, 'ch_all.tsv'))
     
     #### now save a summary of IBD sharing between all pairs of individuals
     min_cms = [float(l) for l in args.bin.split(',')]
-    create_ind_ibd_df(ibd_data = os.path.join(oDir, 'ch_all.tsv'),
+    if not args.IBD2:
+        create_ind_ibd_df(ibd_data = os.path.join(oDir, 'ch_all.tsv'),
+                      min_cms = min_cms, snp_cm = args.snp_cm, min_cm = min_cms[0], sort_col = 0,
+                      savepath = os.path.join(oDir, "ibd_ind.tsv"))
+    else:
+        create_ind_ibd_df_IBD2(ibd_data = os.path.join(oDir, 'ch_all.tsv'),
                       min_cms = min_cms, snp_cm = args.snp_cm, min_cm = min_cms[0], sort_col = 0,
                       savepath = os.path.join(oDir, "ibd_ind.tsv"))
```

### Comparing `ancIBD-0.5/ancIBD/cfunc.c` & `ancIBD-0.6/ancIBD/cfunc.c`

 * *Files identical despite different names*

### Comparing `ancIBD-0.5/ancIBD/cfunc.pyx` & `ancIBD-0.6/ancIBD/cfunc.pyx`

 * *Files identical despite different names*

### Comparing `ancIBD-0.5/ancIBD/emission.py` & `ancIBD-0.6/ancIBD/emission.py`

 * *Files 15% similar despite different names*

```diff
@@ -139,21 +139,25 @@
 
 class HaplotypeSharingEmissions3(HaplotypeSharingEmissions2):
     """
     Basically the same as HaplotypeSharingEmissions2, but with two additional states to account for IBD2 region
     """
 
 
-    def give_emission_matrix(self, hts_p, p, dtype='float'):
+    def give_emission_matrix(self, hts_p, p, p_min=1e-3, dtype='float'):
         """
         Give emission matrix for 7-state HMM.
         0th state: non-IBD state
         1st-4th state: IBD1 state
         5-7th state: IBD2 state
         """
+        # to avoid division by zero error, set p to be at least p_min and at most 1 - p_min
+        p = np.maximum(p, p_min)
+        p = np.minimum(p, 1-p_min)
+        
         l = np.shape(hts_p)[1]
         e_mat = np.zeros((7,l), dtype=dtype)
         e_mat[:5,:] = super().give_emission_matrix(hts_p, p, dtype)
 
         x1A = 1 - hts_p[0,:]
         x1B = 1 - hts_p[1,:]
         x2A = 1 - hts_p[2,:]
@@ -168,21 +172,64 @@
         e_mat[6,:] = (1-x1A)*(1-x1B)*(1-x2A)*(1-x2B)/((1-p)**2) + \
                 (1-x1A)*x1B*x2A*(1-x2B)/(p*(1-p)) + \
                 x1A*(1-x1B)*(1-x2A)*x2B/(p*(1-p)) + \
                 x1A*x1B*x2A*x2B/(p**2)
 
         return e_mat
 
+############################################ Experimental with X chromosomes ############################################
+class HaplotypeSharing_twoHaploid(HaplotypeSharingEmissions2):
+    """Class for emission probabilities of two haploid genomes (e.g, two male X chromosome) 
+    who possibly share one haplotype"""
+    
+    def give_emission_matrix(self, hts_p, p, dtype="float"):
+        """Give emission Matrix for 2-state HMM.
+        0th state: HW 1st State: Haplotype Copying
+        Input: p: [l] Array of (derived) allele frequencies
+        hts_p: [4,l] Array of two ancestral haplotype probabilities. 
+            Note that for haploid samples, hts_p[1,:] and hts_p[4,:] are not used and the values there are meaningless.
+            I keep these two rows only for consistency with the diploid case.
+        Return: emission matrix [2,l]."""
+        l = np.shape(hts_p)[1]
+        e_mat = np.zeros((2,l), dtype=dtype)
+        e_mat[0,:] = 1 # Because simply proportional to P(D)
+        e_mat[1,:] = self.hw_probs_shared(hts_p, p=p, shared=[0,2])
+        return e_mat
+    
+class HaplotypeSharing_hapVSdiploid(HaplotypeSharingEmissions2):
+    """Class for emission probabilities of one haploid and one diploid genomes (e.g, between a male and a female chromosome)
+    who possibly share one haplotype"""
+
+    def give_emission_matrix(self, hts_p, p, dtype="float"):
+        """Give emission Matrix for 3-state HMM. 
+        Note that the code assumes that the first sample is haploid and the second sample is diploid.
+        0th state: HW 
+        1st-2nd State: Haplotype Copying
+        Input: p: [l] Array of (derived) allele frequencies
+        hts_p: [4,l] Array of two ancestral haplotype probabilities. 
+            Note that for hts_p[1,:] is not used and the values there are meaningless.
+            I keep these it only for consistency with the diploid case.
+        Return: emission matrix [3,l]."""
 
+        l = np.shape(hts_p)[1]
+        e_mat = np.zeros((3,l), dtype=dtype)
+        e_mat[0,:] = 1 # Because simply proportional to P(D)
+        e_mat[1,:] = self.hw_probs_shared(hts_p, p=p, shared=[0,2])
+        e_mat[2,:] = self.hw_probs_shared(hts_p, p=p, shared=[0,3])
+        return e_mat
 
 
 def load_emission_model(e_model="haploid_gl"):
     """Factory method to return the right Emission Model"""
     if e_model == "haploid_gl":
         e_obj = HaplotypeSharingEmissions()
     elif e_model == "haploid_gl2":
         e_obj = HaplotypeSharingEmissions2()
     elif e_model == 'IBD2':
         e_obj = HaplotypeSharingEmissions3()
+    elif e_model == "twoHaploid":
+        e_obj = HaplotypeSharing_twoHaploid()
+    elif e_model == "hapVSdiploid":
+        e_obj = HaplotypeSharing_hapVSdiploid()
     else:
         raise NotImplementedError("Emission Model not found!")
     return e_obj
```

### Comparing `ancIBD-0.5/ancIBD/hmm.py` & `ancIBD-0.6/ancIBD/hmm.py`

 * *Files identical despite different names*

### Comparing `ancIBD-0.5/ancIBD/ibd_stats/funcs.py` & `ancIBD-0.6/ancIBD/ibd_stats/funcs.py`

 * *Files identical despite different names*

### Comparing `ancIBD-0.5/ancIBD/loaddata.py` & `ancIBD-0.6/ancIBD/loaddata.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 @ Author: Harald Ringbauer, September 2020
 """
 
 import pickle as pickle
 import numpy as np
 import os as os
 import h5py as h5py
+import warnings
 
 ###############################
 ###############################
 
 class LoadData(object):
     """Class to load data in uniform format"""
     path = "" # Path to load from (usually folder)
@@ -113,18 +114,20 @@
                 p = p[:,0]
         return p
         
     def get_individual_idx(self, f, iid="", f_col="samples"):
         """Return index of individual iid"""
         samples = f[f_col].asstr()[:]
         idx = (samples == iid)
-        if np.sum(idx)!=1:
-            raise RuntimeWarning(f"{np.sum(idx)} entries found for {iid}")
-        assert(np.sum(idx)>0) # Sanity Check
-        idx=np.where(idx)[0][0]
+        
+        if np.sum(idx)==0:  # Sanity Check wheter IID found at all (raise stop)
+            raise RuntimeWarning(f"No entry in H5 found for iid: {iid}") 
+        if np.sum(idx)>1:   # Sanity Check wether multiple IIDs found (warning only)
+            warnings.warn(f"{np.sum(idx)} entries found for iid: {iid}", RuntimeWarning)    
+        idx=np.where(idx)[0][0] # Get the first IID match index
         return idx  
     
     def get_haplo_prob(self, f, idx):
         """Get haploid ancestral probability for indivual [2,l]"""
         h1 = f["calldata/GT"][:,idx,:].T
         m = np.max(f["calldata/GP"][:,idx,:], axis=1)
         m = np.minimum(m,  1 - self.min_error)
@@ -155,14 +158,15 @@
     path_h5=""
     iids = []
     ch = 3   # Which chromosome to load
     min_error = 1e-5 # Minimum Probability of genotyping error  
     p_col = "" # The hdf5 column with der. all freqs. If given, use the field
     # If "default" use p=0.5 everywhere
     # default value for p_col in my hdf5s: variants/AF_ALL
+    ploidy = 2 # ploidy of the individuals
     
     def get_haplo_prob(self, f, idcs):
         """Get haploid ancestral probability for n individuals 
         Return [n,l,2] array"""
         h1 = f["calldata/GT"][:,idcs,:] ### Get l, n, 2
         l,n,_ = np.shape(h1) # Get the nr loci
         m = np.max(f["calldata/GP"][:,idcs,:], axis=2)  
@@ -170,52 +174,54 @@
         h1 = (1-h1) * m[:,:,None] + h1 * (1 - m[:,:,None]) # Probability of being ancestral
         h1 = np.swapaxes(h1, 0, 1) # ->n,l,2
         h1 = np.swapaxes(h1, 1, 2) #-> n,2,l
         h1 = h1.reshape((2*n,l))
         #h1 = np.swapaxes(h1, 0, 1)
         return h1
     
-    def filter_valid_data(self, hts, p, m):
+    def filter_valid_data(self, hts, p, m, bp):
         """Filter to SNPs with fully valid data. 
         Return filtered data."""
         idx = ~(np.isnan(hts).any(axis=0)) # Flag all markers that are not null
         
         ### Output and Raise warning if too much data missing:
         if self.output:
             print(f"Filtering to {np.sum(idx)}/{len(idx)} SNPs with GP data (on target iids)")   
         if np.mean(idx)<1:  # Missing Data detected
             print(f"Attention: Some data in GP field is missing. Ideally, all GP entries are set.")   
         if np.mean(idx)<0.8:  # Less than 80 percent of data there
-            raise RuntimeWarning(f"Too much data missing: {np.sum(idx)}/{len(idx)} SNPs are NULL for GP")
+            print(f"Too much data missing: {np.sum(idx)}/{len(idx)} SNPs have GP ({np.mean(idx)*100}% there)")
             
-        return hts[:,idx], p[idx], m[idx]
+        return hts[:,idx], p[idx], m[idx], bp[idx]
     
     def load_all_data(self, **kwargs):
         """ Return haplotype likelihoods [n*2,l] for anc. allele.
         along first axis: 2*i, 2*(i+1) haplotype of ind i
         derived allele frequencies [l]
-        map in Morgan [l]"""
+        map in Morgan [l]
+        bp positions [l]
+        """
         path_h5_ch = f"{self.path}{self.ch}.h5"
         with h5py.File(path_h5_ch, "r") as f:
             m = self.return_map(f)            
             idcs = np.array([self.get_individual_idx(f, iid) for iid in self.iids])
             sort = np.argsort(idcs)   # Get the sorting Indices [has to go low to high]
             samples = self.iids[sort] # Get them in sorted order
-            hts = self.get_haplo_prob(f, idcs[sort])
-        
+            hts = self.get_haplo_prob(f, idcs[sort]) # Still does old loading
+            bp = f['variants/POS'][:]
             if len(self.p_col)>0:
                 p = self.get_p_hdf5(f, self.p_col)
             else:
                 p = self.get_p(hts)  # Calculate Mean allele frequency from sample subset
                 
         ### Filter to Valid data
-        hts, p, m = self.filter_valid_data(hts, p, m)
+        hts, p, m, bp = self.filter_valid_data(hts, p, m, bp)
         
         self.check_valid_data(hts, p, m)
-        return hts, p, m, samples
+        return hts, p, m, bp, samples
     
     def get_p(self, htsl):
         """Get Allele frequency from haplotype probabilities.
         Return array of derived allele freqs [l]"""
         p_anc = np.mean(htsl, axis=0) # Take the expected AF of ancestral.
         p_der = 1 - p_anc             # Get the derived allele frequency
         return p_der
@@ -245,76 +251,92 @@
     ch = 3   # Which chromosome to load
     min_error = 1e-3  # Minimum Probability of genotyping error  
     pph_error = 1e-2 #1e-3 # Point Phase Error
     p_col = "" # The hdf5 column with der. all freqs. If given, use the field
     # If "default" use p=0.5 everywhere
     # default value for p_col in my hdf5s: variants/AF_ALL
     
-    def get_haplo_prob(self, f, idcs):
+    def get_haplo_prob(self, f, idcs, ploidy=2):
         """Get haploid ancestral probability for n individuals 
         Return [n,l,2] array. Calculated from GP and GT
-        in the proper way."""
-        
+        in the proper way.
+        ploidy: it can be either an integer or an array of integers
+        when it's an integer, it must be either 1 or 2 and then we assume that all individuals have the same ploidy
+        when it's an array, it must have the same length as idcs and then it specifies the ploidy of each individual
+        """
+            
         gt = f["calldata/GT"][:,idcs,:] ### Get l, n, 2 array of gt
         l,n,_ = np.shape(gt) # Get the nr loci
         gp = f["calldata/GP"][:,idcs,:] ### Get l, n, 3 array of gp
         
-        ### The homozygotes
-        g00 = gp[:,:,0]  # homo 00 prob.
-        ### Heterozygote prob
-        gp1 = gp[:,:,1]
-        ## g11 not needed
-        
-        ### The max GT probabilities
-        g01 = gp1[:,:] * (gt[:,:,0]==0) * (gt[:,:,1]==1) # het 01 prob.
-        g10 = gp1[:,:] * (gt[:,:,0]==1) * (gt[:,:,1]==0) # het 10 prob.
-        
-        ### The default probability from the non-max GT ones
-        # Assume it is split up 50/50 between 01 10 states
-        idx = (gt[:,:,0]==0) * (gt[:,:,1]==0)
-        g01[idx] = gp1[idx]/2
-        g10[idx] = gp1[idx]/2
-        
-        idx = (gt[:,:,0]==1) * (gt[:,:,1]==1)
-        g01[idx] = gp1[idx]/2
-        g10[idx] = gp1[idx]/2
-        ### The added probability from the non-max GT ones
-        
-        # Add point phasing error  here (swap g01 and g10 with prob. x)
-        g01t = g01 * (1 - self.pph_error) + g10 * self.pph_error
-        g10t = g10 * (1 - self.pph_error) + g01 * self.pph_error
-        
-        h1 = np.zeros((l,n,2), dtype=np.float64)
-        h1[:,:,0] = g00 + g01t 
-        h1[:,:,1] = g00 + g10t
+        if isinstance(ploidy, int) and ploidy == 1:
+            # for haploid samples, the entry in h1[:,:,1] will never be used, so it's fine to leave it as all zeros
+            h1 = np.zeros((l,n,2), dtype=np.float64)
+            h1[:,:,0] = gp[:,:,0]
+        else:
+            # ploidy is either an integer or an array of integers
+            if isinstance(ploidy, int):
+                assert ploidy == 2
+                ploidy = 2*np.ones(n, dtype=np.int64)
+            ### The homozygotes
+            g00 = gp[:,:,0]  # homo 00 prob.
+            ### Heterozygote prob
+            gp1 = gp[:,:,1]
+            # set the het prob for haploid samples to be 0
+            # for haploid samples the gp[:,:,1] actually encodes g11
+            gp1[:, ploidy == 1] = 0.0 
+            ## g11 not needed
+        
+            ### The max GT probabilities
+            g01 = gp1[:,:] * (gt[:,:,0]==0) * (gt[:,:,1]==1) # het 01 prob.
+            g10 = gp1[:,:] * (gt[:,:,0]==1) * (gt[:,:,1]==0) # het 10 prob.
+        
+            ### The default probability from the non-max GT ones
+            # Assume it is split up 50/50 between 01 10 states
+            idx = (gt[:,:,0]==0) * (gt[:,:,1]==0)
+            g01[idx] = gp1[idx]/2
+            g10[idx] = gp1[idx]/2
+        
+            idx = (gt[:,:,0]==1) * (gt[:,:,1]==1)
+            g01[idx] = gp1[idx]/2
+            g10[idx] = gp1[idx]/2
+            ### The added probability from the non-max GT ones
+        
+            # Add point phasing error  here (swap g01 and g10 with prob. x)
+            #g01t = g01 * (1 - self.pph_error) + g10 * self.pph_error
+            #g10t = g10 * (1 - self.pph_error) + g01 * self.pph_error
+        
+            h1 = np.zeros((l,n,2), dtype=np.float64)
+            h1[:,:,0] = g00 + g01
+            h1[:,:,1] = g00 + g10
         
         h1 = np.swapaxes(h1, 0, 1) #  l,n,2->n,l,2
         h1 = np.swapaxes(h1, 1, 2) # -> n,2,l
         h1 = h1.reshape((2*n,l))
         
         ### Add minimum error to avoid overly extreme confidence genotypes
         h1 = np.maximum(h1, self.min_error)
         h1 = np.minimum(h1, 1-self.min_error)
         
         if self.output:
-            print(f"Min. Error added: {self.min_error}")
-            print(f"Phase. Error added: {self.pph_error}")
+            print(f"Thresholding GP at {1 - self.min_error}")
+            #print(f"Phase. Error added: {self.pph_error}")
         
         return h1
     
 ###############################    
 ###############################
 ### Factory Method
     
 def load_loaddata(l_model="simulated", path="", **kwargs):
     """Factory method to return the right loading Model"""
     if l_model == "simulated":
         l_obj = LoadSimulated(path=path, **kwargs)
     elif l_model == "hdf5double":  # use overall allele frequency
         l_obj = LoadHDF5(path=path, **kwargs)
-    elif l_model == "hdf5":
+    elif l_model == "hdf5": # Original model, for legacy reasons
         l_obj = LoadHDF5Multi(path=path, **kwargs)
     elif l_model == "h5":  # Latest model, as described in paper.
         l_obj = LoadH5Multi2(path=path, **kwargs)
     else:
         raise NotImplementedError("Loading Model not found!")
     return l_obj
```

### Comparing `ancIBD-0.5/ancIBD/main.py` & `ancIBD-0.6/ancIBD/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -61,28 +61,28 @@
         ### pass on output parameter
         for o in [self.l_obj, self.t_obj, self.e_obj, self.p_obj]:
             o.set_params(output=self.output)
     
     
     def run_fwd_bwd(self, full=True):
         """Run Forward Backward algorithm."""
-        htsl, p, r_vec, _ =  self.l_obj.load_all_data()
+        htsl, p, r_vec, bp, samples =  self.l_obj.load_all_data()
         e_mat = self.e_obj.give_emission_matrix(htsl, p)
         t_mat = self.t_obj.full_transition_matrix(r_vec, n=4, submat33=self.submat33)
         
         if full:
             post, fwd, bwd, tot_ll = self.fwd_bwd(e_mat, t_mat, in_val = self.in_val, 
                                                   full=full, output=self.output)
-            self.p_obj.call_roh(r_vec, post)
-            return post, r_vec, fwd, bwd, tot_ll
+            #self.p_obj.call_roh(r_vec, post)
+            return post, r_vec, bp, fwd, bwd, tot_ll
         else:
             post = self.fwd_bwd(e_mat, t_mat, in_val = self.in_val, 
                                 full=full, output=self.output)
-            self.p_obj.call_roh(r_vec, post)
-            return post, r_vec  
+            #self.p_obj.call_roh(r_vec, post)
+            return post, r_vec, bp  
     
     ##################################################
     ### Run FWD-BWD timed [LEGACY code]
     
     def run_fwd_bwd_timed(self, full=True):
         """Run Forward Backward algorithm.
         Legacy: Timed version."""
```

### Comparing `ancIBD-0.5/ancIBD/plot/plot_df.py` & `ancIBD-0.6/ancIBD/plot/plot_df.py`

 * *Files identical despite different names*

### Comparing `ancIBD-0.5/ancIBD/plot/plot_karyotype.py` & `ancIBD-0.6/ancIBD/plot/plot_karyotype.py`

 * *Files identical despite different names*

### Comparing `ancIBD-0.5/ancIBD/plot/plot_opphomos.py` & `ancIBD-0.6/ancIBD/plot/plot_opphomos.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,41 +16,52 @@
     """Return opposing homozygotes"""
     o1 = (g1 == 0) & (g2 == 2)
     o2 = (g1 == 2) & (g2 == 0)
     return (o1 | o2)
 
 def plot_hets(map_het=[], het=[], ax=None, het_c="slateblue", c_roh="seagreen", 
               figsize=(14,2), cm_lim=[], ylim=[-0.1, 1.1], fs = 12,
-              alpha=0.3, ms=1, lw = 12, title="", min_cm=0, xtickl=True,
+              alpha=0.3, ms=1, lw = 12, title="", min_cm=0, xtickl=True, df_ibd=None,
               xlabel="centimorgan", ylabel = f"Opp. Homozygote (y/n)", 
               plot=True, savepath=""):
     """Plot Heterozygotes against genenetic map,
     plus ROH calls.
     lw: Linewidth of ROH""" 
     if ax==None:
         plt.figure(figsize=figsize)
         ax = plt.gca()
     ax.plot(map_het*100, (het * 1.1 - 0.05), "o", ms=ms, alpha=alpha, zorder=0, color=het_c)
     ax.set_xlabel(xlabel, fontsize=fs)
     if not xtickl:
         ax.set_xticklabels([])
-    ax.set_ylim(ylim)
+    #ax.set_ylim(ylim)
     
     ax2 = ax.twinx()
     ax2.set_ylim(ax.get_ylim())
     ax2.set_yticks(np.array([1,0]) * 1.1 - 0.05)
     ax2.set_yticklabels([])
     ax.set_yticklabels([])
     ax2.set_ylabel(ylabel, fontsize=fs*0.8, color=het_c, rotation=270, labelpad=fs)
     
     if len(cm_lim)==2:
         ax.set_xlim(cm_lim)
         
     if len(title)>0:
         ax.set_title(title, fontsize=fs)
+    
+    if df_ibd is not None:
+        print(f'df_ibd is not , found {len(df_ibd)} IBD segments')
+        y_ibd = 1.2
+        c_ibd = 'slateblue'
+        lw_ibd = 10
+        ax.hlines(y=[y_ibd]*len(df_ibd), xmin=100 * df_ibd["StartM"], xmax= 100 * df_ibd["EndM"], 
+                        colors=c_ibd, linewidth=lw_ibd)
+        ax.set_ylim([-0.1, 1.27])
+    else:
+        ax.set_ylim(ylim)
         
     if len(savepath)>0:
         plt.savefig(savepath, bbox_inches = 'tight', pad_inches = 0, dpi=300)
         print(f"Saved figure to: {savepath}")
         #plt.savefig(folder + "posterior_cm.png", bbox_inches = 'tight', pad_inches = 0, dpi=300)
     
     if plot:
@@ -65,17 +76,17 @@
     g1, g2, m = get_genos_pairs(f, sample1=iids[0], sample2=iids[1], 
                                 cutoff=cutoff, output=output, exact=exact)
     o_homos = opp_homos(g1, g2)
     plot_hets(m, o_homos, title=f"{iids[0]} - {iids[1]}, Chromosome {ch}, Opposing Homozygotes", ms=ms,
               cm_lim=cm_lim, savepath=savepath) # ./figs/principle_proof/siblings.png
     
 def plot_identical_gts(path_h5 = f"/n/groups/reich/hringbauer/hapsburg_runs/data/data_eirini/h5/all_ch", ch = 16,
-                  iids = ["MYG001.A0101", "MYG006.A0101"], cutoff=0.99, output=True, exact=True,
+                  iids = ["MYG001.A0101", "MYG006.A0101"], df_ibd=None, cutoff=0.99, output=True, exact=True,
                   cm_lim=[], ms=4, savepath=""):
     """Plot pairwise opp. homoyzgotes. Loads f5 data, and calls and plots opp. homos"""
     path_h5 = f"{path_h5}{ch}.h5"
     f = h5py.File(path_h5, "r") # Load for Sanity Check. See below!
     g1, g2, m = get_genos_pairs(f, sample1=iids[0], sample2=iids[1], 
                                 cutoff=cutoff, output=output, exact=exact)
-    diff = (g1!=g2)
+    diff = (g1 != g2)
     plot_hets(m, diff, title=f"{iids[0]} - {iids[1]}, Chromosome {ch}, Different Diploid Genotyeps", ms=ms,
-              cm_lim=cm_lim, ylabel = f"Diff. Genotypes (y/n)", savepath=savepath) # ./figs/principle_proof/siblings.png
+              cm_lim=cm_lim, ylabel = f"Diff. Genotypes (y/n)", df_ibd=df_ibd, savepath=savepath) # ./figs/principle_proof/siblings.png
```

### Comparing `ancIBD-0.5/ancIBD/plot/plot_posterior.py` & `ancIBD-0.6/ancIBD/plot/plot_posterior.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import matplotlib.pyplot as plt
 from matplotlib import gridspec
 import numpy as np
 import h5py as h5py
 
 from matplotlib import rcParams
-rcParams['font.family'] = 'sans-serif'   # Set the default
-rcParams['font.sans-serif'] = ['Arial']  # Make sure to have the font installed (it is on cluster for Harald)
+#rcParams['font.family'] = 'sans-serif'   # Set the default
+#rcParams['font.sans-serif'] = ['Arial']  # Make sure to have the font installed (it is on cluster for Harald)
 
 def plot_posterior(ax=0, morgan=[], post=[], het=[], het_m=[], 
                    df_ibd=[], df_truth=[], state=0, figsize=(12,3), 
                    xlim=[], ylim=[-0.08,1.27], ylabel="Posterior", xlabel="Position",
                    c="maroon", het_c="gray", c_truth="green", ms=1,
                    lw=3, lw_ibd=10, c_ibd="slateblue", y_ibd=1.2, dpi=400, 
                    fs_l=12, show=True, min_cm=4, title="", savepath=""):
@@ -44,26 +44,27 @@
                         colors=c_ibd, linewidth=lw_ibd)
     if len(df_truth)>0:  # Plot Ground truth dataframe
         ### Plot them
         plt.hlines(y=[1.12]*len(df_truth), xmin=100 * df_truth["IBD_Begin"], 
                    xmax=100 * df_truth["IBD_End"], colors=c_truth, linewidth=lw_ibd)
         
     if len(savepath)>0:
+        plt.gcf().set_facecolor('white')
         plt.savefig(savepath, bbox_inches ='tight', pad_inches = 0, dpi=dpi)
         print(f"Saved to {savepath}")
     if show:
         plt.show()
     else: 
         return ax
     
-def plot_hets(ax, het_m, het, alpha=0.3, ms=1, het_c="slateblue",
+def plot_hets(ax, het_m, het, ypos=1.1, alpha=0.3, ms=1, het_c="slateblue",
               ylabel = "Opp. Homozygotes (no/yes)", fs_l=12, ylim=[]):
     """Plot Heterozygote Markers onto Axis"""
     ax2 = ax.twinx()
-    ax2.plot(het_m*100, (het * 1.1 - 0.05), "o", ms=ms, alpha=alpha, zorder=0, color=het_c)
+    ax2.plot(het_m*100, (het * ypos - 0.05), "o", ms=ms, alpha=alpha, zorder=0, color=het_c)
     ax2.set_yticks([-0.05, 1.05])
     ax2.set_yticklabels([])
     ax2.set_ylabel(ylabel, fontsize=fs_l, color=het_c)
     if len(ylim)>0:
         ax2.set_ylim(ylim)
     
 ########################################################
@@ -105,8 +106,67 @@
     
 def get_map(path_h5= "./data/hdf5/1240k_v43/ch", ch=3, 
             col_map="variants/MAP"):
     """Get Map position in Morgan"""
     path_load = f"{path_h5}{ch}.h5"
     f = h5py.File(path_load, "r") # Load for Sanity Check. See below!
     m = f[col_map][:]
-    return m
+    return m
+
+
+def plot_posterior_IBD2(ax=0, morgan=[], post=[], het=[], het_m=[], idengt=[], idengt_m=[],
+                   df_ibd=[], df_truth=[], state=0, figsize=(12,3), 
+                   xlim=[], ylim=[-0.08,1.37], ylabel="Posterior", xlabel="Position",
+                   c="maroon", het_c="gray", c_truth="green", ms=1,
+                   lw=0.5, lw_ibd=10, c_ibd="slateblue", y_ibd=1.3, dpi=400, 
+                   fs_l=12, show=True, min_cm1=4, min_cm2=2, title="", savepath=""):
+    """Plot Posterior [k,l] array. If morgan given, plot in centimorgan.
+    Can then also plot hapROH formatted IBD blocks (df_ibd).
+    And plot ground truth hapROH formatted IBD blocks (df_truth).
+    If het is given [array boolean], plot het using het_m coordinates"""
+    if ax==0:
+        plt.figure(figsize=figsize)
+        ax=plt.gca()
+    if len(morgan)==0:
+        morgan = np.arange(np.shape(post)[1])
+    #ax.plot(morgan*100, post[state,:], color=c, lw=lw)
+    ax.plot(morgan*100, 1 - np.sum(post[-2:,:], axis=0), color='orangered', lw=lw)
+    ax.set_yticks([0., 0.2, 0.4, 0.6, 0.8, 1.0])
+    ### Do optional plotting
+    # Hets
+    if len(xlabel)>0:
+        ax.set_xlabel(xlabel, fontsize=fs_l)
+    if len(ylabel)>0:
+        ax.set_ylabel(ylabel, fontsize=fs_l)
+    if len(xlim)>0:
+        ax.set_xlim(xlim)
+    if len(ylim)>0:
+        ax.set_ylim(ylim)
+    if len(het)>0:
+        plot_hets(ax, het_m, het, ms=ms, het_c=het_c, fs_l=fs_l, ylim=ylim, ylabel="")
+    if len(idengt)>0:
+        plot_hets(ax, idengt_m, idengt, ms=ms, het_c=het_c, fs_l=fs_l, ylim=ylim, ypos=1.2, ylabel="Opp. Hom. / Diff. GT (n/y)")
+    if len(title)>0:
+        ax.set_title(title, fontsize=fs_l)
+    if len(df_ibd)>0:
+        df_ibd1 = df_ibd[df_ibd['segment_type']=='IBD1']
+        df_ibd1 = df_ibd1[df_ibd1["lengthM"] > min_cm1/100]  # Filter out long enough calls
+        ax.hlines(y=[y_ibd]*len(df_ibd1), xmin=100 * df_ibd1["StartM"], xmax= 100 * df_ibd1["EndM"], 
+                        colors='slateblue', linewidth=lw_ibd)
+        
+        df_ibd2 = df_ibd[df_ibd['segment_type']=='IBD2']
+        df_ibd2 = df_ibd2[df_ibd2["lengthM"] > min_cm2/100]
+        ax.hlines(y=[y_ibd]*len(df_ibd2), xmin=100 * df_ibd2["StartM"], xmax= 100 * df_ibd2["EndM"], 
+                        colors='maroon', linewidth=lw_ibd)
+    if len(df_truth)>0:  # Plot Ground truth dataframe
+        ### Plot them
+        plt.hlines(y=[1.12]*len(df_truth), xmin=100 * df_truth["IBD_Begin"], 
+                   xmax=100 * df_truth["IBD_End"], colors=c_truth, linewidth=lw_ibd)
+        
+    if len(savepath)>0:
+        plt.savefig(savepath, bbox_inches ='tight', pad_inches = 0, dpi=dpi)
+        print(f"Saved to {savepath}")
+    if show:
+        plt.show()
+    else: 
+        return ax
+
```

### Comparing `ancIBD-0.5/ancIBD/run_ancIBD.py` & `ancIBD-0.6/ancIBD/run_ancIBDX.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,36 +1,48 @@
-# run ancIBD given an input vcf file
+# run ancIBDX given an input vcf file
 
 import argparse
-from ancIBD.run import hapBLOCK_chroms
+from ancIBD.run import hapBLOCK_chroms_mixedPloidy
 from ancIBD.IO.prepare_h5 import vcf_to_1240K_hdf
+from ancIBD.IO.ind_ibd import create_ind_ibd_df
 from pathlib import Path
 import h5py
 import os
-
+import warnings
 
 def main():
-    parser = argparse.ArgumentParser(description='Run ancIBD.')
+    parser = argparse.ArgumentParser(description='Run ancIBD (on Autosomes).')
     parser.add_argument('--vcf', action="store", dest="vcf", type=str, required=False,
                         help="path to the imputed vcf file")
     parser.add_argument('--h5', action="store", dest="h5", type=str, required=False,
                         help="path to hdf5 file. If specified, ancIBD will skip the vcf to hdf5 conversion step. \
                         Only one of --vcf and --h5 should be specified.\
                         But please make sure that the hdf5 file has suffix ch{chromosome number}.h5 (e.g, test.ch20.h5).")
-    parser.add_argument('--ch', action="store", dest="ch", type=int, required=True, help='chromosome number (1-22).')
+    parser.add_argument('--ch', action="store", dest="ch", type=str, required=False, default='X', help='chromosome name, default by X.')
     parser.add_argument('--marker_path', action="store", dest="marker_path", type=str, required=False, help='path to the marker file')
     parser.add_argument('--map_path', action="store", dest="map_path", type=str, required=False, help='path to the map file')
     parser.add_argument('--af_path', action="store", dest="af_path", type=str, required=False, default="", help='path to the allele frequency file (optional)')
     parser.add_argument('--af_column', action='store', dest='af_column', type=str, required=False, default='', help='column name of the allele frequency in the hdf5. For example, "variants/AF_ALL" or "variants/AF_SAMPLE".')
     parser.add_argument('--out', action="store", dest="out", type=str, required=False, help='output folder to store IBD results and the intermediary .hdf5 file. If not specified, the results will be stored in the same folder as the input vcf file.')
     parser.add_argument('--prefix', action="store", dest="prefix", type=str, required=False,
                         help="prefix of output file. If not specified, the prefix will be the same as the input vcf")
+    parser.add_argument('--ibd-in', action="store", dest="ibd_in", type=float, required=False, default=1, help="IBD in rate. Default is 1.")
+    parser.add_argument('--ibd-out', action="store", dest="ibd_out", type=float, required=False, default=10, help="IBD out rate. Default is 10.")
+    parser.add_argument('--ibd-jump', action="store", dest="ibd_jump", type=float, required=False, default=400, help="IBD jump rate. Default is 400.")
     parser.add_argument('--min', action="store", dest="min", type=float, required=False, default=8, help="minimum length of IBD segment in cM. Default is 8.")
-    parser.add_argument('--iid', action="store", dest="iid", type=str, required=False, help="A list of sample iids to run ancIBD on (each line contains one sample IID). The sample list must match the sample name in the provided vcf file. If unspecified, ancIBD will run on all samples in the vcf file")
+    parser.add_argument('--ploidy', action="store", dest="ploidy", type=str, required=True, default='1', 
+                        help="path to a .txt file listing the ploidy of each sample. \
+                        Each sample takes one line, the first column is sample iid and the second column is the ploidy. \
+                        The two columns can be separted by any white space.\
+                        ancIBD will only run on individuals listed in this file, even if others exist in the vcf/hdf5 file.")
     parser.add_argument('--pair', action="store", dest="pair", type=str, required=False, help="A list of sample pairs to run ancIBD on (each line contains two sample IIDs separated by a whitespace). The sample list must match the sample name in the provided vcf file, and, if --iid is specified, all samples must also appear in the iid file. If unspecified, ancIBD will run on all pairs of samples in the vcf file")
+    parser.add_argument('--mask', action='store', dest='mask', type=str, required=False, default="", help='Mask file to mask out regions for IBD calling.')
+    parser.add_argument('--bin', action="store", dest="bin", type=str, required=False, default='8,12,16,20', help='length bin over which IBD sharing summary statistics for pairs of samples will be calculated. Default is 8,12,16,20.')
+    parser.add_argument('--snpcm', action="store", dest="snpcm", type=int, required=False, default=180, help='minimum number of SNPs per cM. Default is 180.')
+    parser.add_argument('-v', '--verbose', action='store_true', dest='verbose', required=False, help='turn on verbose mode')
     args = parser.parse_args()
 
     if args.vcf is None and args.h5 is None:
         raise ValueError("One of --vcf and --h5 must be specified.")
     elif args.vcf is not None and args.h5 is not None:
         raise ValueError("Only one of --vcf and --h5 should be specified.")
 
@@ -50,55 +62,76 @@
     else:
         # create the output folder if it does not already exist
         if os.path.isdir(oDir) is False:
             # create the output folder and its parental folders if they do not exist
             Path(oDir).mkdir(parents=True)
 
     if args.vcf is not None:
-        path_vcf_1240k = os.path.join(f"{oDir}", f"{prefix}.1240k.vcf")
+        path_vcf_1240k = os.path.join(f"{oDir}", f"{prefix}.1240k.vcf") # temporary vcf file
         path_h5 = os.path.join(f"{oDir}", f"{prefix}.h5")
         col_sample_af = "" if len(args.af_path) > 0 else "AF_SAMPLE"
-        if len(args.af_path) == 0:
-            print("WARNING: allele frequency file not provided. The allele frequency will be calculated from the input vcf file. Make sure you have enough sample size to have good estimates of allele frequencies ")
+        if len(args.af_path) == 0 and len(args.af_column) == 0:
+            print("WARNING: allele frequency file or entries in VCF that stores AF not provided. \
+                The allele frequency will be calculated from the input vcf file. \
+                  Make sure you have enough sample size to have good estimates of allele frequencies ")
             print('The sample allele frequency will be stored in the "variants/AF_SAMPLE" column of the output hdf5 file.')
         vcf_to_1240K_hdf(in_vcf_path = args.vcf,
                  path_vcf = path_vcf_1240k, path_h5 = path_h5,
                  marker_path = args.marker_path,
                  map_path = args.map_path,
                  af_path = args.af_path,
                  col_sample_af = col_sample_af,
                  buffer_size=20000, chunk_width=8, chunk_length=20000,
                  ch=ch)
         os.remove(path_vcf_1240k) # remove intermediary vcf files
     else:
         path_h5 = args.h5
 
-    if args.iid is None:
-        with h5py.File(path_h5, 'r') as f:
-            iids = f['samples'][:].astype('str')
-    else:
-        iids = []
-        with open(args.iid, 'r') as f:
-            for line in f:
-                iids.append(line.strip())
+    with h5py.File(path_h5, 'r') as f:
+        iids = f['samples'][:].astype('str')
+    iids2run = []
+    ploidy = []
+    with open(args.ploidy, 'r') as f:
+        for line in f:
+            iid, p = line.strip().split()
+            if iid in iids:
+                iids2run.append(iid)
+                ploidy.append(int(p))
+            else:
+                warn = f'{iid} in the ploidy file is not in the hdf5 file. It will be ignored...'
+                warnings.warn(warn)
+    assert(len(iids2run) == len(ploidy))
+    # check if all samples in iids are in iids2run
+    for iid in iids:
+        if iid not in iids2run:
+            warn = f'{iid} in the hdf5 file is not in the ploidy file. It will be ignored...'
+            warnings.warn(warn)
     
     run_iids = []
     if not args.pair is None:
         with open(args.pair, 'r') as f:
             for line in f:
                 id1, id2 = line.strip().split()
+                if (not id1 in iids2run) or (not id2 in iids2run):
+                    warn = f'{id1} or {id2} not in the ploidy/hdf5 file. It will be ignored...'
+                    warnings.warn(warn)
+                    continue
                 run_iids.append((id1, id2))
     
     # I set folder_out to an empty string because I save the output file separately in the code below
     p_col = args.af_column
     if len(p_col) == 0:
         p_col = 'variants/AF_ALL' if len(args.af_path) > 0 else 'variants/AF_SAMPLE'
-    df_ibd = hapBLOCK_chroms(folder_in=path_h5[:2+path_h5.rfind('ch')],
-                             iids=iids, run_iids=run_iids,
+    df_ibd = hapBLOCK_chroms_mixedPloidy(folder_in=path_h5[:2+path_h5.rfind('ch')],
+                             iids=iids2run, ploidy=ploidy, run_iids=run_iids,
                              ch=ch, folder_out="",
-                             output=False, prefix_out='', logfile=False,
-                             l_model='h5', e_model='haploid_gl', h_model='FiveStateScaled', t_model='standard', p_col=p_col,
-                             ibd_in=1, ibd_out=10, ibd_jump=400,
-                             min_cm=args.min, cutoff_post=0.99, max_gap=0.0075)
-    
+                             output=args.verbose, prefix_out='', logfile=False, p_col=p_col,
+                             ibd_in=args.ibd_in, ibd_out=args.ibd_out, ibd_jump=args.ibd_jump,
+                             min_cm=args.min, cutoff_post=0.99, max_gap=0.0075,
+                             mask=args.mask)
     df_ibd.to_csv(os.path.join(f"{oDir}", f"{prefix}.tsv"), sep='\t', index=False)
+    # create a IBD summary statistics file
+    min_cms = [float(l) for l in args.bin.split(',')]
+    create_ind_ibd_df(ibd_data = os.path.join(oDir, f"{prefix}.tsv"),
+                      min_cms = min_cms, snp_cm = args.snpcm, min_cm = min_cms[0], sort_col = 0,
+                      savepath = os.path.join(oDir, "ibd_ind.tsv"))
```

### Comparing `ancIBD-0.5/ancIBD/transition.py` & `ancIBD-0.6/ancIBD/transition.py`

 * *Files 18% similar despite different names*

```diff
@@ -207,28 +207,153 @@
     # We might want to consider a slower rate of jumping into IBD2 than jumping into IBD1, but let's leave it to be the same for now
     ibd_in = 1    # The rate of jumping into IBD copying state
     ibd_out = 20     # The rate of jumping out of IBD state
     ibd_jump = 500     # The rate of jumping within IBD to other haplotype pair
     #ibd_switch = 20  # the rate of jumping between IBD1 and IBD2 state, actually let's leave it the same as ibd_out for now
     
 
+    def exponentiate_r(self, rates, rec_v):
+        """Calculates exponentiation of the rates matrix with rec_v
+        rates: 2D Matrix of transitions
+        rec_v: Array of length l"""
+        eva, evec = np.linalg.eig(rates)  # Do the Eigenvalue Decomposition
+        assert(np.max(eva) <= 1)   # Sanity Check whether rate Matrix
+        evec_r = np.linalg.inv(evec)    # Do the Inversion
+        # Create vector of the exponentiated diagonals
+        d = np.exp(rec_v[:, None] * eva)
+        # Use some Einstein Sum Convention Fun (C Speed):
+        res = np.einsum('...ik, ...k, ...kj ->...ij', evec, d, evec_r)
+        # Make sure that all transition rates are valuable
+        res[res<0] = 0.0 # numerical issues cause some entries to be very very small negative values, so we just set them to 0
+        assert(0 <= np.min(res))
+        return res
+
     def calc_transition_rate(self):
         """Return Transition Rate Matrix [k,k] to exponate.
         n: Number of symetric IBD states. Usually four (2x2 copying possibilities)
         submat33: Whether to only fill in the first 3 states """
         t_mat = -np.ones((7, 7))
 
         t_mat[1:5, 0] = self.ibd_out  # The rate of jumping out IBD1 to nonIBD
-        t_mat[5:7, 0] = 1e-6 # the rate of jumping out IBD2 to nonIBD
+        t_mat[5:7, 0] = 0 # the rate of jumping out IBD2 to nonIBD
         t_mat[0, 1:5] = self.ibd_in / 4  # Jumping into any IBD1 State from IBD0
-        t_mat[0, 5:7] = 1e-6 # jumping into any IBD2 state from IBD0
+        t_mat[0, 5:7] = 0 # jumping into any IBD2 state from IBD0
         t_mat[1:5, 1:5] = self.ibd_jump / 4  # Jumping between IBD1 State
         t_mat[5:7, 5:7] = self.ibd_jump / 2  # Jumping between IBD2 State
-        t_mat[1:5, 5:7] = 0.01 # jumping from IBD1 to IBD2 State
-        t_mat[5:7, 1:5] = 200 # jumping from IBD2 to IBD1 state
+        t_mat[1:5, 5:7] = self.ibd_in / 2 # jumping from IBD1 to IBD2 State
+        t_mat[5:7, 1:5] = self.ibd_in / 4 # jumping from IBD2 to IBD1 state
+
+        # Do the Diagonal (do the usual model - for inf. substract 1)
+        di = np.diag_indices(np.shape(t_mat)[0])
+        t_mat[di] = -np.sum(t_mat, axis=1) + np.diag(t_mat)
+
+        # Sanity Check if everything was filled correctly
+        assert(np.allclose(np.sum(t_mat, axis=1), 0))
+        self.trans_mat = t_mat
+        return t_mat
+    
+    def full_transition_matrix(self, r_vec, t=[], n=4, submat33=True):
+        """Compute and return the full transition Matrix.
+        Calculates the first 3 states (not more needed by symmetry)
+        t full Transition Matrix [k,k]. NO LOG STATE. If not given caluclate
+        r_vec Map Length of Jumps [l] in Morgan
+        n: Number of symmetric, non-background states, not used by this method, keeping it here to just keep function signature the same as that of the 5state HMM.
+        submat33: also not used by this function, keeping it here just to keep consistency with the 5 state hmm
+        Note: this is the only function called by outside code
+        """
+        ### infinitesimal rate
+        if len(t) == 0:
+            t = self.calc_transition_rate()
+            
+        ### Full matrix
+        r_vec = self.rmap_to_gaps(r_map=r_vec)
+        t_mat = self.exponentiate_r(t, r_vec)
+
+        # Normalize to transition rate into non-collapsed state
+        return t_mat
+
+class TwoStateTransitions(FiveStateTransitions):
+    ibd_in = 1    # The rate of jumping into IBD copying state
+    ibd_out = 20     # The rate of jumping out of IBD state
+    def calc_transition_rate(self):
+        """Return Transition Rate Matrix [k,k] to exponate.
+        n: Number of symetric IBD states. Usually four (2x2 copying possibilities)
+        submat33: Whether to only fill in the first 3 states """
+        t_mat = -np.ones((2, 2))
+        t_mat[0, 1] = self.ibd_in
+        t_mat[1, 0] = self.ibd_out
+
+        # Do the Diagonal (do the usual model - for inf. substract 1)
+        di = np.diag_indices(np.shape(t_mat)[0])
+        t_mat[di] = -np.sum(t_mat, axis=1) + np.diag(t_mat)
+
+        # Sanity Check if everything was filled correctly
+        assert(np.allclose(np.sum(t_mat, axis=1), 0))
+        self.trans_mat = t_mat
+        return t_mat
+    
+    def full_transition_matrix(self, r_vec, t=[], n=4, submat33=True):
+        """
+        The last two arguments n and submat33 are not used. They are retained just for compatibility with the one Harald wrote.
+        """
+        if len(t) == 0:
+            t = self.calc_transition_rate()
+            
+        ### Full matrix
+        r_vec = self.rmap_to_gaps(r_map=r_vec)
+        t_mat = self.exponentiate_r(t, r_vec)
+        return t_mat
+    
+class ThreeStateTransitions(FiveStateTransitions):
+    ibd_in = 1    # The rate of jumping into IBD copying state
+    ibd_out = 20     # The rate of jumping out of IBD state
+    ibd_jump = 400     # The rate of jumping within IBD to other haplotype pair
+    def calc_transition_rate(self):
+        """Return Transition Rate Matrix [k,k] to exponate.
+        n: Number of symetric IBD states. Usually four (2x2 copying possibilities)
+        submat33: Whether to only fill in the first 3 states """
+        t_mat = -np.ones((3, 3))
+        t_mat[0, 1:] = self.ibd_in/2
+        t_mat[1:, 0] = self.ibd_out
+        t_mat[1:, 1:] = self.ibd_jump/2
+
+        # Do the Diagonal (do the usual model - for inf. substract 1)
+        di = np.diag_indices(np.shape(t_mat)[0])
+        t_mat[di] = -np.sum(t_mat, axis=1) + np.diag(t_mat)
+
+        # Sanity Check if everything was filled correctly
+        assert(np.allclose(np.sum(t_mat, axis=1), 0))
+        self.trans_mat = t_mat
+        return t_mat
+    
+    def full_transition_matrix(self, r_vec, t=[], n=4, submat33=True):
+        """
+        The last two arguments n and submat33 are not used. They are retained just for compatibility with the one Harald wrote.
+        """
+        if len(t) == 0:
+            t = self.calc_transition_rate()
+            
+        ### Full matrix
+        r_vec = self.rmap_to_gaps(r_map=r_vec)
+        t_mat = self.exponentiate_r(t, r_vec)
+        return t_mat
+    
+class FiveStatGeneric(FiveStateTransitions):
+    """A transition model for detecting IBD. Same as FiveStateTransitions, except that the 3x3 speed-up is not implemented here."""
+    ibd_in = 1
+    ibd_out = 20
+    ibd_jump = 400 # IBD jump rate for ancient haplotypes
+
+    def calc_transition_rate(self):
+        """Return Transition Rate Matrix [k,k] to exponate. """
+        t_mat = -np.ones((5, 5))
+
+        t_mat[1:5, 0] = self.ibd_out  # The rate of jumping out IBD1 to nonIBD
+        t_mat[0, 1:5] = self.ibd_in / 4  # Jumping into any IBD1 State from IBD0
+        t_mat[1:5, 1:5] = self.ibd_jump / 4  # Jumping between IBD1 State
 
         # Do the Diagonal (do the usual model - for inf. substract 1)
         di = np.diag_indices(np.shape(t_mat)[0])
         t_mat[di] = -np.sum(t_mat, axis=1) + np.diag(t_mat)
 
         # Sanity Check if everything was filled correctly
         assert(np.allclose(np.sum(t_mat, axis=1), 0))
@@ -263,10 +388,16 @@
     """Load the Transition Model"""
     if t_model == "standard":
         t_obj = FiveStateTransitions()
     elif t_model == "asymmetric":
         t_obj = FiveStateAsymmetric()
     elif t_model == 'IBD2':
         t_obj = SevenStateTransitions()
+    elif t_model == 'twoHaploid':
+        t_obj = TwoStateTransitions()
+    elif t_model == "hapVSdiploid":
+        t_obj = ThreeStateTransitions()
+    elif t_model == "fiveStateGeneric":
+        t_obj = FiveStatGeneric()
     else:
         raise NotImplementedError("Transition Model not found!")
     return t_obj
```

### Comparing `ancIBD-0.5/ancIBD.egg-info/PKG-INFO` & `ancIBD-0.6/ancIBD.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ancIBD
-Version: 0.5
+Version: 0.6
 Summary: Identify IBD segments between pairs of individuals in ancient human DNA data
 Home-page: https://github.com/hringbauer/ancIBD
 Author: Harald Ringbauer
 Author-email: harald_ringbauer@eva.mpg.de
 License: UNKNOWN
 Description: # ancIBD
         This Python software package screens ancient human DNA for long IBD blocks (Identity by Descent segments) shared between pairs of individuals.
```

### Comparing `ancIBD-0.5/ancIBD.egg-info/SOURCES.txt` & `ancIBD-0.6/ancIBD.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 ancIBD/emission.py
 ancIBD/hmm.py
 ancIBD/loaddata.py
 ancIBD/main.py
 ancIBD/postprocessing.py
 ancIBD/run.py
 ancIBD/run_ancIBD.py
+ancIBD/run_ancIBDX.py
 ancIBD/transition.py
 ancIBD.egg-info/PKG-INFO
 ancIBD.egg-info/SOURCES.txt
 ancIBD.egg-info/dependency_links.txt
 ancIBD.egg-info/entry_points.txt
 ancIBD.egg-info/requires.txt
 ancIBD.egg-info/top_level.txt
```

### Comparing `ancIBD-0.5/setup.py` & `ancIBD-0.6/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     extensions = cythonize(extensions)
   
 with open("README.md", "r") as fh:
     long_description = fh.read()
     
 setup(
     name="ancIBD",
-    version="0.5",  # a means alpha
+    version="0.6",  # a means alpha
     author="Harald Ringbauer",
     author_email="harald_ringbauer@eva.mpg.de",
     description="Identify IBD segments between pairs of individuals in ancient human DNA data",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/hringbauer/ancIBD",
     packages=find_packages(),
@@ -38,11 +38,12 @@
     ],
     python_requires='>=3.6',
     install_requires=['numpy', 'pandas', 'scipy', 'h5py', 
                       'psutil', 'cython', 'matplotlib', 'pysam', 'scikit-allel'],
     entry_points ={
             'console_scripts': [
                 'ancIBD-summary = ancIBD.ancIBD_summary:main',
-                'ancIBD-run = ancIBD.run_ancIBD:main'
+                'ancIBD-run = ancIBD.run_ancIBD:main',
+                'ancIBDX = ancIBD.run_ancIBDX:main',
             ]
         },
 )
```

