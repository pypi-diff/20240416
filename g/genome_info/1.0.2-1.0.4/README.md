# Comparing `tmp/genome_info-1.0.2.tar.gz` & `tmp/genome_info-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "genome_info-1.0.2.tar", max compression
+gzip compressed data, was "genome_info-1.0.4.tar", max compression
```

## Comparing `genome_info-1.0.2.tar` & `genome_info-1.0.4.tar`

### file list

```diff
@@ -1,30 +1,30 @@
--rwxr-xr-x   0        0        0    17895 2019-08-12 18:05:36.000000 genome_info-1.0.2/LICENSE.md
--rwxr-xr-x   0        0        0     1009 2023-05-08 14:48:14.194704 genome_info-1.0.2/README.md
--rw-r--r--   0        0        0     3023 2023-11-03 19:01:00.908409 genome_info-1.0.2/build.py
--rw-r--r--   0        0        0     8196 2023-11-21 03:28:25.710728 genome_info-1.0.2/genome_info/.DS_Store
--rwxr-xr-x   0        0        0      299 2023-11-21 03:31:10.149604 genome_info-1.0.2/genome_info/__init__.py
--rw-r--r--   0        0        0     9923 2023-11-21 03:29:16.392651 genome_info-1.0.2/genome_info/core/info.py
--rw-r--r--   0        0        0     3843 2023-08-30 17:43:27.311750 genome_info-1.0.2/genome_info/core/utilities.py
--rw-r--r--   0        0        0     6148 2023-11-03 15:52:30.106010 genome_info-1.0.2/genome_info/genomes/.DS_Store
--rw-r--r--   0        0        0     4049 2023-08-29 20:47:40.469608 genome_info-1.0.2/genome_info/genomes/__pycache__/genomes.cpython-311.pyc
--rw-r--r--   0        0        0     3300 2023-08-29 20:41:49.397034 genome_info-1.0.2/genome_info/genomes/__pycache__/readers.cpython-311.pyc
--rw-r--r--   0        0        0     6148 2023-10-31 17:50:47.961053 genome_info-1.0.2/genome_info/genomes/base/.DS_Store
--rwxr-xr-x   0        0        0       31 2023-10-31 19:31:42.845166 genome_info-1.0.2/genome_info/genomes/base/__init__.py
--rw-r--r--   0        0        0     6148 2023-10-31 17:32:14.049726 genome_info-1.0.2/genome_info/genomes/data/.DS_Store
--rwxr-xr-x   0        0        0       31 2023-10-31 19:31:42.845166 genome_info-1.0.2/genome_info/genomes/data/__init__.py
--rw-r--r--   0        0        0     4298 2023-08-29 20:53:48.341138 genome_info-1.0.2/genome_info/genomes/download.py
--rw-r--r--   0        0        0     2792 2023-08-29 20:54:58.210255 genome_info-1.0.2/genome_info/genomes/genomes.py
--rw-r--r--   0        0        0     1830 2023-11-01 20:27:24.383790 genome_info-1.0.2/genome_info/genomes/readers.py
--rw-r--r--   0        0        0    22597 2021-12-16 23:34:30.000000 genome_info-1.0.2/genome_info/kmers/2bit.c
--rw-r--r--   0        0        0     7000 2022-07-16 15:37:50.000000 genome_info-1.0.2/genome_info/kmers/2bit.h
--rwxr-xr-x   0        0        0      113 2023-02-10 22:07:44.953713 genome_info-1.0.2/genome_info/kmers/__init__.py
--rw-r--r--   0        0        0      338 2023-04-07 18:12:21.743749 genome_info-1.0.2/genome_info/kmers/__pycache__/__init__.cpython-310.pyc
--rw-r--r--   0        0        0     9639 2023-11-08 15:16:34.796355 genome_info-1.0.2/genome_info/kmers/interval_kmer.c
--rw-r--r--   0        0        0     1567 2023-11-08 02:50:40.129293 genome_info-1.0.2/genome_info/kmers/interval_kmer.h
--rw-r--r--   0        0        0   961865 2023-11-21 03:18:33.588947 genome_info-1.0.2/genome_info/kmers/kmer_reader.c
--rw-r--r--   0        0        0   259832 2023-05-17 13:44:17.886650 genome_info-1.0.2/genome_info/kmers/kmer_reader.cpython-310-darwin.so
--rw-r--r--   0        0        0   277912 2023-11-21 03:18:40.591906 genome_info-1.0.2/genome_info/kmers/kmer_reader.cpython-311-darwin.so
--rw-r--r--   0        0        0     2028 2023-11-08 02:52:47.043725 genome_info-1.0.2/genome_info/kmers/kmer_reader.pxd
--rw-r--r--   0        0        0     2695 2023-11-08 03:03:31.462518 genome_info-1.0.2/genome_info/kmers/kmer_reader.pyx
--rw-r--r--   0        0        0     2228 2023-11-21 03:31:22.044743 genome_info-1.0.2/pyproject.toml
--rw-r--r--   0        0        0     2719 1970-01-01 00:00:00.000000 genome_info-1.0.2/PKG-INFO
+-rwxr-xr-x   0        0        0    17895 2019-08-12 18:05:36.000000 genome_info-1.0.4/LICENSE.md
+-rwxr-xr-x   0        0        0     1009 2023-05-08 14:48:14.194704 genome_info-1.0.4/README.md
+-rw-r--r--   0        0        0     3023 2023-11-03 19:01:00.908409 genome_info-1.0.4/build.py
+-rw-r--r--   0        0        0    10244 2024-03-21 01:47:28.982128 genome_info-1.0.4/genome_info/.DS_Store
+-rwxr-xr-x   0        0        0      299 2024-04-16 03:18:47.427535 genome_info-1.0.4/genome_info/__init__.py
+-rw-r--r--   0        0        0    13284 2023-12-05 18:37:53.635097 genome_info-1.0.4/genome_info/core/info.py
+-rw-r--r--   0        0        0     3843 2023-08-30 17:43:27.311750 genome_info-1.0.4/genome_info/core/utilities.py
+-rw-r--r--   0        0        0     6148 2023-11-03 15:52:30.106010 genome_info-1.0.4/genome_info/genomes/.DS_Store
+-rw-r--r--   0        0        0     4049 2023-08-29 20:47:40.469608 genome_info-1.0.4/genome_info/genomes/__pycache__/genomes.cpython-311.pyc
+-rw-r--r--   0        0        0     3300 2023-08-29 20:41:49.397034 genome_info-1.0.4/genome_info/genomes/__pycache__/readers.cpython-311.pyc
+-rw-r--r--   0        0        0     6148 2023-10-31 17:50:47.961053 genome_info-1.0.4/genome_info/genomes/base/.DS_Store
+-rwxr-xr-x   0        0        0       31 2023-10-31 19:31:42.845166 genome_info-1.0.4/genome_info/genomes/base/__init__.py
+-rw-r--r--   0        0        0     6148 2023-10-31 17:32:14.049726 genome_info-1.0.4/genome_info/genomes/data/.DS_Store
+-rwxr-xr-x   0        0        0       31 2023-10-31 19:31:42.845166 genome_info-1.0.4/genome_info/genomes/data/__init__.py
+-rw-r--r--   0        0        0     4298 2023-08-29 20:53:48.341138 genome_info-1.0.4/genome_info/genomes/download.py
+-rw-r--r--   0        0        0     2792 2023-08-29 20:54:58.210255 genome_info-1.0.4/genome_info/genomes/genomes.py
+-rw-r--r--   0        0        0     1830 2023-11-01 20:27:24.383790 genome_info-1.0.4/genome_info/genomes/readers.py
+-rw-r--r--   0        0        0    22597 2021-12-16 23:34:30.000000 genome_info-1.0.4/genome_info/kmers/2bit.c
+-rw-r--r--   0        0        0     7000 2022-07-16 15:37:50.000000 genome_info-1.0.4/genome_info/kmers/2bit.h
+-rwxr-xr-x   0        0        0      113 2023-02-10 22:07:44.953713 genome_info-1.0.4/genome_info/kmers/__init__.py
+-rw-r--r--   0        0        0      338 2023-04-07 18:12:21.743749 genome_info-1.0.4/genome_info/kmers/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0        0        0    32972 2024-01-24 18:05:02.004099 genome_info-1.0.4/genome_info/kmers/interval_kmer.c
+-rw-r--r--   0        0        0     3144 2024-01-24 19:02:16.135021 genome_info-1.0.4/genome_info/kmers/interval_kmer.h
+-rw-r--r--   0        0        0  1151009 2024-01-10 21:34:51.118273 genome_info-1.0.4/genome_info/kmers/kmer_reader.c
+-rw-r--r--   0        0        0   259832 2023-05-17 13:44:17.886650 genome_info-1.0.4/genome_info/kmers/kmer_reader.cpython-310-darwin.so
+-rw-r--r--   0        0        0   277912 2023-11-21 03:34:29.052722 genome_info-1.0.4/genome_info/kmers/kmer_reader.cpython-311-darwin.so
+-rw-r--r--   0        0        0     3651 2024-01-10 19:54:26.228186 genome_info-1.0.4/genome_info/kmers/kmer_reader.pxd
+-rw-r--r--   0        0        0     9796 2024-01-10 21:33:08.248742 genome_info-1.0.4/genome_info/kmers/kmer_reader.pyx
+-rw-r--r--   0        0        0     2228 2024-04-16 03:19:09.943261 genome_info-1.0.4/pyproject.toml
+-rw-r--r--   0        0        0     2719 1970-01-01 00:00:00.000000 genome_info-1.0.4/PKG-INFO
```

### Comparing `genome_info-1.0.2/LICENSE.md` & `genome_info-1.0.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `genome_info-1.0.2/README.md` & `genome_info-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `genome_info-1.0.2/build.py` & `genome_info-1.0.4/build.py`

 * *Files identical despite different names*

### Comparing `genome_info-1.0.2/genome_info/core/info.py` & `genome_info-1.0.4/genome_info/core/info.py`

 * *Files 22% similar despite different names*

```diff
@@ -161,14 +161,23 @@
         kmers = read_kmers(self.seq_file, intervals, k)
 
         return kmers
 
 
     def load_pfm_scanner(self):
         """
+        Load PFM scanner
+
+        Parameters
+        ----------
+            None
+
+        Returns
+        -------
+            None
         """
 
         import MOODS.parsers
         import MOODS.tools
         import MOODS.scan
 
         # Get PFM scanner
@@ -226,14 +235,34 @@
                         upstream: int = 0,
                         downstream: int = 0,
                         filter_column: str = None,
                         filter_selection: str = None,
                         filter_duplicates: bool = True) -> IntervalFrame:
         """
         Get an item from the info file.
+
+        Parameters
+        ----------
+            key : str
+                Key to get
+            upstream : int
+                Upstream of intervals
+            downstream : int
+                Downstream of intervals
+            filter_column : str
+                Column to filter on
+            filter_selection : str
+                Selection to filter on
+            filter_duplicates : bool
+                Flag to filter duplicates
+
+        Returns
+        -------
+            value : IntervalFrame
+                Intervals
         """
         
         # Read intervals
         value = self.info[key]
         if not isinstance(value, IntervalFrame):
             return None
         
@@ -271,15 +300,15 @@
                 Flag to include repeat
             include_gc : bool
                 Flag to include gc
             include_mappability : bool
                 Flag to include mappability
 
         Returns
-        ----------
+        -------
             bias_record : IntervalFrame
                 Bias for given intervals
         """
 
 
         # Initialize bias records
         bias_record = IntervalFrame(intervals=intervals)
@@ -325,15 +354,15 @@
                 Flag to include repeat
             include_gc : bool
                 Flag to include gc
             include_mappability : bool
                 Flag to include mappability
 
         Returns
-        ----------
+        -------
             bias_record : IntervalFrame
                 Bias for given bin size
         """
 
         # Check previous calculation
         key = "bin_bias_%d" % bin_size
         if key in self.keys:
@@ -359,19 +388,99 @@
 
         Parameters
         ----------
             names : np.ndarray
                 Gene names
         
         Returns
-        ----------
+        -------
             converted_names : np.ndarray
                 Converted gene names
         """
 
         # Read gene names
         gene_names = self["gene_names"]
 
         # Convert gene names
         converted_names = np.array([gene_names[name] for name in names])
 
-        return converted_names
+        return converted_names
+    
+
+    def annotate_regions(self,
+                        intervals: LabeledIntervalArray,
+                        promoter_upstream: int = 1000,
+                        promoter_downstream: int = 1000) -> np.ndarray:
+        """
+        Annotate regions
+
+        Parameters
+        ----------
+            intervals : LabeledIntervalArray
+                Labeled intervals
+            promoter_upstream : int
+                Upstream of promoter
+            promoter_downstream : int
+                Downstream of promoter
+
+        Returns
+        -------
+            anno_record : np.ndarray
+                Annotation for given intervals
+        """
+
+
+        # Initialize bias records
+        anno_record = IntervalFrame(intervals=intervals)
+
+        # Calculate exons
+        regions = self["exon"].merge(1)
+        anno_record.df.loc[:,"exon"] = intervals.percent_coverage(regions.index)
+
+        # Calculate introns
+        regions = self["intron"].merge(1)
+        anno_record.df.loc[:,"intron"] = intervals.percent_coverage(regions.index)
+
+        # Calculate promoters
+        regions = self.get_intervals(key = "tss",
+                                     upstream = promoter_upstream,
+                                     downstream = promoter_downstream,
+                                     filter_column = "gene_type",
+                                     filter_selection = "protein_coding",
+                                     filter_duplicates = True).merge(1)
+        anno_record.df.loc[:,"promoter"] = intervals.percent_coverage(regions.index)
+
+        # Determine calls
+        anno_call = np.repeat("intergenic", anno_record.df.shape[0])
+        anno_call[anno_record.df.loc[:,"intron"].values > 0.5] = "intron"
+        anno_call[anno_record.df.loc[:,"exon"].values > 0.5] = "exon"
+        anno_call[anno_record.df.loc[:,"promoter"].values > 0.5] = "promoter"
+
+        return anno_call
+    
+
+    def filter_blacklist(self,
+                         intervals: IntervalFrame,
+                         blacklist_cutoff: float = 0.1) -> IntervalFrame:
+        """
+        Filter intervals by blacklist
+
+        Parameters
+        ----------
+            intervals : IntervalFrame
+                Intervals to filter
+            blacklist_cutoff : float
+                Cutoff for blacklist
+
+        Returns
+        -------
+            filtered_intervals : IntervalFrame
+                Filtered intervals
+        """
+
+
+        # Calculate blacklist
+        blacklist = self["blacklist"]
+        blacklist_overlap = intervals.index.percent_coverage(blacklist.index)
+        filtered_intervals = intervals.iloc[blacklist_overlap < blacklist_cutoff,:]
+
+        return filtered_intervals
```

### Comparing `genome_info-1.0.2/genome_info/core/utilities.py` & `genome_info-1.0.4/genome_info/core/utilities.py`

 * *Files identical despite different names*

### Comparing `genome_info-1.0.2/genome_info/genomes/.DS_Store` & `genome_info-1.0.4/genome_info/genomes/.DS_Store`

 * *Files identical despite different names*

### Comparing `genome_info-1.0.2/genome_info/genomes/__pycache__/genomes.cpython-311.pyc` & `genome_info-1.0.4/genome_info/genomes/__pycache__/genomes.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `genome_info-1.0.2/genome_info/genomes/__pycache__/readers.cpython-311.pyc` & `genome_info-1.0.4/genome_info/genomes/__pycache__/readers.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `genome_info-1.0.2/genome_info/genomes/base/.DS_Store` & `genome_info-1.0.4/genome_info/genomes/base/.DS_Store`

 * *Files identical despite different names*

### Comparing `genome_info-1.0.2/genome_info/genomes/data/.DS_Store` & `genome_info-1.0.4/genome_info/genomes/data/.DS_Store`

 * *Files identical despite different names*

### Comparing `genome_info-1.0.2/genome_info/genomes/download.py` & `genome_info-1.0.4/genome_info/genomes/download.py`

 * *Files identical despite different names*

### Comparing `genome_info-1.0.2/genome_info/genomes/genomes.py` & `genome_info-1.0.4/genome_info/genomes/genomes.py`

 * *Files identical despite different names*

### Comparing `genome_info-1.0.2/genome_info/genomes/readers.py` & `genome_info-1.0.4/genome_info/genomes/readers.py`

 * *Files identical despite different names*

### Comparing `genome_info-1.0.2/genome_info/kmers/2bit.c` & `genome_info-1.0.4/genome_info/kmers/2bit.c`

 * *Files identical despite different names*

### Comparing `genome_info-1.0.2/genome_info/kmers/2bit.h` & `genome_info-1.0.4/genome_info/kmers/2bit.h`

 * *Files identical despite different names*

### Comparing `genome_info-1.0.2/genome_info/kmers/kmer_reader.c` & `genome_info-1.0.4/genome_info/kmers/kmer_reader.c`

 * *Files 18% similar despite different names*

```diff
@@ -1,77 +1,76 @@
 /* Generated by Cython 0.29.36 */
 
 /* BEGIN: Cython Metadata
 {
     "distutils": {
         "depends": [
-            "/var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/ailist/src/ailist/ailist_add.c",
-            "/var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/ailist/src/ailist/ailist_closest.c",
-            "/var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/ailist/src/ailist/ailist_construct.c",
-            "/var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/ailist/src/ailist/ailist_coverage.c",
-            "/var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/ailist/src/ailist/ailist_extract.c",
-            "/var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/ailist/src/ailist/ailist_filter.c",
-            "/var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/ailist/src/ailist/ailist_get_id.c",
-            "/var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/ailist/src/ailist/ailist_iter.c",
-            "/var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/ailist/src/ailist/ailist_merge.c",
-            "/var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/ailist/src/ailist/ailist_nhits.c",
-            "/var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/ailist/src/ailist/ailist_ops.c",
-            "/var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/ailist/src/ailist/ailist_query.c",
-            "/var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/ailist/src/ailist/ailist_simulate.c",
-            "/var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/ailist/src/ailist/ailist_wps.c",
-            "/var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/ailist/src/ailist/augmented_interval_list.c",
-            "/var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/ailist/src/ailist/augmented_interval_list.h",
-            "/var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/ailist/src/ailist/interval.c",
-            "/var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/ailist/src/ailist/interval.h",
-            "/var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/ailist/src/ailist/overlap_index.c",
-            "/var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/ailist/src/array_query/array_query_utilities.c",
-            "/var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/ailist/src/array_query/array_query_utilities.h",
-            "/var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/ailist/src/labeled_aiarray/khash.h",
-            "/var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/ailist/src/labeled_aiarray/labeled_aiarray_add.c",
-            "/var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/ailist/src/labeled_aiarray/labeled_aiarray_construct.c",
-            "/var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/ailist/src/labeled_aiarray/labeled_aiarray_coverage.c",
-            "/var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/ailist/src/labeled_aiarray/labeled_aiarray_extract.c",
-            "/var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/ailist/src/labeled_aiarray/labeled_aiarray_filter.c",
-            "/var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/ailist/src/labeled_aiarray/labeled_aiarray_get.c",
-            "/var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/ailist/src/labeled_aiarray/labeled_aiarray_index.c",
-            "/var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/ailist/src/labeled_aiarray/labeled_aiarray_iter.c",
-            "/var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/ailist/src/labeled_aiarray/labeled_aiarray_match.c",
-            "/var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/ailist/src/labeled_aiarray/labeled_aiarray_merge.c",
-            "/var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/ailist/src/labeled_aiarray/labeled_aiarray_nhits.c",
-            "/var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/ailist/src/labeled_aiarray/labeled_aiarray_ops.c",
-            "/var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/ailist/src/labeled_aiarray/labeled_aiarray_percent.c",
-            "/var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/ailist/src/labeled_aiarray/labeled_aiarray_query_array.c",
-            "/var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/ailist/src/labeled_aiarray/labeled_aiarray_query_index.c",
-            "/var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/ailist/src/labeled_aiarray/labeled_aiarray_query_single.c",
-            "/var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/ailist/src/labeled_aiarray/labeled_aiarray_simulate.c",
-            "/var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/ailist/src/labeled_aiarray/labeled_aiarray_sort.c",
-            "/var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/ailist/src/labeled_aiarray/labeled_aiarray_wps.c",
-            "/var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/ailist/src/labeled_aiarray/labeled_augmented_array.c",
-            "/var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/ailist/src/labeled_aiarray/labeled_augmented_array.h",
-            "/var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/ailist/src/labeled_aiarray/overlap_label_index.c",
-            "/var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/ailist/src/utilities/utilities.h",
-            "/var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "/var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "/var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "/var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/numpy/core/include/numpy/ufuncobject.h",
+            "/opt/anaconda3/envs/ailist/lib/python3.11/site-packages/ailist-2.1.1-py3.11-macosx-10.9-x86_64.egg/ailist/src/ailist/ailist_add.c",
+            "/opt/anaconda3/envs/ailist/lib/python3.11/site-packages/ailist-2.1.1-py3.11-macosx-10.9-x86_64.egg/ailist/src/ailist/ailist_closest.c",
+            "/opt/anaconda3/envs/ailist/lib/python3.11/site-packages/ailist-2.1.1-py3.11-macosx-10.9-x86_64.egg/ailist/src/ailist/ailist_construct.c",
+            "/opt/anaconda3/envs/ailist/lib/python3.11/site-packages/ailist-2.1.1-py3.11-macosx-10.9-x86_64.egg/ailist/src/ailist/ailist_coverage.c",
+            "/opt/anaconda3/envs/ailist/lib/python3.11/site-packages/ailist-2.1.1-py3.11-macosx-10.9-x86_64.egg/ailist/src/ailist/ailist_extract.c",
+            "/opt/anaconda3/envs/ailist/lib/python3.11/site-packages/ailist-2.1.1-py3.11-macosx-10.9-x86_64.egg/ailist/src/ailist/ailist_filter.c",
+            "/opt/anaconda3/envs/ailist/lib/python3.11/site-packages/ailist-2.1.1-py3.11-macosx-10.9-x86_64.egg/ailist/src/ailist/ailist_get_id.c",
+            "/opt/anaconda3/envs/ailist/lib/python3.11/site-packages/ailist-2.1.1-py3.11-macosx-10.9-x86_64.egg/ailist/src/ailist/ailist_iter.c",
+            "/opt/anaconda3/envs/ailist/lib/python3.11/site-packages/ailist-2.1.1-py3.11-macosx-10.9-x86_64.egg/ailist/src/ailist/ailist_merge.c",
+            "/opt/anaconda3/envs/ailist/lib/python3.11/site-packages/ailist-2.1.1-py3.11-macosx-10.9-x86_64.egg/ailist/src/ailist/ailist_nhits.c",
+            "/opt/anaconda3/envs/ailist/lib/python3.11/site-packages/ailist-2.1.1-py3.11-macosx-10.9-x86_64.egg/ailist/src/ailist/ailist_ops.c",
+            "/opt/anaconda3/envs/ailist/lib/python3.11/site-packages/ailist-2.1.1-py3.11-macosx-10.9-x86_64.egg/ailist/src/ailist/ailist_query.c",
+            "/opt/anaconda3/envs/ailist/lib/python3.11/site-packages/ailist-2.1.1-py3.11-macosx-10.9-x86_64.egg/ailist/src/ailist/ailist_simulate.c",
+            "/opt/anaconda3/envs/ailist/lib/python3.11/site-packages/ailist-2.1.1-py3.11-macosx-10.9-x86_64.egg/ailist/src/ailist/ailist_wps.c",
+            "/opt/anaconda3/envs/ailist/lib/python3.11/site-packages/ailist-2.1.1-py3.11-macosx-10.9-x86_64.egg/ailist/src/ailist/augmented_interval_list.c",
+            "/opt/anaconda3/envs/ailist/lib/python3.11/site-packages/ailist-2.1.1-py3.11-macosx-10.9-x86_64.egg/ailist/src/ailist/augmented_interval_list.h",
+            "/opt/anaconda3/envs/ailist/lib/python3.11/site-packages/ailist-2.1.1-py3.11-macosx-10.9-x86_64.egg/ailist/src/ailist/interval.c",
+            "/opt/anaconda3/envs/ailist/lib/python3.11/site-packages/ailist-2.1.1-py3.11-macosx-10.9-x86_64.egg/ailist/src/ailist/interval.h",
+            "/opt/anaconda3/envs/ailist/lib/python3.11/site-packages/ailist-2.1.1-py3.11-macosx-10.9-x86_64.egg/ailist/src/ailist/overlap_index.c",
+            "/opt/anaconda3/envs/ailist/lib/python3.11/site-packages/ailist-2.1.1-py3.11-macosx-10.9-x86_64.egg/ailist/src/array_query/array_query_utilities.c",
+            "/opt/anaconda3/envs/ailist/lib/python3.11/site-packages/ailist-2.1.1-py3.11-macosx-10.9-x86_64.egg/ailist/src/array_query/array_query_utilities.h",
+            "/opt/anaconda3/envs/ailist/lib/python3.11/site-packages/ailist-2.1.1-py3.11-macosx-10.9-x86_64.egg/ailist/src/labeled_aiarray/khash.h",
+            "/opt/anaconda3/envs/ailist/lib/python3.11/site-packages/ailist-2.1.1-py3.11-macosx-10.9-x86_64.egg/ailist/src/labeled_aiarray/labeled_aiarray_add.c",
+            "/opt/anaconda3/envs/ailist/lib/python3.11/site-packages/ailist-2.1.1-py3.11-macosx-10.9-x86_64.egg/ailist/src/labeled_aiarray/labeled_aiarray_construct.c",
+            "/opt/anaconda3/envs/ailist/lib/python3.11/site-packages/ailist-2.1.1-py3.11-macosx-10.9-x86_64.egg/ailist/src/labeled_aiarray/labeled_aiarray_coverage.c",
+            "/opt/anaconda3/envs/ailist/lib/python3.11/site-packages/ailist-2.1.1-py3.11-macosx-10.9-x86_64.egg/ailist/src/labeled_aiarray/labeled_aiarray_extract.c",
+            "/opt/anaconda3/envs/ailist/lib/python3.11/site-packages/ailist-2.1.1-py3.11-macosx-10.9-x86_64.egg/ailist/src/labeled_aiarray/labeled_aiarray_filter.c",
+            "/opt/anaconda3/envs/ailist/lib/python3.11/site-packages/ailist-2.1.1-py3.11-macosx-10.9-x86_64.egg/ailist/src/labeled_aiarray/labeled_aiarray_get.c",
+            "/opt/anaconda3/envs/ailist/lib/python3.11/site-packages/ailist-2.1.1-py3.11-macosx-10.9-x86_64.egg/ailist/src/labeled_aiarray/labeled_aiarray_index.c",
+            "/opt/anaconda3/envs/ailist/lib/python3.11/site-packages/ailist-2.1.1-py3.11-macosx-10.9-x86_64.egg/ailist/src/labeled_aiarray/labeled_aiarray_iter.c",
+            "/opt/anaconda3/envs/ailist/lib/python3.11/site-packages/ailist-2.1.1-py3.11-macosx-10.9-x86_64.egg/ailist/src/labeled_aiarray/labeled_aiarray_match.c",
+            "/opt/anaconda3/envs/ailist/lib/python3.11/site-packages/ailist-2.1.1-py3.11-macosx-10.9-x86_64.egg/ailist/src/labeled_aiarray/labeled_aiarray_merge.c",
+            "/opt/anaconda3/envs/ailist/lib/python3.11/site-packages/ailist-2.1.1-py3.11-macosx-10.9-x86_64.egg/ailist/src/labeled_aiarray/labeled_aiarray_nhits.c",
+            "/opt/anaconda3/envs/ailist/lib/python3.11/site-packages/ailist-2.1.1-py3.11-macosx-10.9-x86_64.egg/ailist/src/labeled_aiarray/labeled_aiarray_ops.c",
+            "/opt/anaconda3/envs/ailist/lib/python3.11/site-packages/ailist-2.1.1-py3.11-macosx-10.9-x86_64.egg/ailist/src/labeled_aiarray/labeled_aiarray_percent.c",
+            "/opt/anaconda3/envs/ailist/lib/python3.11/site-packages/ailist-2.1.1-py3.11-macosx-10.9-x86_64.egg/ailist/src/labeled_aiarray/labeled_aiarray_query_array.c",
+            "/opt/anaconda3/envs/ailist/lib/python3.11/site-packages/ailist-2.1.1-py3.11-macosx-10.9-x86_64.egg/ailist/src/labeled_aiarray/labeled_aiarray_query_index.c",
+            "/opt/anaconda3/envs/ailist/lib/python3.11/site-packages/ailist-2.1.1-py3.11-macosx-10.9-x86_64.egg/ailist/src/labeled_aiarray/labeled_aiarray_query_single.c",
+            "/opt/anaconda3/envs/ailist/lib/python3.11/site-packages/ailist-2.1.1-py3.11-macosx-10.9-x86_64.egg/ailist/src/labeled_aiarray/labeled_aiarray_simulate.c",
+            "/opt/anaconda3/envs/ailist/lib/python3.11/site-packages/ailist-2.1.1-py3.11-macosx-10.9-x86_64.egg/ailist/src/labeled_aiarray/labeled_aiarray_sort.c",
+            "/opt/anaconda3/envs/ailist/lib/python3.11/site-packages/ailist-2.1.1-py3.11-macosx-10.9-x86_64.egg/ailist/src/labeled_aiarray/labeled_aiarray_wps.c",
+            "/opt/anaconda3/envs/ailist/lib/python3.11/site-packages/ailist-2.1.1-py3.11-macosx-10.9-x86_64.egg/ailist/src/labeled_aiarray/labeled_augmented_array.c",
+            "/opt/anaconda3/envs/ailist/lib/python3.11/site-packages/ailist-2.1.1-py3.11-macosx-10.9-x86_64.egg/ailist/src/labeled_aiarray/labeled_augmented_array.h",
+            "/opt/anaconda3/envs/ailist/lib/python3.11/site-packages/ailist-2.1.1-py3.11-macosx-10.9-x86_64.egg/ailist/src/labeled_aiarray/overlap_label_index.c",
+            "/opt/anaconda3/envs/ailist/lib/python3.11/site-packages/ailist-2.1.1-py3.11-macosx-10.9-x86_64.egg/ailist/src/utilities/utilities.h",
+            "/opt/anaconda3/envs/ailist/lib/python3.11/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/opt/anaconda3/envs/ailist/lib/python3.11/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/opt/anaconda3/envs/ailist/lib/python3.11/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/opt/anaconda3/envs/ailist/lib/python3.11/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/opt/anaconda3/envs/ailist/lib/python3.11/site-packages/numpy/core/include/numpy/ufuncobject.h",
             "genome_info/kmers/2bit.c",
             "genome_info/kmers/2bit.h",
             "genome_info/kmers/interval_kmer.c",
             "genome_info/kmers/interval_kmer.h"
         ],
         "extra_compile_args": [
-            "-O3"
+            "-O2"
         ],
         "include_dirs": [
             "genome_info/kmers",
-            "/var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/ailist",
+            "/opt/anaconda3/envs/ailist/lib/python3.11/site-packages/ailist-2.1.1-py3.11-macosx-10.9-x86_64.egg/ailist",
             ".",
-            "/var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/numpy/core/include",
-            "/private/var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/ailist"
+            "/opt/anaconda3/envs/ailist/lib/python3.11/site-packages/numpy/core/include"
         ],
         "name": "genome_info.kmers.kmer_reader",
         "sources": [
             "genome_info/kmers/kmer_reader.pyx"
         ]
     },
     "module_name": "genome_info.kmers.kmer_reader"
@@ -1228,177 +1227,195 @@
   char enc_type;
   char new_packmode;
   char enc_packmode;
   char is_valid_array;
 } __Pyx_BufFmt_Context;
 
 
-/* "../../../../../../../var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/numpy/__init__.pxd":688
+/* "../../../../../../../opt/anaconda3/envs/ailist/lib/python3.11/site-packages/numpy/__init__.pxd":689
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../../../../var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/numpy/__init__.pxd":689
+/* "../../../../../../../opt/anaconda3/envs/ailist/lib/python3.11/site-packages/numpy/__init__.pxd":690
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../../../../var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/numpy/__init__.pxd":690
+/* "../../../../../../../opt/anaconda3/envs/ailist/lib/python3.11/site-packages/numpy/__init__.pxd":691
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../../../../var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/numpy/__init__.pxd":691
+/* "../../../../../../../opt/anaconda3/envs/ailist/lib/python3.11/site-packages/numpy/__init__.pxd":692
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../../../../var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/numpy/__init__.pxd":695
+/* "../../../../../../../opt/anaconda3/envs/ailist/lib/python3.11/site-packages/numpy/__init__.pxd":696
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../../../../var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/numpy/__init__.pxd":696
+/* "../../../../../../../opt/anaconda3/envs/ailist/lib/python3.11/site-packages/numpy/__init__.pxd":697
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../../../../var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/numpy/__init__.pxd":697
+/* "../../../../../../../opt/anaconda3/envs/ailist/lib/python3.11/site-packages/numpy/__init__.pxd":698
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../../../../var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/numpy/__init__.pxd":698
+/* "../../../../../../../opt/anaconda3/envs/ailist/lib/python3.11/site-packages/numpy/__init__.pxd":699
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../../../../var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/numpy/__init__.pxd":702
+/* "../../../../../../../opt/anaconda3/envs/ailist/lib/python3.11/site-packages/numpy/__init__.pxd":703
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../../../../var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/numpy/__init__.pxd":703
+/* "../../../../../../../opt/anaconda3/envs/ailist/lib/python3.11/site-packages/numpy/__init__.pxd":704
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../../../../var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/numpy/__init__.pxd":712
+/* "../../../../../../../opt/anaconda3/envs/ailist/lib/python3.11/site-packages/numpy/__init__.pxd":713
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
+ * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
- * 
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../../../../var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/numpy/__init__.pxd":713
+/* "../../../../../../../opt/anaconda3/envs/ailist/lib/python3.11/site-packages/numpy/__init__.pxd":714
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
+ * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
+ * ctypedef npy_longlong   longlong_t
+ * 
+ */
+typedef npy_longlong __pyx_t_5numpy_long_t;
+
+/* "../../../../../../../opt/anaconda3/envs/ailist/lib/python3.11/site-packages/numpy/__init__.pxd":715
+ * ctypedef npy_long       int_t
+ * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../../../../var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/numpy/__init__.pxd":715
+/* "../../../../../../../opt/anaconda3/envs/ailist/lib/python3.11/site-packages/numpy/__init__.pxd":717
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
+ * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
- * 
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../../../../var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/numpy/__init__.pxd":716
+/* "../../../../../../../opt/anaconda3/envs/ailist/lib/python3.11/site-packages/numpy/__init__.pxd":718
  * 
  * ctypedef npy_ulong      uint_t
+ * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
+ * ctypedef npy_ulonglong  ulonglong_t
+ * 
+ */
+typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
+
+/* "../../../../../../../opt/anaconda3/envs/ailist/lib/python3.11/site-packages/numpy/__init__.pxd":719
+ * ctypedef npy_ulong      uint_t
+ * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../../../../var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/numpy/__init__.pxd":718
+/* "../../../../../../../opt/anaconda3/envs/ailist/lib/python3.11/site-packages/numpy/__init__.pxd":721
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../../../../var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/numpy/__init__.pxd":719
+/* "../../../../../../../opt/anaconda3/envs/ailist/lib/python3.11/site-packages/numpy/__init__.pxd":722
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../../../../var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/numpy/__init__.pxd":721
+/* "../../../../../../../opt/anaconda3/envs/ailist/lib/python3.11/site-packages/numpy/__init__.pxd":724
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../../../../var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/numpy/__init__.pxd":722
+/* "../../../../../../../opt/anaconda3/envs/ailist/lib/python3.11/site-packages/numpy/__init__.pxd":725
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../../../../var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/numpy/__init__.pxd":723
+/* "../../../../../../../opt/anaconda3/envs/ailist/lib/python3.11/site-packages/numpy/__init__.pxd":726
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1442,42 +1459,42 @@
 struct __pyx_obj_6ailist_25LabeledIntervalArray_core_LabeledInterval;
 struct __pyx_obj_6ailist_25LabeledIntervalArray_core_LabeledIntervalArray;
 struct __pyx_array_obj;
 struct __pyx_MemviewEnum_obj;
 struct __pyx_memoryview_obj;
 struct __pyx_memoryviewslice_obj;
 
-/* "../../../../../../../var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/numpy/__init__.pxd":725
+/* "../../../../../../../opt/anaconda3/envs/ailist/lib/python3.11/site-packages/numpy/__init__.pxd":728
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../../../../var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/numpy/__init__.pxd":726
+/* "../../../../../../../opt/anaconda3/envs/ailist/lib/python3.11/site-packages/numpy/__init__.pxd":729
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../../../../var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/numpy/__init__.pxd":727
+/* "../../../../../../../opt/anaconda3/envs/ailist/lib/python3.11/site-packages/numpy/__init__.pxd":730
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../../../../var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/numpy/__init__.pxd":729
+/* "../../../../../../../opt/anaconda3/envs/ailist/lib/python3.11/site-packages/numpy/__init__.pxd":732
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -2703,14 +2720,79 @@
 static const char __pyx_k_i[] = "i";
 static const char __pyx_k_k[] = "k";
 static const char __pyx_k_t[] = "t";
 static const char __pyx_k_gc[] = "gc";
 static const char __pyx_k_id[] = "id";
 static const char __pyx_k_kc[] = "kc";
 static const char __pyx_k_np[] = "np";
+static const char __pyx_k_pd[] = "pd";
+static const char __pyx_k_AAA[] = "AAA";
+static const char __pyx_k_AAC[] = "AAC";
+static const char __pyx_k_AAG[] = "AAG";
+static const char __pyx_k_AAT[] = "AAT";
+static const char __pyx_k_ACA[] = "ACA";
+static const char __pyx_k_ACC[] = "ACC";
+static const char __pyx_k_ACG[] = "ACG";
+static const char __pyx_k_ACT[] = "ACT";
+static const char __pyx_k_AGA[] = "AGA";
+static const char __pyx_k_AGC[] = "AGC";
+static const char __pyx_k_AGG[] = "AGG";
+static const char __pyx_k_AGT[] = "AGT";
+static const char __pyx_k_ATA[] = "ATA";
+static const char __pyx_k_ATC[] = "ATC";
+static const char __pyx_k_ATG[] = "ATG";
+static const char __pyx_k_ATT[] = "ATT";
+static const char __pyx_k_CAA[] = "CAA";
+static const char __pyx_k_CAC[] = "CAC";
+static const char __pyx_k_CAG[] = "CAG";
+static const char __pyx_k_CAT[] = "CAT";
+static const char __pyx_k_CCA[] = "CCA";
+static const char __pyx_k_CCC[] = "CCC";
+static const char __pyx_k_CCG[] = "CCG";
+static const char __pyx_k_CCT[] = "CCT";
+static const char __pyx_k_CGA[] = "CGA";
+static const char __pyx_k_CGC[] = "CGC";
+static const char __pyx_k_CGG[] = "CGG";
+static const char __pyx_k_CGT[] = "CGT";
+static const char __pyx_k_CTA[] = "CTA";
+static const char __pyx_k_CTC[] = "CTC";
+static const char __pyx_k_CTG[] = "CTG";
+static const char __pyx_k_CTT[] = "CTT";
+static const char __pyx_k_GAA[] = "GAA";
+static const char __pyx_k_GAC[] = "GAC";
+static const char __pyx_k_GAG[] = "GAG";
+static const char __pyx_k_GAT[] = "GAT";
+static const char __pyx_k_GCA[] = "GCA";
+static const char __pyx_k_GCC[] = "GCC";
+static const char __pyx_k_GCG[] = "GCG";
+static const char __pyx_k_GCT[] = "GCT";
+static const char __pyx_k_GGA[] = "GGA";
+static const char __pyx_k_GGC[] = "GGC";
+static const char __pyx_k_GGG[] = "GGG";
+static const char __pyx_k_GGT[] = "GGT";
+static const char __pyx_k_GTA[] = "GTA";
+static const char __pyx_k_GTC[] = "GTC";
+static const char __pyx_k_GTG[] = "GTG";
+static const char __pyx_k_GTT[] = "GTT";
+static const char __pyx_k_TAA[] = "TAA";
+static const char __pyx_k_TAC[] = "TAC";
+static const char __pyx_k_TAG[] = "TAG";
+static const char __pyx_k_TAT[] = "TAT";
+static const char __pyx_k_TCA[] = "TCA";
+static const char __pyx_k_TCC[] = "TCC";
+static const char __pyx_k_TCG[] = "TCG";
+static const char __pyx_k_TCT[] = "TCT";
+static const char __pyx_k_TGA[] = "TGA";
+static const char __pyx_k_TGC[] = "TGC";
+static const char __pyx_k_TGG[] = "TGG";
+static const char __pyx_k_TGT[] = "TGT";
+static const char __pyx_k_TTA[] = "TTA";
+static const char __pyx_k_TTC[] = "TTC";
+static const char __pyx_k_TTG[] = "TTG";
+static const char __pyx_k_TTT[] = "TTT";
 static const char __pyx_k_end[] = "end";
 static const char __pyx_k_ibf[] = "ibf";
 static const char __pyx_k_new[] = "__new__";
 static const char __pyx_k_obj[] = "obj";
 static const char __pyx_k_seq[] = "seq";
 static const char __pyx_k_base[] = "base";
 static const char __pyx_k_dict[] = "__dict__";
@@ -2729,25 +2811,27 @@
 static const char __pyx_k_chrom[] = "chrom";
 static const char __pyx_k_class[] = "__class__";
 static const char __pyx_k_count[] = "count";
 static const char __pyx_k_dtype[] = "dtype";
 static const char __pyx_k_error[] = "error";
 static const char __pyx_k_flags[] = "flags";
 static const char __pyx_k_fname[] = "fname";
+static const char __pyx_k_index[] = "index";
 static const char __pyx_k_numpy[] = "numpy";
 static const char __pyx_k_range[] = "range";
 static const char __pyx_k_shape[] = "shape";
 static const char __pyx_k_start[] = "start";
 static const char __pyx_k_zeros[] = "zeros";
 static const char __pyx_k_encode[] = "encode";
 static const char __pyx_k_format[] = "format";
 static const char __pyx_k_gc_mem[] = "gc_mem";
 static const char __pyx_k_import[] = "__import__";
 static const char __pyx_k_last_n[] = "last_n";
 static const char __pyx_k_name_2[] = "__name__";
+static const char __pyx_k_pandas[] = "pandas";
 static const char __pyx_k_pickle[] = "pickle";
 static const char __pyx_k_py_seq[] = "py_seq";
 static const char __pyx_k_reduce[] = "__reduce__";
 static const char __pyx_k_result[] = "result";
 static const char __pyx_k_seq_fn[] = "seq_fn";
 static const char __pyx_k_single[] = "single";
 static const char __pyx_k_struct[] = "struct";
@@ -2759,14 +2843,16 @@
 static const char __pyx_k_Ellipsis[] = "Ellipsis";
 static const char __pyx_k_end_freq[] = "end_freq";
 static const char __pyx_k_getstate[] = "__getstate__";
 static const char __pyx_k_itemsize[] = "itemsize";
 static const char __pyx_k_kmer_seq[] = "kmer_seq";
 static const char __pyx_k_pyx_type[] = "__pyx_type";
 static const char __pyx_k_setstate[] = "__setstate__";
+static const char __pyx_k_tribases[] = "tribases";
+static const char __pyx_k_DataFrame[] = "DataFrame";
 static const char __pyx_k_TypeError[] = "TypeError";
 static const char __pyx_k_enumerate[] = "enumerate";
 static const char __pyx_k_pyx_state[] = "__pyx_state";
 static const char __pyx_k_reduce_ex[] = "__reduce_ex__";
 static const char __pyx_k_IndexError[] = "IndexError";
 static const char __pyx_k_InfoReader[] = "InfoReader";
 static const char __pyx_k_ValueError[] = "ValueError";
@@ -2774,20 +2860,22 @@
 static const char __pyx_k_pyx_result[] = "__pyx_result";
 static const char __pyx_k_pyx_vtable[] = "__pyx_vtable__";
 static const char __pyx_k_read_kmers[] = "read_kmers";
 static const char __pyx_k_start_freq[] = "start_freq";
 static const char __pyx_k_ImportError[] = "ImportError";
 static const char __pyx_k_MemoryError[] = "MemoryError";
 static const char __pyx_k_PickleError[] = "PickleError";
+static const char __pyx_k_end_results[] = "end_results";
 static const char __pyx_k_twobit_name[] = "twobit_name";
 static const char __pyx_k_pyx_checksum[] = "__pyx_checksum";
 static const char __pyx_k_stringsource[] = "stringsource";
 static const char __pyx_k_pyx_getbuffer[] = "__pyx_getbuffer";
 static const char __pyx_k_read_sequence[] = "read_sequence";
 static const char __pyx_k_reduce_cython[] = "__reduce_cython__";
+static const char __pyx_k_start_results[] = "start_results";
 static const char __pyx_k_genome_version[] = "genome_version";
 static const char __pyx_k_View_MemoryView[] = "View.MemoryView";
 static const char __pyx_k_allocate_buffer[] = "allocate_buffer";
 static const char __pyx_k_dtype_is_object[] = "dtype_is_object";
 static const char __pyx_k_genomes_genomes[] = "genomes.genomes";
 static const char __pyx_k_pyx_PickleError[] = "__pyx_PickleError";
 static const char __pyx_k_setstate_cython[] = "__setstate_cython__";
@@ -2797,14 +2885,15 @@
 static const char __pyx_k_strided_and_indirect[] = "<strided and indirect>";
 static const char __pyx_k_contiguous_and_direct[] = "<contiguous and direct>";
 static const char __pyx_k_read_bounds_base_freq[] = "read_bounds_base_freq";
 static const char __pyx_k_MemoryView_of_r_object[] = "<MemoryView of %r object>";
 static const char __pyx_k_MemoryView_of_r_at_0x_x[] = "<MemoryView of %r at 0x%x>";
 static const char __pyx_k_contiguous_and_indirect[] = "<contiguous and indirect>";
 static const char __pyx_k_Cannot_index_with_type_s[] = "Cannot index with type '%s'";
+static const char __pyx_k_read_bounds_tribase_freq[] = "read_bounds_tribase_freq";
 static const char __pyx_k_Invalid_shape_in_axis_d_d[] = "Invalid shape in axis %d: %d.";
 static const char __pyx_k_itemsize_0_for_cython_array[] = "itemsize <= 0 for cython.array";
 static const char __pyx_k_genome_info_kmers_kmer_reader[] = "genome_info.kmers.kmer_reader";
 static const char __pyx_k_unable_to_allocate_array_data[] = "unable to allocate array data.";
 static const char __pyx_k_strided_and_direct_or_indirect[] = "<strided and direct or indirect>";
 static const char __pyx_k_numpy_core_multiarray_failed_to[] = "numpy.core.multiarray failed to import";
 static const char __pyx_k_Buffer_view_does_not_expose_stri[] = "Buffer view does not expose strides";
@@ -2818,35 +2907,100 @@
 static const char __pyx_k_Out_of_bounds_on_buffer_access_a[] = "Out of bounds on buffer access (axis %d)";
 static const char __pyx_k_Unable_to_convert_item_to_object[] = "Unable to convert item to object";
 static const char __pyx_k_genome_info_kmers_kmer_reader_py[] = "genome_info/kmers/kmer_reader.pyx";
 static const char __pyx_k_got_differing_extents_in_dimensi[] = "got differing extents in dimension %d (got %d and %d)";
 static const char __pyx_k_no_default___reduce___due_to_non[] = "no default __reduce__ due to non-trivial __cinit__";
 static const char __pyx_k_numpy_core_umath_failed_to_impor[] = "numpy.core.umath failed to import";
 static const char __pyx_k_unable_to_allocate_shape_and_str[] = "unable to allocate shape and strides.";
+static PyObject *__pyx_n_u_AAA;
+static PyObject *__pyx_n_u_AAC;
+static PyObject *__pyx_n_u_AAG;
+static PyObject *__pyx_n_u_AAT;
+static PyObject *__pyx_n_u_ACA;
+static PyObject *__pyx_n_u_ACC;
+static PyObject *__pyx_n_u_ACG;
+static PyObject *__pyx_n_u_ACT;
+static PyObject *__pyx_n_u_AGA;
+static PyObject *__pyx_n_u_AGC;
+static PyObject *__pyx_n_u_AGG;
+static PyObject *__pyx_n_u_AGT;
 static PyObject *__pyx_n_s_ASCII;
+static PyObject *__pyx_n_u_ATA;
+static PyObject *__pyx_n_u_ATC;
+static PyObject *__pyx_n_u_ATG;
+static PyObject *__pyx_n_u_ATT;
 static PyObject *__pyx_kp_s_Buffer_view_does_not_expose_stri;
+static PyObject *__pyx_n_u_CAA;
+static PyObject *__pyx_n_u_CAC;
+static PyObject *__pyx_n_u_CAG;
+static PyObject *__pyx_n_u_CAT;
+static PyObject *__pyx_n_u_CCA;
+static PyObject *__pyx_n_u_CCC;
+static PyObject *__pyx_n_u_CCG;
+static PyObject *__pyx_n_u_CCT;
+static PyObject *__pyx_n_u_CGA;
+static PyObject *__pyx_n_u_CGC;
+static PyObject *__pyx_n_u_CGG;
+static PyObject *__pyx_n_u_CGT;
+static PyObject *__pyx_n_u_CTA;
+static PyObject *__pyx_n_u_CTC;
+static PyObject *__pyx_n_u_CTG;
+static PyObject *__pyx_n_u_CTT;
 static PyObject *__pyx_kp_s_Can_only_create_a_buffer_that_is;
 static PyObject *__pyx_kp_s_Cannot_assign_to_read_only_memor;
 static PyObject *__pyx_kp_s_Cannot_create_writable_memory_vi;
 static PyObject *__pyx_kp_s_Cannot_index_with_type_s;
+static PyObject *__pyx_n_s_DataFrame;
 static PyObject *__pyx_n_s_Ellipsis;
 static PyObject *__pyx_kp_s_Empty_shape_tuple_for_cython_arr;
+static PyObject *__pyx_n_u_GAA;
+static PyObject *__pyx_n_u_GAC;
+static PyObject *__pyx_n_u_GAG;
+static PyObject *__pyx_n_u_GAT;
+static PyObject *__pyx_n_u_GCA;
+static PyObject *__pyx_n_u_GCC;
+static PyObject *__pyx_n_u_GCG;
+static PyObject *__pyx_n_u_GCT;
+static PyObject *__pyx_n_u_GGA;
+static PyObject *__pyx_n_u_GGC;
+static PyObject *__pyx_n_u_GGG;
+static PyObject *__pyx_n_u_GGT;
+static PyObject *__pyx_n_u_GTA;
+static PyObject *__pyx_n_u_GTC;
+static PyObject *__pyx_n_u_GTG;
+static PyObject *__pyx_n_u_GTT;
 static PyObject *__pyx_n_s_ImportError;
 static PyObject *__pyx_kp_s_Incompatible_checksums_0x_x_vs_0;
 static PyObject *__pyx_n_s_IndexError;
 static PyObject *__pyx_kp_s_Indirect_dimensions_not_supporte;
 static PyObject *__pyx_n_s_InfoReader;
 static PyObject *__pyx_kp_s_Invalid_mode_expected_c_or_fortr;
 static PyObject *__pyx_kp_s_Invalid_shape_in_axis_d_d;
 static PyObject *__pyx_n_s_MemoryError;
 static PyObject *__pyx_kp_s_MemoryView_of_r_at_0x_x;
 static PyObject *__pyx_kp_s_MemoryView_of_r_object;
 static PyObject *__pyx_n_b_O;
 static PyObject *__pyx_kp_s_Out_of_bounds_on_buffer_access_a;
 static PyObject *__pyx_n_s_PickleError;
+static PyObject *__pyx_n_u_TAA;
+static PyObject *__pyx_n_u_TAC;
+static PyObject *__pyx_n_u_TAG;
+static PyObject *__pyx_n_u_TAT;
+static PyObject *__pyx_n_u_TCA;
+static PyObject *__pyx_n_u_TCC;
+static PyObject *__pyx_n_u_TCG;
+static PyObject *__pyx_n_u_TCT;
+static PyObject *__pyx_n_u_TGA;
+static PyObject *__pyx_n_u_TGC;
+static PyObject *__pyx_n_u_TGG;
+static PyObject *__pyx_n_u_TGT;
+static PyObject *__pyx_n_u_TTA;
+static PyObject *__pyx_n_u_TTC;
+static PyObject *__pyx_n_u_TTG;
+static PyObject *__pyx_n_u_TTT;
 static PyObject *__pyx_n_s_TypeError;
 static PyObject *__pyx_kp_s_Unable_to_convert_item_to_object;
 static PyObject *__pyx_n_s_ValueError;
 static PyObject *__pyx_n_s_View_MemoryView;
 static PyObject *__pyx_n_s_allocate_buffer;
 static PyObject *__pyx_n_s_base;
 static PyObject *__pyx_n_s_c;
@@ -2859,14 +3013,15 @@
 static PyObject *__pyx_n_s_count;
 static PyObject *__pyx_n_s_dict;
 static PyObject *__pyx_n_s_dtype;
 static PyObject *__pyx_n_s_dtype_is_object;
 static PyObject *__pyx_n_s_encode;
 static PyObject *__pyx_n_s_end;
 static PyObject *__pyx_n_s_end_freq;
+static PyObject *__pyx_n_s_end_results;
 static PyObject *__pyx_n_s_enumerate;
 static PyObject *__pyx_n_s_error;
 static PyObject *__pyx_n_s_flags;
 static PyObject *__pyx_n_s_fname;
 static PyObject *__pyx_n_s_format;
 static PyObject *__pyx_n_s_fortran;
 static PyObject *__pyx_n_u_fortran;
@@ -2880,14 +3035,15 @@
 static PyObject *__pyx_n_s_getstate;
 static PyObject *__pyx_kp_s_got_differing_extents_in_dimensi;
 static PyObject *__pyx_n_u_hg38;
 static PyObject *__pyx_n_s_i;
 static PyObject *__pyx_n_s_ibf;
 static PyObject *__pyx_n_s_id;
 static PyObject *__pyx_n_s_import;
+static PyObject *__pyx_n_s_index;
 static PyObject *__pyx_n_s_itemsize;
 static PyObject *__pyx_kp_s_itemsize_0_for_cython_array;
 static PyObject *__pyx_n_s_k;
 static PyObject *__pyx_n_s_kc;
 static PyObject *__pyx_n_s_kmer_seq;
 static PyObject *__pyx_n_s_laia;
 static PyObject *__pyx_n_s_last_n;
@@ -2902,26 +3058,29 @@
 static PyObject *__pyx_kp_s_no_default___reduce___due_to_non;
 static PyObject *__pyx_n_s_np;
 static PyObject *__pyx_n_s_numpy;
 static PyObject *__pyx_kp_u_numpy_core_multiarray_failed_to;
 static PyObject *__pyx_kp_u_numpy_core_umath_failed_to_impor;
 static PyObject *__pyx_n_s_obj;
 static PyObject *__pyx_n_s_pack;
+static PyObject *__pyx_n_s_pandas;
+static PyObject *__pyx_n_s_pd;
 static PyObject *__pyx_n_s_pickle;
 static PyObject *__pyx_n_s_py_seq;
 static PyObject *__pyx_n_s_pyx_PickleError;
 static PyObject *__pyx_n_s_pyx_checksum;
 static PyObject *__pyx_n_s_pyx_getbuffer;
 static PyObject *__pyx_n_s_pyx_result;
 static PyObject *__pyx_n_s_pyx_state;
 static PyObject *__pyx_n_s_pyx_type;
 static PyObject *__pyx_n_s_pyx_unpickle_Enum;
 static PyObject *__pyx_n_s_pyx_vtable;
 static PyObject *__pyx_n_s_range;
 static PyObject *__pyx_n_s_read_bounds_base_freq;
+static PyObject *__pyx_n_s_read_bounds_tribase_freq;
 static PyObject *__pyx_n_s_read_kmers;
 static PyObject *__pyx_n_s_read_sequence;
 static PyObject *__pyx_n_s_reduce;
 static PyObject *__pyx_n_s_reduce_cython;
 static PyObject *__pyx_n_s_reduce_ex;
 static PyObject *__pyx_n_s_result;
 static PyObject *__pyx_n_s_seq;
@@ -2929,33 +3088,36 @@
 static PyObject *__pyx_n_s_setstate;
 static PyObject *__pyx_n_s_setstate_cython;
 static PyObject *__pyx_n_s_shape;
 static PyObject *__pyx_n_s_single;
 static PyObject *__pyx_n_s_size;
 static PyObject *__pyx_n_s_start;
 static PyObject *__pyx_n_s_start_freq;
+static PyObject *__pyx_n_s_start_results;
 static PyObject *__pyx_n_s_step;
 static PyObject *__pyx_n_s_stop;
 static PyObject *__pyx_kp_s_strided_and_direct;
 static PyObject *__pyx_kp_s_strided_and_direct_or_indirect;
 static PyObject *__pyx_kp_s_strided_and_indirect;
 static PyObject *__pyx_kp_s_stringsource;
 static PyObject *__pyx_n_s_struct;
 static PyObject *__pyx_n_s_t;
 static PyObject *__pyx_n_s_test;
+static PyObject *__pyx_n_s_tribases;
 static PyObject *__pyx_n_s_twobit_name;
 static PyObject *__pyx_kp_s_unable_to_allocate_array_data;
 static PyObject *__pyx_kp_s_unable_to_allocate_shape_and_str;
 static PyObject *__pyx_n_s_unpack;
 static PyObject *__pyx_n_s_update;
 static PyObject *__pyx_n_s_zeros;
 static PyObject *__pyx_pf_11genome_info_5kmers_11kmer_reader_read_kmers(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_seq_fn, struct __pyx_obj_6ailist_25LabeledIntervalArray_core_LabeledIntervalArray *__pyx_v_laia, int __pyx_v_k, int __pyx_v_last_n); /* proto */
 static PyObject *__pyx_pf_11genome_info_5kmers_11kmer_reader_2read_sequence(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_seq_fn, PyObject *__pyx_v_chrom, int __pyx_v_start, int __pyx_v_end); /* proto */
 static PyObject *__pyx_pf_11genome_info_5kmers_11kmer_reader_4gc_percent(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_seq_fn, struct __pyx_obj_6ailist_25LabeledIntervalArray_core_LabeledIntervalArray *__pyx_v_laia, CYTHON_UNUSED PyObject *__pyx_v_genome_version); /* proto */
 static PyObject *__pyx_pf_11genome_info_5kmers_11kmer_reader_6read_bounds_base_freq(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_seq_fn, struct __pyx_obj_6ailist_25LabeledIntervalArray_core_LabeledIntervalArray *__pyx_v_laia, int __pyx_v_n_bases); /* proto */
+static PyObject *__pyx_pf_11genome_info_5kmers_11kmer_reader_8read_bounds_tribase_freq(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_seq_fn, struct __pyx_obj_6ailist_25LabeledIntervalArray_core_LabeledIntervalArray *__pyx_v_laia, int __pyx_v_n_bases); /* proto */
 static int __pyx_array___pyx_pf_15View_dot_MemoryView_5array___cinit__(struct __pyx_array_obj *__pyx_v_self, PyObject *__pyx_v_shape, Py_ssize_t __pyx_v_itemsize, PyObject *__pyx_v_format, PyObject *__pyx_v_mode, int __pyx_v_allocate_buffer); /* proto */
 static int __pyx_array___pyx_pf_15View_dot_MemoryView_5array_2__getbuffer__(struct __pyx_array_obj *__pyx_v_self, Py_buffer *__pyx_v_info, int __pyx_v_flags); /* proto */
 static void __pyx_array___pyx_pf_15View_dot_MemoryView_5array_4__dealloc__(struct __pyx_array_obj *__pyx_v_self); /* proto */
 static PyObject *__pyx_pf_15View_dot_MemoryView_5array_7memview___get__(struct __pyx_array_obj *__pyx_v_self); /* proto */
 static Py_ssize_t __pyx_array___pyx_pf_15View_dot_MemoryView_5array_6__len__(struct __pyx_array_obj *__pyx_v_self); /* proto */
 static PyObject *__pyx_array___pyx_pf_15View_dot_MemoryView_5array_8__getattr__(struct __pyx_array_obj *__pyx_v_self, PyObject *__pyx_v_attr); /* proto */
 static PyObject *__pyx_array___pyx_pf_15View_dot_MemoryView_5array_10__getitem__(struct __pyx_array_obj *__pyx_v_self, PyObject *__pyx_v_item); /* proto */
@@ -2999,14 +3161,74 @@
 static PyObject *__pyx_tp_new_memoryview(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_tp_new__memoryviewslice(PyTypeObject *t, PyObject *a, PyObject *k); /*proto*/
 static PyObject *__pyx_int_0;
 static PyObject *__pyx_int_1;
 static PyObject *__pyx_int_2;
 static PyObject *__pyx_int_3;
 static PyObject *__pyx_int_4;
+static PyObject *__pyx_int_5;
+static PyObject *__pyx_int_6;
+static PyObject *__pyx_int_7;
+static PyObject *__pyx_int_8;
+static PyObject *__pyx_int_9;
+static PyObject *__pyx_int_10;
+static PyObject *__pyx_int_11;
+static PyObject *__pyx_int_12;
+static PyObject *__pyx_int_13;
+static PyObject *__pyx_int_14;
+static PyObject *__pyx_int_15;
+static PyObject *__pyx_int_16;
+static PyObject *__pyx_int_17;
+static PyObject *__pyx_int_18;
+static PyObject *__pyx_int_19;
+static PyObject *__pyx_int_20;
+static PyObject *__pyx_int_21;
+static PyObject *__pyx_int_22;
+static PyObject *__pyx_int_23;
+static PyObject *__pyx_int_24;
+static PyObject *__pyx_int_25;
+static PyObject *__pyx_int_26;
+static PyObject *__pyx_int_27;
+static PyObject *__pyx_int_28;
+static PyObject *__pyx_int_29;
+static PyObject *__pyx_int_30;
+static PyObject *__pyx_int_31;
+static PyObject *__pyx_int_32;
+static PyObject *__pyx_int_33;
+static PyObject *__pyx_int_34;
+static PyObject *__pyx_int_35;
+static PyObject *__pyx_int_36;
+static PyObject *__pyx_int_37;
+static PyObject *__pyx_int_38;
+static PyObject *__pyx_int_39;
+static PyObject *__pyx_int_40;
+static PyObject *__pyx_int_41;
+static PyObject *__pyx_int_42;
+static PyObject *__pyx_int_43;
+static PyObject *__pyx_int_44;
+static PyObject *__pyx_int_45;
+static PyObject *__pyx_int_46;
+static PyObject *__pyx_int_47;
+static PyObject *__pyx_int_48;
+static PyObject *__pyx_int_49;
+static PyObject *__pyx_int_50;
+static PyObject *__pyx_int_51;
+static PyObject *__pyx_int_52;
+static PyObject *__pyx_int_53;
+static PyObject *__pyx_int_54;
+static PyObject *__pyx_int_55;
+static PyObject *__pyx_int_56;
+static PyObject *__pyx_int_57;
+static PyObject *__pyx_int_58;
+static PyObject *__pyx_int_59;
+static PyObject *__pyx_int_60;
+static PyObject *__pyx_int_61;
+static PyObject *__pyx_int_62;
+static PyObject *__pyx_int_63;
+static PyObject *__pyx_int_64;
 static PyObject *__pyx_int_112105877;
 static PyObject *__pyx_int_136983863;
 static PyObject *__pyx_int_184977713;
 static PyObject *__pyx_int_neg_1;
 static PyObject *__pyx_tuple_;
 static PyObject *__pyx_tuple__2;
 static PyObject *__pyx_tuple__3;
@@ -3029,74 +3251,76 @@
 static PyObject *__pyx_tuple__20;
 static PyObject *__pyx_tuple__21;
 static PyObject *__pyx_tuple__22;
 static PyObject *__pyx_tuple__24;
 static PyObject *__pyx_tuple__26;
 static PyObject *__pyx_tuple__28;
 static PyObject *__pyx_tuple__30;
-static PyObject *__pyx_tuple__31;
 static PyObject *__pyx_tuple__32;
 static PyObject *__pyx_tuple__33;
 static PyObject *__pyx_tuple__34;
 static PyObject *__pyx_tuple__35;
+static PyObject *__pyx_tuple__36;
+static PyObject *__pyx_tuple__37;
 static PyObject *__pyx_codeobj__23;
 static PyObject *__pyx_codeobj__25;
 static PyObject *__pyx_codeobj__27;
 static PyObject *__pyx_codeobj__29;
-static PyObject *__pyx_codeobj__36;
+static PyObject *__pyx_codeobj__31;
+static PyObject *__pyx_codeobj__38;
 /* Late includes */
 
-/* "genome_info/kmers/kmer_reader.pyx":12
+/* "genome_info/kmers/kmer_reader.pyx":13
  * 
  * 
  * cdef kmer_count_t *_read_kmers(char *fname, labeled_aiarray_t *laia, int k, int last_n):             # <<<<<<<<<<<<<<
  *     cdef kmer_count_t *kc = interval_kmer_count(laia, fname, k, last_n)
  * 
  */
 
 static kmer_count_t *__pyx_f_11genome_info_5kmers_11kmer_reader__read_kmers(char *__pyx_v_fname, labeled_aiarray_t *__pyx_v_laia, int __pyx_v_k, int __pyx_v_last_n) {
   kmer_count_t *__pyx_v_kc;
   kmer_count_t *__pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("_read_kmers", 0);
 
-  /* "genome_info/kmers/kmer_reader.pyx":13
+  /* "genome_info/kmers/kmer_reader.pyx":14
  * 
  * cdef kmer_count_t *_read_kmers(char *fname, labeled_aiarray_t *laia, int k, int last_n):
  *     cdef kmer_count_t *kc = interval_kmer_count(laia, fname, k, last_n)             # <<<<<<<<<<<<<<
  * 
  *     return kc
  */
   __pyx_v_kc = interval_kmer_count(__pyx_v_laia, __pyx_v_fname, __pyx_v_k, __pyx_v_last_n);
 
-  /* "genome_info/kmers/kmer_reader.pyx":15
+  /* "genome_info/kmers/kmer_reader.pyx":16
  *     cdef kmer_count_t *kc = interval_kmer_count(laia, fname, k, last_n)
  * 
  *     return kc             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = __pyx_v_kc;
   goto __pyx_L0;
 
-  /* "genome_info/kmers/kmer_reader.pyx":12
+  /* "genome_info/kmers/kmer_reader.pyx":13
  * 
  * 
  * cdef kmer_count_t *_read_kmers(char *fname, labeled_aiarray_t *laia, int k, int last_n):             # <<<<<<<<<<<<<<
  *     cdef kmer_count_t *kc = interval_kmer_count(laia, fname, k, last_n)
  * 
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "genome_info/kmers/kmer_reader.pyx":18
+/* "genome_info/kmers/kmer_reader.pyx":19
  * 
  * 
  * def read_kmers(str seq_fn, LabeledIntervalArray laia, int k, int last_n = 0):             # <<<<<<<<<<<<<<
  * 
  *     cdef str twobit_name = seq_fn
  */
 
@@ -3138,62 +3362,62 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_seq_fn)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_laia)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("read_kmers", 0, 3, 4, 1); __PYX_ERR(0, 18, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("read_kmers", 0, 3, 4, 1); __PYX_ERR(0, 19, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_k)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("read_kmers", 0, 3, 4, 2); __PYX_ERR(0, 18, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("read_kmers", 0, 3, 4, 2); __PYX_ERR(0, 19, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_last_n);
           if (value) { values[3] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "read_kmers") < 0)) __PYX_ERR(0, 18, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "read_kmers") < 0)) __PYX_ERR(0, 19, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  4: values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
         CYTHON_FALLTHROUGH;
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
         break;
         default: goto __pyx_L5_argtuple_error;
       }
     }
     __pyx_v_seq_fn = ((PyObject*)values[0]);
     __pyx_v_laia = ((struct __pyx_obj_6ailist_25LabeledIntervalArray_core_LabeledIntervalArray *)values[1]);
-    __pyx_v_k = __Pyx_PyInt_As_int(values[2]); if (unlikely((__pyx_v_k == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 18, __pyx_L3_error)
+    __pyx_v_k = __Pyx_PyInt_As_int(values[2]); if (unlikely((__pyx_v_k == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 19, __pyx_L3_error)
     if (values[3]) {
-      __pyx_v_last_n = __Pyx_PyInt_As_int(values[3]); if (unlikely((__pyx_v_last_n == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 18, __pyx_L3_error)
+      __pyx_v_last_n = __Pyx_PyInt_As_int(values[3]); if (unlikely((__pyx_v_last_n == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 19, __pyx_L3_error)
     } else {
       __pyx_v_last_n = ((int)0);
     }
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("read_kmers", 0, 3, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 18, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("read_kmers", 0, 3, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 19, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("genome_info.kmers.kmer_reader.read_kmers", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_seq_fn), (&PyUnicode_Type), 1, "seq_fn", 1))) __PYX_ERR(0, 18, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_laia), __pyx_ptype_6ailist_25LabeledIntervalArray_core_LabeledIntervalArray, 1, "laia", 0))) __PYX_ERR(0, 18, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_seq_fn), (&PyUnicode_Type), 1, "seq_fn", 1))) __PYX_ERR(0, 19, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_laia), __pyx_ptype_6ailist_25LabeledIntervalArray_core_LabeledIntervalArray, 1, "laia", 0))) __PYX_ERR(0, 19, __pyx_L1_error)
   __pyx_r = __pyx_pf_11genome_info_5kmers_11kmer_reader_read_kmers(__pyx_self, __pyx_v_seq_fn, __pyx_v_laia, __pyx_v_k, __pyx_v_last_n);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -3218,138 +3442,138 @@
   uint32_t __pyx_t_5;
   PyObject *__pyx_t_6 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("read_kmers", 0);
 
-  /* "genome_info/kmers/kmer_reader.pyx":20
+  /* "genome_info/kmers/kmer_reader.pyx":21
  * def read_kmers(str seq_fn, LabeledIntervalArray laia, int k, int last_n = 0):
  * 
  *     cdef str twobit_name = seq_fn             # <<<<<<<<<<<<<<
  *     cdef bytes fname = twobit_name.encode()
  *     cdef kmer_count_t *kc = _read_kmers(fname, laia.laia, k, last_n)
  */
   __Pyx_INCREF(__pyx_v_seq_fn);
   __pyx_v_twobit_name = __pyx_v_seq_fn;
 
-  /* "genome_info/kmers/kmer_reader.pyx":21
+  /* "genome_info/kmers/kmer_reader.pyx":22
  * 
  *     cdef str twobit_name = seq_fn
  *     cdef bytes fname = twobit_name.encode()             # <<<<<<<<<<<<<<
  *     cdef kmer_count_t *kc = _read_kmers(fname, laia.laia, k, last_n)
  * 
  */
   if (unlikely(__pyx_v_twobit_name == Py_None)) {
     PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "encode");
-    __PYX_ERR(0, 21, __pyx_L1_error)
+    __PYX_ERR(0, 22, __pyx_L1_error)
   }
-  __pyx_t_1 = PyUnicode_AsEncodedString(__pyx_v_twobit_name, NULL, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 21, __pyx_L1_error)
+  __pyx_t_1 = PyUnicode_AsEncodedString(__pyx_v_twobit_name, NULL, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 22, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_fname = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "genome_info/kmers/kmer_reader.pyx":22
+  /* "genome_info/kmers/kmer_reader.pyx":23
  *     cdef str twobit_name = seq_fn
  *     cdef bytes fname = twobit_name.encode()
  *     cdef kmer_count_t *kc = _read_kmers(fname, laia.laia, k, last_n)             # <<<<<<<<<<<<<<
  * 
  *     result = {}
  */
   if (unlikely(__pyx_v_fname == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "expected bytes, NoneType found");
-    __PYX_ERR(0, 22, __pyx_L1_error)
+    __PYX_ERR(0, 23, __pyx_L1_error)
   }
-  __pyx_t_2 = __Pyx_PyBytes_AsWritableString(__pyx_v_fname); if (unlikely((!__pyx_t_2) && PyErr_Occurred())) __PYX_ERR(0, 22, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyBytes_AsWritableString(__pyx_v_fname); if (unlikely((!__pyx_t_2) && PyErr_Occurred())) __PYX_ERR(0, 23, __pyx_L1_error)
   __pyx_v_kc = __pyx_f_11genome_info_5kmers_11kmer_reader__read_kmers(__pyx_t_2, __pyx_v_laia->laia, __pyx_v_k, __pyx_v_last_n);
 
-  /* "genome_info/kmers/kmer_reader.pyx":24
+  /* "genome_info/kmers/kmer_reader.pyx":25
  *     cdef kmer_count_t *kc = _read_kmers(fname, laia.laia, k, last_n)
  * 
  *     result = {}             # <<<<<<<<<<<<<<
  *     cdef bytes kmer_seq
  *     cdef int count
  */
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 24, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 25, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_result = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "genome_info/kmers/kmer_reader.pyx":28
+  /* "genome_info/kmers/kmer_reader.pyx":29
  *     cdef int count
  *     cdef uint32_t t
  *     for t in range(kc.n_kmers):             # <<<<<<<<<<<<<<
  *         kmer_seq = kc.kmers[t].name
  *         count = fetch_kmer(kc, kmer_seq)
  */
   __pyx_t_3 = __pyx_v_kc->n_kmers;
   __pyx_t_4 = __pyx_t_3;
   for (__pyx_t_5 = 0; __pyx_t_5 < __pyx_t_4; __pyx_t_5+=1) {
     __pyx_v_t = __pyx_t_5;
 
-    /* "genome_info/kmers/kmer_reader.pyx":29
+    /* "genome_info/kmers/kmer_reader.pyx":30
  *     cdef uint32_t t
  *     for t in range(kc.n_kmers):
  *         kmer_seq = kc.kmers[t].name             # <<<<<<<<<<<<<<
  *         count = fetch_kmer(kc, kmer_seq)
  * 
  */
-    __pyx_t_1 = __Pyx_PyBytes_FromString((__pyx_v_kc->kmers[__pyx_v_t]).name); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 29, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyBytes_FromString((__pyx_v_kc->kmers[__pyx_v_t]).name); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 30, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_XDECREF_SET(__pyx_v_kmer_seq, ((PyObject*)__pyx_t_1));
     __pyx_t_1 = 0;
 
-    /* "genome_info/kmers/kmer_reader.pyx":30
+    /* "genome_info/kmers/kmer_reader.pyx":31
  *     for t in range(kc.n_kmers):
  *         kmer_seq = kc.kmers[t].name
  *         count = fetch_kmer(kc, kmer_seq)             # <<<<<<<<<<<<<<
  * 
  *         result[kmer_seq.decode()] = count
  */
-    __pyx_t_2 = __Pyx_PyBytes_AsWritableString(__pyx_v_kmer_seq); if (unlikely((!__pyx_t_2) && PyErr_Occurred())) __PYX_ERR(0, 30, __pyx_L1_error)
+    __pyx_t_2 = __Pyx_PyBytes_AsWritableString(__pyx_v_kmer_seq); if (unlikely((!__pyx_t_2) && PyErr_Occurred())) __PYX_ERR(0, 31, __pyx_L1_error)
     __pyx_v_count = fetch_kmer(__pyx_v_kc, __pyx_t_2);
 
-    /* "genome_info/kmers/kmer_reader.pyx":32
+    /* "genome_info/kmers/kmer_reader.pyx":33
  *         count = fetch_kmer(kc, kmer_seq)
  * 
  *         result[kmer_seq.decode()] = count             # <<<<<<<<<<<<<<
  * 
  *     # Delete
  */
-    __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_count); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 32, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_count); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 33, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_6 = __Pyx_decode_bytes(__pyx_v_kmer_seq, 0, PY_SSIZE_T_MAX, NULL, NULL, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 32, __pyx_L1_error)
+    __pyx_t_6 = __Pyx_decode_bytes(__pyx_v_kmer_seq, 0, PY_SSIZE_T_MAX, NULL, NULL, NULL); if (unlikely(!__pyx_t_6)) __PYX_ERR(0, 33, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_6);
-    if (unlikely(PyDict_SetItem(__pyx_v_result, __pyx_t_6, __pyx_t_1) < 0)) __PYX_ERR(0, 32, __pyx_L1_error)
+    if (unlikely(PyDict_SetItem(__pyx_v_result, __pyx_t_6, __pyx_t_1) < 0)) __PYX_ERR(0, 33, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_6); __pyx_t_6 = 0;
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   }
 
-  /* "genome_info/kmers/kmer_reader.pyx":35
+  /* "genome_info/kmers/kmer_reader.pyx":36
  * 
  *     # Delete
  *     kmer_count_destroy(kc)             # <<<<<<<<<<<<<<
  * 
  *     return result
  */
   kmer_count_destroy(__pyx_v_kc);
 
-  /* "genome_info/kmers/kmer_reader.pyx":37
+  /* "genome_info/kmers/kmer_reader.pyx":38
  *     kmer_count_destroy(kc)
  * 
  *     return result             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_result);
   __pyx_r = __pyx_v_result;
   goto __pyx_L0;
 
-  /* "genome_info/kmers/kmer_reader.pyx":18
+  /* "genome_info/kmers/kmer_reader.pyx":19
  * 
  * 
  * def read_kmers(str seq_fn, LabeledIntervalArray laia, int k, int last_n = 0):             # <<<<<<<<<<<<<<
  * 
  *     cdef str twobit_name = seq_fn
  */
 
@@ -3365,15 +3589,15 @@
   __Pyx_XDECREF(__pyx_v_result);
   __Pyx_XDECREF(__pyx_v_kmer_seq);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "genome_info/kmers/kmer_reader.pyx":40
+/* "genome_info/kmers/kmer_reader.pyx":41
  * 
  * 
  * cdef bytes _fetch_sequence(char *fname, char *name, int start, int end):             # <<<<<<<<<<<<<<
  *     cdef bytes seq = fetch_sequence(fname, name, start, end)
  * 
  */
 
@@ -3383,39 +3607,39 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_fetch_sequence", 0);
 
-  /* "genome_info/kmers/kmer_reader.pyx":41
+  /* "genome_info/kmers/kmer_reader.pyx":42
  * 
  * cdef bytes _fetch_sequence(char *fname, char *name, int start, int end):
  *     cdef bytes seq = fetch_sequence(fname, name, start, end)             # <<<<<<<<<<<<<<
  * 
  *     return seq
  */
-  __pyx_t_1 = __Pyx_PyBytes_FromString(fetch_sequence(__pyx_v_fname, __pyx_v_name, __pyx_v_start, __pyx_v_end)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 41, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyBytes_FromString(fetch_sequence(__pyx_v_fname, __pyx_v_name, __pyx_v_start, __pyx_v_end)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 42, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_seq = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "genome_info/kmers/kmer_reader.pyx":43
+  /* "genome_info/kmers/kmer_reader.pyx":44
  *     cdef bytes seq = fetch_sequence(fname, name, start, end)
  * 
  *     return seq             # <<<<<<<<<<<<<<
  * 
  * def read_sequence(str seq_fn, str chrom, int start, int end):
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_seq);
   __pyx_r = __pyx_v_seq;
   goto __pyx_L0;
 
-  /* "genome_info/kmers/kmer_reader.pyx":40
+  /* "genome_info/kmers/kmer_reader.pyx":41
  * 
  * 
  * cdef bytes _fetch_sequence(char *fname, char *name, int start, int end):             # <<<<<<<<<<<<<<
  *     cdef bytes seq = fetch_sequence(fname, name, start, end)
  * 
  */
 
@@ -3427,15 +3651,15 @@
   __pyx_L0:;
   __Pyx_XDECREF(__pyx_v_seq);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "genome_info/kmers/kmer_reader.pyx":45
+/* "genome_info/kmers/kmer_reader.pyx":46
  *     return seq
  * 
  * def read_sequence(str seq_fn, str chrom, int start, int end):             # <<<<<<<<<<<<<<
  * 
  *     cdef str twobit_name = seq_fn
  */
 
@@ -3477,55 +3701,55 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_seq_fn)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_chrom)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("read_sequence", 1, 4, 4, 1); __PYX_ERR(0, 45, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("read_sequence", 1, 4, 4, 1); __PYX_ERR(0, 46, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_start)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("read_sequence", 1, 4, 4, 2); __PYX_ERR(0, 45, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("read_sequence", 1, 4, 4, 2); __PYX_ERR(0, 46, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  3:
         if (likely((values[3] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_end)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("read_sequence", 1, 4, 4, 3); __PYX_ERR(0, 45, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("read_sequence", 1, 4, 4, 3); __PYX_ERR(0, 46, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "read_sequence") < 0)) __PYX_ERR(0, 45, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "read_sequence") < 0)) __PYX_ERR(0, 46, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 4) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
       values[3] = PyTuple_GET_ITEM(__pyx_args, 3);
     }
     __pyx_v_seq_fn = ((PyObject*)values[0]);
     __pyx_v_chrom = ((PyObject*)values[1]);
-    __pyx_v_start = __Pyx_PyInt_As_int(values[2]); if (unlikely((__pyx_v_start == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 45, __pyx_L3_error)
-    __pyx_v_end = __Pyx_PyInt_As_int(values[3]); if (unlikely((__pyx_v_end == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 45, __pyx_L3_error)
+    __pyx_v_start = __Pyx_PyInt_As_int(values[2]); if (unlikely((__pyx_v_start == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 46, __pyx_L3_error)
+    __pyx_v_end = __Pyx_PyInt_As_int(values[3]); if (unlikely((__pyx_v_end == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 46, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("read_sequence", 1, 4, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 45, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("read_sequence", 1, 4, 4, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 46, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("genome_info.kmers.kmer_reader.read_sequence", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_seq_fn), (&PyUnicode_Type), 1, "seq_fn", 1))) __PYX_ERR(0, 45, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_chrom), (&PyUnicode_Type), 1, "chrom", 1))) __PYX_ERR(0, 45, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_seq_fn), (&PyUnicode_Type), 1, "seq_fn", 1))) __PYX_ERR(0, 46, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_chrom), (&PyUnicode_Type), 1, "chrom", 1))) __PYX_ERR(0, 46, __pyx_L1_error)
   __pyx_r = __pyx_pf_11genome_info_5kmers_11kmer_reader_2read_sequence(__pyx_self, __pyx_v_seq_fn, __pyx_v_chrom, __pyx_v_start, __pyx_v_end);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -3545,107 +3769,107 @@
   char *__pyx_t_2;
   char *__pyx_t_3;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("read_sequence", 0);
 
-  /* "genome_info/kmers/kmer_reader.pyx":47
+  /* "genome_info/kmers/kmer_reader.pyx":48
  * def read_sequence(str seq_fn, str chrom, int start, int end):
  * 
  *     cdef str twobit_name = seq_fn             # <<<<<<<<<<<<<<
  *     cdef bytes fname = twobit_name.encode()
  *     cdef bytes name = chrom.encode()
  */
   __Pyx_INCREF(__pyx_v_seq_fn);
   __pyx_v_twobit_name = __pyx_v_seq_fn;
 
-  /* "genome_info/kmers/kmer_reader.pyx":48
+  /* "genome_info/kmers/kmer_reader.pyx":49
  * 
  *     cdef str twobit_name = seq_fn
  *     cdef bytes fname = twobit_name.encode()             # <<<<<<<<<<<<<<
  *     cdef bytes name = chrom.encode()
  * 
  */
   if (unlikely(__pyx_v_twobit_name == Py_None)) {
     PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "encode");
-    __PYX_ERR(0, 48, __pyx_L1_error)
+    __PYX_ERR(0, 49, __pyx_L1_error)
   }
-  __pyx_t_1 = PyUnicode_AsEncodedString(__pyx_v_twobit_name, NULL, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 48, __pyx_L1_error)
+  __pyx_t_1 = PyUnicode_AsEncodedString(__pyx_v_twobit_name, NULL, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 49, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_fname = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "genome_info/kmers/kmer_reader.pyx":49
+  /* "genome_info/kmers/kmer_reader.pyx":50
  *     cdef str twobit_name = seq_fn
  *     cdef bytes fname = twobit_name.encode()
  *     cdef bytes name = chrom.encode()             # <<<<<<<<<<<<<<
  * 
  *     cdef bytes seq = _fetch_sequence(fname, name, start, end)
  */
   if (unlikely(__pyx_v_chrom == Py_None)) {
     PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "encode");
-    __PYX_ERR(0, 49, __pyx_L1_error)
+    __PYX_ERR(0, 50, __pyx_L1_error)
   }
-  __pyx_t_1 = PyUnicode_AsEncodedString(__pyx_v_chrom, NULL, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 49, __pyx_L1_error)
+  __pyx_t_1 = PyUnicode_AsEncodedString(__pyx_v_chrom, NULL, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 50, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_name = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "genome_info/kmers/kmer_reader.pyx":51
+  /* "genome_info/kmers/kmer_reader.pyx":52
  *     cdef bytes name = chrom.encode()
  * 
  *     cdef bytes seq = _fetch_sequence(fname, name, start, end)             # <<<<<<<<<<<<<<
  *     cdef str py_seq = seq.decode()
  * 
  */
   if (unlikely(__pyx_v_fname == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "expected bytes, NoneType found");
-    __PYX_ERR(0, 51, __pyx_L1_error)
+    __PYX_ERR(0, 52, __pyx_L1_error)
   }
-  __pyx_t_2 = __Pyx_PyBytes_AsWritableString(__pyx_v_fname); if (unlikely((!__pyx_t_2) && PyErr_Occurred())) __PYX_ERR(0, 51, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyBytes_AsWritableString(__pyx_v_fname); if (unlikely((!__pyx_t_2) && PyErr_Occurred())) __PYX_ERR(0, 52, __pyx_L1_error)
   if (unlikely(__pyx_v_name == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "expected bytes, NoneType found");
-    __PYX_ERR(0, 51, __pyx_L1_error)
+    __PYX_ERR(0, 52, __pyx_L1_error)
   }
-  __pyx_t_3 = __Pyx_PyBytes_AsWritableString(__pyx_v_name); if (unlikely((!__pyx_t_3) && PyErr_Occurred())) __PYX_ERR(0, 51, __pyx_L1_error)
-  __pyx_t_1 = __pyx_f_11genome_info_5kmers_11kmer_reader__fetch_sequence(__pyx_t_2, __pyx_t_3, __pyx_v_start, __pyx_v_end); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 51, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyBytes_AsWritableString(__pyx_v_name); if (unlikely((!__pyx_t_3) && PyErr_Occurred())) __PYX_ERR(0, 52, __pyx_L1_error)
+  __pyx_t_1 = __pyx_f_11genome_info_5kmers_11kmer_reader__fetch_sequence(__pyx_t_2, __pyx_t_3, __pyx_v_start, __pyx_v_end); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 52, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_seq = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "genome_info/kmers/kmer_reader.pyx":52
+  /* "genome_info/kmers/kmer_reader.pyx":53
  * 
  *     cdef bytes seq = _fetch_sequence(fname, name, start, end)
  *     cdef str py_seq = seq.decode()             # <<<<<<<<<<<<<<
  * 
  *     return py_seq
  */
   if (unlikely(__pyx_v_seq == Py_None)) {
     PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "decode");
-    __PYX_ERR(0, 52, __pyx_L1_error)
+    __PYX_ERR(0, 53, __pyx_L1_error)
   }
-  __pyx_t_1 = __Pyx_decode_bytes(__pyx_v_seq, 0, PY_SSIZE_T_MAX, NULL, NULL, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 52, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_decode_bytes(__pyx_v_seq, 0, PY_SSIZE_T_MAX, NULL, NULL, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 53, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_py_seq = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "genome_info/kmers/kmer_reader.pyx":54
+  /* "genome_info/kmers/kmer_reader.pyx":55
  *     cdef str py_seq = seq.decode()
  * 
  *     return py_seq             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(__pyx_v_py_seq);
   __pyx_r = __pyx_v_py_seq;
   goto __pyx_L0;
 
-  /* "genome_info/kmers/kmer_reader.pyx":45
+  /* "genome_info/kmers/kmer_reader.pyx":46
  *     return seq
  * 
  * def read_sequence(str seq_fn, str chrom, int start, int end):             # <<<<<<<<<<<<<<
  * 
  *     cdef str twobit_name = seq_fn
  */
 
@@ -3661,15 +3885,15 @@
   __Pyx_XDECREF(__pyx_v_seq);
   __Pyx_XDECREF(__pyx_v_py_seq);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "genome_info/kmers/kmer_reader.pyx":57
+/* "genome_info/kmers/kmer_reader.pyx":58
  * 
  * 
  * cdef void _gc_percent(char *fname, labeled_aiarray_t *laia, float[::1] gc):             # <<<<<<<<<<<<<<
  *     gc_content(laia, fname, &gc[0])
  * 
  */
 
@@ -3678,58 +3902,58 @@
   Py_ssize_t __pyx_t_1;
   int __pyx_t_2;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_gc_percent", 0);
 
-  /* "genome_info/kmers/kmer_reader.pyx":58
+  /* "genome_info/kmers/kmer_reader.pyx":59
  * 
  * cdef void _gc_percent(char *fname, labeled_aiarray_t *laia, float[::1] gc):
  *     gc_content(laia, fname, &gc[0])             # <<<<<<<<<<<<<<
  * 
  *     return
  */
   __pyx_t_1 = 0;
   __pyx_t_2 = -1;
   if (__pyx_t_1 < 0) {
     __pyx_t_1 += __pyx_v_gc.shape[0];
     if (unlikely(__pyx_t_1 < 0)) __pyx_t_2 = 0;
   } else if (unlikely(__pyx_t_1 >= __pyx_v_gc.shape[0])) __pyx_t_2 = 0;
   if (unlikely(__pyx_t_2 != -1)) {
     __Pyx_RaiseBufferIndexError(__pyx_t_2);
-    __PYX_ERR(0, 58, __pyx_L1_error)
+    __PYX_ERR(0, 59, __pyx_L1_error)
   }
   gc_content(__pyx_v_laia, __pyx_v_fname, (&(*((float *) ( /* dim=0 */ ((char *) (((float *) __pyx_v_gc.data) + __pyx_t_1)) )))));
 
-  /* "genome_info/kmers/kmer_reader.pyx":60
+  /* "genome_info/kmers/kmer_reader.pyx":61
  *     gc_content(laia, fname, &gc[0])
  * 
  *     return             # <<<<<<<<<<<<<<
  * 
  * 
  */
   goto __pyx_L0;
 
-  /* "genome_info/kmers/kmer_reader.pyx":57
+  /* "genome_info/kmers/kmer_reader.pyx":58
  * 
  * 
  * cdef void _gc_percent(char *fname, labeled_aiarray_t *laia, float[::1] gc):             # <<<<<<<<<<<<<<
  *     gc_content(laia, fname, &gc[0])
  * 
  */
 
   /* function exit code */
   __pyx_L1_error:;
   __Pyx_WriteUnraisable("genome_info.kmers.kmer_reader._gc_percent", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
 }
 
-/* "genome_info/kmers/kmer_reader.pyx":63
+/* "genome_info/kmers/kmer_reader.pyx":64
  * 
  * 
  * def gc_percent(str seq_fn, LabeledIntervalArray laia, str genome_version = "hg38"):             # <<<<<<<<<<<<<<
  *     cdef str twobit_name = seq_fn
  *     cdef bytes fname = twobit_name.encode()
  */
 
@@ -3769,25 +3993,25 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_seq_fn)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_laia)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("gc_percent", 0, 2, 3, 1); __PYX_ERR(0, 63, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("gc_percent", 0, 2, 3, 1); __PYX_ERR(0, 64, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (kw_args > 0) {
           PyObject* value = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_genome_version);
           if (value) { values[2] = value; kw_args--; }
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "gc_percent") < 0)) __PYX_ERR(0, 63, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "gc_percent") < 0)) __PYX_ERR(0, 64, __pyx_L3_error)
       }
     } else {
       switch (PyTuple_GET_SIZE(__pyx_args)) {
         case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
         CYTHON_FALLTHROUGH;
         case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
         values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
@@ -3797,23 +4021,23 @@
     }
     __pyx_v_seq_fn = ((PyObject*)values[0]);
     __pyx_v_laia = ((struct __pyx_obj_6ailist_25LabeledIntervalArray_core_LabeledIntervalArray *)values[1]);
     __pyx_v_genome_version = ((PyObject*)values[2]);
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("gc_percent", 0, 2, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 63, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("gc_percent", 0, 2, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 64, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("genome_info.kmers.kmer_reader.gc_percent", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_seq_fn), (&PyUnicode_Type), 1, "seq_fn", 1))) __PYX_ERR(0, 63, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_laia), __pyx_ptype_6ailist_25LabeledIntervalArray_core_LabeledIntervalArray, 1, "laia", 0))) __PYX_ERR(0, 63, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_genome_version), (&PyUnicode_Type), 1, "genome_version", 1))) __PYX_ERR(0, 63, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_seq_fn), (&PyUnicode_Type), 1, "seq_fn", 1))) __PYX_ERR(0, 64, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_laia), __pyx_ptype_6ailist_25LabeledIntervalArray_core_LabeledIntervalArray, 1, "laia", 0))) __PYX_ERR(0, 64, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_genome_version), (&PyUnicode_Type), 1, "genome_version", 1))) __PYX_ERR(0, 64, __pyx_L1_error)
   __pyx_r = __pyx_pf_11genome_info_5kmers_11kmer_reader_4gc_percent(__pyx_self, __pyx_v_seq_fn, __pyx_v_laia, __pyx_v_genome_version);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -3836,116 +4060,116 @@
   __Pyx_memviewslice __pyx_t_6 = { 0, 0, { 0 }, { 0 }, { 0 } };
   char *__pyx_t_7;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("gc_percent", 0);
 
-  /* "genome_info/kmers/kmer_reader.pyx":64
+  /* "genome_info/kmers/kmer_reader.pyx":65
  * 
  * def gc_percent(str seq_fn, LabeledIntervalArray laia, str genome_version = "hg38"):
  *     cdef str twobit_name = seq_fn             # <<<<<<<<<<<<<<
  *     cdef bytes fname = twobit_name.encode()
  * 
  */
   __Pyx_INCREF(__pyx_v_seq_fn);
   __pyx_v_twobit_name = __pyx_v_seq_fn;
 
-  /* "genome_info/kmers/kmer_reader.pyx":65
+  /* "genome_info/kmers/kmer_reader.pyx":66
  * def gc_percent(str seq_fn, LabeledIntervalArray laia, str genome_version = "hg38"):
  *     cdef str twobit_name = seq_fn
  *     cdef bytes fname = twobit_name.encode()             # <<<<<<<<<<<<<<
  * 
  *     cdef np.ndarray gc = np.zeros(laia.size, dtype=np.single)
  */
   if (unlikely(__pyx_v_twobit_name == Py_None)) {
     PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "encode");
-    __PYX_ERR(0, 65, __pyx_L1_error)
+    __PYX_ERR(0, 66, __pyx_L1_error)
   }
-  __pyx_t_1 = PyUnicode_AsEncodedString(__pyx_v_twobit_name, NULL, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 65, __pyx_L1_error)
+  __pyx_t_1 = PyUnicode_AsEncodedString(__pyx_v_twobit_name, NULL, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 66, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_fname = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "genome_info/kmers/kmer_reader.pyx":67
+  /* "genome_info/kmers/kmer_reader.pyx":68
  *     cdef bytes fname = twobit_name.encode()
  * 
  *     cdef np.ndarray gc = np.zeros(laia.size, dtype=np.single)             # <<<<<<<<<<<<<<
  *     cdef float[::1] gc_mem = gc
  * 
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 67, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 68, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_zeros); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 67, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_zeros); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 68, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_laia), __pyx_n_s_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 67, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_laia), __pyx_n_s_size); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 68, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 67, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 68, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_t_1);
   __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 67, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 68, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 67, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 68, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_single); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 67, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_single); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 68, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_dtype, __pyx_t_5) < 0) __PYX_ERR(0, 67, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_dtype, __pyx_t_5) < 0) __PYX_ERR(0, 68, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_5); __pyx_t_5 = 0;
-  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_3, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 67, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_3, __pyx_t_1); if (unlikely(!__pyx_t_5)) __PYX_ERR(0, 68, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_5);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (!(likely(((__pyx_t_5) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_5, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 67, __pyx_L1_error)
+  if (!(likely(((__pyx_t_5) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_5, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 68, __pyx_L1_error)
   __pyx_v_gc = ((PyArrayObject *)__pyx_t_5);
   __pyx_t_5 = 0;
 
-  /* "genome_info/kmers/kmer_reader.pyx":68
+  /* "genome_info/kmers/kmer_reader.pyx":69
  * 
  *     cdef np.ndarray gc = np.zeros(laia.size, dtype=np.single)
  *     cdef float[::1] gc_mem = gc             # <<<<<<<<<<<<<<
  * 
  *     _gc_percent(fname, laia.laia, gc_mem)
  */
-  __pyx_t_6 = __Pyx_PyObject_to_MemoryviewSlice_dc_float(((PyObject *)__pyx_v_gc), PyBUF_WRITABLE); if (unlikely(!__pyx_t_6.memview)) __PYX_ERR(0, 68, __pyx_L1_error)
+  __pyx_t_6 = __Pyx_PyObject_to_MemoryviewSlice_dc_float(((PyObject *)__pyx_v_gc), PyBUF_WRITABLE); if (unlikely(!__pyx_t_6.memview)) __PYX_ERR(0, 69, __pyx_L1_error)
   __pyx_v_gc_mem = __pyx_t_6;
   __pyx_t_6.memview = NULL;
   __pyx_t_6.data = NULL;
 
-  /* "genome_info/kmers/kmer_reader.pyx":70
+  /* "genome_info/kmers/kmer_reader.pyx":71
  *     cdef float[::1] gc_mem = gc
  * 
  *     _gc_percent(fname, laia.laia, gc_mem)             # <<<<<<<<<<<<<<
  * 
  *     return gc
  */
   if (unlikely(__pyx_v_fname == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "expected bytes, NoneType found");
-    __PYX_ERR(0, 70, __pyx_L1_error)
+    __PYX_ERR(0, 71, __pyx_L1_error)
   }
-  __pyx_t_7 = __Pyx_PyBytes_AsWritableString(__pyx_v_fname); if (unlikely((!__pyx_t_7) && PyErr_Occurred())) __PYX_ERR(0, 70, __pyx_L1_error)
+  __pyx_t_7 = __Pyx_PyBytes_AsWritableString(__pyx_v_fname); if (unlikely((!__pyx_t_7) && PyErr_Occurred())) __PYX_ERR(0, 71, __pyx_L1_error)
   __pyx_f_11genome_info_5kmers_11kmer_reader__gc_percent(__pyx_t_7, __pyx_v_laia->laia, __pyx_v_gc_mem);
 
-  /* "genome_info/kmers/kmer_reader.pyx":72
+  /* "genome_info/kmers/kmer_reader.pyx":73
  *     _gc_percent(fname, laia.laia, gc_mem)
  * 
  *     return gc             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_gc));
   __pyx_r = ((PyObject *)__pyx_v_gc);
   goto __pyx_L0;
 
-  /* "genome_info/kmers/kmer_reader.pyx":63
+  /* "genome_info/kmers/kmer_reader.pyx":64
  * 
  * 
  * def gc_percent(str seq_fn, LabeledIntervalArray laia, str genome_version = "hg38"):             # <<<<<<<<<<<<<<
  *     cdef str twobit_name = seq_fn
  *     cdef bytes fname = twobit_name.encode()
  */
 
@@ -3965,15 +4189,15 @@
   __Pyx_XDECREF((PyObject *)__pyx_v_gc);
   __PYX_XDEC_MEMVIEW(&__pyx_v_gc_mem, 1);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "genome_info/kmers/kmer_reader.pyx":75
+/* "genome_info/kmers/kmer_reader.pyx":76
  * 
  * 
  * def read_bounds_base_freq(str seq_fn, LabeledIntervalArray laia, int n_bases):             # <<<<<<<<<<<<<<
  * 
  *     cdef str twobit_name = seq_fn
  */
 
@@ -4012,47 +4236,47 @@
         case  0:
         if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_seq_fn)) != 0)) kw_args--;
         else goto __pyx_L5_argtuple_error;
         CYTHON_FALLTHROUGH;
         case  1:
         if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_laia)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("read_bounds_base_freq", 1, 3, 3, 1); __PYX_ERR(0, 75, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("read_bounds_base_freq", 1, 3, 3, 1); __PYX_ERR(0, 76, __pyx_L3_error)
         }
         CYTHON_FALLTHROUGH;
         case  2:
         if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_n_bases)) != 0)) kw_args--;
         else {
-          __Pyx_RaiseArgtupleInvalid("read_bounds_base_freq", 1, 3, 3, 2); __PYX_ERR(0, 75, __pyx_L3_error)
+          __Pyx_RaiseArgtupleInvalid("read_bounds_base_freq", 1, 3, 3, 2); __PYX_ERR(0, 76, __pyx_L3_error)
         }
       }
       if (unlikely(kw_args > 0)) {
-        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "read_bounds_base_freq") < 0)) __PYX_ERR(0, 75, __pyx_L3_error)
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "read_bounds_base_freq") < 0)) __PYX_ERR(0, 76, __pyx_L3_error)
       }
     } else if (PyTuple_GET_SIZE(__pyx_args) != 3) {
       goto __pyx_L5_argtuple_error;
     } else {
       values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
       values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
       values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
     }
     __pyx_v_seq_fn = ((PyObject*)values[0]);
     __pyx_v_laia = ((struct __pyx_obj_6ailist_25LabeledIntervalArray_core_LabeledIntervalArray *)values[1]);
-    __pyx_v_n_bases = __Pyx_PyInt_As_int(values[2]); if (unlikely((__pyx_v_n_bases == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 75, __pyx_L3_error)
+    __pyx_v_n_bases = __Pyx_PyInt_As_int(values[2]); if (unlikely((__pyx_v_n_bases == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 76, __pyx_L3_error)
   }
   goto __pyx_L4_argument_unpacking_done;
   __pyx_L5_argtuple_error:;
-  __Pyx_RaiseArgtupleInvalid("read_bounds_base_freq", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 75, __pyx_L3_error)
+  __Pyx_RaiseArgtupleInvalid("read_bounds_base_freq", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 76, __pyx_L3_error)
   __pyx_L3_error:;
   __Pyx_AddTraceback("genome_info.kmers.kmer_reader.read_bounds_base_freq", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __Pyx_RefNannyFinishContext();
   return NULL;
   __pyx_L4_argument_unpacking_done:;
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_seq_fn), (&PyUnicode_Type), 1, "seq_fn", 1))) __PYX_ERR(0, 75, __pyx_L1_error)
-  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_laia), __pyx_ptype_6ailist_25LabeledIntervalArray_core_LabeledIntervalArray, 1, "laia", 0))) __PYX_ERR(0, 75, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_seq_fn), (&PyUnicode_Type), 1, "seq_fn", 1))) __PYX_ERR(0, 76, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_laia), __pyx_ptype_6ailist_25LabeledIntervalArray_core_LabeledIntervalArray, 1, "laia", 0))) __PYX_ERR(0, 76, __pyx_L1_error)
   __pyx_r = __pyx_pf_11genome_info_5kmers_11kmer_reader_6read_bounds_base_freq(__pyx_self, __pyx_v_seq_fn, __pyx_v_laia, __pyx_v_n_bases);
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __pyx_r = NULL;
   __pyx_L0:;
@@ -4078,359 +4302,359 @@
   int __pyx_t_7;
   int __pyx_t_8;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("read_bounds_base_freq", 0);
 
-  /* "genome_info/kmers/kmer_reader.pyx":77
+  /* "genome_info/kmers/kmer_reader.pyx":78
  * def read_bounds_base_freq(str seq_fn, LabeledIntervalArray laia, int n_bases):
  * 
  *     cdef str twobit_name = seq_fn             # <<<<<<<<<<<<<<
  *     cdef bytes fname = twobit_name.encode()
  * 
  */
   __Pyx_INCREF(__pyx_v_seq_fn);
   __pyx_v_twobit_name = __pyx_v_seq_fn;
 
-  /* "genome_info/kmers/kmer_reader.pyx":78
+  /* "genome_info/kmers/kmer_reader.pyx":79
  * 
  *     cdef str twobit_name = seq_fn
  *     cdef bytes fname = twobit_name.encode()             # <<<<<<<<<<<<<<
  * 
  *     cdef np.ndarray start_freq = np.zeros((4, n_bases), dtype=float)
  */
   if (unlikely(__pyx_v_twobit_name == Py_None)) {
     PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "encode");
-    __PYX_ERR(0, 78, __pyx_L1_error)
+    __PYX_ERR(0, 79, __pyx_L1_error)
   }
-  __pyx_t_1 = PyUnicode_AsEncodedString(__pyx_v_twobit_name, NULL, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 78, __pyx_L1_error)
+  __pyx_t_1 = PyUnicode_AsEncodedString(__pyx_v_twobit_name, NULL, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 79, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_v_fname = ((PyObject*)__pyx_t_1);
   __pyx_t_1 = 0;
 
-  /* "genome_info/kmers/kmer_reader.pyx":80
+  /* "genome_info/kmers/kmer_reader.pyx":81
  *     cdef bytes fname = twobit_name.encode()
  * 
  *     cdef np.ndarray start_freq = np.zeros((4, n_bases), dtype=float)             # <<<<<<<<<<<<<<
  *     cdef np.ndarray end_freq = np.zeros((4, n_bases), dtype=float)
  *     cdef interval_base_freq_t *ibf = read_interval_base_freq(laia.laia, fname, n_bases)
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 80, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 81, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_zeros); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 80, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_zeros); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 81, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_n_bases); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 80, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_n_bases); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 81, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 80, __pyx_L1_error)
+  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 81, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_INCREF(__pyx_int_4);
   __Pyx_GIVEREF(__pyx_int_4);
   PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_int_4);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_1);
   __pyx_t_1 = 0;
-  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 80, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 81, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_GIVEREF(__pyx_t_3);
   PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_3);
   __pyx_t_3 = 0;
-  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 80, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 81, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
-  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_dtype, ((PyObject *)(&PyFloat_Type))) < 0) __PYX_ERR(0, 80, __pyx_L1_error)
-  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_1, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 80, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_dtype, ((PyObject *)(&PyFloat_Type))) < 0) __PYX_ERR(0, 81, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_1, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 81, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
-  if (!(likely(((__pyx_t_4) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_4, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 80, __pyx_L1_error)
+  if (!(likely(((__pyx_t_4) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_4, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 81, __pyx_L1_error)
   __pyx_v_start_freq = ((PyArrayObject *)__pyx_t_4);
   __pyx_t_4 = 0;
 
-  /* "genome_info/kmers/kmer_reader.pyx":81
+  /* "genome_info/kmers/kmer_reader.pyx":82
  * 
  *     cdef np.ndarray start_freq = np.zeros((4, n_bases), dtype=float)
  *     cdef np.ndarray end_freq = np.zeros((4, n_bases), dtype=float)             # <<<<<<<<<<<<<<
  *     cdef interval_base_freq_t *ibf = read_interval_base_freq(laia.laia, fname, n_bases)
  *     cdef int i
  */
-  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 81, __pyx_L1_error)
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 82, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_zeros); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 81, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_zeros); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 82, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_3);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
-  __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_n_bases); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 81, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_n_bases); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 82, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
-  __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 81, __pyx_L1_error)
+  __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 82, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_int_4);
   __Pyx_GIVEREF(__pyx_int_4);
   PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_int_4);
   __Pyx_GIVEREF(__pyx_t_4);
   PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_4);
   __pyx_t_4 = 0;
-  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 81, __pyx_L1_error)
+  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 82, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __Pyx_GIVEREF(__pyx_t_1);
   PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_1);
   __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 81, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 82, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_dtype, ((PyObject *)(&PyFloat_Type))) < 0) __PYX_ERR(0, 81, __pyx_L1_error)
-  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_4, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 81, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_dtype, ((PyObject *)(&PyFloat_Type))) < 0) __PYX_ERR(0, 82, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_4, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 82, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  if (!(likely(((__pyx_t_2) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_2, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 81, __pyx_L1_error)
+  if (!(likely(((__pyx_t_2) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_2, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 82, __pyx_L1_error)
   __pyx_v_end_freq = ((PyArrayObject *)__pyx_t_2);
   __pyx_t_2 = 0;
 
-  /* "genome_info/kmers/kmer_reader.pyx":82
+  /* "genome_info/kmers/kmer_reader.pyx":83
  *     cdef np.ndarray start_freq = np.zeros((4, n_bases), dtype=float)
  *     cdef np.ndarray end_freq = np.zeros((4, n_bases), dtype=float)
  *     cdef interval_base_freq_t *ibf = read_interval_base_freq(laia.laia, fname, n_bases)             # <<<<<<<<<<<<<<
  *     cdef int i
  *     for i in range(n_bases):
  */
   if (unlikely(__pyx_v_fname == Py_None)) {
     PyErr_SetString(PyExc_TypeError, "expected bytes, NoneType found");
-    __PYX_ERR(0, 82, __pyx_L1_error)
+    __PYX_ERR(0, 83, __pyx_L1_error)
   }
-  __pyx_t_5 = __Pyx_PyBytes_AsWritableString(__pyx_v_fname); if (unlikely((!__pyx_t_5) && PyErr_Occurred())) __PYX_ERR(0, 82, __pyx_L1_error)
+  __pyx_t_5 = __Pyx_PyBytes_AsWritableString(__pyx_v_fname); if (unlikely((!__pyx_t_5) && PyErr_Occurred())) __PYX_ERR(0, 83, __pyx_L1_error)
   __pyx_v_ibf = read_interval_base_freq(__pyx_v_laia->laia, __pyx_t_5, __pyx_v_n_bases);
 
-  /* "genome_info/kmers/kmer_reader.pyx":84
+  /* "genome_info/kmers/kmer_reader.pyx":85
  *     cdef interval_base_freq_t *ibf = read_interval_base_freq(laia.laia, fname, n_bases)
  *     cdef int i
  *     for i in range(n_bases):             # <<<<<<<<<<<<<<
  *         start_freq[0, i] = ibf.start.A[i]
  *         start_freq[1, i] = ibf.start.T[i]
  */
   __pyx_t_6 = __pyx_v_n_bases;
   __pyx_t_7 = __pyx_t_6;
   for (__pyx_t_8 = 0; __pyx_t_8 < __pyx_t_7; __pyx_t_8+=1) {
     __pyx_v_i = __pyx_t_8;
 
-    /* "genome_info/kmers/kmer_reader.pyx":85
+    /* "genome_info/kmers/kmer_reader.pyx":86
  *     cdef int i
  *     for i in range(n_bases):
  *         start_freq[0, i] = ibf.start.A[i]             # <<<<<<<<<<<<<<
  *         start_freq[1, i] = ibf.start.T[i]
  *         start_freq[2, i] = ibf.start.G[i]
  */
-    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->start->A[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 85, __pyx_L1_error)
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->start->A[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 86, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 85, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 86, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 85, __pyx_L1_error)
+    __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 86, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_INCREF(__pyx_int_0);
     __Pyx_GIVEREF(__pyx_int_0);
     PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_int_0);
     __Pyx_GIVEREF(__pyx_t_1);
     PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_1);
     __pyx_t_1 = 0;
-    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_start_freq), __pyx_t_4, __pyx_t_2) < 0)) __PYX_ERR(0, 85, __pyx_L1_error)
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_start_freq), __pyx_t_4, __pyx_t_2) < 0)) __PYX_ERR(0, 86, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "genome_info/kmers/kmer_reader.pyx":86
+    /* "genome_info/kmers/kmer_reader.pyx":87
  *     for i in range(n_bases):
  *         start_freq[0, i] = ibf.start.A[i]
  *         start_freq[1, i] = ibf.start.T[i]             # <<<<<<<<<<<<<<
  *         start_freq[2, i] = ibf.start.G[i]
  *         start_freq[3, i] = ibf.start.C[i]
  */
-    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->start->T[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 86, __pyx_L1_error)
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->start->T[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 87, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 86, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 87, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 86, __pyx_L1_error)
+    __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 87, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(__pyx_int_1);
     __Pyx_GIVEREF(__pyx_int_1);
     PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_int_1);
     __Pyx_GIVEREF(__pyx_t_4);
     PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_4);
     __pyx_t_4 = 0;
-    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_start_freq), __pyx_t_1, __pyx_t_2) < 0)) __PYX_ERR(0, 86, __pyx_L1_error)
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_start_freq), __pyx_t_1, __pyx_t_2) < 0)) __PYX_ERR(0, 87, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "genome_info/kmers/kmer_reader.pyx":87
+    /* "genome_info/kmers/kmer_reader.pyx":88
  *         start_freq[0, i] = ibf.start.A[i]
  *         start_freq[1, i] = ibf.start.T[i]
  *         start_freq[2, i] = ibf.start.G[i]             # <<<<<<<<<<<<<<
  *         start_freq[3, i] = ibf.start.C[i]
  *         end_freq[0, i] = ibf.end.A[i]
  */
-    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->start->G[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 87, __pyx_L1_error)
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->start->G[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 88, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 87, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 88, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 87, __pyx_L1_error)
+    __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 88, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_INCREF(__pyx_int_2);
     __Pyx_GIVEREF(__pyx_int_2);
     PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_int_2);
     __Pyx_GIVEREF(__pyx_t_1);
     PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_1);
     __pyx_t_1 = 0;
-    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_start_freq), __pyx_t_4, __pyx_t_2) < 0)) __PYX_ERR(0, 87, __pyx_L1_error)
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_start_freq), __pyx_t_4, __pyx_t_2) < 0)) __PYX_ERR(0, 88, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "genome_info/kmers/kmer_reader.pyx":88
+    /* "genome_info/kmers/kmer_reader.pyx":89
  *         start_freq[1, i] = ibf.start.T[i]
  *         start_freq[2, i] = ibf.start.G[i]
  *         start_freq[3, i] = ibf.start.C[i]             # <<<<<<<<<<<<<<
  *         end_freq[0, i] = ibf.end.A[i]
  *         end_freq[1, i] = ibf.end.T[i]
  */
-    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->start->C[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 88, __pyx_L1_error)
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->start->C[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 89, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 88, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 89, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 88, __pyx_L1_error)
+    __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 89, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(__pyx_int_3);
     __Pyx_GIVEREF(__pyx_int_3);
     PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_int_3);
     __Pyx_GIVEREF(__pyx_t_4);
     PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_4);
     __pyx_t_4 = 0;
-    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_start_freq), __pyx_t_1, __pyx_t_2) < 0)) __PYX_ERR(0, 88, __pyx_L1_error)
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_start_freq), __pyx_t_1, __pyx_t_2) < 0)) __PYX_ERR(0, 89, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "genome_info/kmers/kmer_reader.pyx":89
+    /* "genome_info/kmers/kmer_reader.pyx":90
  *         start_freq[2, i] = ibf.start.G[i]
  *         start_freq[3, i] = ibf.start.C[i]
  *         end_freq[0, i] = ibf.end.A[i]             # <<<<<<<<<<<<<<
  *         end_freq[1, i] = ibf.end.T[i]
  *         end_freq[2, i] = ibf.end.G[i]
  */
-    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->end->A[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 89, __pyx_L1_error)
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->end->A[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 90, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 89, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 90, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 89, __pyx_L1_error)
+    __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 90, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_INCREF(__pyx_int_0);
     __Pyx_GIVEREF(__pyx_int_0);
     PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_int_0);
     __Pyx_GIVEREF(__pyx_t_1);
     PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_1);
     __pyx_t_1 = 0;
-    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_end_freq), __pyx_t_4, __pyx_t_2) < 0)) __PYX_ERR(0, 89, __pyx_L1_error)
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_end_freq), __pyx_t_4, __pyx_t_2) < 0)) __PYX_ERR(0, 90, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "genome_info/kmers/kmer_reader.pyx":90
+    /* "genome_info/kmers/kmer_reader.pyx":91
  *         start_freq[3, i] = ibf.start.C[i]
  *         end_freq[0, i] = ibf.end.A[i]
  *         end_freq[1, i] = ibf.end.T[i]             # <<<<<<<<<<<<<<
  *         end_freq[2, i] = ibf.end.G[i]
  *         end_freq[3, i] = ibf.end.C[i]
  */
-    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->end->T[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 90, __pyx_L1_error)
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->end->T[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 91, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 90, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 91, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 90, __pyx_L1_error)
+    __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 91, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(__pyx_int_1);
     __Pyx_GIVEREF(__pyx_int_1);
     PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_int_1);
     __Pyx_GIVEREF(__pyx_t_4);
     PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_4);
     __pyx_t_4 = 0;
-    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_end_freq), __pyx_t_1, __pyx_t_2) < 0)) __PYX_ERR(0, 90, __pyx_L1_error)
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_end_freq), __pyx_t_1, __pyx_t_2) < 0)) __PYX_ERR(0, 91, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "genome_info/kmers/kmer_reader.pyx":91
+    /* "genome_info/kmers/kmer_reader.pyx":92
  *         end_freq[0, i] = ibf.end.A[i]
  *         end_freq[1, i] = ibf.end.T[i]
  *         end_freq[2, i] = ibf.end.G[i]             # <<<<<<<<<<<<<<
  *         end_freq[3, i] = ibf.end.C[i]
  * 
  */
-    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->end->G[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 91, __pyx_L1_error)
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->end->G[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 92, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 91, __pyx_L1_error)
+    __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 92, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
-    __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 91, __pyx_L1_error)
+    __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 92, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_INCREF(__pyx_int_2);
     __Pyx_GIVEREF(__pyx_int_2);
     PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_int_2);
     __Pyx_GIVEREF(__pyx_t_1);
     PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_1);
     __pyx_t_1 = 0;
-    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_end_freq), __pyx_t_4, __pyx_t_2) < 0)) __PYX_ERR(0, 91, __pyx_L1_error)
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_end_freq), __pyx_t_4, __pyx_t_2) < 0)) __PYX_ERR(0, 92, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-    /* "genome_info/kmers/kmer_reader.pyx":92
+    /* "genome_info/kmers/kmer_reader.pyx":93
  *         end_freq[1, i] = ibf.end.T[i]
  *         end_freq[2, i] = ibf.end.G[i]
  *         end_freq[3, i] = ibf.end.C[i]             # <<<<<<<<<<<<<<
  * 
  *     interval_base_freq_destroy(ibf)
  */
-    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->end->C[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 92, __pyx_L1_error)
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->end->C[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 93, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_2);
-    __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 92, __pyx_L1_error)
+    __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 93, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
-    __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 92, __pyx_L1_error)
+    __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 93, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_1);
     __Pyx_INCREF(__pyx_int_3);
     __Pyx_GIVEREF(__pyx_int_3);
     PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_int_3);
     __Pyx_GIVEREF(__pyx_t_4);
     PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_4);
     __pyx_t_4 = 0;
-    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_end_freq), __pyx_t_1, __pyx_t_2) < 0)) __PYX_ERR(0, 92, __pyx_L1_error)
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_end_freq), __pyx_t_1, __pyx_t_2) < 0)) __PYX_ERR(0, 93, __pyx_L1_error)
     __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
   }
 
-  /* "genome_info/kmers/kmer_reader.pyx":94
+  /* "genome_info/kmers/kmer_reader.pyx":95
  *         end_freq[3, i] = ibf.end.C[i]
  * 
  *     interval_base_freq_destroy(ibf)             # <<<<<<<<<<<<<<
  * 
  *     return start_freq, end_freq
  */
   interval_base_freq_destroy(__pyx_v_ibf);
 
-  /* "genome_info/kmers/kmer_reader.pyx":96
+  /* "genome_info/kmers/kmer_reader.pyx":97
  *     interval_base_freq_destroy(ibf)
  * 
  *     return start_freq, end_freq             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 96, __pyx_L1_error)
+  __pyx_t_2 = PyTuple_New(2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 97, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_INCREF(((PyObject *)__pyx_v_start_freq));
   __Pyx_GIVEREF(((PyObject *)__pyx_v_start_freq));
   PyTuple_SET_ITEM(__pyx_t_2, 0, ((PyObject *)__pyx_v_start_freq));
   __Pyx_INCREF(((PyObject *)__pyx_v_end_freq));
   __Pyx_GIVEREF(((PyObject *)__pyx_v_end_freq));
   PyTuple_SET_ITEM(__pyx_t_2, 1, ((PyObject *)__pyx_v_end_freq));
   __pyx_r = __pyx_t_2;
   __pyx_t_2 = 0;
   goto __pyx_L0;
 
-  /* "genome_info/kmers/kmer_reader.pyx":75
+  /* "genome_info/kmers/kmer_reader.pyx":76
  * 
  * 
  * def read_bounds_base_freq(str seq_fn, LabeledIntervalArray laia, int n_bases):             # <<<<<<<<<<<<<<
  * 
  *     cdef str twobit_name = seq_fn
  */
 
@@ -4448,15 +4672,3522 @@
   __Pyx_XDECREF((PyObject *)__pyx_v_start_freq);
   __Pyx_XDECREF((PyObject *)__pyx_v_end_freq);
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../../var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/numpy/__init__.pxd":731
+/* "genome_info/kmers/kmer_reader.pyx":100
+ * 
+ * 
+ * def read_bounds_tribase_freq(str seq_fn, LabeledIntervalArray laia, int n_bases):             # <<<<<<<<<<<<<<
+ * 
+ *     cdef str twobit_name = seq_fn
+ */
+
+/* Python wrapper */
+static PyObject *__pyx_pw_11genome_info_5kmers_11kmer_reader_9read_bounds_tribase_freq(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds); /*proto*/
+static char __pyx_doc_11genome_info_5kmers_11kmer_reader_8read_bounds_tribase_freq[] = "read_bounds_tribase_freq(unicode seq_fn, LabeledIntervalArray laia, int n_bases)";
+static PyMethodDef __pyx_mdef_11genome_info_5kmers_11kmer_reader_9read_bounds_tribase_freq = {"read_bounds_tribase_freq", (PyCFunction)(void*)(PyCFunctionWithKeywords)__pyx_pw_11genome_info_5kmers_11kmer_reader_9read_bounds_tribase_freq, METH_VARARGS|METH_KEYWORDS, __pyx_doc_11genome_info_5kmers_11kmer_reader_8read_bounds_tribase_freq};
+static PyObject *__pyx_pw_11genome_info_5kmers_11kmer_reader_9read_bounds_tribase_freq(PyObject *__pyx_self, PyObject *__pyx_args, PyObject *__pyx_kwds) {
+  PyObject *__pyx_v_seq_fn = 0;
+  struct __pyx_obj_6ailist_25LabeledIntervalArray_core_LabeledIntervalArray *__pyx_v_laia = 0;
+  int __pyx_v_n_bases;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  PyObject *__pyx_r = 0;
+  __Pyx_RefNannyDeclarations
+  __Pyx_RefNannySetupContext("read_bounds_tribase_freq (wrapper)", 0);
+  {
+    static PyObject **__pyx_pyargnames[] = {&__pyx_n_s_seq_fn,&__pyx_n_s_laia,&__pyx_n_s_n_bases,0};
+    PyObject* values[3] = {0,0,0};
+    if (unlikely(__pyx_kwds)) {
+      Py_ssize_t kw_args;
+      const Py_ssize_t pos_args = PyTuple_GET_SIZE(__pyx_args);
+      switch (pos_args) {
+        case  3: values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
+        CYTHON_FALLTHROUGH;
+        case  2: values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+        CYTHON_FALLTHROUGH;
+        case  1: values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+        CYTHON_FALLTHROUGH;
+        case  0: break;
+        default: goto __pyx_L5_argtuple_error;
+      }
+      kw_args = PyDict_Size(__pyx_kwds);
+      switch (pos_args) {
+        case  0:
+        if (likely((values[0] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_seq_fn)) != 0)) kw_args--;
+        else goto __pyx_L5_argtuple_error;
+        CYTHON_FALLTHROUGH;
+        case  1:
+        if (likely((values[1] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_laia)) != 0)) kw_args--;
+        else {
+          __Pyx_RaiseArgtupleInvalid("read_bounds_tribase_freq", 1, 3, 3, 1); __PYX_ERR(0, 100, __pyx_L3_error)
+        }
+        CYTHON_FALLTHROUGH;
+        case  2:
+        if (likely((values[2] = __Pyx_PyDict_GetItemStr(__pyx_kwds, __pyx_n_s_n_bases)) != 0)) kw_args--;
+        else {
+          __Pyx_RaiseArgtupleInvalid("read_bounds_tribase_freq", 1, 3, 3, 2); __PYX_ERR(0, 100, __pyx_L3_error)
+        }
+      }
+      if (unlikely(kw_args > 0)) {
+        if (unlikely(__Pyx_ParseOptionalKeywords(__pyx_kwds, __pyx_pyargnames, 0, values, pos_args, "read_bounds_tribase_freq") < 0)) __PYX_ERR(0, 100, __pyx_L3_error)
+      }
+    } else if (PyTuple_GET_SIZE(__pyx_args) != 3) {
+      goto __pyx_L5_argtuple_error;
+    } else {
+      values[0] = PyTuple_GET_ITEM(__pyx_args, 0);
+      values[1] = PyTuple_GET_ITEM(__pyx_args, 1);
+      values[2] = PyTuple_GET_ITEM(__pyx_args, 2);
+    }
+    __pyx_v_seq_fn = ((PyObject*)values[0]);
+    __pyx_v_laia = ((struct __pyx_obj_6ailist_25LabeledIntervalArray_core_LabeledIntervalArray *)values[1]);
+    __pyx_v_n_bases = __Pyx_PyInt_As_int(values[2]); if (unlikely((__pyx_v_n_bases == (int)-1) && PyErr_Occurred())) __PYX_ERR(0, 100, __pyx_L3_error)
+  }
+  goto __pyx_L4_argument_unpacking_done;
+  __pyx_L5_argtuple_error:;
+  __Pyx_RaiseArgtupleInvalid("read_bounds_tribase_freq", 1, 3, 3, PyTuple_GET_SIZE(__pyx_args)); __PYX_ERR(0, 100, __pyx_L3_error)
+  __pyx_L3_error:;
+  __Pyx_AddTraceback("genome_info.kmers.kmer_reader.read_bounds_tribase_freq", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __Pyx_RefNannyFinishContext();
+  return NULL;
+  __pyx_L4_argument_unpacking_done:;
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_seq_fn), (&PyUnicode_Type), 1, "seq_fn", 1))) __PYX_ERR(0, 100, __pyx_L1_error)
+  if (unlikely(!__Pyx_ArgTypeTest(((PyObject *)__pyx_v_laia), __pyx_ptype_6ailist_25LabeledIntervalArray_core_LabeledIntervalArray, 1, "laia", 0))) __PYX_ERR(0, 100, __pyx_L1_error)
+  __pyx_r = __pyx_pf_11genome_info_5kmers_11kmer_reader_8read_bounds_tribase_freq(__pyx_self, __pyx_v_seq_fn, __pyx_v_laia, __pyx_v_n_bases);
+
+  /* function exit code */
+  goto __pyx_L0;
+  __pyx_L1_error:;
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+static PyObject *__pyx_pf_11genome_info_5kmers_11kmer_reader_8read_bounds_tribase_freq(CYTHON_UNUSED PyObject *__pyx_self, PyObject *__pyx_v_seq_fn, struct __pyx_obj_6ailist_25LabeledIntervalArray_core_LabeledIntervalArray *__pyx_v_laia, int __pyx_v_n_bases) {
+  PyObject *__pyx_v_twobit_name = 0;
+  PyObject *__pyx_v_fname = 0;
+  PyArrayObject *__pyx_v_start_freq = 0;
+  PyArrayObject *__pyx_v_end_freq = 0;
+  interval_tribase_freq_t *__pyx_v_ibf;
+  int __pyx_v_i;
+  PyObject *__pyx_v_tribases = NULL;
+  PyObject *__pyx_v_start_results = NULL;
+  PyObject *__pyx_v_end_results = NULL;
+  PyObject *__pyx_r = NULL;
+  __Pyx_RefNannyDeclarations
+  PyObject *__pyx_t_1 = NULL;
+  PyObject *__pyx_t_2 = NULL;
+  PyObject *__pyx_t_3 = NULL;
+  PyObject *__pyx_t_4 = NULL;
+  char *__pyx_t_5;
+  int __pyx_t_6;
+  int __pyx_t_7;
+  int __pyx_t_8;
+  int __pyx_lineno = 0;
+  const char *__pyx_filename = NULL;
+  int __pyx_clineno = 0;
+  __Pyx_RefNannySetupContext("read_bounds_tribase_freq", 0);
+
+  /* "genome_info/kmers/kmer_reader.pyx":102
+ * def read_bounds_tribase_freq(str seq_fn, LabeledIntervalArray laia, int n_bases):
+ * 
+ *     cdef str twobit_name = seq_fn             # <<<<<<<<<<<<<<
+ *     cdef bytes fname = twobit_name.encode()
+ * 
+ */
+  __Pyx_INCREF(__pyx_v_seq_fn);
+  __pyx_v_twobit_name = __pyx_v_seq_fn;
+
+  /* "genome_info/kmers/kmer_reader.pyx":103
+ * 
+ *     cdef str twobit_name = seq_fn
+ *     cdef bytes fname = twobit_name.encode()             # <<<<<<<<<<<<<<
+ * 
+ *     cdef np.ndarray start_freq = np.zeros((64, n_bases), dtype=float)
+ */
+  if (unlikely(__pyx_v_twobit_name == Py_None)) {
+    PyErr_Format(PyExc_AttributeError, "'NoneType' object has no attribute '%.30s'", "encode");
+    __PYX_ERR(0, 103, __pyx_L1_error)
+  }
+  __pyx_t_1 = PyUnicode_AsEncodedString(__pyx_v_twobit_name, NULL, NULL); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 103, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_v_fname = ((PyObject*)__pyx_t_1);
+  __pyx_t_1 = 0;
+
+  /* "genome_info/kmers/kmer_reader.pyx":105
+ *     cdef bytes fname = twobit_name.encode()
+ * 
+ *     cdef np.ndarray start_freq = np.zeros((64, n_bases), dtype=float)             # <<<<<<<<<<<<<<
+ *     cdef np.ndarray end_freq = np.zeros((64, n_bases), dtype=float)
+ * 
+ */
+  __Pyx_GetModuleGlobalName(__pyx_t_1, __pyx_n_s_np); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 105, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_zeros); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 105, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_n_bases); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 105, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __pyx_t_3 = PyTuple_New(2); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 105, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_INCREF(__pyx_int_64);
+  __Pyx_GIVEREF(__pyx_int_64);
+  PyTuple_SET_ITEM(__pyx_t_3, 0, __pyx_int_64);
+  __Pyx_GIVEREF(__pyx_t_1);
+  PyTuple_SET_ITEM(__pyx_t_3, 1, __pyx_t_1);
+  __pyx_t_1 = 0;
+  __pyx_t_1 = PyTuple_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 105, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_GIVEREF(__pyx_t_3);
+  PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_t_3);
+  __pyx_t_3 = 0;
+  __pyx_t_3 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 105, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  if (PyDict_SetItem(__pyx_t_3, __pyx_n_s_dtype, ((PyObject *)(&PyFloat_Type))) < 0) __PYX_ERR(0, 105, __pyx_L1_error)
+  __pyx_t_4 = __Pyx_PyObject_Call(__pyx_t_2, __pyx_t_1, __pyx_t_3); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 105, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  if (!(likely(((__pyx_t_4) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_4, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 105, __pyx_L1_error)
+  __pyx_v_start_freq = ((PyArrayObject *)__pyx_t_4);
+  __pyx_t_4 = 0;
+
+  /* "genome_info/kmers/kmer_reader.pyx":106
+ * 
+ *     cdef np.ndarray start_freq = np.zeros((64, n_bases), dtype=float)
+ *     cdef np.ndarray end_freq = np.zeros((64, n_bases), dtype=float)             # <<<<<<<<<<<<<<
+ * 
+ *     cdef interval_tribase_freq_t *ibf = read_interval_tribase_freq(laia.laia, fname, n_bases)
+ */
+  __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 106, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_zeros); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 106, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_n_bases); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 106, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 106, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_INCREF(__pyx_int_64);
+  __Pyx_GIVEREF(__pyx_int_64);
+  PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_int_64);
+  __Pyx_GIVEREF(__pyx_t_4);
+  PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_4);
+  __pyx_t_4 = 0;
+  __pyx_t_4 = PyTuple_New(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 106, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_GIVEREF(__pyx_t_1);
+  PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_t_1);
+  __pyx_t_1 = 0;
+  __pyx_t_1 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 106, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (PyDict_SetItem(__pyx_t_1, __pyx_n_s_dtype, ((PyObject *)(&PyFloat_Type))) < 0) __PYX_ERR(0, 106, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Call(__pyx_t_3, __pyx_t_4, __pyx_t_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 106, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  if (!(likely(((__pyx_t_2) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_2, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 106, __pyx_L1_error)
+  __pyx_v_end_freq = ((PyArrayObject *)__pyx_t_2);
+  __pyx_t_2 = 0;
+
+  /* "genome_info/kmers/kmer_reader.pyx":108
+ *     cdef np.ndarray end_freq = np.zeros((64, n_bases), dtype=float)
+ * 
+ *     cdef interval_tribase_freq_t *ibf = read_interval_tribase_freq(laia.laia, fname, n_bases)             # <<<<<<<<<<<<<<
+ *     cdef int i
+ *     for i in range(n_bases):
+ */
+  if (unlikely(__pyx_v_fname == Py_None)) {
+    PyErr_SetString(PyExc_TypeError, "expected bytes, NoneType found");
+    __PYX_ERR(0, 108, __pyx_L1_error)
+  }
+  __pyx_t_5 = __Pyx_PyBytes_AsWritableString(__pyx_v_fname); if (unlikely((!__pyx_t_5) && PyErr_Occurred())) __PYX_ERR(0, 108, __pyx_L1_error)
+  __pyx_v_ibf = read_interval_tribase_freq(__pyx_v_laia->laia, __pyx_t_5, __pyx_v_n_bases);
+
+  /* "genome_info/kmers/kmer_reader.pyx":110
+ *     cdef interval_tribase_freq_t *ibf = read_interval_tribase_freq(laia.laia, fname, n_bases)
+ *     cdef int i
+ *     for i in range(n_bases):             # <<<<<<<<<<<<<<
+ *         start_freq[0, i] = ibf.start.AAA[i]
+ *         start_freq[1, i] = ibf.start.AAC[i]
+ */
+  __pyx_t_6 = __pyx_v_n_bases;
+  __pyx_t_7 = __pyx_t_6;
+  for (__pyx_t_8 = 0; __pyx_t_8 < __pyx_t_7; __pyx_t_8+=1) {
+    __pyx_v_i = __pyx_t_8;
+
+    /* "genome_info/kmers/kmer_reader.pyx":111
+ *     cdef int i
+ *     for i in range(n_bases):
+ *         start_freq[0, i] = ibf.start.AAA[i]             # <<<<<<<<<<<<<<
+ *         start_freq[1, i] = ibf.start.AAC[i]
+ *         start_freq[2, i] = ibf.start.AAG[i]
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->start->AAA[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 111, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 111, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 111, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_INCREF(__pyx_int_0);
+    __Pyx_GIVEREF(__pyx_int_0);
+    PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_int_0);
+    __Pyx_GIVEREF(__pyx_t_1);
+    PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_1);
+    __pyx_t_1 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_start_freq), __pyx_t_4, __pyx_t_2) < 0)) __PYX_ERR(0, 111, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "genome_info/kmers/kmer_reader.pyx":112
+ *     for i in range(n_bases):
+ *         start_freq[0, i] = ibf.start.AAA[i]
+ *         start_freq[1, i] = ibf.start.AAC[i]             # <<<<<<<<<<<<<<
+ *         start_freq[2, i] = ibf.start.AAG[i]
+ *         start_freq[3, i] = ibf.start.AAT[i]
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->start->AAC[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 112, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 112, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 112, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_int_1);
+    __Pyx_GIVEREF(__pyx_int_1);
+    PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_int_1);
+    __Pyx_GIVEREF(__pyx_t_4);
+    PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_4);
+    __pyx_t_4 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_start_freq), __pyx_t_1, __pyx_t_2) < 0)) __PYX_ERR(0, 112, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "genome_info/kmers/kmer_reader.pyx":113
+ *         start_freq[0, i] = ibf.start.AAA[i]
+ *         start_freq[1, i] = ibf.start.AAC[i]
+ *         start_freq[2, i] = ibf.start.AAG[i]             # <<<<<<<<<<<<<<
+ *         start_freq[3, i] = ibf.start.AAT[i]
+ *         start_freq[4, i] = ibf.start.ACA[i]
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->start->AAG[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 113, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 113, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 113, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_INCREF(__pyx_int_2);
+    __Pyx_GIVEREF(__pyx_int_2);
+    PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_int_2);
+    __Pyx_GIVEREF(__pyx_t_1);
+    PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_1);
+    __pyx_t_1 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_start_freq), __pyx_t_4, __pyx_t_2) < 0)) __PYX_ERR(0, 113, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "genome_info/kmers/kmer_reader.pyx":114
+ *         start_freq[1, i] = ibf.start.AAC[i]
+ *         start_freq[2, i] = ibf.start.AAG[i]
+ *         start_freq[3, i] = ibf.start.AAT[i]             # <<<<<<<<<<<<<<
+ *         start_freq[4, i] = ibf.start.ACA[i]
+ *         start_freq[5, i] = ibf.start.ACC[i]
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->start->AAT[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 114, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 114, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 114, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_int_3);
+    __Pyx_GIVEREF(__pyx_int_3);
+    PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_int_3);
+    __Pyx_GIVEREF(__pyx_t_4);
+    PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_4);
+    __pyx_t_4 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_start_freq), __pyx_t_1, __pyx_t_2) < 0)) __PYX_ERR(0, 114, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "genome_info/kmers/kmer_reader.pyx":115
+ *         start_freq[2, i] = ibf.start.AAG[i]
+ *         start_freq[3, i] = ibf.start.AAT[i]
+ *         start_freq[4, i] = ibf.start.ACA[i]             # <<<<<<<<<<<<<<
+ *         start_freq[5, i] = ibf.start.ACC[i]
+ *         start_freq[6, i] = ibf.start.ACG[i]
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->start->ACA[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 115, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 115, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 115, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_INCREF(__pyx_int_4);
+    __Pyx_GIVEREF(__pyx_int_4);
+    PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_int_4);
+    __Pyx_GIVEREF(__pyx_t_1);
+    PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_1);
+    __pyx_t_1 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_start_freq), __pyx_t_4, __pyx_t_2) < 0)) __PYX_ERR(0, 115, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "genome_info/kmers/kmer_reader.pyx":116
+ *         start_freq[3, i] = ibf.start.AAT[i]
+ *         start_freq[4, i] = ibf.start.ACA[i]
+ *         start_freq[5, i] = ibf.start.ACC[i]             # <<<<<<<<<<<<<<
+ *         start_freq[6, i] = ibf.start.ACG[i]
+ *         start_freq[7, i] = ibf.start.ACT[i]
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->start->ACC[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 116, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 116, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 116, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_int_5);
+    __Pyx_GIVEREF(__pyx_int_5);
+    PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_int_5);
+    __Pyx_GIVEREF(__pyx_t_4);
+    PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_4);
+    __pyx_t_4 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_start_freq), __pyx_t_1, __pyx_t_2) < 0)) __PYX_ERR(0, 116, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "genome_info/kmers/kmer_reader.pyx":117
+ *         start_freq[4, i] = ibf.start.ACA[i]
+ *         start_freq[5, i] = ibf.start.ACC[i]
+ *         start_freq[6, i] = ibf.start.ACG[i]             # <<<<<<<<<<<<<<
+ *         start_freq[7, i] = ibf.start.ACT[i]
+ *         start_freq[8, i] = ibf.start.AGA[i]
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->start->ACG[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 117, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 117, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 117, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_INCREF(__pyx_int_6);
+    __Pyx_GIVEREF(__pyx_int_6);
+    PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_int_6);
+    __Pyx_GIVEREF(__pyx_t_1);
+    PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_1);
+    __pyx_t_1 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_start_freq), __pyx_t_4, __pyx_t_2) < 0)) __PYX_ERR(0, 117, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "genome_info/kmers/kmer_reader.pyx":118
+ *         start_freq[5, i] = ibf.start.ACC[i]
+ *         start_freq[6, i] = ibf.start.ACG[i]
+ *         start_freq[7, i] = ibf.start.ACT[i]             # <<<<<<<<<<<<<<
+ *         start_freq[8, i] = ibf.start.AGA[i]
+ *         start_freq[9, i] = ibf.start.AGC[i]
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->start->ACT[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 118, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 118, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 118, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_int_7);
+    __Pyx_GIVEREF(__pyx_int_7);
+    PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_int_7);
+    __Pyx_GIVEREF(__pyx_t_4);
+    PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_4);
+    __pyx_t_4 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_start_freq), __pyx_t_1, __pyx_t_2) < 0)) __PYX_ERR(0, 118, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "genome_info/kmers/kmer_reader.pyx":119
+ *         start_freq[6, i] = ibf.start.ACG[i]
+ *         start_freq[7, i] = ibf.start.ACT[i]
+ *         start_freq[8, i] = ibf.start.AGA[i]             # <<<<<<<<<<<<<<
+ *         start_freq[9, i] = ibf.start.AGC[i]
+ *         start_freq[10, i] = ibf.start.AGG[i]
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->start->AGA[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 119, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 119, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 119, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_INCREF(__pyx_int_8);
+    __Pyx_GIVEREF(__pyx_int_8);
+    PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_int_8);
+    __Pyx_GIVEREF(__pyx_t_1);
+    PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_1);
+    __pyx_t_1 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_start_freq), __pyx_t_4, __pyx_t_2) < 0)) __PYX_ERR(0, 119, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "genome_info/kmers/kmer_reader.pyx":120
+ *         start_freq[7, i] = ibf.start.ACT[i]
+ *         start_freq[8, i] = ibf.start.AGA[i]
+ *         start_freq[9, i] = ibf.start.AGC[i]             # <<<<<<<<<<<<<<
+ *         start_freq[10, i] = ibf.start.AGG[i]
+ *         start_freq[11, i] = ibf.start.AGT[i]
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->start->AGC[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 120, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 120, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 120, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_int_9);
+    __Pyx_GIVEREF(__pyx_int_9);
+    PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_int_9);
+    __Pyx_GIVEREF(__pyx_t_4);
+    PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_4);
+    __pyx_t_4 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_start_freq), __pyx_t_1, __pyx_t_2) < 0)) __PYX_ERR(0, 120, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "genome_info/kmers/kmer_reader.pyx":121
+ *         start_freq[8, i] = ibf.start.AGA[i]
+ *         start_freq[9, i] = ibf.start.AGC[i]
+ *         start_freq[10, i] = ibf.start.AGG[i]             # <<<<<<<<<<<<<<
+ *         start_freq[11, i] = ibf.start.AGT[i]
+ *         start_freq[12, i] = ibf.start.ATA[i]
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->start->AGG[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 121, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 121, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 121, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_INCREF(__pyx_int_10);
+    __Pyx_GIVEREF(__pyx_int_10);
+    PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_int_10);
+    __Pyx_GIVEREF(__pyx_t_1);
+    PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_1);
+    __pyx_t_1 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_start_freq), __pyx_t_4, __pyx_t_2) < 0)) __PYX_ERR(0, 121, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "genome_info/kmers/kmer_reader.pyx":122
+ *         start_freq[9, i] = ibf.start.AGC[i]
+ *         start_freq[10, i] = ibf.start.AGG[i]
+ *         start_freq[11, i] = ibf.start.AGT[i]             # <<<<<<<<<<<<<<
+ *         start_freq[12, i] = ibf.start.ATA[i]
+ *         start_freq[13, i] = ibf.start.ATC[i]
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->start->AGT[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 122, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 122, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 122, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_int_11);
+    __Pyx_GIVEREF(__pyx_int_11);
+    PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_int_11);
+    __Pyx_GIVEREF(__pyx_t_4);
+    PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_4);
+    __pyx_t_4 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_start_freq), __pyx_t_1, __pyx_t_2) < 0)) __PYX_ERR(0, 122, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "genome_info/kmers/kmer_reader.pyx":123
+ *         start_freq[10, i] = ibf.start.AGG[i]
+ *         start_freq[11, i] = ibf.start.AGT[i]
+ *         start_freq[12, i] = ibf.start.ATA[i]             # <<<<<<<<<<<<<<
+ *         start_freq[13, i] = ibf.start.ATC[i]
+ *         start_freq[14, i] = ibf.start.ATG[i]
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->start->ATA[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 123, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 123, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 123, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_INCREF(__pyx_int_12);
+    __Pyx_GIVEREF(__pyx_int_12);
+    PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_int_12);
+    __Pyx_GIVEREF(__pyx_t_1);
+    PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_1);
+    __pyx_t_1 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_start_freq), __pyx_t_4, __pyx_t_2) < 0)) __PYX_ERR(0, 123, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "genome_info/kmers/kmer_reader.pyx":124
+ *         start_freq[11, i] = ibf.start.AGT[i]
+ *         start_freq[12, i] = ibf.start.ATA[i]
+ *         start_freq[13, i] = ibf.start.ATC[i]             # <<<<<<<<<<<<<<
+ *         start_freq[14, i] = ibf.start.ATG[i]
+ *         start_freq[15, i] = ibf.start.ATT[i]
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->start->ATC[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 124, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 124, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 124, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_int_13);
+    __Pyx_GIVEREF(__pyx_int_13);
+    PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_int_13);
+    __Pyx_GIVEREF(__pyx_t_4);
+    PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_4);
+    __pyx_t_4 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_start_freq), __pyx_t_1, __pyx_t_2) < 0)) __PYX_ERR(0, 124, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "genome_info/kmers/kmer_reader.pyx":125
+ *         start_freq[12, i] = ibf.start.ATA[i]
+ *         start_freq[13, i] = ibf.start.ATC[i]
+ *         start_freq[14, i] = ibf.start.ATG[i]             # <<<<<<<<<<<<<<
+ *         start_freq[15, i] = ibf.start.ATT[i]
+ *         start_freq[16, i] = ibf.start.CAA[i]
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->start->ATG[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 125, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 125, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 125, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_INCREF(__pyx_int_14);
+    __Pyx_GIVEREF(__pyx_int_14);
+    PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_int_14);
+    __Pyx_GIVEREF(__pyx_t_1);
+    PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_1);
+    __pyx_t_1 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_start_freq), __pyx_t_4, __pyx_t_2) < 0)) __PYX_ERR(0, 125, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "genome_info/kmers/kmer_reader.pyx":126
+ *         start_freq[13, i] = ibf.start.ATC[i]
+ *         start_freq[14, i] = ibf.start.ATG[i]
+ *         start_freq[15, i] = ibf.start.ATT[i]             # <<<<<<<<<<<<<<
+ *         start_freq[16, i] = ibf.start.CAA[i]
+ *         start_freq[17, i] = ibf.start.CAC[i]
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->start->ATT[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 126, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 126, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 126, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_int_15);
+    __Pyx_GIVEREF(__pyx_int_15);
+    PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_int_15);
+    __Pyx_GIVEREF(__pyx_t_4);
+    PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_4);
+    __pyx_t_4 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_start_freq), __pyx_t_1, __pyx_t_2) < 0)) __PYX_ERR(0, 126, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "genome_info/kmers/kmer_reader.pyx":127
+ *         start_freq[14, i] = ibf.start.ATG[i]
+ *         start_freq[15, i] = ibf.start.ATT[i]
+ *         start_freq[16, i] = ibf.start.CAA[i]             # <<<<<<<<<<<<<<
+ *         start_freq[17, i] = ibf.start.CAC[i]
+ *         start_freq[18, i] = ibf.start.CAG[i]
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->start->CAA[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 127, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 127, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 127, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_INCREF(__pyx_int_16);
+    __Pyx_GIVEREF(__pyx_int_16);
+    PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_int_16);
+    __Pyx_GIVEREF(__pyx_t_1);
+    PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_1);
+    __pyx_t_1 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_start_freq), __pyx_t_4, __pyx_t_2) < 0)) __PYX_ERR(0, 127, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "genome_info/kmers/kmer_reader.pyx":128
+ *         start_freq[15, i] = ibf.start.ATT[i]
+ *         start_freq[16, i] = ibf.start.CAA[i]
+ *         start_freq[17, i] = ibf.start.CAC[i]             # <<<<<<<<<<<<<<
+ *         start_freq[18, i] = ibf.start.CAG[i]
+ *         start_freq[19, i] = ibf.start.CAT[i]
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->start->CAC[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 128, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 128, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 128, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_int_17);
+    __Pyx_GIVEREF(__pyx_int_17);
+    PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_int_17);
+    __Pyx_GIVEREF(__pyx_t_4);
+    PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_4);
+    __pyx_t_4 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_start_freq), __pyx_t_1, __pyx_t_2) < 0)) __PYX_ERR(0, 128, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "genome_info/kmers/kmer_reader.pyx":129
+ *         start_freq[16, i] = ibf.start.CAA[i]
+ *         start_freq[17, i] = ibf.start.CAC[i]
+ *         start_freq[18, i] = ibf.start.CAG[i]             # <<<<<<<<<<<<<<
+ *         start_freq[19, i] = ibf.start.CAT[i]
+ *         start_freq[20, i] = ibf.start.CCA[i]
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->start->CAG[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 129, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 129, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 129, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_INCREF(__pyx_int_18);
+    __Pyx_GIVEREF(__pyx_int_18);
+    PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_int_18);
+    __Pyx_GIVEREF(__pyx_t_1);
+    PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_1);
+    __pyx_t_1 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_start_freq), __pyx_t_4, __pyx_t_2) < 0)) __PYX_ERR(0, 129, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "genome_info/kmers/kmer_reader.pyx":130
+ *         start_freq[17, i] = ibf.start.CAC[i]
+ *         start_freq[18, i] = ibf.start.CAG[i]
+ *         start_freq[19, i] = ibf.start.CAT[i]             # <<<<<<<<<<<<<<
+ *         start_freq[20, i] = ibf.start.CCA[i]
+ *         start_freq[21, i] = ibf.start.CCC[i]
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->start->CAT[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 130, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 130, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 130, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_int_19);
+    __Pyx_GIVEREF(__pyx_int_19);
+    PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_int_19);
+    __Pyx_GIVEREF(__pyx_t_4);
+    PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_4);
+    __pyx_t_4 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_start_freq), __pyx_t_1, __pyx_t_2) < 0)) __PYX_ERR(0, 130, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "genome_info/kmers/kmer_reader.pyx":131
+ *         start_freq[18, i] = ibf.start.CAG[i]
+ *         start_freq[19, i] = ibf.start.CAT[i]
+ *         start_freq[20, i] = ibf.start.CCA[i]             # <<<<<<<<<<<<<<
+ *         start_freq[21, i] = ibf.start.CCC[i]
+ *         start_freq[22, i] = ibf.start.CCG[i]
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->start->CCA[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 131, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 131, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 131, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_INCREF(__pyx_int_20);
+    __Pyx_GIVEREF(__pyx_int_20);
+    PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_int_20);
+    __Pyx_GIVEREF(__pyx_t_1);
+    PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_1);
+    __pyx_t_1 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_start_freq), __pyx_t_4, __pyx_t_2) < 0)) __PYX_ERR(0, 131, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "genome_info/kmers/kmer_reader.pyx":132
+ *         start_freq[19, i] = ibf.start.CAT[i]
+ *         start_freq[20, i] = ibf.start.CCA[i]
+ *         start_freq[21, i] = ibf.start.CCC[i]             # <<<<<<<<<<<<<<
+ *         start_freq[22, i] = ibf.start.CCG[i]
+ *         start_freq[23, i] = ibf.start.CCT[i]
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->start->CCC[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 132, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 132, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 132, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_int_21);
+    __Pyx_GIVEREF(__pyx_int_21);
+    PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_int_21);
+    __Pyx_GIVEREF(__pyx_t_4);
+    PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_4);
+    __pyx_t_4 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_start_freq), __pyx_t_1, __pyx_t_2) < 0)) __PYX_ERR(0, 132, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "genome_info/kmers/kmer_reader.pyx":133
+ *         start_freq[20, i] = ibf.start.CCA[i]
+ *         start_freq[21, i] = ibf.start.CCC[i]
+ *         start_freq[22, i] = ibf.start.CCG[i]             # <<<<<<<<<<<<<<
+ *         start_freq[23, i] = ibf.start.CCT[i]
+ *         start_freq[24, i] = ibf.start.CGA[i]
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->start->CCG[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 133, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 133, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 133, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_INCREF(__pyx_int_22);
+    __Pyx_GIVEREF(__pyx_int_22);
+    PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_int_22);
+    __Pyx_GIVEREF(__pyx_t_1);
+    PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_1);
+    __pyx_t_1 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_start_freq), __pyx_t_4, __pyx_t_2) < 0)) __PYX_ERR(0, 133, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "genome_info/kmers/kmer_reader.pyx":134
+ *         start_freq[21, i] = ibf.start.CCC[i]
+ *         start_freq[22, i] = ibf.start.CCG[i]
+ *         start_freq[23, i] = ibf.start.CCT[i]             # <<<<<<<<<<<<<<
+ *         start_freq[24, i] = ibf.start.CGA[i]
+ *         start_freq[25, i] = ibf.start.CGC[i]
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->start->CCT[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 134, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 134, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 134, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_int_23);
+    __Pyx_GIVEREF(__pyx_int_23);
+    PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_int_23);
+    __Pyx_GIVEREF(__pyx_t_4);
+    PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_4);
+    __pyx_t_4 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_start_freq), __pyx_t_1, __pyx_t_2) < 0)) __PYX_ERR(0, 134, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "genome_info/kmers/kmer_reader.pyx":135
+ *         start_freq[22, i] = ibf.start.CCG[i]
+ *         start_freq[23, i] = ibf.start.CCT[i]
+ *         start_freq[24, i] = ibf.start.CGA[i]             # <<<<<<<<<<<<<<
+ *         start_freq[25, i] = ibf.start.CGC[i]
+ *         start_freq[26, i] = ibf.start.CGG[i]
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->start->CGA[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 135, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 135, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 135, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_INCREF(__pyx_int_24);
+    __Pyx_GIVEREF(__pyx_int_24);
+    PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_int_24);
+    __Pyx_GIVEREF(__pyx_t_1);
+    PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_1);
+    __pyx_t_1 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_start_freq), __pyx_t_4, __pyx_t_2) < 0)) __PYX_ERR(0, 135, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "genome_info/kmers/kmer_reader.pyx":136
+ *         start_freq[23, i] = ibf.start.CCT[i]
+ *         start_freq[24, i] = ibf.start.CGA[i]
+ *         start_freq[25, i] = ibf.start.CGC[i]             # <<<<<<<<<<<<<<
+ *         start_freq[26, i] = ibf.start.CGG[i]
+ *         start_freq[27, i] = ibf.start.CGT[i]
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->start->CGC[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 136, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 136, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 136, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_int_25);
+    __Pyx_GIVEREF(__pyx_int_25);
+    PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_int_25);
+    __Pyx_GIVEREF(__pyx_t_4);
+    PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_4);
+    __pyx_t_4 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_start_freq), __pyx_t_1, __pyx_t_2) < 0)) __PYX_ERR(0, 136, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "genome_info/kmers/kmer_reader.pyx":137
+ *         start_freq[24, i] = ibf.start.CGA[i]
+ *         start_freq[25, i] = ibf.start.CGC[i]
+ *         start_freq[26, i] = ibf.start.CGG[i]             # <<<<<<<<<<<<<<
+ *         start_freq[27, i] = ibf.start.CGT[i]
+ *         start_freq[28, i] = ibf.start.CTA[i]
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->start->CGG[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 137, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 137, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 137, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_INCREF(__pyx_int_26);
+    __Pyx_GIVEREF(__pyx_int_26);
+    PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_int_26);
+    __Pyx_GIVEREF(__pyx_t_1);
+    PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_1);
+    __pyx_t_1 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_start_freq), __pyx_t_4, __pyx_t_2) < 0)) __PYX_ERR(0, 137, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "genome_info/kmers/kmer_reader.pyx":138
+ *         start_freq[25, i] = ibf.start.CGC[i]
+ *         start_freq[26, i] = ibf.start.CGG[i]
+ *         start_freq[27, i] = ibf.start.CGT[i]             # <<<<<<<<<<<<<<
+ *         start_freq[28, i] = ibf.start.CTA[i]
+ *         start_freq[29, i] = ibf.start.CTC[i]
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->start->CGT[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 138, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 138, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 138, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_int_27);
+    __Pyx_GIVEREF(__pyx_int_27);
+    PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_int_27);
+    __Pyx_GIVEREF(__pyx_t_4);
+    PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_4);
+    __pyx_t_4 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_start_freq), __pyx_t_1, __pyx_t_2) < 0)) __PYX_ERR(0, 138, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "genome_info/kmers/kmer_reader.pyx":139
+ *         start_freq[26, i] = ibf.start.CGG[i]
+ *         start_freq[27, i] = ibf.start.CGT[i]
+ *         start_freq[28, i] = ibf.start.CTA[i]             # <<<<<<<<<<<<<<
+ *         start_freq[29, i] = ibf.start.CTC[i]
+ *         start_freq[30, i] = ibf.start.CTG[i]
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->start->CTA[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 139, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 139, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 139, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_INCREF(__pyx_int_28);
+    __Pyx_GIVEREF(__pyx_int_28);
+    PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_int_28);
+    __Pyx_GIVEREF(__pyx_t_1);
+    PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_1);
+    __pyx_t_1 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_start_freq), __pyx_t_4, __pyx_t_2) < 0)) __PYX_ERR(0, 139, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "genome_info/kmers/kmer_reader.pyx":140
+ *         start_freq[27, i] = ibf.start.CGT[i]
+ *         start_freq[28, i] = ibf.start.CTA[i]
+ *         start_freq[29, i] = ibf.start.CTC[i]             # <<<<<<<<<<<<<<
+ *         start_freq[30, i] = ibf.start.CTG[i]
+ *         start_freq[31, i] = ibf.start.CTT[i]
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->start->CTC[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 140, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 140, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 140, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_int_29);
+    __Pyx_GIVEREF(__pyx_int_29);
+    PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_int_29);
+    __Pyx_GIVEREF(__pyx_t_4);
+    PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_4);
+    __pyx_t_4 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_start_freq), __pyx_t_1, __pyx_t_2) < 0)) __PYX_ERR(0, 140, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "genome_info/kmers/kmer_reader.pyx":141
+ *         start_freq[28, i] = ibf.start.CTA[i]
+ *         start_freq[29, i] = ibf.start.CTC[i]
+ *         start_freq[30, i] = ibf.start.CTG[i]             # <<<<<<<<<<<<<<
+ *         start_freq[31, i] = ibf.start.CTT[i]
+ *         start_freq[32, i] = ibf.start.GAA[i]
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->start->CTG[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 141, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 141, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 141, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_INCREF(__pyx_int_30);
+    __Pyx_GIVEREF(__pyx_int_30);
+    PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_int_30);
+    __Pyx_GIVEREF(__pyx_t_1);
+    PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_1);
+    __pyx_t_1 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_start_freq), __pyx_t_4, __pyx_t_2) < 0)) __PYX_ERR(0, 141, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "genome_info/kmers/kmer_reader.pyx":142
+ *         start_freq[29, i] = ibf.start.CTC[i]
+ *         start_freq[30, i] = ibf.start.CTG[i]
+ *         start_freq[31, i] = ibf.start.CTT[i]             # <<<<<<<<<<<<<<
+ *         start_freq[32, i] = ibf.start.GAA[i]
+ *         start_freq[33, i] = ibf.start.GAC[i]
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->start->CTT[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 142, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 142, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 142, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_int_31);
+    __Pyx_GIVEREF(__pyx_int_31);
+    PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_int_31);
+    __Pyx_GIVEREF(__pyx_t_4);
+    PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_4);
+    __pyx_t_4 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_start_freq), __pyx_t_1, __pyx_t_2) < 0)) __PYX_ERR(0, 142, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "genome_info/kmers/kmer_reader.pyx":143
+ *         start_freq[30, i] = ibf.start.CTG[i]
+ *         start_freq[31, i] = ibf.start.CTT[i]
+ *         start_freq[32, i] = ibf.start.GAA[i]             # <<<<<<<<<<<<<<
+ *         start_freq[33, i] = ibf.start.GAC[i]
+ *         start_freq[34, i] = ibf.start.GAG[i]
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->start->GAA[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 143, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 143, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 143, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_INCREF(__pyx_int_32);
+    __Pyx_GIVEREF(__pyx_int_32);
+    PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_int_32);
+    __Pyx_GIVEREF(__pyx_t_1);
+    PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_1);
+    __pyx_t_1 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_start_freq), __pyx_t_4, __pyx_t_2) < 0)) __PYX_ERR(0, 143, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "genome_info/kmers/kmer_reader.pyx":144
+ *         start_freq[31, i] = ibf.start.CTT[i]
+ *         start_freq[32, i] = ibf.start.GAA[i]
+ *         start_freq[33, i] = ibf.start.GAC[i]             # <<<<<<<<<<<<<<
+ *         start_freq[34, i] = ibf.start.GAG[i]
+ *         start_freq[35, i] = ibf.start.GAT[i]
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->start->GAC[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 144, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 144, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 144, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_int_33);
+    __Pyx_GIVEREF(__pyx_int_33);
+    PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_int_33);
+    __Pyx_GIVEREF(__pyx_t_4);
+    PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_4);
+    __pyx_t_4 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_start_freq), __pyx_t_1, __pyx_t_2) < 0)) __PYX_ERR(0, 144, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "genome_info/kmers/kmer_reader.pyx":145
+ *         start_freq[32, i] = ibf.start.GAA[i]
+ *         start_freq[33, i] = ibf.start.GAC[i]
+ *         start_freq[34, i] = ibf.start.GAG[i]             # <<<<<<<<<<<<<<
+ *         start_freq[35, i] = ibf.start.GAT[i]
+ *         start_freq[36, i] = ibf.start.GCA[i]
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->start->GAG[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 145, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 145, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 145, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_INCREF(__pyx_int_34);
+    __Pyx_GIVEREF(__pyx_int_34);
+    PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_int_34);
+    __Pyx_GIVEREF(__pyx_t_1);
+    PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_1);
+    __pyx_t_1 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_start_freq), __pyx_t_4, __pyx_t_2) < 0)) __PYX_ERR(0, 145, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "genome_info/kmers/kmer_reader.pyx":146
+ *         start_freq[33, i] = ibf.start.GAC[i]
+ *         start_freq[34, i] = ibf.start.GAG[i]
+ *         start_freq[35, i] = ibf.start.GAT[i]             # <<<<<<<<<<<<<<
+ *         start_freq[36, i] = ibf.start.GCA[i]
+ *         start_freq[37, i] = ibf.start.GCC[i]
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->start->GAT[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 146, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 146, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 146, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_int_35);
+    __Pyx_GIVEREF(__pyx_int_35);
+    PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_int_35);
+    __Pyx_GIVEREF(__pyx_t_4);
+    PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_4);
+    __pyx_t_4 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_start_freq), __pyx_t_1, __pyx_t_2) < 0)) __PYX_ERR(0, 146, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "genome_info/kmers/kmer_reader.pyx":147
+ *         start_freq[34, i] = ibf.start.GAG[i]
+ *         start_freq[35, i] = ibf.start.GAT[i]
+ *         start_freq[36, i] = ibf.start.GCA[i]             # <<<<<<<<<<<<<<
+ *         start_freq[37, i] = ibf.start.GCC[i]
+ *         start_freq[38, i] = ibf.start.GCG[i]
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->start->GCA[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 147, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 147, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 147, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_INCREF(__pyx_int_36);
+    __Pyx_GIVEREF(__pyx_int_36);
+    PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_int_36);
+    __Pyx_GIVEREF(__pyx_t_1);
+    PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_1);
+    __pyx_t_1 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_start_freq), __pyx_t_4, __pyx_t_2) < 0)) __PYX_ERR(0, 147, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "genome_info/kmers/kmer_reader.pyx":148
+ *         start_freq[35, i] = ibf.start.GAT[i]
+ *         start_freq[36, i] = ibf.start.GCA[i]
+ *         start_freq[37, i] = ibf.start.GCC[i]             # <<<<<<<<<<<<<<
+ *         start_freq[38, i] = ibf.start.GCG[i]
+ *         start_freq[39, i] = ibf.start.GCT[i]
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->start->GCC[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 148, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 148, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 148, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_int_37);
+    __Pyx_GIVEREF(__pyx_int_37);
+    PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_int_37);
+    __Pyx_GIVEREF(__pyx_t_4);
+    PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_4);
+    __pyx_t_4 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_start_freq), __pyx_t_1, __pyx_t_2) < 0)) __PYX_ERR(0, 148, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "genome_info/kmers/kmer_reader.pyx":149
+ *         start_freq[36, i] = ibf.start.GCA[i]
+ *         start_freq[37, i] = ibf.start.GCC[i]
+ *         start_freq[38, i] = ibf.start.GCG[i]             # <<<<<<<<<<<<<<
+ *         start_freq[39, i] = ibf.start.GCT[i]
+ *         start_freq[40, i] = ibf.start.GGA[i]
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->start->GCG[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 149, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 149, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 149, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_INCREF(__pyx_int_38);
+    __Pyx_GIVEREF(__pyx_int_38);
+    PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_int_38);
+    __Pyx_GIVEREF(__pyx_t_1);
+    PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_1);
+    __pyx_t_1 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_start_freq), __pyx_t_4, __pyx_t_2) < 0)) __PYX_ERR(0, 149, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "genome_info/kmers/kmer_reader.pyx":150
+ *         start_freq[37, i] = ibf.start.GCC[i]
+ *         start_freq[38, i] = ibf.start.GCG[i]
+ *         start_freq[39, i] = ibf.start.GCT[i]             # <<<<<<<<<<<<<<
+ *         start_freq[40, i] = ibf.start.GGA[i]
+ *         start_freq[41, i] = ibf.start.GGC[i]
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->start->GCT[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 150, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 150, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 150, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_int_39);
+    __Pyx_GIVEREF(__pyx_int_39);
+    PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_int_39);
+    __Pyx_GIVEREF(__pyx_t_4);
+    PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_4);
+    __pyx_t_4 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_start_freq), __pyx_t_1, __pyx_t_2) < 0)) __PYX_ERR(0, 150, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "genome_info/kmers/kmer_reader.pyx":151
+ *         start_freq[38, i] = ibf.start.GCG[i]
+ *         start_freq[39, i] = ibf.start.GCT[i]
+ *         start_freq[40, i] = ibf.start.GGA[i]             # <<<<<<<<<<<<<<
+ *         start_freq[41, i] = ibf.start.GGC[i]
+ *         start_freq[42, i] = ibf.start.GGG[i]
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->start->GGA[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 151, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 151, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 151, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_INCREF(__pyx_int_40);
+    __Pyx_GIVEREF(__pyx_int_40);
+    PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_int_40);
+    __Pyx_GIVEREF(__pyx_t_1);
+    PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_1);
+    __pyx_t_1 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_start_freq), __pyx_t_4, __pyx_t_2) < 0)) __PYX_ERR(0, 151, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "genome_info/kmers/kmer_reader.pyx":152
+ *         start_freq[39, i] = ibf.start.GCT[i]
+ *         start_freq[40, i] = ibf.start.GGA[i]
+ *         start_freq[41, i] = ibf.start.GGC[i]             # <<<<<<<<<<<<<<
+ *         start_freq[42, i] = ibf.start.GGG[i]
+ *         start_freq[43, i] = ibf.start.GGT[i]
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->start->GGC[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 152, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 152, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 152, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_int_41);
+    __Pyx_GIVEREF(__pyx_int_41);
+    PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_int_41);
+    __Pyx_GIVEREF(__pyx_t_4);
+    PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_4);
+    __pyx_t_4 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_start_freq), __pyx_t_1, __pyx_t_2) < 0)) __PYX_ERR(0, 152, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "genome_info/kmers/kmer_reader.pyx":153
+ *         start_freq[40, i] = ibf.start.GGA[i]
+ *         start_freq[41, i] = ibf.start.GGC[i]
+ *         start_freq[42, i] = ibf.start.GGG[i]             # <<<<<<<<<<<<<<
+ *         start_freq[43, i] = ibf.start.GGT[i]
+ *         start_freq[44, i] = ibf.start.GTA[i]
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->start->GGG[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 153, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 153, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 153, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_INCREF(__pyx_int_42);
+    __Pyx_GIVEREF(__pyx_int_42);
+    PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_int_42);
+    __Pyx_GIVEREF(__pyx_t_1);
+    PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_1);
+    __pyx_t_1 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_start_freq), __pyx_t_4, __pyx_t_2) < 0)) __PYX_ERR(0, 153, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "genome_info/kmers/kmer_reader.pyx":154
+ *         start_freq[41, i] = ibf.start.GGC[i]
+ *         start_freq[42, i] = ibf.start.GGG[i]
+ *         start_freq[43, i] = ibf.start.GGT[i]             # <<<<<<<<<<<<<<
+ *         start_freq[44, i] = ibf.start.GTA[i]
+ *         start_freq[45, i] = ibf.start.GTC[i]
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->start->GGT[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 154, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 154, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 154, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_int_43);
+    __Pyx_GIVEREF(__pyx_int_43);
+    PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_int_43);
+    __Pyx_GIVEREF(__pyx_t_4);
+    PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_4);
+    __pyx_t_4 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_start_freq), __pyx_t_1, __pyx_t_2) < 0)) __PYX_ERR(0, 154, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "genome_info/kmers/kmer_reader.pyx":155
+ *         start_freq[42, i] = ibf.start.GGG[i]
+ *         start_freq[43, i] = ibf.start.GGT[i]
+ *         start_freq[44, i] = ibf.start.GTA[i]             # <<<<<<<<<<<<<<
+ *         start_freq[45, i] = ibf.start.GTC[i]
+ *         start_freq[46, i] = ibf.start.GTG[i]
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->start->GTA[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 155, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 155, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 155, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_INCREF(__pyx_int_44);
+    __Pyx_GIVEREF(__pyx_int_44);
+    PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_int_44);
+    __Pyx_GIVEREF(__pyx_t_1);
+    PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_1);
+    __pyx_t_1 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_start_freq), __pyx_t_4, __pyx_t_2) < 0)) __PYX_ERR(0, 155, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "genome_info/kmers/kmer_reader.pyx":156
+ *         start_freq[43, i] = ibf.start.GGT[i]
+ *         start_freq[44, i] = ibf.start.GTA[i]
+ *         start_freq[45, i] = ibf.start.GTC[i]             # <<<<<<<<<<<<<<
+ *         start_freq[46, i] = ibf.start.GTG[i]
+ *         start_freq[47, i] = ibf.start.GTT[i]
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->start->GTC[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 156, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 156, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 156, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_int_45);
+    __Pyx_GIVEREF(__pyx_int_45);
+    PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_int_45);
+    __Pyx_GIVEREF(__pyx_t_4);
+    PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_4);
+    __pyx_t_4 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_start_freq), __pyx_t_1, __pyx_t_2) < 0)) __PYX_ERR(0, 156, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "genome_info/kmers/kmer_reader.pyx":157
+ *         start_freq[44, i] = ibf.start.GTA[i]
+ *         start_freq[45, i] = ibf.start.GTC[i]
+ *         start_freq[46, i] = ibf.start.GTG[i]             # <<<<<<<<<<<<<<
+ *         start_freq[47, i] = ibf.start.GTT[i]
+ *         start_freq[48, i] = ibf.start.TAA[i]
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->start->GTG[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 157, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 157, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 157, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_INCREF(__pyx_int_46);
+    __Pyx_GIVEREF(__pyx_int_46);
+    PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_int_46);
+    __Pyx_GIVEREF(__pyx_t_1);
+    PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_1);
+    __pyx_t_1 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_start_freq), __pyx_t_4, __pyx_t_2) < 0)) __PYX_ERR(0, 157, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "genome_info/kmers/kmer_reader.pyx":158
+ *         start_freq[45, i] = ibf.start.GTC[i]
+ *         start_freq[46, i] = ibf.start.GTG[i]
+ *         start_freq[47, i] = ibf.start.GTT[i]             # <<<<<<<<<<<<<<
+ *         start_freq[48, i] = ibf.start.TAA[i]
+ *         start_freq[49, i] = ibf.start.TAC[i]
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->start->GTT[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 158, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 158, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 158, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_int_47);
+    __Pyx_GIVEREF(__pyx_int_47);
+    PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_int_47);
+    __Pyx_GIVEREF(__pyx_t_4);
+    PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_4);
+    __pyx_t_4 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_start_freq), __pyx_t_1, __pyx_t_2) < 0)) __PYX_ERR(0, 158, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "genome_info/kmers/kmer_reader.pyx":159
+ *         start_freq[46, i] = ibf.start.GTG[i]
+ *         start_freq[47, i] = ibf.start.GTT[i]
+ *         start_freq[48, i] = ibf.start.TAA[i]             # <<<<<<<<<<<<<<
+ *         start_freq[49, i] = ibf.start.TAC[i]
+ *         start_freq[50, i] = ibf.start.TAG[i]
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->start->TAA[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 159, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 159, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 159, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_INCREF(__pyx_int_48);
+    __Pyx_GIVEREF(__pyx_int_48);
+    PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_int_48);
+    __Pyx_GIVEREF(__pyx_t_1);
+    PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_1);
+    __pyx_t_1 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_start_freq), __pyx_t_4, __pyx_t_2) < 0)) __PYX_ERR(0, 159, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "genome_info/kmers/kmer_reader.pyx":160
+ *         start_freq[47, i] = ibf.start.GTT[i]
+ *         start_freq[48, i] = ibf.start.TAA[i]
+ *         start_freq[49, i] = ibf.start.TAC[i]             # <<<<<<<<<<<<<<
+ *         start_freq[50, i] = ibf.start.TAG[i]
+ *         start_freq[51, i] = ibf.start.TAT[i]
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->start->TAC[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 160, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 160, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 160, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_int_49);
+    __Pyx_GIVEREF(__pyx_int_49);
+    PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_int_49);
+    __Pyx_GIVEREF(__pyx_t_4);
+    PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_4);
+    __pyx_t_4 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_start_freq), __pyx_t_1, __pyx_t_2) < 0)) __PYX_ERR(0, 160, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "genome_info/kmers/kmer_reader.pyx":161
+ *         start_freq[48, i] = ibf.start.TAA[i]
+ *         start_freq[49, i] = ibf.start.TAC[i]
+ *         start_freq[50, i] = ibf.start.TAG[i]             # <<<<<<<<<<<<<<
+ *         start_freq[51, i] = ibf.start.TAT[i]
+ *         start_freq[52, i] = ibf.start.TCA[i]
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->start->TAG[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 161, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 161, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 161, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_INCREF(__pyx_int_50);
+    __Pyx_GIVEREF(__pyx_int_50);
+    PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_int_50);
+    __Pyx_GIVEREF(__pyx_t_1);
+    PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_1);
+    __pyx_t_1 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_start_freq), __pyx_t_4, __pyx_t_2) < 0)) __PYX_ERR(0, 161, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "genome_info/kmers/kmer_reader.pyx":162
+ *         start_freq[49, i] = ibf.start.TAC[i]
+ *         start_freq[50, i] = ibf.start.TAG[i]
+ *         start_freq[51, i] = ibf.start.TAT[i]             # <<<<<<<<<<<<<<
+ *         start_freq[52, i] = ibf.start.TCA[i]
+ *         start_freq[53, i] = ibf.start.TCC[i]
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->start->TAT[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 162, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 162, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 162, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_int_51);
+    __Pyx_GIVEREF(__pyx_int_51);
+    PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_int_51);
+    __Pyx_GIVEREF(__pyx_t_4);
+    PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_4);
+    __pyx_t_4 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_start_freq), __pyx_t_1, __pyx_t_2) < 0)) __PYX_ERR(0, 162, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "genome_info/kmers/kmer_reader.pyx":163
+ *         start_freq[50, i] = ibf.start.TAG[i]
+ *         start_freq[51, i] = ibf.start.TAT[i]
+ *         start_freq[52, i] = ibf.start.TCA[i]             # <<<<<<<<<<<<<<
+ *         start_freq[53, i] = ibf.start.TCC[i]
+ *         start_freq[54, i] = ibf.start.TCG[i]
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->start->TCA[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 163, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 163, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 163, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_INCREF(__pyx_int_52);
+    __Pyx_GIVEREF(__pyx_int_52);
+    PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_int_52);
+    __Pyx_GIVEREF(__pyx_t_1);
+    PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_1);
+    __pyx_t_1 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_start_freq), __pyx_t_4, __pyx_t_2) < 0)) __PYX_ERR(0, 163, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "genome_info/kmers/kmer_reader.pyx":164
+ *         start_freq[51, i] = ibf.start.TAT[i]
+ *         start_freq[52, i] = ibf.start.TCA[i]
+ *         start_freq[53, i] = ibf.start.TCC[i]             # <<<<<<<<<<<<<<
+ *         start_freq[54, i] = ibf.start.TCG[i]
+ *         start_freq[55, i] = ibf.start.TCT[i]
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->start->TCC[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 164, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 164, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 164, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_int_53);
+    __Pyx_GIVEREF(__pyx_int_53);
+    PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_int_53);
+    __Pyx_GIVEREF(__pyx_t_4);
+    PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_4);
+    __pyx_t_4 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_start_freq), __pyx_t_1, __pyx_t_2) < 0)) __PYX_ERR(0, 164, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "genome_info/kmers/kmer_reader.pyx":165
+ *         start_freq[52, i] = ibf.start.TCA[i]
+ *         start_freq[53, i] = ibf.start.TCC[i]
+ *         start_freq[54, i] = ibf.start.TCG[i]             # <<<<<<<<<<<<<<
+ *         start_freq[55, i] = ibf.start.TCT[i]
+ *         start_freq[56, i] = ibf.start.TGA[i]
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->start->TCG[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 165, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 165, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 165, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_INCREF(__pyx_int_54);
+    __Pyx_GIVEREF(__pyx_int_54);
+    PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_int_54);
+    __Pyx_GIVEREF(__pyx_t_1);
+    PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_1);
+    __pyx_t_1 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_start_freq), __pyx_t_4, __pyx_t_2) < 0)) __PYX_ERR(0, 165, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "genome_info/kmers/kmer_reader.pyx":166
+ *         start_freq[53, i] = ibf.start.TCC[i]
+ *         start_freq[54, i] = ibf.start.TCG[i]
+ *         start_freq[55, i] = ibf.start.TCT[i]             # <<<<<<<<<<<<<<
+ *         start_freq[56, i] = ibf.start.TGA[i]
+ *         start_freq[57, i] = ibf.start.TGC[i]
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->start->TCT[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 166, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 166, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 166, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_int_55);
+    __Pyx_GIVEREF(__pyx_int_55);
+    PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_int_55);
+    __Pyx_GIVEREF(__pyx_t_4);
+    PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_4);
+    __pyx_t_4 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_start_freq), __pyx_t_1, __pyx_t_2) < 0)) __PYX_ERR(0, 166, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "genome_info/kmers/kmer_reader.pyx":167
+ *         start_freq[54, i] = ibf.start.TCG[i]
+ *         start_freq[55, i] = ibf.start.TCT[i]
+ *         start_freq[56, i] = ibf.start.TGA[i]             # <<<<<<<<<<<<<<
+ *         start_freq[57, i] = ibf.start.TGC[i]
+ *         start_freq[58, i] = ibf.start.TGG[i]
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->start->TGA[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 167, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 167, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 167, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_INCREF(__pyx_int_56);
+    __Pyx_GIVEREF(__pyx_int_56);
+    PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_int_56);
+    __Pyx_GIVEREF(__pyx_t_1);
+    PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_1);
+    __pyx_t_1 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_start_freq), __pyx_t_4, __pyx_t_2) < 0)) __PYX_ERR(0, 167, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "genome_info/kmers/kmer_reader.pyx":168
+ *         start_freq[55, i] = ibf.start.TCT[i]
+ *         start_freq[56, i] = ibf.start.TGA[i]
+ *         start_freq[57, i] = ibf.start.TGC[i]             # <<<<<<<<<<<<<<
+ *         start_freq[58, i] = ibf.start.TGG[i]
+ *         start_freq[59, i] = ibf.start.TGT[i]
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->start->TGC[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 168, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 168, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 168, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_int_57);
+    __Pyx_GIVEREF(__pyx_int_57);
+    PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_int_57);
+    __Pyx_GIVEREF(__pyx_t_4);
+    PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_4);
+    __pyx_t_4 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_start_freq), __pyx_t_1, __pyx_t_2) < 0)) __PYX_ERR(0, 168, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "genome_info/kmers/kmer_reader.pyx":169
+ *         start_freq[56, i] = ibf.start.TGA[i]
+ *         start_freq[57, i] = ibf.start.TGC[i]
+ *         start_freq[58, i] = ibf.start.TGG[i]             # <<<<<<<<<<<<<<
+ *         start_freq[59, i] = ibf.start.TGT[i]
+ *         start_freq[60, i] = ibf.start.TTA[i]
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->start->TGG[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 169, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 169, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 169, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_INCREF(__pyx_int_58);
+    __Pyx_GIVEREF(__pyx_int_58);
+    PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_int_58);
+    __Pyx_GIVEREF(__pyx_t_1);
+    PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_1);
+    __pyx_t_1 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_start_freq), __pyx_t_4, __pyx_t_2) < 0)) __PYX_ERR(0, 169, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "genome_info/kmers/kmer_reader.pyx":170
+ *         start_freq[57, i] = ibf.start.TGC[i]
+ *         start_freq[58, i] = ibf.start.TGG[i]
+ *         start_freq[59, i] = ibf.start.TGT[i]             # <<<<<<<<<<<<<<
+ *         start_freq[60, i] = ibf.start.TTA[i]
+ *         start_freq[61, i] = ibf.start.TTC[i]
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->start->TGT[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 170, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 170, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 170, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_int_59);
+    __Pyx_GIVEREF(__pyx_int_59);
+    PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_int_59);
+    __Pyx_GIVEREF(__pyx_t_4);
+    PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_4);
+    __pyx_t_4 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_start_freq), __pyx_t_1, __pyx_t_2) < 0)) __PYX_ERR(0, 170, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "genome_info/kmers/kmer_reader.pyx":171
+ *         start_freq[58, i] = ibf.start.TGG[i]
+ *         start_freq[59, i] = ibf.start.TGT[i]
+ *         start_freq[60, i] = ibf.start.TTA[i]             # <<<<<<<<<<<<<<
+ *         start_freq[61, i] = ibf.start.TTC[i]
+ *         start_freq[62, i] = ibf.start.TTG[i]
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->start->TTA[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 171, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 171, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 171, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_INCREF(__pyx_int_60);
+    __Pyx_GIVEREF(__pyx_int_60);
+    PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_int_60);
+    __Pyx_GIVEREF(__pyx_t_1);
+    PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_1);
+    __pyx_t_1 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_start_freq), __pyx_t_4, __pyx_t_2) < 0)) __PYX_ERR(0, 171, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "genome_info/kmers/kmer_reader.pyx":172
+ *         start_freq[59, i] = ibf.start.TGT[i]
+ *         start_freq[60, i] = ibf.start.TTA[i]
+ *         start_freq[61, i] = ibf.start.TTC[i]             # <<<<<<<<<<<<<<
+ *         start_freq[62, i] = ibf.start.TTG[i]
+ *         start_freq[63, i] = ibf.start.TTT[i]
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->start->TTC[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 172, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 172, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 172, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_int_61);
+    __Pyx_GIVEREF(__pyx_int_61);
+    PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_int_61);
+    __Pyx_GIVEREF(__pyx_t_4);
+    PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_4);
+    __pyx_t_4 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_start_freq), __pyx_t_1, __pyx_t_2) < 0)) __PYX_ERR(0, 172, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "genome_info/kmers/kmer_reader.pyx":173
+ *         start_freq[60, i] = ibf.start.TTA[i]
+ *         start_freq[61, i] = ibf.start.TTC[i]
+ *         start_freq[62, i] = ibf.start.TTG[i]             # <<<<<<<<<<<<<<
+ *         start_freq[63, i] = ibf.start.TTT[i]
+ *         end_freq[0, i] = ibf.end.AAA[i]
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->start->TTG[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 173, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 173, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 173, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_INCREF(__pyx_int_62);
+    __Pyx_GIVEREF(__pyx_int_62);
+    PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_int_62);
+    __Pyx_GIVEREF(__pyx_t_1);
+    PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_1);
+    __pyx_t_1 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_start_freq), __pyx_t_4, __pyx_t_2) < 0)) __PYX_ERR(0, 173, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "genome_info/kmers/kmer_reader.pyx":174
+ *         start_freq[61, i] = ibf.start.TTC[i]
+ *         start_freq[62, i] = ibf.start.TTG[i]
+ *         start_freq[63, i] = ibf.start.TTT[i]             # <<<<<<<<<<<<<<
+ *         end_freq[0, i] = ibf.end.AAA[i]
+ *         end_freq[1, i] = ibf.end.AAC[i]
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->start->TTT[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 174, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 174, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 174, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_int_63);
+    __Pyx_GIVEREF(__pyx_int_63);
+    PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_int_63);
+    __Pyx_GIVEREF(__pyx_t_4);
+    PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_4);
+    __pyx_t_4 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_start_freq), __pyx_t_1, __pyx_t_2) < 0)) __PYX_ERR(0, 174, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "genome_info/kmers/kmer_reader.pyx":175
+ *         start_freq[62, i] = ibf.start.TTG[i]
+ *         start_freq[63, i] = ibf.start.TTT[i]
+ *         end_freq[0, i] = ibf.end.AAA[i]             # <<<<<<<<<<<<<<
+ *         end_freq[1, i] = ibf.end.AAC[i]
+ *         end_freq[2, i] = ibf.end.AAG[i]
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->end->AAA[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 175, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 175, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 175, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_INCREF(__pyx_int_0);
+    __Pyx_GIVEREF(__pyx_int_0);
+    PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_int_0);
+    __Pyx_GIVEREF(__pyx_t_1);
+    PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_1);
+    __pyx_t_1 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_end_freq), __pyx_t_4, __pyx_t_2) < 0)) __PYX_ERR(0, 175, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "genome_info/kmers/kmer_reader.pyx":176
+ *         start_freq[63, i] = ibf.start.TTT[i]
+ *         end_freq[0, i] = ibf.end.AAA[i]
+ *         end_freq[1, i] = ibf.end.AAC[i]             # <<<<<<<<<<<<<<
+ *         end_freq[2, i] = ibf.end.AAG[i]
+ *         end_freq[3, i] = ibf.end.AAT[i]
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->end->AAC[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 176, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 176, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 176, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_int_1);
+    __Pyx_GIVEREF(__pyx_int_1);
+    PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_int_1);
+    __Pyx_GIVEREF(__pyx_t_4);
+    PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_4);
+    __pyx_t_4 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_end_freq), __pyx_t_1, __pyx_t_2) < 0)) __PYX_ERR(0, 176, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "genome_info/kmers/kmer_reader.pyx":177
+ *         end_freq[0, i] = ibf.end.AAA[i]
+ *         end_freq[1, i] = ibf.end.AAC[i]
+ *         end_freq[2, i] = ibf.end.AAG[i]             # <<<<<<<<<<<<<<
+ *         end_freq[3, i] = ibf.end.AAT[i]
+ *         end_freq[4, i] = ibf.end.ACA[i]
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->end->AAG[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 177, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 177, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 177, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_INCREF(__pyx_int_2);
+    __Pyx_GIVEREF(__pyx_int_2);
+    PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_int_2);
+    __Pyx_GIVEREF(__pyx_t_1);
+    PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_1);
+    __pyx_t_1 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_end_freq), __pyx_t_4, __pyx_t_2) < 0)) __PYX_ERR(0, 177, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "genome_info/kmers/kmer_reader.pyx":178
+ *         end_freq[1, i] = ibf.end.AAC[i]
+ *         end_freq[2, i] = ibf.end.AAG[i]
+ *         end_freq[3, i] = ibf.end.AAT[i]             # <<<<<<<<<<<<<<
+ *         end_freq[4, i] = ibf.end.ACA[i]
+ *         end_freq[5, i] = ibf.end.ACC[i]
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->end->AAT[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 178, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 178, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 178, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_int_3);
+    __Pyx_GIVEREF(__pyx_int_3);
+    PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_int_3);
+    __Pyx_GIVEREF(__pyx_t_4);
+    PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_4);
+    __pyx_t_4 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_end_freq), __pyx_t_1, __pyx_t_2) < 0)) __PYX_ERR(0, 178, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "genome_info/kmers/kmer_reader.pyx":179
+ *         end_freq[2, i] = ibf.end.AAG[i]
+ *         end_freq[3, i] = ibf.end.AAT[i]
+ *         end_freq[4, i] = ibf.end.ACA[i]             # <<<<<<<<<<<<<<
+ *         end_freq[5, i] = ibf.end.ACC[i]
+ *         end_freq[6, i] = ibf.end.ACG[i]
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->end->ACA[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 179, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 179, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 179, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_INCREF(__pyx_int_4);
+    __Pyx_GIVEREF(__pyx_int_4);
+    PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_int_4);
+    __Pyx_GIVEREF(__pyx_t_1);
+    PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_1);
+    __pyx_t_1 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_end_freq), __pyx_t_4, __pyx_t_2) < 0)) __PYX_ERR(0, 179, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "genome_info/kmers/kmer_reader.pyx":180
+ *         end_freq[3, i] = ibf.end.AAT[i]
+ *         end_freq[4, i] = ibf.end.ACA[i]
+ *         end_freq[5, i] = ibf.end.ACC[i]             # <<<<<<<<<<<<<<
+ *         end_freq[6, i] = ibf.end.ACG[i]
+ *         end_freq[7, i] = ibf.end.ACT[i]
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->end->ACC[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 180, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 180, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 180, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_int_5);
+    __Pyx_GIVEREF(__pyx_int_5);
+    PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_int_5);
+    __Pyx_GIVEREF(__pyx_t_4);
+    PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_4);
+    __pyx_t_4 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_end_freq), __pyx_t_1, __pyx_t_2) < 0)) __PYX_ERR(0, 180, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "genome_info/kmers/kmer_reader.pyx":181
+ *         end_freq[4, i] = ibf.end.ACA[i]
+ *         end_freq[5, i] = ibf.end.ACC[i]
+ *         end_freq[6, i] = ibf.end.ACG[i]             # <<<<<<<<<<<<<<
+ *         end_freq[7, i] = ibf.end.ACT[i]
+ *         end_freq[8, i] = ibf.end.AGA[i]
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->end->ACG[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 181, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 181, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 181, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_INCREF(__pyx_int_6);
+    __Pyx_GIVEREF(__pyx_int_6);
+    PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_int_6);
+    __Pyx_GIVEREF(__pyx_t_1);
+    PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_1);
+    __pyx_t_1 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_end_freq), __pyx_t_4, __pyx_t_2) < 0)) __PYX_ERR(0, 181, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "genome_info/kmers/kmer_reader.pyx":182
+ *         end_freq[5, i] = ibf.end.ACC[i]
+ *         end_freq[6, i] = ibf.end.ACG[i]
+ *         end_freq[7, i] = ibf.end.ACT[i]             # <<<<<<<<<<<<<<
+ *         end_freq[8, i] = ibf.end.AGA[i]
+ *         end_freq[9, i] = ibf.end.AGC[i]
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->end->ACT[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 182, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 182, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 182, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_int_7);
+    __Pyx_GIVEREF(__pyx_int_7);
+    PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_int_7);
+    __Pyx_GIVEREF(__pyx_t_4);
+    PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_4);
+    __pyx_t_4 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_end_freq), __pyx_t_1, __pyx_t_2) < 0)) __PYX_ERR(0, 182, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "genome_info/kmers/kmer_reader.pyx":183
+ *         end_freq[6, i] = ibf.end.ACG[i]
+ *         end_freq[7, i] = ibf.end.ACT[i]
+ *         end_freq[8, i] = ibf.end.AGA[i]             # <<<<<<<<<<<<<<
+ *         end_freq[9, i] = ibf.end.AGC[i]
+ *         end_freq[10, i] = ibf.end.AGG[i]
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->end->AGA[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 183, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 183, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 183, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_INCREF(__pyx_int_8);
+    __Pyx_GIVEREF(__pyx_int_8);
+    PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_int_8);
+    __Pyx_GIVEREF(__pyx_t_1);
+    PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_1);
+    __pyx_t_1 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_end_freq), __pyx_t_4, __pyx_t_2) < 0)) __PYX_ERR(0, 183, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "genome_info/kmers/kmer_reader.pyx":184
+ *         end_freq[7, i] = ibf.end.ACT[i]
+ *         end_freq[8, i] = ibf.end.AGA[i]
+ *         end_freq[9, i] = ibf.end.AGC[i]             # <<<<<<<<<<<<<<
+ *         end_freq[10, i] = ibf.end.AGG[i]
+ *         end_freq[11, i] = ibf.end.AGT[i]
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->end->AGC[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 184, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 184, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 184, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_int_9);
+    __Pyx_GIVEREF(__pyx_int_9);
+    PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_int_9);
+    __Pyx_GIVEREF(__pyx_t_4);
+    PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_4);
+    __pyx_t_4 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_end_freq), __pyx_t_1, __pyx_t_2) < 0)) __PYX_ERR(0, 184, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "genome_info/kmers/kmer_reader.pyx":185
+ *         end_freq[8, i] = ibf.end.AGA[i]
+ *         end_freq[9, i] = ibf.end.AGC[i]
+ *         end_freq[10, i] = ibf.end.AGG[i]             # <<<<<<<<<<<<<<
+ *         end_freq[11, i] = ibf.end.AGT[i]
+ *         end_freq[12, i] = ibf.end.ATA[i]
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->end->AGG[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 185, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 185, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 185, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_INCREF(__pyx_int_10);
+    __Pyx_GIVEREF(__pyx_int_10);
+    PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_int_10);
+    __Pyx_GIVEREF(__pyx_t_1);
+    PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_1);
+    __pyx_t_1 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_end_freq), __pyx_t_4, __pyx_t_2) < 0)) __PYX_ERR(0, 185, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "genome_info/kmers/kmer_reader.pyx":186
+ *         end_freq[9, i] = ibf.end.AGC[i]
+ *         end_freq[10, i] = ibf.end.AGG[i]
+ *         end_freq[11, i] = ibf.end.AGT[i]             # <<<<<<<<<<<<<<
+ *         end_freq[12, i] = ibf.end.ATA[i]
+ *         end_freq[13, i] = ibf.end.ATC[i]
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->end->AGT[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 186, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 186, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 186, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_int_11);
+    __Pyx_GIVEREF(__pyx_int_11);
+    PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_int_11);
+    __Pyx_GIVEREF(__pyx_t_4);
+    PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_4);
+    __pyx_t_4 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_end_freq), __pyx_t_1, __pyx_t_2) < 0)) __PYX_ERR(0, 186, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "genome_info/kmers/kmer_reader.pyx":187
+ *         end_freq[10, i] = ibf.end.AGG[i]
+ *         end_freq[11, i] = ibf.end.AGT[i]
+ *         end_freq[12, i] = ibf.end.ATA[i]             # <<<<<<<<<<<<<<
+ *         end_freq[13, i] = ibf.end.ATC[i]
+ *         end_freq[14, i] = ibf.end.ATG[i]
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->end->ATA[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 187, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 187, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 187, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_INCREF(__pyx_int_12);
+    __Pyx_GIVEREF(__pyx_int_12);
+    PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_int_12);
+    __Pyx_GIVEREF(__pyx_t_1);
+    PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_1);
+    __pyx_t_1 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_end_freq), __pyx_t_4, __pyx_t_2) < 0)) __PYX_ERR(0, 187, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "genome_info/kmers/kmer_reader.pyx":188
+ *         end_freq[11, i] = ibf.end.AGT[i]
+ *         end_freq[12, i] = ibf.end.ATA[i]
+ *         end_freq[13, i] = ibf.end.ATC[i]             # <<<<<<<<<<<<<<
+ *         end_freq[14, i] = ibf.end.ATG[i]
+ *         end_freq[15, i] = ibf.end.ATT[i]
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->end->ATC[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 188, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 188, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 188, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_int_13);
+    __Pyx_GIVEREF(__pyx_int_13);
+    PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_int_13);
+    __Pyx_GIVEREF(__pyx_t_4);
+    PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_4);
+    __pyx_t_4 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_end_freq), __pyx_t_1, __pyx_t_2) < 0)) __PYX_ERR(0, 188, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "genome_info/kmers/kmer_reader.pyx":189
+ *         end_freq[12, i] = ibf.end.ATA[i]
+ *         end_freq[13, i] = ibf.end.ATC[i]
+ *         end_freq[14, i] = ibf.end.ATG[i]             # <<<<<<<<<<<<<<
+ *         end_freq[15, i] = ibf.end.ATT[i]
+ *         end_freq[16, i] = ibf.end.CAA[i]
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->end->ATG[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 189, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 189, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 189, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_INCREF(__pyx_int_14);
+    __Pyx_GIVEREF(__pyx_int_14);
+    PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_int_14);
+    __Pyx_GIVEREF(__pyx_t_1);
+    PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_1);
+    __pyx_t_1 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_end_freq), __pyx_t_4, __pyx_t_2) < 0)) __PYX_ERR(0, 189, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "genome_info/kmers/kmer_reader.pyx":190
+ *         end_freq[13, i] = ibf.end.ATC[i]
+ *         end_freq[14, i] = ibf.end.ATG[i]
+ *         end_freq[15, i] = ibf.end.ATT[i]             # <<<<<<<<<<<<<<
+ *         end_freq[16, i] = ibf.end.CAA[i]
+ *         end_freq[17, i] = ibf.end.CAC[i]
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->end->ATT[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 190, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 190, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 190, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_int_15);
+    __Pyx_GIVEREF(__pyx_int_15);
+    PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_int_15);
+    __Pyx_GIVEREF(__pyx_t_4);
+    PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_4);
+    __pyx_t_4 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_end_freq), __pyx_t_1, __pyx_t_2) < 0)) __PYX_ERR(0, 190, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "genome_info/kmers/kmer_reader.pyx":191
+ *         end_freq[14, i] = ibf.end.ATG[i]
+ *         end_freq[15, i] = ibf.end.ATT[i]
+ *         end_freq[16, i] = ibf.end.CAA[i]             # <<<<<<<<<<<<<<
+ *         end_freq[17, i] = ibf.end.CAC[i]
+ *         end_freq[18, i] = ibf.end.CAG[i]
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->end->CAA[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 191, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 191, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 191, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_INCREF(__pyx_int_16);
+    __Pyx_GIVEREF(__pyx_int_16);
+    PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_int_16);
+    __Pyx_GIVEREF(__pyx_t_1);
+    PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_1);
+    __pyx_t_1 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_end_freq), __pyx_t_4, __pyx_t_2) < 0)) __PYX_ERR(0, 191, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "genome_info/kmers/kmer_reader.pyx":192
+ *         end_freq[15, i] = ibf.end.ATT[i]
+ *         end_freq[16, i] = ibf.end.CAA[i]
+ *         end_freq[17, i] = ibf.end.CAC[i]             # <<<<<<<<<<<<<<
+ *         end_freq[18, i] = ibf.end.CAG[i]
+ *         end_freq[19, i] = ibf.end.CAT[i]
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->end->CAC[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 192, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 192, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 192, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_int_17);
+    __Pyx_GIVEREF(__pyx_int_17);
+    PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_int_17);
+    __Pyx_GIVEREF(__pyx_t_4);
+    PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_4);
+    __pyx_t_4 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_end_freq), __pyx_t_1, __pyx_t_2) < 0)) __PYX_ERR(0, 192, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "genome_info/kmers/kmer_reader.pyx":193
+ *         end_freq[16, i] = ibf.end.CAA[i]
+ *         end_freq[17, i] = ibf.end.CAC[i]
+ *         end_freq[18, i] = ibf.end.CAG[i]             # <<<<<<<<<<<<<<
+ *         end_freq[19, i] = ibf.end.CAT[i]
+ *         end_freq[20, i] = ibf.end.CCA[i]
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->end->CAG[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 193, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 193, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 193, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_INCREF(__pyx_int_18);
+    __Pyx_GIVEREF(__pyx_int_18);
+    PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_int_18);
+    __Pyx_GIVEREF(__pyx_t_1);
+    PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_1);
+    __pyx_t_1 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_end_freq), __pyx_t_4, __pyx_t_2) < 0)) __PYX_ERR(0, 193, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "genome_info/kmers/kmer_reader.pyx":194
+ *         end_freq[17, i] = ibf.end.CAC[i]
+ *         end_freq[18, i] = ibf.end.CAG[i]
+ *         end_freq[19, i] = ibf.end.CAT[i]             # <<<<<<<<<<<<<<
+ *         end_freq[20, i] = ibf.end.CCA[i]
+ *         end_freq[21, i] = ibf.end.CCC[i]
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->end->CAT[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 194, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 194, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 194, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_int_19);
+    __Pyx_GIVEREF(__pyx_int_19);
+    PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_int_19);
+    __Pyx_GIVEREF(__pyx_t_4);
+    PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_4);
+    __pyx_t_4 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_end_freq), __pyx_t_1, __pyx_t_2) < 0)) __PYX_ERR(0, 194, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "genome_info/kmers/kmer_reader.pyx":195
+ *         end_freq[18, i] = ibf.end.CAG[i]
+ *         end_freq[19, i] = ibf.end.CAT[i]
+ *         end_freq[20, i] = ibf.end.CCA[i]             # <<<<<<<<<<<<<<
+ *         end_freq[21, i] = ibf.end.CCC[i]
+ *         end_freq[22, i] = ibf.end.CCG[i]
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->end->CCA[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 195, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 195, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 195, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_INCREF(__pyx_int_20);
+    __Pyx_GIVEREF(__pyx_int_20);
+    PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_int_20);
+    __Pyx_GIVEREF(__pyx_t_1);
+    PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_1);
+    __pyx_t_1 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_end_freq), __pyx_t_4, __pyx_t_2) < 0)) __PYX_ERR(0, 195, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "genome_info/kmers/kmer_reader.pyx":196
+ *         end_freq[19, i] = ibf.end.CAT[i]
+ *         end_freq[20, i] = ibf.end.CCA[i]
+ *         end_freq[21, i] = ibf.end.CCC[i]             # <<<<<<<<<<<<<<
+ *         end_freq[22, i] = ibf.end.CCG[i]
+ *         end_freq[23, i] = ibf.end.CCT[i]
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->end->CCC[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 196, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 196, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 196, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_int_21);
+    __Pyx_GIVEREF(__pyx_int_21);
+    PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_int_21);
+    __Pyx_GIVEREF(__pyx_t_4);
+    PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_4);
+    __pyx_t_4 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_end_freq), __pyx_t_1, __pyx_t_2) < 0)) __PYX_ERR(0, 196, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "genome_info/kmers/kmer_reader.pyx":197
+ *         end_freq[20, i] = ibf.end.CCA[i]
+ *         end_freq[21, i] = ibf.end.CCC[i]
+ *         end_freq[22, i] = ibf.end.CCG[i]             # <<<<<<<<<<<<<<
+ *         end_freq[23, i] = ibf.end.CCT[i]
+ *         end_freq[24, i] = ibf.end.CGA[i]
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->end->CCG[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 197, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 197, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 197, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_INCREF(__pyx_int_22);
+    __Pyx_GIVEREF(__pyx_int_22);
+    PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_int_22);
+    __Pyx_GIVEREF(__pyx_t_1);
+    PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_1);
+    __pyx_t_1 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_end_freq), __pyx_t_4, __pyx_t_2) < 0)) __PYX_ERR(0, 197, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "genome_info/kmers/kmer_reader.pyx":198
+ *         end_freq[21, i] = ibf.end.CCC[i]
+ *         end_freq[22, i] = ibf.end.CCG[i]
+ *         end_freq[23, i] = ibf.end.CCT[i]             # <<<<<<<<<<<<<<
+ *         end_freq[24, i] = ibf.end.CGA[i]
+ *         end_freq[25, i] = ibf.end.CGC[i]
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->end->CCT[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 198, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 198, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 198, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_int_23);
+    __Pyx_GIVEREF(__pyx_int_23);
+    PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_int_23);
+    __Pyx_GIVEREF(__pyx_t_4);
+    PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_4);
+    __pyx_t_4 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_end_freq), __pyx_t_1, __pyx_t_2) < 0)) __PYX_ERR(0, 198, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "genome_info/kmers/kmer_reader.pyx":199
+ *         end_freq[22, i] = ibf.end.CCG[i]
+ *         end_freq[23, i] = ibf.end.CCT[i]
+ *         end_freq[24, i] = ibf.end.CGA[i]             # <<<<<<<<<<<<<<
+ *         end_freq[25, i] = ibf.end.CGC[i]
+ *         end_freq[26, i] = ibf.end.CGG[i]
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->end->CGA[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 199, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 199, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 199, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_INCREF(__pyx_int_24);
+    __Pyx_GIVEREF(__pyx_int_24);
+    PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_int_24);
+    __Pyx_GIVEREF(__pyx_t_1);
+    PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_1);
+    __pyx_t_1 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_end_freq), __pyx_t_4, __pyx_t_2) < 0)) __PYX_ERR(0, 199, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "genome_info/kmers/kmer_reader.pyx":200
+ *         end_freq[23, i] = ibf.end.CCT[i]
+ *         end_freq[24, i] = ibf.end.CGA[i]
+ *         end_freq[25, i] = ibf.end.CGC[i]             # <<<<<<<<<<<<<<
+ *         end_freq[26, i] = ibf.end.CGG[i]
+ *         end_freq[27, i] = ibf.end.CGT[i]
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->end->CGC[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 200, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 200, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 200, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_int_25);
+    __Pyx_GIVEREF(__pyx_int_25);
+    PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_int_25);
+    __Pyx_GIVEREF(__pyx_t_4);
+    PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_4);
+    __pyx_t_4 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_end_freq), __pyx_t_1, __pyx_t_2) < 0)) __PYX_ERR(0, 200, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "genome_info/kmers/kmer_reader.pyx":201
+ *         end_freq[24, i] = ibf.end.CGA[i]
+ *         end_freq[25, i] = ibf.end.CGC[i]
+ *         end_freq[26, i] = ibf.end.CGG[i]             # <<<<<<<<<<<<<<
+ *         end_freq[27, i] = ibf.end.CGT[i]
+ *         end_freq[28, i] = ibf.end.CTA[i]
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->end->CGG[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 201, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 201, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 201, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_INCREF(__pyx_int_26);
+    __Pyx_GIVEREF(__pyx_int_26);
+    PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_int_26);
+    __Pyx_GIVEREF(__pyx_t_1);
+    PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_1);
+    __pyx_t_1 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_end_freq), __pyx_t_4, __pyx_t_2) < 0)) __PYX_ERR(0, 201, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "genome_info/kmers/kmer_reader.pyx":202
+ *         end_freq[25, i] = ibf.end.CGC[i]
+ *         end_freq[26, i] = ibf.end.CGG[i]
+ *         end_freq[27, i] = ibf.end.CGT[i]             # <<<<<<<<<<<<<<
+ *         end_freq[28, i] = ibf.end.CTA[i]
+ *         end_freq[29, i] = ibf.end.CTC[i]
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->end->CGT[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 202, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 202, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 202, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_int_27);
+    __Pyx_GIVEREF(__pyx_int_27);
+    PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_int_27);
+    __Pyx_GIVEREF(__pyx_t_4);
+    PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_4);
+    __pyx_t_4 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_end_freq), __pyx_t_1, __pyx_t_2) < 0)) __PYX_ERR(0, 202, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "genome_info/kmers/kmer_reader.pyx":203
+ *         end_freq[26, i] = ibf.end.CGG[i]
+ *         end_freq[27, i] = ibf.end.CGT[i]
+ *         end_freq[28, i] = ibf.end.CTA[i]             # <<<<<<<<<<<<<<
+ *         end_freq[29, i] = ibf.end.CTC[i]
+ *         end_freq[30, i] = ibf.end.CTG[i]
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->end->CTA[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 203, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 203, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 203, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_INCREF(__pyx_int_28);
+    __Pyx_GIVEREF(__pyx_int_28);
+    PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_int_28);
+    __Pyx_GIVEREF(__pyx_t_1);
+    PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_1);
+    __pyx_t_1 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_end_freq), __pyx_t_4, __pyx_t_2) < 0)) __PYX_ERR(0, 203, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "genome_info/kmers/kmer_reader.pyx":204
+ *         end_freq[27, i] = ibf.end.CGT[i]
+ *         end_freq[28, i] = ibf.end.CTA[i]
+ *         end_freq[29, i] = ibf.end.CTC[i]             # <<<<<<<<<<<<<<
+ *         end_freq[30, i] = ibf.end.CTG[i]
+ *         end_freq[31, i] = ibf.end.CTT[i]
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->end->CTC[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 204, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 204, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 204, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_int_29);
+    __Pyx_GIVEREF(__pyx_int_29);
+    PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_int_29);
+    __Pyx_GIVEREF(__pyx_t_4);
+    PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_4);
+    __pyx_t_4 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_end_freq), __pyx_t_1, __pyx_t_2) < 0)) __PYX_ERR(0, 204, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "genome_info/kmers/kmer_reader.pyx":205
+ *         end_freq[28, i] = ibf.end.CTA[i]
+ *         end_freq[29, i] = ibf.end.CTC[i]
+ *         end_freq[30, i] = ibf.end.CTG[i]             # <<<<<<<<<<<<<<
+ *         end_freq[31, i] = ibf.end.CTT[i]
+ *         end_freq[32, i] = ibf.end.GAA[i]
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->end->CTG[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 205, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 205, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 205, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_INCREF(__pyx_int_30);
+    __Pyx_GIVEREF(__pyx_int_30);
+    PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_int_30);
+    __Pyx_GIVEREF(__pyx_t_1);
+    PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_1);
+    __pyx_t_1 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_end_freq), __pyx_t_4, __pyx_t_2) < 0)) __PYX_ERR(0, 205, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "genome_info/kmers/kmer_reader.pyx":206
+ *         end_freq[29, i] = ibf.end.CTC[i]
+ *         end_freq[30, i] = ibf.end.CTG[i]
+ *         end_freq[31, i] = ibf.end.CTT[i]             # <<<<<<<<<<<<<<
+ *         end_freq[32, i] = ibf.end.GAA[i]
+ *         end_freq[33, i] = ibf.end.GAC[i]
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->end->CTT[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 206, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 206, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 206, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_int_31);
+    __Pyx_GIVEREF(__pyx_int_31);
+    PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_int_31);
+    __Pyx_GIVEREF(__pyx_t_4);
+    PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_4);
+    __pyx_t_4 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_end_freq), __pyx_t_1, __pyx_t_2) < 0)) __PYX_ERR(0, 206, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "genome_info/kmers/kmer_reader.pyx":207
+ *         end_freq[30, i] = ibf.end.CTG[i]
+ *         end_freq[31, i] = ibf.end.CTT[i]
+ *         end_freq[32, i] = ibf.end.GAA[i]             # <<<<<<<<<<<<<<
+ *         end_freq[33, i] = ibf.end.GAC[i]
+ *         end_freq[34, i] = ibf.end.GAG[i]
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->end->GAA[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 207, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 207, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 207, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_INCREF(__pyx_int_32);
+    __Pyx_GIVEREF(__pyx_int_32);
+    PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_int_32);
+    __Pyx_GIVEREF(__pyx_t_1);
+    PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_1);
+    __pyx_t_1 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_end_freq), __pyx_t_4, __pyx_t_2) < 0)) __PYX_ERR(0, 207, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "genome_info/kmers/kmer_reader.pyx":208
+ *         end_freq[31, i] = ibf.end.CTT[i]
+ *         end_freq[32, i] = ibf.end.GAA[i]
+ *         end_freq[33, i] = ibf.end.GAC[i]             # <<<<<<<<<<<<<<
+ *         end_freq[34, i] = ibf.end.GAG[i]
+ *         end_freq[35, i] = ibf.end.GAT[i]
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->end->GAC[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 208, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 208, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 208, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_int_33);
+    __Pyx_GIVEREF(__pyx_int_33);
+    PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_int_33);
+    __Pyx_GIVEREF(__pyx_t_4);
+    PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_4);
+    __pyx_t_4 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_end_freq), __pyx_t_1, __pyx_t_2) < 0)) __PYX_ERR(0, 208, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "genome_info/kmers/kmer_reader.pyx":209
+ *         end_freq[32, i] = ibf.end.GAA[i]
+ *         end_freq[33, i] = ibf.end.GAC[i]
+ *         end_freq[34, i] = ibf.end.GAG[i]             # <<<<<<<<<<<<<<
+ *         end_freq[35, i] = ibf.end.GAT[i]
+ *         end_freq[36, i] = ibf.end.GCA[i]
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->end->GAG[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 209, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 209, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 209, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_INCREF(__pyx_int_34);
+    __Pyx_GIVEREF(__pyx_int_34);
+    PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_int_34);
+    __Pyx_GIVEREF(__pyx_t_1);
+    PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_1);
+    __pyx_t_1 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_end_freq), __pyx_t_4, __pyx_t_2) < 0)) __PYX_ERR(0, 209, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "genome_info/kmers/kmer_reader.pyx":210
+ *         end_freq[33, i] = ibf.end.GAC[i]
+ *         end_freq[34, i] = ibf.end.GAG[i]
+ *         end_freq[35, i] = ibf.end.GAT[i]             # <<<<<<<<<<<<<<
+ *         end_freq[36, i] = ibf.end.GCA[i]
+ *         end_freq[37, i] = ibf.end.GCC[i]
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->end->GAT[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 210, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 210, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 210, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_int_35);
+    __Pyx_GIVEREF(__pyx_int_35);
+    PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_int_35);
+    __Pyx_GIVEREF(__pyx_t_4);
+    PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_4);
+    __pyx_t_4 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_end_freq), __pyx_t_1, __pyx_t_2) < 0)) __PYX_ERR(0, 210, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "genome_info/kmers/kmer_reader.pyx":211
+ *         end_freq[34, i] = ibf.end.GAG[i]
+ *         end_freq[35, i] = ibf.end.GAT[i]
+ *         end_freq[36, i] = ibf.end.GCA[i]             # <<<<<<<<<<<<<<
+ *         end_freq[37, i] = ibf.end.GCC[i]
+ *         end_freq[38, i] = ibf.end.GCG[i]
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->end->GCA[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 211, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 211, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 211, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_INCREF(__pyx_int_36);
+    __Pyx_GIVEREF(__pyx_int_36);
+    PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_int_36);
+    __Pyx_GIVEREF(__pyx_t_1);
+    PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_1);
+    __pyx_t_1 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_end_freq), __pyx_t_4, __pyx_t_2) < 0)) __PYX_ERR(0, 211, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "genome_info/kmers/kmer_reader.pyx":212
+ *         end_freq[35, i] = ibf.end.GAT[i]
+ *         end_freq[36, i] = ibf.end.GCA[i]
+ *         end_freq[37, i] = ibf.end.GCC[i]             # <<<<<<<<<<<<<<
+ *         end_freq[38, i] = ibf.end.GCG[i]
+ *         end_freq[39, i] = ibf.end.GCT[i]
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->end->GCC[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 212, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 212, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 212, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_int_37);
+    __Pyx_GIVEREF(__pyx_int_37);
+    PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_int_37);
+    __Pyx_GIVEREF(__pyx_t_4);
+    PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_4);
+    __pyx_t_4 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_end_freq), __pyx_t_1, __pyx_t_2) < 0)) __PYX_ERR(0, 212, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "genome_info/kmers/kmer_reader.pyx":213
+ *         end_freq[36, i] = ibf.end.GCA[i]
+ *         end_freq[37, i] = ibf.end.GCC[i]
+ *         end_freq[38, i] = ibf.end.GCG[i]             # <<<<<<<<<<<<<<
+ *         end_freq[39, i] = ibf.end.GCT[i]
+ *         end_freq[40, i] = ibf.end.GGA[i]
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->end->GCG[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 213, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 213, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 213, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_INCREF(__pyx_int_38);
+    __Pyx_GIVEREF(__pyx_int_38);
+    PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_int_38);
+    __Pyx_GIVEREF(__pyx_t_1);
+    PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_1);
+    __pyx_t_1 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_end_freq), __pyx_t_4, __pyx_t_2) < 0)) __PYX_ERR(0, 213, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "genome_info/kmers/kmer_reader.pyx":214
+ *         end_freq[37, i] = ibf.end.GCC[i]
+ *         end_freq[38, i] = ibf.end.GCG[i]
+ *         end_freq[39, i] = ibf.end.GCT[i]             # <<<<<<<<<<<<<<
+ *         end_freq[40, i] = ibf.end.GGA[i]
+ *         end_freq[41, i] = ibf.end.GGC[i]
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->end->GCT[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 214, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 214, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 214, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_int_39);
+    __Pyx_GIVEREF(__pyx_int_39);
+    PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_int_39);
+    __Pyx_GIVEREF(__pyx_t_4);
+    PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_4);
+    __pyx_t_4 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_end_freq), __pyx_t_1, __pyx_t_2) < 0)) __PYX_ERR(0, 214, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "genome_info/kmers/kmer_reader.pyx":215
+ *         end_freq[38, i] = ibf.end.GCG[i]
+ *         end_freq[39, i] = ibf.end.GCT[i]
+ *         end_freq[40, i] = ibf.end.GGA[i]             # <<<<<<<<<<<<<<
+ *         end_freq[41, i] = ibf.end.GGC[i]
+ *         end_freq[42, i] = ibf.end.GGG[i]
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->end->GGA[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 215, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 215, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 215, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_INCREF(__pyx_int_40);
+    __Pyx_GIVEREF(__pyx_int_40);
+    PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_int_40);
+    __Pyx_GIVEREF(__pyx_t_1);
+    PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_1);
+    __pyx_t_1 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_end_freq), __pyx_t_4, __pyx_t_2) < 0)) __PYX_ERR(0, 215, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "genome_info/kmers/kmer_reader.pyx":216
+ *         end_freq[39, i] = ibf.end.GCT[i]
+ *         end_freq[40, i] = ibf.end.GGA[i]
+ *         end_freq[41, i] = ibf.end.GGC[i]             # <<<<<<<<<<<<<<
+ *         end_freq[42, i] = ibf.end.GGG[i]
+ *         end_freq[43, i] = ibf.end.GGT[i]
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->end->GGC[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 216, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 216, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 216, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_int_41);
+    __Pyx_GIVEREF(__pyx_int_41);
+    PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_int_41);
+    __Pyx_GIVEREF(__pyx_t_4);
+    PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_4);
+    __pyx_t_4 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_end_freq), __pyx_t_1, __pyx_t_2) < 0)) __PYX_ERR(0, 216, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "genome_info/kmers/kmer_reader.pyx":217
+ *         end_freq[40, i] = ibf.end.GGA[i]
+ *         end_freq[41, i] = ibf.end.GGC[i]
+ *         end_freq[42, i] = ibf.end.GGG[i]             # <<<<<<<<<<<<<<
+ *         end_freq[43, i] = ibf.end.GGT[i]
+ *         end_freq[44, i] = ibf.end.GTA[i]
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->end->GGG[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 217, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 217, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 217, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_INCREF(__pyx_int_42);
+    __Pyx_GIVEREF(__pyx_int_42);
+    PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_int_42);
+    __Pyx_GIVEREF(__pyx_t_1);
+    PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_1);
+    __pyx_t_1 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_end_freq), __pyx_t_4, __pyx_t_2) < 0)) __PYX_ERR(0, 217, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "genome_info/kmers/kmer_reader.pyx":218
+ *         end_freq[41, i] = ibf.end.GGC[i]
+ *         end_freq[42, i] = ibf.end.GGG[i]
+ *         end_freq[43, i] = ibf.end.GGT[i]             # <<<<<<<<<<<<<<
+ *         end_freq[44, i] = ibf.end.GTA[i]
+ *         end_freq[45, i] = ibf.end.GTC[i]
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->end->GGT[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 218, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 218, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 218, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_int_43);
+    __Pyx_GIVEREF(__pyx_int_43);
+    PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_int_43);
+    __Pyx_GIVEREF(__pyx_t_4);
+    PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_4);
+    __pyx_t_4 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_end_freq), __pyx_t_1, __pyx_t_2) < 0)) __PYX_ERR(0, 218, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "genome_info/kmers/kmer_reader.pyx":219
+ *         end_freq[42, i] = ibf.end.GGG[i]
+ *         end_freq[43, i] = ibf.end.GGT[i]
+ *         end_freq[44, i] = ibf.end.GTA[i]             # <<<<<<<<<<<<<<
+ *         end_freq[45, i] = ibf.end.GTC[i]
+ *         end_freq[46, i] = ibf.end.GTG[i]
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->end->GTA[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 219, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 219, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 219, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_INCREF(__pyx_int_44);
+    __Pyx_GIVEREF(__pyx_int_44);
+    PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_int_44);
+    __Pyx_GIVEREF(__pyx_t_1);
+    PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_1);
+    __pyx_t_1 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_end_freq), __pyx_t_4, __pyx_t_2) < 0)) __PYX_ERR(0, 219, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "genome_info/kmers/kmer_reader.pyx":220
+ *         end_freq[43, i] = ibf.end.GGT[i]
+ *         end_freq[44, i] = ibf.end.GTA[i]
+ *         end_freq[45, i] = ibf.end.GTC[i]             # <<<<<<<<<<<<<<
+ *         end_freq[46, i] = ibf.end.GTG[i]
+ *         end_freq[47, i] = ibf.end.GTT[i]
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->end->GTC[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 220, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 220, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 220, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_int_45);
+    __Pyx_GIVEREF(__pyx_int_45);
+    PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_int_45);
+    __Pyx_GIVEREF(__pyx_t_4);
+    PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_4);
+    __pyx_t_4 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_end_freq), __pyx_t_1, __pyx_t_2) < 0)) __PYX_ERR(0, 220, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "genome_info/kmers/kmer_reader.pyx":221
+ *         end_freq[44, i] = ibf.end.GTA[i]
+ *         end_freq[45, i] = ibf.end.GTC[i]
+ *         end_freq[46, i] = ibf.end.GTG[i]             # <<<<<<<<<<<<<<
+ *         end_freq[47, i] = ibf.end.GTT[i]
+ *         end_freq[48, i] = ibf.end.TAA[i]
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->end->GTG[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 221, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 221, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 221, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_INCREF(__pyx_int_46);
+    __Pyx_GIVEREF(__pyx_int_46);
+    PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_int_46);
+    __Pyx_GIVEREF(__pyx_t_1);
+    PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_1);
+    __pyx_t_1 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_end_freq), __pyx_t_4, __pyx_t_2) < 0)) __PYX_ERR(0, 221, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "genome_info/kmers/kmer_reader.pyx":222
+ *         end_freq[45, i] = ibf.end.GTC[i]
+ *         end_freq[46, i] = ibf.end.GTG[i]
+ *         end_freq[47, i] = ibf.end.GTT[i]             # <<<<<<<<<<<<<<
+ *         end_freq[48, i] = ibf.end.TAA[i]
+ *         end_freq[49, i] = ibf.end.TAC[i]
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->end->GTT[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 222, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 222, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 222, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_int_47);
+    __Pyx_GIVEREF(__pyx_int_47);
+    PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_int_47);
+    __Pyx_GIVEREF(__pyx_t_4);
+    PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_4);
+    __pyx_t_4 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_end_freq), __pyx_t_1, __pyx_t_2) < 0)) __PYX_ERR(0, 222, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "genome_info/kmers/kmer_reader.pyx":223
+ *         end_freq[46, i] = ibf.end.GTG[i]
+ *         end_freq[47, i] = ibf.end.GTT[i]
+ *         end_freq[48, i] = ibf.end.TAA[i]             # <<<<<<<<<<<<<<
+ *         end_freq[49, i] = ibf.end.TAC[i]
+ *         end_freq[50, i] = ibf.end.TAG[i]
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->end->TAA[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 223, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 223, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 223, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_INCREF(__pyx_int_48);
+    __Pyx_GIVEREF(__pyx_int_48);
+    PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_int_48);
+    __Pyx_GIVEREF(__pyx_t_1);
+    PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_1);
+    __pyx_t_1 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_end_freq), __pyx_t_4, __pyx_t_2) < 0)) __PYX_ERR(0, 223, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "genome_info/kmers/kmer_reader.pyx":224
+ *         end_freq[47, i] = ibf.end.GTT[i]
+ *         end_freq[48, i] = ibf.end.TAA[i]
+ *         end_freq[49, i] = ibf.end.TAC[i]             # <<<<<<<<<<<<<<
+ *         end_freq[50, i] = ibf.end.TAG[i]
+ *         end_freq[51, i] = ibf.end.TAT[i]
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->end->TAC[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 224, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 224, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 224, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_int_49);
+    __Pyx_GIVEREF(__pyx_int_49);
+    PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_int_49);
+    __Pyx_GIVEREF(__pyx_t_4);
+    PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_4);
+    __pyx_t_4 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_end_freq), __pyx_t_1, __pyx_t_2) < 0)) __PYX_ERR(0, 224, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "genome_info/kmers/kmer_reader.pyx":225
+ *         end_freq[48, i] = ibf.end.TAA[i]
+ *         end_freq[49, i] = ibf.end.TAC[i]
+ *         end_freq[50, i] = ibf.end.TAG[i]             # <<<<<<<<<<<<<<
+ *         end_freq[51, i] = ibf.end.TAT[i]
+ *         end_freq[52, i] = ibf.end.TCA[i]
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->end->TAG[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 225, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 225, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 225, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_INCREF(__pyx_int_50);
+    __Pyx_GIVEREF(__pyx_int_50);
+    PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_int_50);
+    __Pyx_GIVEREF(__pyx_t_1);
+    PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_1);
+    __pyx_t_1 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_end_freq), __pyx_t_4, __pyx_t_2) < 0)) __PYX_ERR(0, 225, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "genome_info/kmers/kmer_reader.pyx":226
+ *         end_freq[49, i] = ibf.end.TAC[i]
+ *         end_freq[50, i] = ibf.end.TAG[i]
+ *         end_freq[51, i] = ibf.end.TAT[i]             # <<<<<<<<<<<<<<
+ *         end_freq[52, i] = ibf.end.TCA[i]
+ *         end_freq[53, i] = ibf.end.TCC[i]
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->end->TAT[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 226, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 226, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 226, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_int_51);
+    __Pyx_GIVEREF(__pyx_int_51);
+    PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_int_51);
+    __Pyx_GIVEREF(__pyx_t_4);
+    PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_4);
+    __pyx_t_4 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_end_freq), __pyx_t_1, __pyx_t_2) < 0)) __PYX_ERR(0, 226, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "genome_info/kmers/kmer_reader.pyx":227
+ *         end_freq[50, i] = ibf.end.TAG[i]
+ *         end_freq[51, i] = ibf.end.TAT[i]
+ *         end_freq[52, i] = ibf.end.TCA[i]             # <<<<<<<<<<<<<<
+ *         end_freq[53, i] = ibf.end.TCC[i]
+ *         end_freq[54, i] = ibf.end.TCG[i]
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->end->TCA[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 227, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 227, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 227, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_INCREF(__pyx_int_52);
+    __Pyx_GIVEREF(__pyx_int_52);
+    PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_int_52);
+    __Pyx_GIVEREF(__pyx_t_1);
+    PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_1);
+    __pyx_t_1 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_end_freq), __pyx_t_4, __pyx_t_2) < 0)) __PYX_ERR(0, 227, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "genome_info/kmers/kmer_reader.pyx":228
+ *         end_freq[51, i] = ibf.end.TAT[i]
+ *         end_freq[52, i] = ibf.end.TCA[i]
+ *         end_freq[53, i] = ibf.end.TCC[i]             # <<<<<<<<<<<<<<
+ *         end_freq[54, i] = ibf.end.TCG[i]
+ *         end_freq[55, i] = ibf.end.TCT[i]
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->end->TCC[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 228, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 228, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 228, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_int_53);
+    __Pyx_GIVEREF(__pyx_int_53);
+    PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_int_53);
+    __Pyx_GIVEREF(__pyx_t_4);
+    PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_4);
+    __pyx_t_4 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_end_freq), __pyx_t_1, __pyx_t_2) < 0)) __PYX_ERR(0, 228, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "genome_info/kmers/kmer_reader.pyx":229
+ *         end_freq[52, i] = ibf.end.TCA[i]
+ *         end_freq[53, i] = ibf.end.TCC[i]
+ *         end_freq[54, i] = ibf.end.TCG[i]             # <<<<<<<<<<<<<<
+ *         end_freq[55, i] = ibf.end.TCT[i]
+ *         end_freq[56, i] = ibf.end.TGA[i]
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->end->TCG[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 229, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 229, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 229, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_INCREF(__pyx_int_54);
+    __Pyx_GIVEREF(__pyx_int_54);
+    PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_int_54);
+    __Pyx_GIVEREF(__pyx_t_1);
+    PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_1);
+    __pyx_t_1 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_end_freq), __pyx_t_4, __pyx_t_2) < 0)) __PYX_ERR(0, 229, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "genome_info/kmers/kmer_reader.pyx":230
+ *         end_freq[53, i] = ibf.end.TCC[i]
+ *         end_freq[54, i] = ibf.end.TCG[i]
+ *         end_freq[55, i] = ibf.end.TCT[i]             # <<<<<<<<<<<<<<
+ *         end_freq[56, i] = ibf.end.TGA[i]
+ *         end_freq[57, i] = ibf.end.TGC[i]
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->end->TCT[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 230, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 230, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 230, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_int_55);
+    __Pyx_GIVEREF(__pyx_int_55);
+    PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_int_55);
+    __Pyx_GIVEREF(__pyx_t_4);
+    PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_4);
+    __pyx_t_4 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_end_freq), __pyx_t_1, __pyx_t_2) < 0)) __PYX_ERR(0, 230, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "genome_info/kmers/kmer_reader.pyx":231
+ *         end_freq[54, i] = ibf.end.TCG[i]
+ *         end_freq[55, i] = ibf.end.TCT[i]
+ *         end_freq[56, i] = ibf.end.TGA[i]             # <<<<<<<<<<<<<<
+ *         end_freq[57, i] = ibf.end.TGC[i]
+ *         end_freq[58, i] = ibf.end.TGG[i]
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->end->TGA[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 231, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 231, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 231, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_INCREF(__pyx_int_56);
+    __Pyx_GIVEREF(__pyx_int_56);
+    PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_int_56);
+    __Pyx_GIVEREF(__pyx_t_1);
+    PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_1);
+    __pyx_t_1 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_end_freq), __pyx_t_4, __pyx_t_2) < 0)) __PYX_ERR(0, 231, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "genome_info/kmers/kmer_reader.pyx":232
+ *         end_freq[55, i] = ibf.end.TCT[i]
+ *         end_freq[56, i] = ibf.end.TGA[i]
+ *         end_freq[57, i] = ibf.end.TGC[i]             # <<<<<<<<<<<<<<
+ *         end_freq[58, i] = ibf.end.TGG[i]
+ *         end_freq[59, i] = ibf.end.TGT[i]
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->end->TGC[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 232, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 232, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 232, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_int_57);
+    __Pyx_GIVEREF(__pyx_int_57);
+    PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_int_57);
+    __Pyx_GIVEREF(__pyx_t_4);
+    PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_4);
+    __pyx_t_4 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_end_freq), __pyx_t_1, __pyx_t_2) < 0)) __PYX_ERR(0, 232, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "genome_info/kmers/kmer_reader.pyx":233
+ *         end_freq[56, i] = ibf.end.TGA[i]
+ *         end_freq[57, i] = ibf.end.TGC[i]
+ *         end_freq[58, i] = ibf.end.TGG[i]             # <<<<<<<<<<<<<<
+ *         end_freq[59, i] = ibf.end.TGT[i]
+ *         end_freq[60, i] = ibf.end.TTA[i]
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->end->TGG[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 233, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 233, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 233, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_INCREF(__pyx_int_58);
+    __Pyx_GIVEREF(__pyx_int_58);
+    PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_int_58);
+    __Pyx_GIVEREF(__pyx_t_1);
+    PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_1);
+    __pyx_t_1 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_end_freq), __pyx_t_4, __pyx_t_2) < 0)) __PYX_ERR(0, 233, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "genome_info/kmers/kmer_reader.pyx":234
+ *         end_freq[57, i] = ibf.end.TGC[i]
+ *         end_freq[58, i] = ibf.end.TGG[i]
+ *         end_freq[59, i] = ibf.end.TGT[i]             # <<<<<<<<<<<<<<
+ *         end_freq[60, i] = ibf.end.TTA[i]
+ *         end_freq[61, i] = ibf.end.TTC[i]
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->end->TGT[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 234, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 234, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 234, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_int_59);
+    __Pyx_GIVEREF(__pyx_int_59);
+    PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_int_59);
+    __Pyx_GIVEREF(__pyx_t_4);
+    PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_4);
+    __pyx_t_4 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_end_freq), __pyx_t_1, __pyx_t_2) < 0)) __PYX_ERR(0, 234, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "genome_info/kmers/kmer_reader.pyx":235
+ *         end_freq[58, i] = ibf.end.TGG[i]
+ *         end_freq[59, i] = ibf.end.TGT[i]
+ *         end_freq[60, i] = ibf.end.TTA[i]             # <<<<<<<<<<<<<<
+ *         end_freq[61, i] = ibf.end.TTC[i]
+ *         end_freq[62, i] = ibf.end.TTG[i]
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->end->TTA[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 235, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 235, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 235, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_INCREF(__pyx_int_60);
+    __Pyx_GIVEREF(__pyx_int_60);
+    PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_int_60);
+    __Pyx_GIVEREF(__pyx_t_1);
+    PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_1);
+    __pyx_t_1 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_end_freq), __pyx_t_4, __pyx_t_2) < 0)) __PYX_ERR(0, 235, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "genome_info/kmers/kmer_reader.pyx":236
+ *         end_freq[59, i] = ibf.end.TGT[i]
+ *         end_freq[60, i] = ibf.end.TTA[i]
+ *         end_freq[61, i] = ibf.end.TTC[i]             # <<<<<<<<<<<<<<
+ *         end_freq[62, i] = ibf.end.TTG[i]
+ *         end_freq[63, i] = ibf.end.TTT[i]
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->end->TTC[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 236, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 236, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 236, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_int_61);
+    __Pyx_GIVEREF(__pyx_int_61);
+    PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_int_61);
+    __Pyx_GIVEREF(__pyx_t_4);
+    PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_4);
+    __pyx_t_4 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_end_freq), __pyx_t_1, __pyx_t_2) < 0)) __PYX_ERR(0, 236, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "genome_info/kmers/kmer_reader.pyx":237
+ *         end_freq[60, i] = ibf.end.TTA[i]
+ *         end_freq[61, i] = ibf.end.TTC[i]
+ *         end_freq[62, i] = ibf.end.TTG[i]             # <<<<<<<<<<<<<<
+ *         end_freq[63, i] = ibf.end.TTT[i]
+ * 
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->end->TTG[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 237, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_1 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 237, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __pyx_t_4 = PyTuple_New(2); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 237, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __Pyx_INCREF(__pyx_int_62);
+    __Pyx_GIVEREF(__pyx_int_62);
+    PyTuple_SET_ITEM(__pyx_t_4, 0, __pyx_int_62);
+    __Pyx_GIVEREF(__pyx_t_1);
+    PyTuple_SET_ITEM(__pyx_t_4, 1, __pyx_t_1);
+    __pyx_t_1 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_end_freq), __pyx_t_4, __pyx_t_2) < 0)) __PYX_ERR(0, 237, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+    /* "genome_info/kmers/kmer_reader.pyx":238
+ *         end_freq[61, i] = ibf.end.TTC[i]
+ *         end_freq[62, i] = ibf.end.TTG[i]
+ *         end_freq[63, i] = ibf.end.TTT[i]             # <<<<<<<<<<<<<<
+ * 
+ *     interval_tribase_freq_destroy(ibf)
+ */
+    __pyx_t_2 = PyFloat_FromDouble((__pyx_v_ibf->end->TTT[__pyx_v_i])); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 238, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_2);
+    __pyx_t_4 = __Pyx_PyInt_From_int(__pyx_v_i); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 238, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_4);
+    __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 238, __pyx_L1_error)
+    __Pyx_GOTREF(__pyx_t_1);
+    __Pyx_INCREF(__pyx_int_63);
+    __Pyx_GIVEREF(__pyx_int_63);
+    PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_int_63);
+    __Pyx_GIVEREF(__pyx_t_4);
+    PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_t_4);
+    __pyx_t_4 = 0;
+    if (unlikely(PyObject_SetItem(((PyObject *)__pyx_v_end_freq), __pyx_t_1, __pyx_t_2) < 0)) __PYX_ERR(0, 238, __pyx_L1_error)
+    __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+    __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  }
+
+  /* "genome_info/kmers/kmer_reader.pyx":240
+ *         end_freq[63, i] = ibf.end.TTT[i]
+ * 
+ *     interval_tribase_freq_destroy(ibf)             # <<<<<<<<<<<<<<
+ * 
+ *     tribases = ["AAA", "AAC",
+ */
+  interval_tribase_freq_destroy(__pyx_v_ibf);
+
+  /* "genome_info/kmers/kmer_reader.pyx":242
+ *     interval_tribase_freq_destroy(ibf)
+ * 
+ *     tribases = ["AAA", "AAC",             # <<<<<<<<<<<<<<
+ *                 "AAG", "AAT",
+ *                 "ACA", "ACC",
+ */
+  __pyx_t_2 = PyList_New(64); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 242, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_INCREF(__pyx_n_u_AAA);
+  __Pyx_GIVEREF(__pyx_n_u_AAA);
+  PyList_SET_ITEM(__pyx_t_2, 0, __pyx_n_u_AAA);
+  __Pyx_INCREF(__pyx_n_u_AAC);
+  __Pyx_GIVEREF(__pyx_n_u_AAC);
+  PyList_SET_ITEM(__pyx_t_2, 1, __pyx_n_u_AAC);
+  __Pyx_INCREF(__pyx_n_u_AAG);
+  __Pyx_GIVEREF(__pyx_n_u_AAG);
+  PyList_SET_ITEM(__pyx_t_2, 2, __pyx_n_u_AAG);
+  __Pyx_INCREF(__pyx_n_u_AAT);
+  __Pyx_GIVEREF(__pyx_n_u_AAT);
+  PyList_SET_ITEM(__pyx_t_2, 3, __pyx_n_u_AAT);
+  __Pyx_INCREF(__pyx_n_u_ACA);
+  __Pyx_GIVEREF(__pyx_n_u_ACA);
+  PyList_SET_ITEM(__pyx_t_2, 4, __pyx_n_u_ACA);
+  __Pyx_INCREF(__pyx_n_u_ACC);
+  __Pyx_GIVEREF(__pyx_n_u_ACC);
+  PyList_SET_ITEM(__pyx_t_2, 5, __pyx_n_u_ACC);
+  __Pyx_INCREF(__pyx_n_u_ACG);
+  __Pyx_GIVEREF(__pyx_n_u_ACG);
+  PyList_SET_ITEM(__pyx_t_2, 6, __pyx_n_u_ACG);
+  __Pyx_INCREF(__pyx_n_u_ACT);
+  __Pyx_GIVEREF(__pyx_n_u_ACT);
+  PyList_SET_ITEM(__pyx_t_2, 7, __pyx_n_u_ACT);
+  __Pyx_INCREF(__pyx_n_u_AGA);
+  __Pyx_GIVEREF(__pyx_n_u_AGA);
+  PyList_SET_ITEM(__pyx_t_2, 8, __pyx_n_u_AGA);
+  __Pyx_INCREF(__pyx_n_u_AGC);
+  __Pyx_GIVEREF(__pyx_n_u_AGC);
+  PyList_SET_ITEM(__pyx_t_2, 9, __pyx_n_u_AGC);
+  __Pyx_INCREF(__pyx_n_u_AGG);
+  __Pyx_GIVEREF(__pyx_n_u_AGG);
+  PyList_SET_ITEM(__pyx_t_2, 10, __pyx_n_u_AGG);
+  __Pyx_INCREF(__pyx_n_u_AGT);
+  __Pyx_GIVEREF(__pyx_n_u_AGT);
+  PyList_SET_ITEM(__pyx_t_2, 11, __pyx_n_u_AGT);
+  __Pyx_INCREF(__pyx_n_u_ATA);
+  __Pyx_GIVEREF(__pyx_n_u_ATA);
+  PyList_SET_ITEM(__pyx_t_2, 12, __pyx_n_u_ATA);
+  __Pyx_INCREF(__pyx_n_u_ATC);
+  __Pyx_GIVEREF(__pyx_n_u_ATC);
+  PyList_SET_ITEM(__pyx_t_2, 13, __pyx_n_u_ATC);
+  __Pyx_INCREF(__pyx_n_u_ATG);
+  __Pyx_GIVEREF(__pyx_n_u_ATG);
+  PyList_SET_ITEM(__pyx_t_2, 14, __pyx_n_u_ATG);
+  __Pyx_INCREF(__pyx_n_u_ATT);
+  __Pyx_GIVEREF(__pyx_n_u_ATT);
+  PyList_SET_ITEM(__pyx_t_2, 15, __pyx_n_u_ATT);
+  __Pyx_INCREF(__pyx_n_u_CAA);
+  __Pyx_GIVEREF(__pyx_n_u_CAA);
+  PyList_SET_ITEM(__pyx_t_2, 16, __pyx_n_u_CAA);
+  __Pyx_INCREF(__pyx_n_u_CAC);
+  __Pyx_GIVEREF(__pyx_n_u_CAC);
+  PyList_SET_ITEM(__pyx_t_2, 17, __pyx_n_u_CAC);
+  __Pyx_INCREF(__pyx_n_u_CAG);
+  __Pyx_GIVEREF(__pyx_n_u_CAG);
+  PyList_SET_ITEM(__pyx_t_2, 18, __pyx_n_u_CAG);
+  __Pyx_INCREF(__pyx_n_u_CAT);
+  __Pyx_GIVEREF(__pyx_n_u_CAT);
+  PyList_SET_ITEM(__pyx_t_2, 19, __pyx_n_u_CAT);
+  __Pyx_INCREF(__pyx_n_u_CCA);
+  __Pyx_GIVEREF(__pyx_n_u_CCA);
+  PyList_SET_ITEM(__pyx_t_2, 20, __pyx_n_u_CCA);
+  __Pyx_INCREF(__pyx_n_u_CCC);
+  __Pyx_GIVEREF(__pyx_n_u_CCC);
+  PyList_SET_ITEM(__pyx_t_2, 21, __pyx_n_u_CCC);
+  __Pyx_INCREF(__pyx_n_u_CCG);
+  __Pyx_GIVEREF(__pyx_n_u_CCG);
+  PyList_SET_ITEM(__pyx_t_2, 22, __pyx_n_u_CCG);
+  __Pyx_INCREF(__pyx_n_u_CCT);
+  __Pyx_GIVEREF(__pyx_n_u_CCT);
+  PyList_SET_ITEM(__pyx_t_2, 23, __pyx_n_u_CCT);
+  __Pyx_INCREF(__pyx_n_u_CGA);
+  __Pyx_GIVEREF(__pyx_n_u_CGA);
+  PyList_SET_ITEM(__pyx_t_2, 24, __pyx_n_u_CGA);
+  __Pyx_INCREF(__pyx_n_u_CGC);
+  __Pyx_GIVEREF(__pyx_n_u_CGC);
+  PyList_SET_ITEM(__pyx_t_2, 25, __pyx_n_u_CGC);
+  __Pyx_INCREF(__pyx_n_u_CGG);
+  __Pyx_GIVEREF(__pyx_n_u_CGG);
+  PyList_SET_ITEM(__pyx_t_2, 26, __pyx_n_u_CGG);
+  __Pyx_INCREF(__pyx_n_u_CGT);
+  __Pyx_GIVEREF(__pyx_n_u_CGT);
+  PyList_SET_ITEM(__pyx_t_2, 27, __pyx_n_u_CGT);
+  __Pyx_INCREF(__pyx_n_u_CTA);
+  __Pyx_GIVEREF(__pyx_n_u_CTA);
+  PyList_SET_ITEM(__pyx_t_2, 28, __pyx_n_u_CTA);
+  __Pyx_INCREF(__pyx_n_u_CTC);
+  __Pyx_GIVEREF(__pyx_n_u_CTC);
+  PyList_SET_ITEM(__pyx_t_2, 29, __pyx_n_u_CTC);
+  __Pyx_INCREF(__pyx_n_u_CTG);
+  __Pyx_GIVEREF(__pyx_n_u_CTG);
+  PyList_SET_ITEM(__pyx_t_2, 30, __pyx_n_u_CTG);
+  __Pyx_INCREF(__pyx_n_u_CTT);
+  __Pyx_GIVEREF(__pyx_n_u_CTT);
+  PyList_SET_ITEM(__pyx_t_2, 31, __pyx_n_u_CTT);
+  __Pyx_INCREF(__pyx_n_u_GAA);
+  __Pyx_GIVEREF(__pyx_n_u_GAA);
+  PyList_SET_ITEM(__pyx_t_2, 32, __pyx_n_u_GAA);
+  __Pyx_INCREF(__pyx_n_u_GAC);
+  __Pyx_GIVEREF(__pyx_n_u_GAC);
+  PyList_SET_ITEM(__pyx_t_2, 33, __pyx_n_u_GAC);
+  __Pyx_INCREF(__pyx_n_u_GAG);
+  __Pyx_GIVEREF(__pyx_n_u_GAG);
+  PyList_SET_ITEM(__pyx_t_2, 34, __pyx_n_u_GAG);
+  __Pyx_INCREF(__pyx_n_u_GAT);
+  __Pyx_GIVEREF(__pyx_n_u_GAT);
+  PyList_SET_ITEM(__pyx_t_2, 35, __pyx_n_u_GAT);
+  __Pyx_INCREF(__pyx_n_u_GCA);
+  __Pyx_GIVEREF(__pyx_n_u_GCA);
+  PyList_SET_ITEM(__pyx_t_2, 36, __pyx_n_u_GCA);
+  __Pyx_INCREF(__pyx_n_u_GCC);
+  __Pyx_GIVEREF(__pyx_n_u_GCC);
+  PyList_SET_ITEM(__pyx_t_2, 37, __pyx_n_u_GCC);
+  __Pyx_INCREF(__pyx_n_u_GCG);
+  __Pyx_GIVEREF(__pyx_n_u_GCG);
+  PyList_SET_ITEM(__pyx_t_2, 38, __pyx_n_u_GCG);
+  __Pyx_INCREF(__pyx_n_u_GCT);
+  __Pyx_GIVEREF(__pyx_n_u_GCT);
+  PyList_SET_ITEM(__pyx_t_2, 39, __pyx_n_u_GCT);
+  __Pyx_INCREF(__pyx_n_u_GGA);
+  __Pyx_GIVEREF(__pyx_n_u_GGA);
+  PyList_SET_ITEM(__pyx_t_2, 40, __pyx_n_u_GGA);
+  __Pyx_INCREF(__pyx_n_u_GGC);
+  __Pyx_GIVEREF(__pyx_n_u_GGC);
+  PyList_SET_ITEM(__pyx_t_2, 41, __pyx_n_u_GGC);
+  __Pyx_INCREF(__pyx_n_u_GGG);
+  __Pyx_GIVEREF(__pyx_n_u_GGG);
+  PyList_SET_ITEM(__pyx_t_2, 42, __pyx_n_u_GGG);
+  __Pyx_INCREF(__pyx_n_u_GGT);
+  __Pyx_GIVEREF(__pyx_n_u_GGT);
+  PyList_SET_ITEM(__pyx_t_2, 43, __pyx_n_u_GGT);
+  __Pyx_INCREF(__pyx_n_u_GTA);
+  __Pyx_GIVEREF(__pyx_n_u_GTA);
+  PyList_SET_ITEM(__pyx_t_2, 44, __pyx_n_u_GTA);
+  __Pyx_INCREF(__pyx_n_u_GTC);
+  __Pyx_GIVEREF(__pyx_n_u_GTC);
+  PyList_SET_ITEM(__pyx_t_2, 45, __pyx_n_u_GTC);
+  __Pyx_INCREF(__pyx_n_u_GTG);
+  __Pyx_GIVEREF(__pyx_n_u_GTG);
+  PyList_SET_ITEM(__pyx_t_2, 46, __pyx_n_u_GTG);
+  __Pyx_INCREF(__pyx_n_u_GTT);
+  __Pyx_GIVEREF(__pyx_n_u_GTT);
+  PyList_SET_ITEM(__pyx_t_2, 47, __pyx_n_u_GTT);
+  __Pyx_INCREF(__pyx_n_u_TAA);
+  __Pyx_GIVEREF(__pyx_n_u_TAA);
+  PyList_SET_ITEM(__pyx_t_2, 48, __pyx_n_u_TAA);
+  __Pyx_INCREF(__pyx_n_u_TAC);
+  __Pyx_GIVEREF(__pyx_n_u_TAC);
+  PyList_SET_ITEM(__pyx_t_2, 49, __pyx_n_u_TAC);
+  __Pyx_INCREF(__pyx_n_u_TAG);
+  __Pyx_GIVEREF(__pyx_n_u_TAG);
+  PyList_SET_ITEM(__pyx_t_2, 50, __pyx_n_u_TAG);
+  __Pyx_INCREF(__pyx_n_u_TAT);
+  __Pyx_GIVEREF(__pyx_n_u_TAT);
+  PyList_SET_ITEM(__pyx_t_2, 51, __pyx_n_u_TAT);
+  __Pyx_INCREF(__pyx_n_u_TCA);
+  __Pyx_GIVEREF(__pyx_n_u_TCA);
+  PyList_SET_ITEM(__pyx_t_2, 52, __pyx_n_u_TCA);
+  __Pyx_INCREF(__pyx_n_u_TCC);
+  __Pyx_GIVEREF(__pyx_n_u_TCC);
+  PyList_SET_ITEM(__pyx_t_2, 53, __pyx_n_u_TCC);
+  __Pyx_INCREF(__pyx_n_u_TCG);
+  __Pyx_GIVEREF(__pyx_n_u_TCG);
+  PyList_SET_ITEM(__pyx_t_2, 54, __pyx_n_u_TCG);
+  __Pyx_INCREF(__pyx_n_u_TCT);
+  __Pyx_GIVEREF(__pyx_n_u_TCT);
+  PyList_SET_ITEM(__pyx_t_2, 55, __pyx_n_u_TCT);
+  __Pyx_INCREF(__pyx_n_u_TGA);
+  __Pyx_GIVEREF(__pyx_n_u_TGA);
+  PyList_SET_ITEM(__pyx_t_2, 56, __pyx_n_u_TGA);
+  __Pyx_INCREF(__pyx_n_u_TGC);
+  __Pyx_GIVEREF(__pyx_n_u_TGC);
+  PyList_SET_ITEM(__pyx_t_2, 57, __pyx_n_u_TGC);
+  __Pyx_INCREF(__pyx_n_u_TGG);
+  __Pyx_GIVEREF(__pyx_n_u_TGG);
+  PyList_SET_ITEM(__pyx_t_2, 58, __pyx_n_u_TGG);
+  __Pyx_INCREF(__pyx_n_u_TGT);
+  __Pyx_GIVEREF(__pyx_n_u_TGT);
+  PyList_SET_ITEM(__pyx_t_2, 59, __pyx_n_u_TGT);
+  __Pyx_INCREF(__pyx_n_u_TTA);
+  __Pyx_GIVEREF(__pyx_n_u_TTA);
+  PyList_SET_ITEM(__pyx_t_2, 60, __pyx_n_u_TTA);
+  __Pyx_INCREF(__pyx_n_u_TTC);
+  __Pyx_GIVEREF(__pyx_n_u_TTC);
+  PyList_SET_ITEM(__pyx_t_2, 61, __pyx_n_u_TTC);
+  __Pyx_INCREF(__pyx_n_u_TTG);
+  __Pyx_GIVEREF(__pyx_n_u_TTG);
+  PyList_SET_ITEM(__pyx_t_2, 62, __pyx_n_u_TTG);
+  __Pyx_INCREF(__pyx_n_u_TTT);
+  __Pyx_GIVEREF(__pyx_n_u_TTT);
+  PyList_SET_ITEM(__pyx_t_2, 63, __pyx_n_u_TTT);
+  __pyx_v_tribases = ((PyObject*)__pyx_t_2);
+  __pyx_t_2 = 0;
+
+  /* "genome_info/kmers/kmer_reader.pyx":274
+ *                 "TTA", "TTC",
+ *                 "TTG", "TTT"]
+ *     start_results = pd.DataFrame(start_freq, index=tribases)             # <<<<<<<<<<<<<<
+ *     end_results = pd.DataFrame(end_freq, index=tribases)
+ * 
+ */
+  __Pyx_GetModuleGlobalName(__pyx_t_2, __pyx_n_s_pd); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 274, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __pyx_t_1 = __Pyx_PyObject_GetAttrStr(__pyx_t_2, __pyx_n_s_DataFrame); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 274, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_t_2 = PyTuple_New(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 274, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  __Pyx_INCREF(((PyObject *)__pyx_v_start_freq));
+  __Pyx_GIVEREF(((PyObject *)__pyx_v_start_freq));
+  PyTuple_SET_ITEM(__pyx_t_2, 0, ((PyObject *)__pyx_v_start_freq));
+  __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 274, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  if (PyDict_SetItem(__pyx_t_4, __pyx_n_s_index, __pyx_v_tribases) < 0) __PYX_ERR(0, 274, __pyx_L1_error)
+  __pyx_t_3 = __Pyx_PyObject_Call(__pyx_t_1, __pyx_t_2, __pyx_t_4); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 274, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __pyx_v_start_results = __pyx_t_3;
+  __pyx_t_3 = 0;
+
+  /* "genome_info/kmers/kmer_reader.pyx":275
+ *                 "TTG", "TTT"]
+ *     start_results = pd.DataFrame(start_freq, index=tribases)
+ *     end_results = pd.DataFrame(end_freq, index=tribases)             # <<<<<<<<<<<<<<
+ * 
+ *     return start_results, end_results
+ */
+  __Pyx_GetModuleGlobalName(__pyx_t_3, __pyx_n_s_pd); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 275, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_DataFrame); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 275, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_4);
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __pyx_t_3 = PyTuple_New(1); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 275, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_3);
+  __Pyx_INCREF(((PyObject *)__pyx_v_end_freq));
+  __Pyx_GIVEREF(((PyObject *)__pyx_v_end_freq));
+  PyTuple_SET_ITEM(__pyx_t_3, 0, ((PyObject *)__pyx_v_end_freq));
+  __pyx_t_2 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 275, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_t_2, __pyx_n_s_index, __pyx_v_tribases) < 0) __PYX_ERR(0, 275, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_PyObject_Call(__pyx_t_4, __pyx_t_3, __pyx_t_2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 275, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
+  __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+  __pyx_v_end_results = __pyx_t_1;
+  __pyx_t_1 = 0;
+
+  /* "genome_info/kmers/kmer_reader.pyx":277
+ *     end_results = pd.DataFrame(end_freq, index=tribases)
+ * 
+ *     return start_results, end_results             # <<<<<<<<<<<<<<
+ */
+  __Pyx_XDECREF(__pyx_r);
+  __pyx_t_1 = PyTuple_New(2); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 277, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  __Pyx_INCREF(__pyx_v_start_results);
+  __Pyx_GIVEREF(__pyx_v_start_results);
+  PyTuple_SET_ITEM(__pyx_t_1, 0, __pyx_v_start_results);
+  __Pyx_INCREF(__pyx_v_end_results);
+  __Pyx_GIVEREF(__pyx_v_end_results);
+  PyTuple_SET_ITEM(__pyx_t_1, 1, __pyx_v_end_results);
+  __pyx_r = __pyx_t_1;
+  __pyx_t_1 = 0;
+  goto __pyx_L0;
+
+  /* "genome_info/kmers/kmer_reader.pyx":100
+ * 
+ * 
+ * def read_bounds_tribase_freq(str seq_fn, LabeledIntervalArray laia, int n_bases):             # <<<<<<<<<<<<<<
+ * 
+ *     cdef str twobit_name = seq_fn
+ */
+
+  /* function exit code */
+  __pyx_L1_error:;
+  __Pyx_XDECREF(__pyx_t_1);
+  __Pyx_XDECREF(__pyx_t_2);
+  __Pyx_XDECREF(__pyx_t_3);
+  __Pyx_XDECREF(__pyx_t_4);
+  __Pyx_AddTraceback("genome_info.kmers.kmer_reader.read_bounds_tribase_freq", __pyx_clineno, __pyx_lineno, __pyx_filename);
+  __pyx_r = NULL;
+  __pyx_L0:;
+  __Pyx_XDECREF(__pyx_v_twobit_name);
+  __Pyx_XDECREF(__pyx_v_fname);
+  __Pyx_XDECREF((PyObject *)__pyx_v_start_freq);
+  __Pyx_XDECREF((PyObject *)__pyx_v_end_freq);
+  __Pyx_XDECREF(__pyx_v_tribases);
+  __Pyx_XDECREF(__pyx_v_start_results);
+  __Pyx_XDECREF(__pyx_v_end_results);
+  __Pyx_XGIVEREF(__pyx_r);
+  __Pyx_RefNannyFinishContext();
+  return __pyx_r;
+}
+
+/* "../../../../../../../opt/anaconda3/envs/ailist/lib/python3.11/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -4465,29 +8196,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../../../../../../var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/numpy/__init__.pxd":732
+  /* "../../../../../../../opt/anaconda3/envs/ailist/lib/python3.11/site-packages/numpy/__init__.pxd":735
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 732, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 735, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../../../var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/numpy/__init__.pxd":731
+  /* "../../../../../../../opt/anaconda3/envs/ailist/lib/python3.11/site-packages/numpy/__init__.pxd":734
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -4498,15 +8229,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../../var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/numpy/__init__.pxd":734
+/* "../../../../../../../opt/anaconda3/envs/ailist/lib/python3.11/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -4515,29 +8246,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../../../../../../var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/numpy/__init__.pxd":735
+  /* "../../../../../../../opt/anaconda3/envs/ailist/lib/python3.11/site-packages/numpy/__init__.pxd":738
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 735, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 738, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../../../var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/numpy/__init__.pxd":734
+  /* "../../../../../../../opt/anaconda3/envs/ailist/lib/python3.11/site-packages/numpy/__init__.pxd":737
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -4548,15 +8279,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../../var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/numpy/__init__.pxd":737
+/* "../../../../../../../opt/anaconda3/envs/ailist/lib/python3.11/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -4565,29 +8296,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../../../../../../var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/numpy/__init__.pxd":738
+  /* "../../../../../../../opt/anaconda3/envs/ailist/lib/python3.11/site-packages/numpy/__init__.pxd":741
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 738, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 741, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../../../var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/numpy/__init__.pxd":737
+  /* "../../../../../../../opt/anaconda3/envs/ailist/lib/python3.11/site-packages/numpy/__init__.pxd":740
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -4598,15 +8329,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../../var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/numpy/__init__.pxd":740
+/* "../../../../../../../opt/anaconda3/envs/ailist/lib/python3.11/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -4615,29 +8346,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../../../../../../var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/numpy/__init__.pxd":741
+  /* "../../../../../../../opt/anaconda3/envs/ailist/lib/python3.11/site-packages/numpy/__init__.pxd":744
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 741, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 744, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../../../var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/numpy/__init__.pxd":740
+  /* "../../../../../../../opt/anaconda3/envs/ailist/lib/python3.11/site-packages/numpy/__init__.pxd":743
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -4648,15 +8379,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../../var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/numpy/__init__.pxd":743
+/* "../../../../../../../opt/anaconda3/envs/ailist/lib/python3.11/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -4665,29 +8396,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../../../../../../var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/numpy/__init__.pxd":744
+  /* "../../../../../../../opt/anaconda3/envs/ailist/lib/python3.11/site-packages/numpy/__init__.pxd":747
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
-  __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 744, __pyx_L1_error)
+  __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 747, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../../../var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/numpy/__init__.pxd":743
+  /* "../../../../../../../opt/anaconda3/envs/ailist/lib/python3.11/site-packages/numpy/__init__.pxd":746
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -4698,220 +8429,212 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../../var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/numpy/__init__.pxd":746
+/* "../../../../../../../opt/anaconda3/envs/ailist/lib/python3.11/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../../../../../../var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/numpy/__init__.pxd":747
+  /* "../../../../../../../opt/anaconda3/envs/ailist/lib/python3.11/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../../../var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/numpy/__init__.pxd":748
+    /* "../../../../../../../opt/anaconda3/envs/ailist/lib/python3.11/site-packages/numpy/__init__.pxd":751
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../../../../var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/numpy/__init__.pxd":747
+    /* "../../../../../../../opt/anaconda3/envs/ailist/lib/python3.11/site-packages/numpy/__init__.pxd":750
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../../../../var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/numpy/__init__.pxd":750
+  /* "../../../../../../../opt/anaconda3/envs/ailist/lib/python3.11/site-packages/numpy/__init__.pxd":753
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../../../../var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/numpy/__init__.pxd":746
+  /* "../../../../../../../opt/anaconda3/envs/ailist/lib/python3.11/site-packages/numpy/__init__.pxd":749
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../../var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/numpy/__init__.pxd":926
+/* "../../../../../../../opt/anaconda3/envs/ailist/lib/python3.11/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   __Pyx_RefNannyDeclarations
-  int __pyx_t_1;
-  int __pyx_lineno = 0;
-  const char *__pyx_filename = NULL;
-  int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../../../../../var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/numpy/__init__.pxd":927
+  /* "../../../../../../../opt/anaconda3/envs/ailist/lib/python3.11/site-packages/numpy/__init__.pxd":929
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../../../../var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/numpy/__init__.pxd":928
+  /* "../../../../../../../opt/anaconda3/envs/ailist/lib/python3.11/site-packages/numpy/__init__.pxd":930
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
-  __pyx_t_1 = PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(1, 928, __pyx_L1_error)
+  (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "../../../../../../../var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/numpy/__init__.pxd":926
+  /* "../../../../../../../opt/anaconda3/envs/ailist/lib/python3.11/site-packages/numpy/__init__.pxd":928
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
-  goto __pyx_L0;
-  __pyx_L1_error:;
-  __Pyx_WriteUnraisable("numpy.set_array_base", __pyx_clineno, __pyx_lineno, __pyx_filename, 1, 0);
-  __pyx_L0:;
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../../../../../var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/numpy/__init__.pxd":930
+/* "../../../../../../../opt/anaconda3/envs/ailist/lib/python3.11/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../../../../../../var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/numpy/__init__.pxd":931
+  /* "../../../../../../../opt/anaconda3/envs/ailist/lib/python3.11/site-packages/numpy/__init__.pxd":933
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../../../../var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/numpy/__init__.pxd":932
+  /* "../../../../../../../opt/anaconda3/envs/ailist/lib/python3.11/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../../../var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/numpy/__init__.pxd":933
+    /* "../../../../../../../opt/anaconda3/envs/ailist/lib/python3.11/site-packages/numpy/__init__.pxd":935
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../../../../var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/numpy/__init__.pxd":932
+    /* "../../../../../../../opt/anaconda3/envs/ailist/lib/python3.11/site-packages/numpy/__init__.pxd":934
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../../../../var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/numpy/__init__.pxd":934
+  /* "../../../../../../../opt/anaconda3/envs/ailist/lib/python3.11/site-packages/numpy/__init__.pxd":936
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../../../../var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/numpy/__init__.pxd":930
+  /* "../../../../../../../opt/anaconda3/envs/ailist/lib/python3.11/site-packages/numpy/__init__.pxd":932
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../../var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/numpy/__init__.pxd":938
+/* "../../../../../../../opt/anaconda3/envs/ailist/lib/python3.11/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -4927,15 +8650,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../../../../../../var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/numpy/__init__.pxd":939
+  /* "../../../../../../../opt/anaconda3/envs/ailist/lib/python3.11/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -4943,84 +8666,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../../../var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/numpy/__init__.pxd":940
+      /* "../../../../../../../opt/anaconda3/envs/ailist/lib/python3.11/site-packages/numpy/__init__.pxd":942
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
-      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 940, __pyx_L3_error)
+      __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 942, __pyx_L3_error)
 
-      /* "../../../../../../../var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/numpy/__init__.pxd":939
+      /* "../../../../../../../opt/anaconda3/envs/ailist/lib/python3.11/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../../../var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/numpy/__init__.pxd":941
+    /* "../../../../../../../opt/anaconda3/envs/ailist/lib/python3.11/site-packages/numpy/__init__.pxd":943
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 941, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 943, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../../../var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/numpy/__init__.pxd":942
+      /* "../../../../../../../opt/anaconda3/envs/ailist/lib/python3.11/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 942, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 944, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 942, __pyx_L5_except_error)
+      __PYX_ERR(1, 944, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../../../var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/numpy/__init__.pxd":939
+    /* "../../../../../../../opt/anaconda3/envs/ailist/lib/python3.11/site-packages/numpy/__init__.pxd":941
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../../../var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/numpy/__init__.pxd":938
+  /* "../../../../../../../opt/anaconda3/envs/ailist/lib/python3.11/site-packages/numpy/__init__.pxd":940
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -5035,15 +8758,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../../var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/numpy/__init__.pxd":944
+/* "../../../../../../../opt/anaconda3/envs/ailist/lib/python3.11/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -5059,15 +8782,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../../../../../../var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/numpy/__init__.pxd":945
+  /* "../../../../../../../opt/anaconda3/envs/ailist/lib/python3.11/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -5075,84 +8798,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../../../var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/numpy/__init__.pxd":946
+      /* "../../../../../../../opt/anaconda3/envs/ailist/lib/python3.11/site-packages/numpy/__init__.pxd":948
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 946, __pyx_L3_error)
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 948, __pyx_L3_error)
 
-      /* "../../../../../../../var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/numpy/__init__.pxd":945
+      /* "../../../../../../../opt/anaconda3/envs/ailist/lib/python3.11/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../../../var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/numpy/__init__.pxd":947
+    /* "../../../../../../../opt/anaconda3/envs/ailist/lib/python3.11/site-packages/numpy/__init__.pxd":949
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 947, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 949, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../../../var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/numpy/__init__.pxd":948
+      /* "../../../../../../../opt/anaconda3/envs/ailist/lib/python3.11/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 948, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 950, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 948, __pyx_L5_except_error)
+      __PYX_ERR(1, 950, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../../../var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/numpy/__init__.pxd":945
+    /* "../../../../../../../opt/anaconda3/envs/ailist/lib/python3.11/site-packages/numpy/__init__.pxd":947
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../../../var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/numpy/__init__.pxd":944
+  /* "../../../../../../../opt/anaconda3/envs/ailist/lib/python3.11/site-packages/numpy/__init__.pxd":946
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -5167,15 +8890,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../../var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/numpy/__init__.pxd":950
+/* "../../../../../../../opt/anaconda3/envs/ailist/lib/python3.11/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -5191,15 +8914,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../../../../../../var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/numpy/__init__.pxd":951
+  /* "../../../../../../../opt/anaconda3/envs/ailist/lib/python3.11/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -5207,84 +8930,84 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../../../var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/numpy/__init__.pxd":952
+      /* "../../../../../../../opt/anaconda3/envs/ailist/lib/python3.11/site-packages/numpy/__init__.pxd":954
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
-      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 952, __pyx_L3_error)
+      __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 954, __pyx_L3_error)
 
-      /* "../../../../../../../var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/numpy/__init__.pxd":951
+      /* "../../../../../../../opt/anaconda3/envs/ailist/lib/python3.11/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../../../var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/numpy/__init__.pxd":953
+    /* "../../../../../../../opt/anaconda3/envs/ailist/lib/python3.11/site-packages/numpy/__init__.pxd":955
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
-      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 953, __pyx_L5_except_error)
+      if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 955, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../../../var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/numpy/__init__.pxd":954
+      /* "../../../../../../../opt/anaconda3/envs/ailist/lib/python3.11/site-packages/numpy/__init__.pxd":956
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
-      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 954, __pyx_L5_except_error)
+      __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 956, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
-      __PYX_ERR(1, 954, __pyx_L5_except_error)
+      __PYX_ERR(1, 956, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../../../var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/numpy/__init__.pxd":951
+    /* "../../../../../../../opt/anaconda3/envs/ailist/lib/python3.11/site-packages/numpy/__init__.pxd":953
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../../../var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/numpy/__init__.pxd":950
+  /* "../../../../../../../opt/anaconda3/envs/ailist/lib/python3.11/site-packages/numpy/__init__.pxd":952
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -5299,176 +9022,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../../var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/numpy/__init__.pxd":964
+/* "../../../../../../../opt/anaconda3/envs/ailist/lib/python3.11/site-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../../../../../../var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/numpy/__init__.pxd":976
+  /* "../../../../../../../opt/anaconda3/envs/ailist/lib/python3.11/site-packages/numpy/__init__.pxd":978
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../../../var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/numpy/__init__.pxd":964
+  /* "../../../../../../../opt/anaconda3/envs/ailist/lib/python3.11/site-packages/numpy/__init__.pxd":966
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../../var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/numpy/__init__.pxd":979
+/* "../../../../../../../opt/anaconda3/envs/ailist/lib/python3.11/site-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../../../../../../var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/numpy/__init__.pxd":991
+  /* "../../../../../../../opt/anaconda3/envs/ailist/lib/python3.11/site-packages/numpy/__init__.pxd":993
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../../../var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/numpy/__init__.pxd":979
+  /* "../../../../../../../opt/anaconda3/envs/ailist/lib/python3.11/site-packages/numpy/__init__.pxd":981
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../../../var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/numpy/__init__.pxd":994
+/* "../../../../../../../opt/anaconda3/envs/ailist/lib/python3.11/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../../../../../var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/numpy/__init__.pxd":1001
+  /* "../../../../../../../opt/anaconda3/envs/ailist/lib/python3.11/site-packages/numpy/__init__.pxd":1003
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../../../var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/numpy/__init__.pxd":994
+  /* "../../../../../../../opt/anaconda3/envs/ailist/lib/python3.11/site-packages/numpy/__init__.pxd":996
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../../../var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/numpy/__init__.pxd":1004
+/* "../../../../../../../opt/anaconda3/envs/ailist/lib/python3.11/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../../../../../var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/numpy/__init__.pxd":1008
+  /* "../../../../../../../opt/anaconda3/envs/ailist/lib/python3.11/site-packages/numpy/__init__.pxd":1010
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../../../var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/numpy/__init__.pxd":1004
+  /* "../../../../../../../opt/anaconda3/envs/ailist/lib/python3.11/site-packages/numpy/__init__.pxd":1006
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../../../var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/numpy/__init__.pxd":1011
+/* "../../../../../../../opt/anaconda3/envs/ailist/lib/python3.11/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../../../../../var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/numpy/__init__.pxd":1015
+  /* "../../../../../../../opt/anaconda3/envs/ailist/lib/python3.11/site-packages/numpy/__init__.pxd":1017
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../../../../var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/numpy/__init__.pxd":1011
+  /* "../../../../../../../opt/anaconda3/envs/ailist/lib/python3.11/site-packages/numpy/__init__.pxd":1013
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -19287,35 +23010,100 @@
     #define CYTHON_SMALL_CODE __attribute__((cold))
 #else
     #define CYTHON_SMALL_CODE
 #endif
 #endif
 
 static __Pyx_StringTabEntry __pyx_string_tab[] = {
+  {&__pyx_n_u_AAA, __pyx_k_AAA, sizeof(__pyx_k_AAA), 0, 1, 0, 1},
+  {&__pyx_n_u_AAC, __pyx_k_AAC, sizeof(__pyx_k_AAC), 0, 1, 0, 1},
+  {&__pyx_n_u_AAG, __pyx_k_AAG, sizeof(__pyx_k_AAG), 0, 1, 0, 1},
+  {&__pyx_n_u_AAT, __pyx_k_AAT, sizeof(__pyx_k_AAT), 0, 1, 0, 1},
+  {&__pyx_n_u_ACA, __pyx_k_ACA, sizeof(__pyx_k_ACA), 0, 1, 0, 1},
+  {&__pyx_n_u_ACC, __pyx_k_ACC, sizeof(__pyx_k_ACC), 0, 1, 0, 1},
+  {&__pyx_n_u_ACG, __pyx_k_ACG, sizeof(__pyx_k_ACG), 0, 1, 0, 1},
+  {&__pyx_n_u_ACT, __pyx_k_ACT, sizeof(__pyx_k_ACT), 0, 1, 0, 1},
+  {&__pyx_n_u_AGA, __pyx_k_AGA, sizeof(__pyx_k_AGA), 0, 1, 0, 1},
+  {&__pyx_n_u_AGC, __pyx_k_AGC, sizeof(__pyx_k_AGC), 0, 1, 0, 1},
+  {&__pyx_n_u_AGG, __pyx_k_AGG, sizeof(__pyx_k_AGG), 0, 1, 0, 1},
+  {&__pyx_n_u_AGT, __pyx_k_AGT, sizeof(__pyx_k_AGT), 0, 1, 0, 1},
   {&__pyx_n_s_ASCII, __pyx_k_ASCII, sizeof(__pyx_k_ASCII), 0, 0, 1, 1},
+  {&__pyx_n_u_ATA, __pyx_k_ATA, sizeof(__pyx_k_ATA), 0, 1, 0, 1},
+  {&__pyx_n_u_ATC, __pyx_k_ATC, sizeof(__pyx_k_ATC), 0, 1, 0, 1},
+  {&__pyx_n_u_ATG, __pyx_k_ATG, sizeof(__pyx_k_ATG), 0, 1, 0, 1},
+  {&__pyx_n_u_ATT, __pyx_k_ATT, sizeof(__pyx_k_ATT), 0, 1, 0, 1},
   {&__pyx_kp_s_Buffer_view_does_not_expose_stri, __pyx_k_Buffer_view_does_not_expose_stri, sizeof(__pyx_k_Buffer_view_does_not_expose_stri), 0, 0, 1, 0},
+  {&__pyx_n_u_CAA, __pyx_k_CAA, sizeof(__pyx_k_CAA), 0, 1, 0, 1},
+  {&__pyx_n_u_CAC, __pyx_k_CAC, sizeof(__pyx_k_CAC), 0, 1, 0, 1},
+  {&__pyx_n_u_CAG, __pyx_k_CAG, sizeof(__pyx_k_CAG), 0, 1, 0, 1},
+  {&__pyx_n_u_CAT, __pyx_k_CAT, sizeof(__pyx_k_CAT), 0, 1, 0, 1},
+  {&__pyx_n_u_CCA, __pyx_k_CCA, sizeof(__pyx_k_CCA), 0, 1, 0, 1},
+  {&__pyx_n_u_CCC, __pyx_k_CCC, sizeof(__pyx_k_CCC), 0, 1, 0, 1},
+  {&__pyx_n_u_CCG, __pyx_k_CCG, sizeof(__pyx_k_CCG), 0, 1, 0, 1},
+  {&__pyx_n_u_CCT, __pyx_k_CCT, sizeof(__pyx_k_CCT), 0, 1, 0, 1},
+  {&__pyx_n_u_CGA, __pyx_k_CGA, sizeof(__pyx_k_CGA), 0, 1, 0, 1},
+  {&__pyx_n_u_CGC, __pyx_k_CGC, sizeof(__pyx_k_CGC), 0, 1, 0, 1},
+  {&__pyx_n_u_CGG, __pyx_k_CGG, sizeof(__pyx_k_CGG), 0, 1, 0, 1},
+  {&__pyx_n_u_CGT, __pyx_k_CGT, sizeof(__pyx_k_CGT), 0, 1, 0, 1},
+  {&__pyx_n_u_CTA, __pyx_k_CTA, sizeof(__pyx_k_CTA), 0, 1, 0, 1},
+  {&__pyx_n_u_CTC, __pyx_k_CTC, sizeof(__pyx_k_CTC), 0, 1, 0, 1},
+  {&__pyx_n_u_CTG, __pyx_k_CTG, sizeof(__pyx_k_CTG), 0, 1, 0, 1},
+  {&__pyx_n_u_CTT, __pyx_k_CTT, sizeof(__pyx_k_CTT), 0, 1, 0, 1},
   {&__pyx_kp_s_Can_only_create_a_buffer_that_is, __pyx_k_Can_only_create_a_buffer_that_is, sizeof(__pyx_k_Can_only_create_a_buffer_that_is), 0, 0, 1, 0},
   {&__pyx_kp_s_Cannot_assign_to_read_only_memor, __pyx_k_Cannot_assign_to_read_only_memor, sizeof(__pyx_k_Cannot_assign_to_read_only_memor), 0, 0, 1, 0},
   {&__pyx_kp_s_Cannot_create_writable_memory_vi, __pyx_k_Cannot_create_writable_memory_vi, sizeof(__pyx_k_Cannot_create_writable_memory_vi), 0, 0, 1, 0},
   {&__pyx_kp_s_Cannot_index_with_type_s, __pyx_k_Cannot_index_with_type_s, sizeof(__pyx_k_Cannot_index_with_type_s), 0, 0, 1, 0},
+  {&__pyx_n_s_DataFrame, __pyx_k_DataFrame, sizeof(__pyx_k_DataFrame), 0, 0, 1, 1},
   {&__pyx_n_s_Ellipsis, __pyx_k_Ellipsis, sizeof(__pyx_k_Ellipsis), 0, 0, 1, 1},
   {&__pyx_kp_s_Empty_shape_tuple_for_cython_arr, __pyx_k_Empty_shape_tuple_for_cython_arr, sizeof(__pyx_k_Empty_shape_tuple_for_cython_arr), 0, 0, 1, 0},
+  {&__pyx_n_u_GAA, __pyx_k_GAA, sizeof(__pyx_k_GAA), 0, 1, 0, 1},
+  {&__pyx_n_u_GAC, __pyx_k_GAC, sizeof(__pyx_k_GAC), 0, 1, 0, 1},
+  {&__pyx_n_u_GAG, __pyx_k_GAG, sizeof(__pyx_k_GAG), 0, 1, 0, 1},
+  {&__pyx_n_u_GAT, __pyx_k_GAT, sizeof(__pyx_k_GAT), 0, 1, 0, 1},
+  {&__pyx_n_u_GCA, __pyx_k_GCA, sizeof(__pyx_k_GCA), 0, 1, 0, 1},
+  {&__pyx_n_u_GCC, __pyx_k_GCC, sizeof(__pyx_k_GCC), 0, 1, 0, 1},
+  {&__pyx_n_u_GCG, __pyx_k_GCG, sizeof(__pyx_k_GCG), 0, 1, 0, 1},
+  {&__pyx_n_u_GCT, __pyx_k_GCT, sizeof(__pyx_k_GCT), 0, 1, 0, 1},
+  {&__pyx_n_u_GGA, __pyx_k_GGA, sizeof(__pyx_k_GGA), 0, 1, 0, 1},
+  {&__pyx_n_u_GGC, __pyx_k_GGC, sizeof(__pyx_k_GGC), 0, 1, 0, 1},
+  {&__pyx_n_u_GGG, __pyx_k_GGG, sizeof(__pyx_k_GGG), 0, 1, 0, 1},
+  {&__pyx_n_u_GGT, __pyx_k_GGT, sizeof(__pyx_k_GGT), 0, 1, 0, 1},
+  {&__pyx_n_u_GTA, __pyx_k_GTA, sizeof(__pyx_k_GTA), 0, 1, 0, 1},
+  {&__pyx_n_u_GTC, __pyx_k_GTC, sizeof(__pyx_k_GTC), 0, 1, 0, 1},
+  {&__pyx_n_u_GTG, __pyx_k_GTG, sizeof(__pyx_k_GTG), 0, 1, 0, 1},
+  {&__pyx_n_u_GTT, __pyx_k_GTT, sizeof(__pyx_k_GTT), 0, 1, 0, 1},
   {&__pyx_n_s_ImportError, __pyx_k_ImportError, sizeof(__pyx_k_ImportError), 0, 0, 1, 1},
   {&__pyx_kp_s_Incompatible_checksums_0x_x_vs_0, __pyx_k_Incompatible_checksums_0x_x_vs_0, sizeof(__pyx_k_Incompatible_checksums_0x_x_vs_0), 0, 0, 1, 0},
   {&__pyx_n_s_IndexError, __pyx_k_IndexError, sizeof(__pyx_k_IndexError), 0, 0, 1, 1},
   {&__pyx_kp_s_Indirect_dimensions_not_supporte, __pyx_k_Indirect_dimensions_not_supporte, sizeof(__pyx_k_Indirect_dimensions_not_supporte), 0, 0, 1, 0},
   {&__pyx_n_s_InfoReader, __pyx_k_InfoReader, sizeof(__pyx_k_InfoReader), 0, 0, 1, 1},
   {&__pyx_kp_s_Invalid_mode_expected_c_or_fortr, __pyx_k_Invalid_mode_expected_c_or_fortr, sizeof(__pyx_k_Invalid_mode_expected_c_or_fortr), 0, 0, 1, 0},
   {&__pyx_kp_s_Invalid_shape_in_axis_d_d, __pyx_k_Invalid_shape_in_axis_d_d, sizeof(__pyx_k_Invalid_shape_in_axis_d_d), 0, 0, 1, 0},
   {&__pyx_n_s_MemoryError, __pyx_k_MemoryError, sizeof(__pyx_k_MemoryError), 0, 0, 1, 1},
   {&__pyx_kp_s_MemoryView_of_r_at_0x_x, __pyx_k_MemoryView_of_r_at_0x_x, sizeof(__pyx_k_MemoryView_of_r_at_0x_x), 0, 0, 1, 0},
   {&__pyx_kp_s_MemoryView_of_r_object, __pyx_k_MemoryView_of_r_object, sizeof(__pyx_k_MemoryView_of_r_object), 0, 0, 1, 0},
   {&__pyx_n_b_O, __pyx_k_O, sizeof(__pyx_k_O), 0, 0, 0, 1},
   {&__pyx_kp_s_Out_of_bounds_on_buffer_access_a, __pyx_k_Out_of_bounds_on_buffer_access_a, sizeof(__pyx_k_Out_of_bounds_on_buffer_access_a), 0, 0, 1, 0},
   {&__pyx_n_s_PickleError, __pyx_k_PickleError, sizeof(__pyx_k_PickleError), 0, 0, 1, 1},
+  {&__pyx_n_u_TAA, __pyx_k_TAA, sizeof(__pyx_k_TAA), 0, 1, 0, 1},
+  {&__pyx_n_u_TAC, __pyx_k_TAC, sizeof(__pyx_k_TAC), 0, 1, 0, 1},
+  {&__pyx_n_u_TAG, __pyx_k_TAG, sizeof(__pyx_k_TAG), 0, 1, 0, 1},
+  {&__pyx_n_u_TAT, __pyx_k_TAT, sizeof(__pyx_k_TAT), 0, 1, 0, 1},
+  {&__pyx_n_u_TCA, __pyx_k_TCA, sizeof(__pyx_k_TCA), 0, 1, 0, 1},
+  {&__pyx_n_u_TCC, __pyx_k_TCC, sizeof(__pyx_k_TCC), 0, 1, 0, 1},
+  {&__pyx_n_u_TCG, __pyx_k_TCG, sizeof(__pyx_k_TCG), 0, 1, 0, 1},
+  {&__pyx_n_u_TCT, __pyx_k_TCT, sizeof(__pyx_k_TCT), 0, 1, 0, 1},
+  {&__pyx_n_u_TGA, __pyx_k_TGA, sizeof(__pyx_k_TGA), 0, 1, 0, 1},
+  {&__pyx_n_u_TGC, __pyx_k_TGC, sizeof(__pyx_k_TGC), 0, 1, 0, 1},
+  {&__pyx_n_u_TGG, __pyx_k_TGG, sizeof(__pyx_k_TGG), 0, 1, 0, 1},
+  {&__pyx_n_u_TGT, __pyx_k_TGT, sizeof(__pyx_k_TGT), 0, 1, 0, 1},
+  {&__pyx_n_u_TTA, __pyx_k_TTA, sizeof(__pyx_k_TTA), 0, 1, 0, 1},
+  {&__pyx_n_u_TTC, __pyx_k_TTC, sizeof(__pyx_k_TTC), 0, 1, 0, 1},
+  {&__pyx_n_u_TTG, __pyx_k_TTG, sizeof(__pyx_k_TTG), 0, 1, 0, 1},
+  {&__pyx_n_u_TTT, __pyx_k_TTT, sizeof(__pyx_k_TTT), 0, 1, 0, 1},
   {&__pyx_n_s_TypeError, __pyx_k_TypeError, sizeof(__pyx_k_TypeError), 0, 0, 1, 1},
   {&__pyx_kp_s_Unable_to_convert_item_to_object, __pyx_k_Unable_to_convert_item_to_object, sizeof(__pyx_k_Unable_to_convert_item_to_object), 0, 0, 1, 0},
   {&__pyx_n_s_ValueError, __pyx_k_ValueError, sizeof(__pyx_k_ValueError), 0, 0, 1, 1},
   {&__pyx_n_s_View_MemoryView, __pyx_k_View_MemoryView, sizeof(__pyx_k_View_MemoryView), 0, 0, 1, 1},
   {&__pyx_n_s_allocate_buffer, __pyx_k_allocate_buffer, sizeof(__pyx_k_allocate_buffer), 0, 0, 1, 1},
   {&__pyx_n_s_base, __pyx_k_base, sizeof(__pyx_k_base), 0, 0, 1, 1},
   {&__pyx_n_s_c, __pyx_k_c, sizeof(__pyx_k_c), 0, 0, 1, 1},
@@ -19328,14 +23116,15 @@
   {&__pyx_n_s_count, __pyx_k_count, sizeof(__pyx_k_count), 0, 0, 1, 1},
   {&__pyx_n_s_dict, __pyx_k_dict, sizeof(__pyx_k_dict), 0, 0, 1, 1},
   {&__pyx_n_s_dtype, __pyx_k_dtype, sizeof(__pyx_k_dtype), 0, 0, 1, 1},
   {&__pyx_n_s_dtype_is_object, __pyx_k_dtype_is_object, sizeof(__pyx_k_dtype_is_object), 0, 0, 1, 1},
   {&__pyx_n_s_encode, __pyx_k_encode, sizeof(__pyx_k_encode), 0, 0, 1, 1},
   {&__pyx_n_s_end, __pyx_k_end, sizeof(__pyx_k_end), 0, 0, 1, 1},
   {&__pyx_n_s_end_freq, __pyx_k_end_freq, sizeof(__pyx_k_end_freq), 0, 0, 1, 1},
+  {&__pyx_n_s_end_results, __pyx_k_end_results, sizeof(__pyx_k_end_results), 0, 0, 1, 1},
   {&__pyx_n_s_enumerate, __pyx_k_enumerate, sizeof(__pyx_k_enumerate), 0, 0, 1, 1},
   {&__pyx_n_s_error, __pyx_k_error, sizeof(__pyx_k_error), 0, 0, 1, 1},
   {&__pyx_n_s_flags, __pyx_k_flags, sizeof(__pyx_k_flags), 0, 0, 1, 1},
   {&__pyx_n_s_fname, __pyx_k_fname, sizeof(__pyx_k_fname), 0, 0, 1, 1},
   {&__pyx_n_s_format, __pyx_k_format, sizeof(__pyx_k_format), 0, 0, 1, 1},
   {&__pyx_n_s_fortran, __pyx_k_fortran, sizeof(__pyx_k_fortran), 0, 0, 1, 1},
   {&__pyx_n_u_fortran, __pyx_k_fortran, sizeof(__pyx_k_fortran), 0, 1, 0, 1},
@@ -19349,14 +23138,15 @@
   {&__pyx_n_s_getstate, __pyx_k_getstate, sizeof(__pyx_k_getstate), 0, 0, 1, 1},
   {&__pyx_kp_s_got_differing_extents_in_dimensi, __pyx_k_got_differing_extents_in_dimensi, sizeof(__pyx_k_got_differing_extents_in_dimensi), 0, 0, 1, 0},
   {&__pyx_n_u_hg38, __pyx_k_hg38, sizeof(__pyx_k_hg38), 0, 1, 0, 1},
   {&__pyx_n_s_i, __pyx_k_i, sizeof(__pyx_k_i), 0, 0, 1, 1},
   {&__pyx_n_s_ibf, __pyx_k_ibf, sizeof(__pyx_k_ibf), 0, 0, 1, 1},
   {&__pyx_n_s_id, __pyx_k_id, sizeof(__pyx_k_id), 0, 0, 1, 1},
   {&__pyx_n_s_import, __pyx_k_import, sizeof(__pyx_k_import), 0, 0, 1, 1},
+  {&__pyx_n_s_index, __pyx_k_index, sizeof(__pyx_k_index), 0, 0, 1, 1},
   {&__pyx_n_s_itemsize, __pyx_k_itemsize, sizeof(__pyx_k_itemsize), 0, 0, 1, 1},
   {&__pyx_kp_s_itemsize_0_for_cython_array, __pyx_k_itemsize_0_for_cython_array, sizeof(__pyx_k_itemsize_0_for_cython_array), 0, 0, 1, 0},
   {&__pyx_n_s_k, __pyx_k_k, sizeof(__pyx_k_k), 0, 0, 1, 1},
   {&__pyx_n_s_kc, __pyx_k_kc, sizeof(__pyx_k_kc), 0, 0, 1, 1},
   {&__pyx_n_s_kmer_seq, __pyx_k_kmer_seq, sizeof(__pyx_k_kmer_seq), 0, 0, 1, 1},
   {&__pyx_n_s_laia, __pyx_k_laia, sizeof(__pyx_k_laia), 0, 0, 1, 1},
   {&__pyx_n_s_last_n, __pyx_k_last_n, sizeof(__pyx_k_last_n), 0, 0, 1, 1},
@@ -19371,26 +23161,29 @@
   {&__pyx_kp_s_no_default___reduce___due_to_non, __pyx_k_no_default___reduce___due_to_non, sizeof(__pyx_k_no_default___reduce___due_to_non), 0, 0, 1, 0},
   {&__pyx_n_s_np, __pyx_k_np, sizeof(__pyx_k_np), 0, 0, 1, 1},
   {&__pyx_n_s_numpy, __pyx_k_numpy, sizeof(__pyx_k_numpy), 0, 0, 1, 1},
   {&__pyx_kp_u_numpy_core_multiarray_failed_to, __pyx_k_numpy_core_multiarray_failed_to, sizeof(__pyx_k_numpy_core_multiarray_failed_to), 0, 1, 0, 0},
   {&__pyx_kp_u_numpy_core_umath_failed_to_impor, __pyx_k_numpy_core_umath_failed_to_impor, sizeof(__pyx_k_numpy_core_umath_failed_to_impor), 0, 1, 0, 0},
   {&__pyx_n_s_obj, __pyx_k_obj, sizeof(__pyx_k_obj), 0, 0, 1, 1},
   {&__pyx_n_s_pack, __pyx_k_pack, sizeof(__pyx_k_pack), 0, 0, 1, 1},
+  {&__pyx_n_s_pandas, __pyx_k_pandas, sizeof(__pyx_k_pandas), 0, 0, 1, 1},
+  {&__pyx_n_s_pd, __pyx_k_pd, sizeof(__pyx_k_pd), 0, 0, 1, 1},
   {&__pyx_n_s_pickle, __pyx_k_pickle, sizeof(__pyx_k_pickle), 0, 0, 1, 1},
   {&__pyx_n_s_py_seq, __pyx_k_py_seq, sizeof(__pyx_k_py_seq), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_PickleError, __pyx_k_pyx_PickleError, sizeof(__pyx_k_pyx_PickleError), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_checksum, __pyx_k_pyx_checksum, sizeof(__pyx_k_pyx_checksum), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_getbuffer, __pyx_k_pyx_getbuffer, sizeof(__pyx_k_pyx_getbuffer), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_result, __pyx_k_pyx_result, sizeof(__pyx_k_pyx_result), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_state, __pyx_k_pyx_state, sizeof(__pyx_k_pyx_state), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_type, __pyx_k_pyx_type, sizeof(__pyx_k_pyx_type), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_unpickle_Enum, __pyx_k_pyx_unpickle_Enum, sizeof(__pyx_k_pyx_unpickle_Enum), 0, 0, 1, 1},
   {&__pyx_n_s_pyx_vtable, __pyx_k_pyx_vtable, sizeof(__pyx_k_pyx_vtable), 0, 0, 1, 1},
   {&__pyx_n_s_range, __pyx_k_range, sizeof(__pyx_k_range), 0, 0, 1, 1},
   {&__pyx_n_s_read_bounds_base_freq, __pyx_k_read_bounds_base_freq, sizeof(__pyx_k_read_bounds_base_freq), 0, 0, 1, 1},
+  {&__pyx_n_s_read_bounds_tribase_freq, __pyx_k_read_bounds_tribase_freq, sizeof(__pyx_k_read_bounds_tribase_freq), 0, 0, 1, 1},
   {&__pyx_n_s_read_kmers, __pyx_k_read_kmers, sizeof(__pyx_k_read_kmers), 0, 0, 1, 1},
   {&__pyx_n_s_read_sequence, __pyx_k_read_sequence, sizeof(__pyx_k_read_sequence), 0, 0, 1, 1},
   {&__pyx_n_s_reduce, __pyx_k_reduce, sizeof(__pyx_k_reduce), 0, 0, 1, 1},
   {&__pyx_n_s_reduce_cython, __pyx_k_reduce_cython, sizeof(__pyx_k_reduce_cython), 0, 0, 1, 1},
   {&__pyx_n_s_reduce_ex, __pyx_k_reduce_ex, sizeof(__pyx_k_reduce_ex), 0, 0, 1, 1},
   {&__pyx_n_s_result, __pyx_k_result, sizeof(__pyx_k_result), 0, 0, 1, 1},
   {&__pyx_n_s_seq, __pyx_k_seq, sizeof(__pyx_k_seq), 0, 0, 1, 1},
@@ -19398,34 +23191,36 @@
   {&__pyx_n_s_setstate, __pyx_k_setstate, sizeof(__pyx_k_setstate), 0, 0, 1, 1},
   {&__pyx_n_s_setstate_cython, __pyx_k_setstate_cython, sizeof(__pyx_k_setstate_cython), 0, 0, 1, 1},
   {&__pyx_n_s_shape, __pyx_k_shape, sizeof(__pyx_k_shape), 0, 0, 1, 1},
   {&__pyx_n_s_single, __pyx_k_single, sizeof(__pyx_k_single), 0, 0, 1, 1},
   {&__pyx_n_s_size, __pyx_k_size, sizeof(__pyx_k_size), 0, 0, 1, 1},
   {&__pyx_n_s_start, __pyx_k_start, sizeof(__pyx_k_start), 0, 0, 1, 1},
   {&__pyx_n_s_start_freq, __pyx_k_start_freq, sizeof(__pyx_k_start_freq), 0, 0, 1, 1},
+  {&__pyx_n_s_start_results, __pyx_k_start_results, sizeof(__pyx_k_start_results), 0, 0, 1, 1},
   {&__pyx_n_s_step, __pyx_k_step, sizeof(__pyx_k_step), 0, 0, 1, 1},
   {&__pyx_n_s_stop, __pyx_k_stop, sizeof(__pyx_k_stop), 0, 0, 1, 1},
   {&__pyx_kp_s_strided_and_direct, __pyx_k_strided_and_direct, sizeof(__pyx_k_strided_and_direct), 0, 0, 1, 0},
   {&__pyx_kp_s_strided_and_direct_or_indirect, __pyx_k_strided_and_direct_or_indirect, sizeof(__pyx_k_strided_and_direct_or_indirect), 0, 0, 1, 0},
   {&__pyx_kp_s_strided_and_indirect, __pyx_k_strided_and_indirect, sizeof(__pyx_k_strided_and_indirect), 0, 0, 1, 0},
   {&__pyx_kp_s_stringsource, __pyx_k_stringsource, sizeof(__pyx_k_stringsource), 0, 0, 1, 0},
   {&__pyx_n_s_struct, __pyx_k_struct, sizeof(__pyx_k_struct), 0, 0, 1, 1},
   {&__pyx_n_s_t, __pyx_k_t, sizeof(__pyx_k_t), 0, 0, 1, 1},
   {&__pyx_n_s_test, __pyx_k_test, sizeof(__pyx_k_test), 0, 0, 1, 1},
+  {&__pyx_n_s_tribases, __pyx_k_tribases, sizeof(__pyx_k_tribases), 0, 0, 1, 1},
   {&__pyx_n_s_twobit_name, __pyx_k_twobit_name, sizeof(__pyx_k_twobit_name), 0, 0, 1, 1},
   {&__pyx_kp_s_unable_to_allocate_array_data, __pyx_k_unable_to_allocate_array_data, sizeof(__pyx_k_unable_to_allocate_array_data), 0, 0, 1, 0},
   {&__pyx_kp_s_unable_to_allocate_shape_and_str, __pyx_k_unable_to_allocate_shape_and_str, sizeof(__pyx_k_unable_to_allocate_shape_and_str), 0, 0, 1, 0},
   {&__pyx_n_s_unpack, __pyx_k_unpack, sizeof(__pyx_k_unpack), 0, 0, 1, 1},
   {&__pyx_n_s_update, __pyx_k_update, sizeof(__pyx_k_update), 0, 0, 1, 1},
   {&__pyx_n_s_zeros, __pyx_k_zeros, sizeof(__pyx_k_zeros), 0, 0, 1, 1},
   {0, 0, 0, 0, 0, 0, 0}
 };
 static CYTHON_SMALL_CODE int __Pyx_InitCachedBuiltins(void) {
-  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 28, __pyx_L1_error)
-  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(1, 942, __pyx_L1_error)
+  __pyx_builtin_range = __Pyx_GetBuiltinName(__pyx_n_s_range); if (!__pyx_builtin_range) __PYX_ERR(0, 29, __pyx_L1_error)
+  __pyx_builtin_ImportError = __Pyx_GetBuiltinName(__pyx_n_s_ImportError); if (!__pyx_builtin_ImportError) __PYX_ERR(1, 944, __pyx_L1_error)
   __pyx_builtin_ValueError = __Pyx_GetBuiltinName(__pyx_n_s_ValueError); if (!__pyx_builtin_ValueError) __PYX_ERR(2, 134, __pyx_L1_error)
   __pyx_builtin_MemoryError = __Pyx_GetBuiltinName(__pyx_n_s_MemoryError); if (!__pyx_builtin_MemoryError) __PYX_ERR(2, 149, __pyx_L1_error)
   __pyx_builtin_enumerate = __Pyx_GetBuiltinName(__pyx_n_s_enumerate); if (!__pyx_builtin_enumerate) __PYX_ERR(2, 152, __pyx_L1_error)
   __pyx_builtin_TypeError = __Pyx_GetBuiltinName(__pyx_n_s_TypeError); if (!__pyx_builtin_TypeError) __PYX_ERR(2, 2, __pyx_L1_error)
   __pyx_builtin_Ellipsis = __Pyx_GetBuiltinName(__pyx_n_s_Ellipsis); if (!__pyx_builtin_Ellipsis) __PYX_ERR(2, 406, __pyx_L1_error)
   __pyx_builtin_id = __Pyx_GetBuiltinName(__pyx_n_s_id); if (!__pyx_builtin_id) __PYX_ERR(2, 615, __pyx_L1_error)
   __pyx_builtin_IndexError = __Pyx_GetBuiltinName(__pyx_n_s_IndexError); if (!__pyx_builtin_IndexError) __PYX_ERR(2, 834, __pyx_L1_error)
@@ -19434,33 +23229,33 @@
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "../../../../../../../var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/numpy/__init__.pxd":942
+  /* "../../../../../../../opt/anaconda3/envs/ailist/lib/python3.11/site-packages/numpy/__init__.pxd":944
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
-  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple_)) __PYX_ERR(1, 942, __pyx_L1_error)
+  __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple_)) __PYX_ERR(1, 944, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple_);
   __Pyx_GIVEREF(__pyx_tuple_);
 
-  /* "../../../../../../../var/folders/9f/jr2rvwvs1594d50cdhzmknp00000gp/T/tmp2dbo3gs2/.venv/lib/python3.11/site-packages/numpy/__init__.pxd":948
+  /* "../../../../../../../opt/anaconda3/envs/ailist/lib/python3.11/site-packages/numpy/__init__.pxd":950
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
-  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 948, __pyx_L1_error)
+  __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 950, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__2);
   __Pyx_GIVEREF(__pyx_tuple__2);
 
   /* "View.MemoryView":134
  * 
  *         if not self.ndim:
  *             raise ValueError("Empty shape tuple for cython.array")             # <<<<<<<<<<<<<<
@@ -19651,126 +23446,138 @@
   __pyx_tuple__20 = PyTuple_Pack(1, __pyx_kp_s_no_default___reduce___due_to_non); if (unlikely(!__pyx_tuple__20)) __PYX_ERR(2, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__20);
   __Pyx_GIVEREF(__pyx_tuple__20);
   __pyx_tuple__21 = PyTuple_Pack(3, __pyx_int_184977713, __pyx_int_136983863, __pyx_int_112105877); if (unlikely(!__pyx_tuple__21)) __PYX_ERR(2, 4, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__21);
   __Pyx_GIVEREF(__pyx_tuple__21);
 
-  /* "genome_info/kmers/kmer_reader.pyx":18
+  /* "genome_info/kmers/kmer_reader.pyx":19
  * 
  * 
  * def read_kmers(str seq_fn, LabeledIntervalArray laia, int k, int last_n = 0):             # <<<<<<<<<<<<<<
  * 
  *     cdef str twobit_name = seq_fn
  */
-  __pyx_tuple__22 = PyTuple_Pack(11, __pyx_n_s_seq_fn, __pyx_n_s_laia, __pyx_n_s_k, __pyx_n_s_last_n, __pyx_n_s_twobit_name, __pyx_n_s_fname, __pyx_n_s_kc, __pyx_n_s_result, __pyx_n_s_kmer_seq, __pyx_n_s_count, __pyx_n_s_t); if (unlikely(!__pyx_tuple__22)) __PYX_ERR(0, 18, __pyx_L1_error)
+  __pyx_tuple__22 = PyTuple_Pack(11, __pyx_n_s_seq_fn, __pyx_n_s_laia, __pyx_n_s_k, __pyx_n_s_last_n, __pyx_n_s_twobit_name, __pyx_n_s_fname, __pyx_n_s_kc, __pyx_n_s_result, __pyx_n_s_kmer_seq, __pyx_n_s_count, __pyx_n_s_t); if (unlikely(!__pyx_tuple__22)) __PYX_ERR(0, 19, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__22);
   __Pyx_GIVEREF(__pyx_tuple__22);
-  __pyx_codeobj__23 = (PyObject*)__Pyx_PyCode_New(4, 0, 11, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__22, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_genome_info_kmers_kmer_reader_py, __pyx_n_s_read_kmers, 18, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__23)) __PYX_ERR(0, 18, __pyx_L1_error)
+  __pyx_codeobj__23 = (PyObject*)__Pyx_PyCode_New(4, 0, 11, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__22, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_genome_info_kmers_kmer_reader_py, __pyx_n_s_read_kmers, 19, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__23)) __PYX_ERR(0, 19, __pyx_L1_error)
 
-  /* "genome_info/kmers/kmer_reader.pyx":45
+  /* "genome_info/kmers/kmer_reader.pyx":46
  *     return seq
  * 
  * def read_sequence(str seq_fn, str chrom, int start, int end):             # <<<<<<<<<<<<<<
  * 
  *     cdef str twobit_name = seq_fn
  */
-  __pyx_tuple__24 = PyTuple_Pack(9, __pyx_n_s_seq_fn, __pyx_n_s_chrom, __pyx_n_s_start, __pyx_n_s_end, __pyx_n_s_twobit_name, __pyx_n_s_fname, __pyx_n_s_name, __pyx_n_s_seq, __pyx_n_s_py_seq); if (unlikely(!__pyx_tuple__24)) __PYX_ERR(0, 45, __pyx_L1_error)
+  __pyx_tuple__24 = PyTuple_Pack(9, __pyx_n_s_seq_fn, __pyx_n_s_chrom, __pyx_n_s_start, __pyx_n_s_end, __pyx_n_s_twobit_name, __pyx_n_s_fname, __pyx_n_s_name, __pyx_n_s_seq, __pyx_n_s_py_seq); if (unlikely(!__pyx_tuple__24)) __PYX_ERR(0, 46, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__24);
   __Pyx_GIVEREF(__pyx_tuple__24);
-  __pyx_codeobj__25 = (PyObject*)__Pyx_PyCode_New(4, 0, 9, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__24, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_genome_info_kmers_kmer_reader_py, __pyx_n_s_read_sequence, 45, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__25)) __PYX_ERR(0, 45, __pyx_L1_error)
+  __pyx_codeobj__25 = (PyObject*)__Pyx_PyCode_New(4, 0, 9, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__24, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_genome_info_kmers_kmer_reader_py, __pyx_n_s_read_sequence, 46, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__25)) __PYX_ERR(0, 46, __pyx_L1_error)
 
-  /* "genome_info/kmers/kmer_reader.pyx":63
+  /* "genome_info/kmers/kmer_reader.pyx":64
  * 
  * 
  * def gc_percent(str seq_fn, LabeledIntervalArray laia, str genome_version = "hg38"):             # <<<<<<<<<<<<<<
  *     cdef str twobit_name = seq_fn
  *     cdef bytes fname = twobit_name.encode()
  */
-  __pyx_tuple__26 = PyTuple_Pack(7, __pyx_n_s_seq_fn, __pyx_n_s_laia, __pyx_n_s_genome_version, __pyx_n_s_twobit_name, __pyx_n_s_fname, __pyx_n_s_gc, __pyx_n_s_gc_mem); if (unlikely(!__pyx_tuple__26)) __PYX_ERR(0, 63, __pyx_L1_error)
+  __pyx_tuple__26 = PyTuple_Pack(7, __pyx_n_s_seq_fn, __pyx_n_s_laia, __pyx_n_s_genome_version, __pyx_n_s_twobit_name, __pyx_n_s_fname, __pyx_n_s_gc, __pyx_n_s_gc_mem); if (unlikely(!__pyx_tuple__26)) __PYX_ERR(0, 64, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__26);
   __Pyx_GIVEREF(__pyx_tuple__26);
-  __pyx_codeobj__27 = (PyObject*)__Pyx_PyCode_New(3, 0, 7, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__26, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_genome_info_kmers_kmer_reader_py, __pyx_n_s_gc_percent, 63, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__27)) __PYX_ERR(0, 63, __pyx_L1_error)
+  __pyx_codeobj__27 = (PyObject*)__Pyx_PyCode_New(3, 0, 7, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__26, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_genome_info_kmers_kmer_reader_py, __pyx_n_s_gc_percent, 64, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__27)) __PYX_ERR(0, 64, __pyx_L1_error)
 
-  /* "genome_info/kmers/kmer_reader.pyx":75
+  /* "genome_info/kmers/kmer_reader.pyx":76
  * 
  * 
  * def read_bounds_base_freq(str seq_fn, LabeledIntervalArray laia, int n_bases):             # <<<<<<<<<<<<<<
  * 
  *     cdef str twobit_name = seq_fn
  */
-  __pyx_tuple__28 = PyTuple_Pack(9, __pyx_n_s_seq_fn, __pyx_n_s_laia, __pyx_n_s_n_bases, __pyx_n_s_twobit_name, __pyx_n_s_fname, __pyx_n_s_start_freq, __pyx_n_s_end_freq, __pyx_n_s_ibf, __pyx_n_s_i); if (unlikely(!__pyx_tuple__28)) __PYX_ERR(0, 75, __pyx_L1_error)
+  __pyx_tuple__28 = PyTuple_Pack(9, __pyx_n_s_seq_fn, __pyx_n_s_laia, __pyx_n_s_n_bases, __pyx_n_s_twobit_name, __pyx_n_s_fname, __pyx_n_s_start_freq, __pyx_n_s_end_freq, __pyx_n_s_ibf, __pyx_n_s_i); if (unlikely(!__pyx_tuple__28)) __PYX_ERR(0, 76, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__28);
   __Pyx_GIVEREF(__pyx_tuple__28);
-  __pyx_codeobj__29 = (PyObject*)__Pyx_PyCode_New(3, 0, 9, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__28, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_genome_info_kmers_kmer_reader_py, __pyx_n_s_read_bounds_base_freq, 75, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__29)) __PYX_ERR(0, 75, __pyx_L1_error)
+  __pyx_codeobj__29 = (PyObject*)__Pyx_PyCode_New(3, 0, 9, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__28, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_genome_info_kmers_kmer_reader_py, __pyx_n_s_read_bounds_base_freq, 76, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__29)) __PYX_ERR(0, 76, __pyx_L1_error)
+
+  /* "genome_info/kmers/kmer_reader.pyx":100
+ * 
+ * 
+ * def read_bounds_tribase_freq(str seq_fn, LabeledIntervalArray laia, int n_bases):             # <<<<<<<<<<<<<<
+ * 
+ *     cdef str twobit_name = seq_fn
+ */
+  __pyx_tuple__30 = PyTuple_Pack(12, __pyx_n_s_seq_fn, __pyx_n_s_laia, __pyx_n_s_n_bases, __pyx_n_s_twobit_name, __pyx_n_s_fname, __pyx_n_s_start_freq, __pyx_n_s_end_freq, __pyx_n_s_ibf, __pyx_n_s_i, __pyx_n_s_tribases, __pyx_n_s_start_results, __pyx_n_s_end_results); if (unlikely(!__pyx_tuple__30)) __PYX_ERR(0, 100, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__30);
+  __Pyx_GIVEREF(__pyx_tuple__30);
+  __pyx_codeobj__31 = (PyObject*)__Pyx_PyCode_New(3, 0, 12, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__30, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_genome_info_kmers_kmer_reader_py, __pyx_n_s_read_bounds_tribase_freq, 100, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__31)) __PYX_ERR(0, 100, __pyx_L1_error)
 
   /* "View.MemoryView":287
  *         return self.name
  * 
  * cdef generic = Enum("<strided and direct or indirect>")             # <<<<<<<<<<<<<<
  * cdef strided = Enum("<strided and direct>") # default
  * cdef indirect = Enum("<strided and indirect>")
  */
-  __pyx_tuple__30 = PyTuple_Pack(1, __pyx_kp_s_strided_and_direct_or_indirect); if (unlikely(!__pyx_tuple__30)) __PYX_ERR(2, 287, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__30);
-  __Pyx_GIVEREF(__pyx_tuple__30);
+  __pyx_tuple__32 = PyTuple_Pack(1, __pyx_kp_s_strided_and_direct_or_indirect); if (unlikely(!__pyx_tuple__32)) __PYX_ERR(2, 287, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__32);
+  __Pyx_GIVEREF(__pyx_tuple__32);
 
   /* "View.MemoryView":288
  * 
  * cdef generic = Enum("<strided and direct or indirect>")
  * cdef strided = Enum("<strided and direct>") # default             # <<<<<<<<<<<<<<
  * cdef indirect = Enum("<strided and indirect>")
  * 
  */
-  __pyx_tuple__31 = PyTuple_Pack(1, __pyx_kp_s_strided_and_direct); if (unlikely(!__pyx_tuple__31)) __PYX_ERR(2, 288, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__31);
-  __Pyx_GIVEREF(__pyx_tuple__31);
+  __pyx_tuple__33 = PyTuple_Pack(1, __pyx_kp_s_strided_and_direct); if (unlikely(!__pyx_tuple__33)) __PYX_ERR(2, 288, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__33);
+  __Pyx_GIVEREF(__pyx_tuple__33);
 
   /* "View.MemoryView":289
  * cdef generic = Enum("<strided and direct or indirect>")
  * cdef strided = Enum("<strided and direct>") # default
  * cdef indirect = Enum("<strided and indirect>")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_tuple__32 = PyTuple_Pack(1, __pyx_kp_s_strided_and_indirect); if (unlikely(!__pyx_tuple__32)) __PYX_ERR(2, 289, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__32);
-  __Pyx_GIVEREF(__pyx_tuple__32);
+  __pyx_tuple__34 = PyTuple_Pack(1, __pyx_kp_s_strided_and_indirect); if (unlikely(!__pyx_tuple__34)) __PYX_ERR(2, 289, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__34);
+  __Pyx_GIVEREF(__pyx_tuple__34);
 
   /* "View.MemoryView":292
  * 
  * 
  * cdef contiguous = Enum("<contiguous and direct>")             # <<<<<<<<<<<<<<
  * cdef indirect_contiguous = Enum("<contiguous and indirect>")
  * 
  */
-  __pyx_tuple__33 = PyTuple_Pack(1, __pyx_kp_s_contiguous_and_direct); if (unlikely(!__pyx_tuple__33)) __PYX_ERR(2, 292, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__33);
-  __Pyx_GIVEREF(__pyx_tuple__33);
+  __pyx_tuple__35 = PyTuple_Pack(1, __pyx_kp_s_contiguous_and_direct); if (unlikely(!__pyx_tuple__35)) __PYX_ERR(2, 292, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__35);
+  __Pyx_GIVEREF(__pyx_tuple__35);
 
   /* "View.MemoryView":293
  * 
  * cdef contiguous = Enum("<contiguous and direct>")
  * cdef indirect_contiguous = Enum("<contiguous and indirect>")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_tuple__34 = PyTuple_Pack(1, __pyx_kp_s_contiguous_and_indirect); if (unlikely(!__pyx_tuple__34)) __PYX_ERR(2, 293, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__34);
-  __Pyx_GIVEREF(__pyx_tuple__34);
+  __pyx_tuple__36 = PyTuple_Pack(1, __pyx_kp_s_contiguous_and_indirect); if (unlikely(!__pyx_tuple__36)) __PYX_ERR(2, 293, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__36);
+  __Pyx_GIVEREF(__pyx_tuple__36);
 
   /* "(tree fragment)":1
  * def __pyx_unpickle_Enum(__pyx_type, long __pyx_checksum, __pyx_state):             # <<<<<<<<<<<<<<
  *     cdef object __pyx_PickleError
  *     cdef object __pyx_result
  */
-  __pyx_tuple__35 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__35)) __PYX_ERR(2, 1, __pyx_L1_error)
-  __Pyx_GOTREF(__pyx_tuple__35);
-  __Pyx_GIVEREF(__pyx_tuple__35);
-  __pyx_codeobj__36 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__35, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_Enum, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__36)) __PYX_ERR(2, 1, __pyx_L1_error)
+  __pyx_tuple__37 = PyTuple_Pack(5, __pyx_n_s_pyx_type, __pyx_n_s_pyx_checksum, __pyx_n_s_pyx_state, __pyx_n_s_pyx_PickleError, __pyx_n_s_pyx_result); if (unlikely(!__pyx_tuple__37)) __PYX_ERR(2, 1, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_tuple__37);
+  __Pyx_GIVEREF(__pyx_tuple__37);
+  __pyx_codeobj__38 = (PyObject*)__Pyx_PyCode_New(3, 0, 5, 0, CO_OPTIMIZED|CO_NEWLOCALS, __pyx_empty_bytes, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_tuple__37, __pyx_empty_tuple, __pyx_empty_tuple, __pyx_kp_s_stringsource, __pyx_n_s_pyx_unpickle_Enum, 1, __pyx_empty_bytes); if (unlikely(!__pyx_codeobj__38)) __PYX_ERR(2, 1, __pyx_L1_error)
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
   __Pyx_RefNannyFinishContext();
   return -1;
 }
 
@@ -19782,14 +23589,74 @@
 
   if (__Pyx_InitStrings(__pyx_string_tab) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_0 = PyInt_FromLong(0); if (unlikely(!__pyx_int_0)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_1 = PyInt_FromLong(1); if (unlikely(!__pyx_int_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_2 = PyInt_FromLong(2); if (unlikely(!__pyx_int_2)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_3 = PyInt_FromLong(3); if (unlikely(!__pyx_int_3)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_4 = PyInt_FromLong(4); if (unlikely(!__pyx_int_4)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_5 = PyInt_FromLong(5); if (unlikely(!__pyx_int_5)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_6 = PyInt_FromLong(6); if (unlikely(!__pyx_int_6)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_7 = PyInt_FromLong(7); if (unlikely(!__pyx_int_7)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_8 = PyInt_FromLong(8); if (unlikely(!__pyx_int_8)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_9 = PyInt_FromLong(9); if (unlikely(!__pyx_int_9)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_10 = PyInt_FromLong(10); if (unlikely(!__pyx_int_10)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_11 = PyInt_FromLong(11); if (unlikely(!__pyx_int_11)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_12 = PyInt_FromLong(12); if (unlikely(!__pyx_int_12)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_13 = PyInt_FromLong(13); if (unlikely(!__pyx_int_13)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_14 = PyInt_FromLong(14); if (unlikely(!__pyx_int_14)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_15 = PyInt_FromLong(15); if (unlikely(!__pyx_int_15)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_16 = PyInt_FromLong(16); if (unlikely(!__pyx_int_16)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_17 = PyInt_FromLong(17); if (unlikely(!__pyx_int_17)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_18 = PyInt_FromLong(18); if (unlikely(!__pyx_int_18)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_19 = PyInt_FromLong(19); if (unlikely(!__pyx_int_19)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_20 = PyInt_FromLong(20); if (unlikely(!__pyx_int_20)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_21 = PyInt_FromLong(21); if (unlikely(!__pyx_int_21)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_22 = PyInt_FromLong(22); if (unlikely(!__pyx_int_22)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_23 = PyInt_FromLong(23); if (unlikely(!__pyx_int_23)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_24 = PyInt_FromLong(24); if (unlikely(!__pyx_int_24)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_25 = PyInt_FromLong(25); if (unlikely(!__pyx_int_25)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_26 = PyInt_FromLong(26); if (unlikely(!__pyx_int_26)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_27 = PyInt_FromLong(27); if (unlikely(!__pyx_int_27)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_28 = PyInt_FromLong(28); if (unlikely(!__pyx_int_28)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_29 = PyInt_FromLong(29); if (unlikely(!__pyx_int_29)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_30 = PyInt_FromLong(30); if (unlikely(!__pyx_int_30)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_31 = PyInt_FromLong(31); if (unlikely(!__pyx_int_31)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_32 = PyInt_FromLong(32); if (unlikely(!__pyx_int_32)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_33 = PyInt_FromLong(33); if (unlikely(!__pyx_int_33)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_34 = PyInt_FromLong(34); if (unlikely(!__pyx_int_34)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_35 = PyInt_FromLong(35); if (unlikely(!__pyx_int_35)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_36 = PyInt_FromLong(36); if (unlikely(!__pyx_int_36)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_37 = PyInt_FromLong(37); if (unlikely(!__pyx_int_37)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_38 = PyInt_FromLong(38); if (unlikely(!__pyx_int_38)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_39 = PyInt_FromLong(39); if (unlikely(!__pyx_int_39)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_40 = PyInt_FromLong(40); if (unlikely(!__pyx_int_40)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_41 = PyInt_FromLong(41); if (unlikely(!__pyx_int_41)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_42 = PyInt_FromLong(42); if (unlikely(!__pyx_int_42)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_43 = PyInt_FromLong(43); if (unlikely(!__pyx_int_43)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_44 = PyInt_FromLong(44); if (unlikely(!__pyx_int_44)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_45 = PyInt_FromLong(45); if (unlikely(!__pyx_int_45)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_46 = PyInt_FromLong(46); if (unlikely(!__pyx_int_46)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_47 = PyInt_FromLong(47); if (unlikely(!__pyx_int_47)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_48 = PyInt_FromLong(48); if (unlikely(!__pyx_int_48)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_49 = PyInt_FromLong(49); if (unlikely(!__pyx_int_49)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_50 = PyInt_FromLong(50); if (unlikely(!__pyx_int_50)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_51 = PyInt_FromLong(51); if (unlikely(!__pyx_int_51)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_52 = PyInt_FromLong(52); if (unlikely(!__pyx_int_52)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_53 = PyInt_FromLong(53); if (unlikely(!__pyx_int_53)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_54 = PyInt_FromLong(54); if (unlikely(!__pyx_int_54)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_55 = PyInt_FromLong(55); if (unlikely(!__pyx_int_55)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_56 = PyInt_FromLong(56); if (unlikely(!__pyx_int_56)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_57 = PyInt_FromLong(57); if (unlikely(!__pyx_int_57)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_58 = PyInt_FromLong(58); if (unlikely(!__pyx_int_58)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_59 = PyInt_FromLong(59); if (unlikely(!__pyx_int_59)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_60 = PyInt_FromLong(60); if (unlikely(!__pyx_int_60)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_61 = PyInt_FromLong(61); if (unlikely(!__pyx_int_61)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_62 = PyInt_FromLong(62); if (unlikely(!__pyx_int_62)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_63 = PyInt_FromLong(63); if (unlikely(!__pyx_int_63)) __PYX_ERR(0, 1, __pyx_L1_error)
+  __pyx_int_64 = PyInt_FromLong(64); if (unlikely(!__pyx_int_64)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_112105877 = PyInt_FromLong(112105877L); if (unlikely(!__pyx_int_112105877)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_136983863 = PyInt_FromLong(136983863L); if (unlikely(!__pyx_int_136983863)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_184977713 = PyInt_FromLong(184977713L); if (unlikely(!__pyx_int_184977713)) __PYX_ERR(0, 1, __pyx_L1_error)
   __pyx_int_neg_1 = PyInt_FromLong(-1); if (unlikely(!__pyx_int_neg_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   return 0;
   __pyx_L1_error:;
   return -1;
@@ -19926,25 +23793,25 @@
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("numpy"); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 199, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_5numpy_dtype = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "dtype", sizeof(PyArray_Descr), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyArray_Descr),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_dtype) __PYX_ERR(1, 199, __pyx_L1_error)
   __pyx_ptype_5numpy_flatiter = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "flatiter", sizeof(PyArrayIterObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyArrayIterObject),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_flatiter) __PYX_ERR(1, 222, __pyx_L1_error)
   __pyx_ptype_5numpy_broadcast = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "broadcast", sizeof(PyArrayMultiIterObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyArrayMultiIterObject),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_broadcast) __PYX_ERR(1, 226, __pyx_L1_error)
   __pyx_ptype_5numpy_ndarray = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "ndarray", sizeof(PyArrayObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyArrayObject),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_ndarray) __PYX_ERR(1, 238, __pyx_L1_error)
-  __pyx_ptype_5numpy_generic = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_generic) __PYX_ERR(1, 767, __pyx_L1_error)
-  __pyx_ptype_5numpy_number = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_number) __PYX_ERR(1, 769, __pyx_L1_error)
-  __pyx_ptype_5numpy_integer = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_integer) __PYX_ERR(1, 771, __pyx_L1_error)
-  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(1, 773, __pyx_L1_error)
-  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(1, 775, __pyx_L1_error)
-  __pyx_ptype_5numpy_inexact = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(1, 777, __pyx_L1_error)
-  __pyx_ptype_5numpy_floating = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_floating) __PYX_ERR(1, 779, __pyx_L1_error)
-  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(1, 781, __pyx_L1_error)
-  __pyx_ptype_5numpy_flexible = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(1, 783, __pyx_L1_error)
-  __pyx_ptype_5numpy_character = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_character) __PYX_ERR(1, 785, __pyx_L1_error)
-  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyUFuncObject),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(1, 824, __pyx_L1_error)
+  __pyx_ptype_5numpy_generic = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "generic", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_generic) __PYX_ERR(1, 770, __pyx_L1_error)
+  __pyx_ptype_5numpy_number = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "number", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_number) __PYX_ERR(1, 772, __pyx_L1_error)
+  __pyx_ptype_5numpy_integer = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "integer", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_integer) __PYX_ERR(1, 774, __pyx_L1_error)
+  __pyx_ptype_5numpy_signedinteger = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "signedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_signedinteger) __PYX_ERR(1, 776, __pyx_L1_error)
+  __pyx_ptype_5numpy_unsignedinteger = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "unsignedinteger", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_unsignedinteger) __PYX_ERR(1, 778, __pyx_L1_error)
+  __pyx_ptype_5numpy_inexact = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "inexact", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_inexact) __PYX_ERR(1, 780, __pyx_L1_error)
+  __pyx_ptype_5numpy_floating = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "floating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_floating) __PYX_ERR(1, 782, __pyx_L1_error)
+  __pyx_ptype_5numpy_complexfloating = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "complexfloating", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_complexfloating) __PYX_ERR(1, 784, __pyx_L1_error)
+  __pyx_ptype_5numpy_flexible = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "flexible", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_flexible) __PYX_ERR(1, 786, __pyx_L1_error)
+  __pyx_ptype_5numpy_character = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "character", sizeof(PyObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyObject),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_5numpy_character) __PYX_ERR(1, 788, __pyx_L1_error)
+  __pyx_ptype_5numpy_ufunc = __Pyx_ImportType_0_29_36(__pyx_t_1, "numpy", "ufunc", sizeof(PyUFuncObject), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(PyUFuncObject),__Pyx_ImportType_CheckSize_Ignore_0_29_36); if (!__pyx_ptype_5numpy_ufunc) __PYX_ERR(1, 826, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("ailist.Interval_core"); if (unlikely(!__pyx_t_1)) __PYX_ERR(4, 21, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_ptype_6ailist_13Interval_core_Interval = __Pyx_ImportType_0_29_36(__pyx_t_1, "ailist.Interval_core", "Interval", sizeof(struct __pyx_obj_6ailist_13Interval_core_Interval), __PYX_GET_STRUCT_ALIGNMENT_0_29_36(struct __pyx_obj_6ailist_13Interval_core_Interval),__Pyx_ImportType_CheckSize_Warn_0_29_36); if (!__pyx_ptype_6ailist_13Interval_core_Interval) __PYX_ERR(4, 21, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __pyx_t_1 = PyImport_ImportModule("ailist.AIList_core"); if (unlikely(!__pyx_t_1)) __PYX_ERR(5, 373, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
@@ -20183,90 +24050,114 @@
   #if defined(__Pyx_Generator_USED) || defined(__Pyx_Coroutine_USED)
   if (__Pyx_patch_abc() < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   #endif
 
   /* "genome_info/kmers/kmer_reader.pyx":4
  * #cython: profile=False
  * 
+ * import pandas as pd             # <<<<<<<<<<<<<<
+ * import numpy as np
+ * cimport numpy as np
+ */
+  __pyx_t_1 = __Pyx_Import(__pyx_n_s_pandas, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 4, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_1);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_pd, __pyx_t_1) < 0) __PYX_ERR(0, 4, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
+
+  /* "genome_info/kmers/kmer_reader.pyx":5
+ * 
+ * import pandas as pd
  * import numpy as np             # <<<<<<<<<<<<<<
  * cimport numpy as np
  * 
  */
-  __pyx_t_1 = __Pyx_Import(__pyx_n_s_numpy, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 4, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_Import(__pyx_n_s_numpy, 0, 0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 5, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_np, __pyx_t_1) < 0) __PYX_ERR(0, 4, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_np, __pyx_t_1) < 0) __PYX_ERR(0, 5, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "genome_info/kmers/kmer_reader.pyx":9
+  /* "genome_info/kmers/kmer_reader.pyx":10
  * from libc.stdint cimport uint32_t, int32_t, int64_t, uint16_t
  * from ailist.LabeledIntervalArray_core cimport LabeledIntervalArray, labeled_aiarray_t
  * from ..genomes.genomes import InfoReader             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 9, __pyx_L1_error)
+  __pyx_t_1 = PyList_New(1); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 10, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __Pyx_INCREF(__pyx_n_s_InfoReader);
   __Pyx_GIVEREF(__pyx_n_s_InfoReader);
   PyList_SET_ITEM(__pyx_t_1, 0, __pyx_n_s_InfoReader);
-  __pyx_t_2 = __Pyx_Import(__pyx_n_s_genomes_genomes, __pyx_t_1, 2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 9, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_Import(__pyx_n_s_genomes_genomes, __pyx_t_1, 2); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 10, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
-  __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_InfoReader); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 9, __pyx_L1_error)
+  __pyx_t_1 = __Pyx_ImportFrom(__pyx_t_2, __pyx_n_s_InfoReader); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 10, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_InfoReader, __pyx_t_1) < 0) __PYX_ERR(0, 9, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_InfoReader, __pyx_t_1) < 0) __PYX_ERR(0, 10, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "genome_info/kmers/kmer_reader.pyx":18
+  /* "genome_info/kmers/kmer_reader.pyx":19
  * 
  * 
  * def read_kmers(str seq_fn, LabeledIntervalArray laia, int k, int last_n = 0):             # <<<<<<<<<<<<<<
  * 
  *     cdef str twobit_name = seq_fn
  */
-  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_11genome_info_5kmers_11kmer_reader_1read_kmers, NULL, __pyx_n_s_genome_info_kmers_kmer_reader); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 18, __pyx_L1_error)
+  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_11genome_info_5kmers_11kmer_reader_1read_kmers, NULL, __pyx_n_s_genome_info_kmers_kmer_reader); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 19, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_read_kmers, __pyx_t_2) < 0) __PYX_ERR(0, 18, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_read_kmers, __pyx_t_2) < 0) __PYX_ERR(0, 19, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "genome_info/kmers/kmer_reader.pyx":45
+  /* "genome_info/kmers/kmer_reader.pyx":46
  *     return seq
  * 
  * def read_sequence(str seq_fn, str chrom, int start, int end):             # <<<<<<<<<<<<<<
  * 
  *     cdef str twobit_name = seq_fn
  */
-  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_11genome_info_5kmers_11kmer_reader_3read_sequence, NULL, __pyx_n_s_genome_info_kmers_kmer_reader); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 45, __pyx_L1_error)
+  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_11genome_info_5kmers_11kmer_reader_3read_sequence, NULL, __pyx_n_s_genome_info_kmers_kmer_reader); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 46, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_read_sequence, __pyx_t_2) < 0) __PYX_ERR(0, 45, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_read_sequence, __pyx_t_2) < 0) __PYX_ERR(0, 46, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "genome_info/kmers/kmer_reader.pyx":63
+  /* "genome_info/kmers/kmer_reader.pyx":64
  * 
  * 
  * def gc_percent(str seq_fn, LabeledIntervalArray laia, str genome_version = "hg38"):             # <<<<<<<<<<<<<<
  *     cdef str twobit_name = seq_fn
  *     cdef bytes fname = twobit_name.encode()
  */
-  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_11genome_info_5kmers_11kmer_reader_5gc_percent, NULL, __pyx_n_s_genome_info_kmers_kmer_reader); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 63, __pyx_L1_error)
+  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_11genome_info_5kmers_11kmer_reader_5gc_percent, NULL, __pyx_n_s_genome_info_kmers_kmer_reader); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 64, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_gc_percent, __pyx_t_2) < 0) __PYX_ERR(0, 63, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_gc_percent, __pyx_t_2) < 0) __PYX_ERR(0, 64, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
-  /* "genome_info/kmers/kmer_reader.pyx":75
+  /* "genome_info/kmers/kmer_reader.pyx":76
  * 
  * 
  * def read_bounds_base_freq(str seq_fn, LabeledIntervalArray laia, int n_bases):             # <<<<<<<<<<<<<<
  * 
  *     cdef str twobit_name = seq_fn
  */
-  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_11genome_info_5kmers_11kmer_reader_7read_bounds_base_freq, NULL, __pyx_n_s_genome_info_kmers_kmer_reader); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 75, __pyx_L1_error)
+  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_11genome_info_5kmers_11kmer_reader_7read_bounds_base_freq, NULL, __pyx_n_s_genome_info_kmers_kmer_reader); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 76, __pyx_L1_error)
+  __Pyx_GOTREF(__pyx_t_2);
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_read_bounds_base_freq, __pyx_t_2) < 0) __PYX_ERR(0, 76, __pyx_L1_error)
+  __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
+
+  /* "genome_info/kmers/kmer_reader.pyx":100
+ * 
+ * 
+ * def read_bounds_tribase_freq(str seq_fn, LabeledIntervalArray laia, int n_bases):             # <<<<<<<<<<<<<<
+ * 
+ *     cdef str twobit_name = seq_fn
+ */
+  __pyx_t_2 = PyCFunction_NewEx(&__pyx_mdef_11genome_info_5kmers_11kmer_reader_9read_bounds_tribase_freq, NULL, __pyx_n_s_genome_info_kmers_kmer_reader); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 100, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
-  if (PyDict_SetItem(__pyx_d, __pyx_n_s_read_bounds_base_freq, __pyx_t_2) < 0) __PYX_ERR(0, 75, __pyx_L1_error)
+  if (PyDict_SetItem(__pyx_d, __pyx_n_s_read_bounds_tribase_freq, __pyx_t_2) < 0) __PYX_ERR(0, 100, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "genome_info/kmers/kmer_reader.pyx":1
  * #cython: embedsignature=True             # <<<<<<<<<<<<<<
  * #cython: profile=False
  * 
  */
@@ -20291,71 +24182,71 @@
   /* "View.MemoryView":287
  *         return self.name
  * 
  * cdef generic = Enum("<strided and direct or indirect>")             # <<<<<<<<<<<<<<
  * cdef strided = Enum("<strided and direct>") # default
  * cdef indirect = Enum("<strided and indirect>")
  */
-  __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__30, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 287, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__32, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 287, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_XGOTREF(generic);
   __Pyx_DECREF_SET(generic, __pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_2);
   __pyx_t_2 = 0;
 
   /* "View.MemoryView":288
  * 
  * cdef generic = Enum("<strided and direct or indirect>")
  * cdef strided = Enum("<strided and direct>") # default             # <<<<<<<<<<<<<<
  * cdef indirect = Enum("<strided and indirect>")
  * 
  */
-  __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__31, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 288, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__33, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 288, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_XGOTREF(strided);
   __Pyx_DECREF_SET(strided, __pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_2);
   __pyx_t_2 = 0;
 
   /* "View.MemoryView":289
  * cdef generic = Enum("<strided and direct or indirect>")
  * cdef strided = Enum("<strided and direct>") # default
  * cdef indirect = Enum("<strided and indirect>")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__32, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 289, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__34, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 289, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_XGOTREF(indirect);
   __Pyx_DECREF_SET(indirect, __pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_2);
   __pyx_t_2 = 0;
 
   /* "View.MemoryView":292
  * 
  * 
  * cdef contiguous = Enum("<contiguous and direct>")             # <<<<<<<<<<<<<<
  * cdef indirect_contiguous = Enum("<contiguous and indirect>")
  * 
  */
-  __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__33, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 292, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__35, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 292, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_XGOTREF(contiguous);
   __Pyx_DECREF_SET(contiguous, __pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_2);
   __pyx_t_2 = 0;
 
   /* "View.MemoryView":293
  * 
  * cdef contiguous = Enum("<contiguous and direct>")
  * cdef indirect_contiguous = Enum("<contiguous and indirect>")             # <<<<<<<<<<<<<<
  * 
  * 
  */
-  __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__34, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 293, __pyx_L1_error)
+  __pyx_t_2 = __Pyx_PyObject_Call(((PyObject *)__pyx_MemviewEnum_type), __pyx_tuple__36, NULL); if (unlikely(!__pyx_t_2)) __PYX_ERR(2, 293, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
   __Pyx_XGOTREF(indirect_contiguous);
   __Pyx_DECREF_SET(indirect_contiguous, __pyx_t_2);
   __Pyx_GIVEREF(__pyx_t_2);
   __pyx_t_2 = 0;
 
   /* "View.MemoryView":317
```

### Comparing `genome_info-1.0.2/genome_info/kmers/kmer_reader.cpython-310-darwin.so` & `genome_info-1.0.4/genome_info/kmers/kmer_reader.cpython-310-darwin.so`

 * *Files identical despite different names*

### Comparing `genome_info-1.0.2/genome_info/kmers/kmer_reader.cpython-311-darwin.so` & `genome_info-1.0.4/genome_info/kmers/kmer_reader.cpython-311-darwin.so`

 * *Files identical despite different names*

### Comparing `genome_info-1.0.2/pyproject.toml` & `genome_info-1.0.4/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "genome_info"
-version = "1.0.2"
+version = "1.0.4"
 description = "Python package genome annotations"
 authors = ["Kyle S. Smith <kyle.smith@stjude.org>"]
 maintainers = ["Kyle S. Smith <kyle.smith@stjude.org>"]
 repository = "https://github.com/kylessmith/genome_info"
 documentation = "https://www.biosciencestack.com/static/genome_info/docs/index.html"
 keywords = ["cython", "annotation", "genome"]
 readme = 'README.md'
@@ -28,15 +28,15 @@
 include = ["genome_info/kmers/*.pyx", "genome_info/kmers/*.pxd", "genome_info/kmers/*.h", "genome_info/kmers/*.c", "genome_info/**/*.so"]
 
 [tool.poetry.dependencies]
 python = "^3.10"
 numpy = "^1.23.5"
 cython = "^0.29.32"
 pandas = "^1.5.2"
-intervalframe = "^1.1.3"
+intervalframe = "^1.1.5"
 tqdm = "^4.65.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "^5.2"
 
 [build-system]
 requires = ["poetry-core>=1.0.0",
```

### Comparing `genome_info-1.0.2/PKG-INFO` & `genome_info-1.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: genome_info
-Version: 1.0.2
+Version: 1.0.4
 Summary: Python package genome annotations
 Home-page: https://github.com/kylessmith/genome_info
 License: GPL-2.0-or-later
 Keywords: cython,annotation,genome
 Author: Kyle S. Smith
 Author-email: kyle.smith@stjude.org
 Maintainer: Kyle S. Smith
@@ -25,15 +25,15 @@
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
 Classifier: Topic :: Scientific/Engineering :: Mathematics
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: cython (>=0.29.32,<0.30.0)
-Requires-Dist: intervalframe (>=1.1.3,<2.0.0)
+Requires-Dist: intervalframe (>=1.1.5,<2.0.0)
 Requires-Dist: numpy (>=1.23.5,<2.0.0)
 Requires-Dist: pandas (>=1.5.2,<2.0.0)
 Requires-Dist: tqdm (>=4.65.0,<5.0.0)
 Project-URL: Documentation, https://www.biosciencestack.com/static/genome_info/docs/index.html
 Project-URL: Repository, https://github.com/kylessmith/genome_info
 Description-Content-Type: text/markdown
```

