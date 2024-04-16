# Comparing `tmp/nanoCEM-0.0.5.5.tar.gz` & `tmp/nanoCEM-0.0.5.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nanoCEM-0.0.5.5.tar", last modified: Tue Apr 16 07:30:24 2024, max compression
+gzip compressed data, was "dist/nanoCEM-0.0.5.6.tar", last modified: Tue Apr 16 08:18:55 2024, max compression
```

## Comparing `nanoCEM-0.0.5.5.tar` & `nanoCEM-0.0.5.6.tar`

### file list

```diff
@@ -1,37 +1,34 @@
-drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2024-04-16 07:30:24.822410 nanoCEM-0.0.5.5/
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1087 2023-05-31 12:16:43.000000 nanoCEM-0.0.5.5/LICENSE
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     2730 2024-04-16 07:30:24.822410 nanoCEM-0.0.5.5/PKG-INFO
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     2100 2024-03-07 07:08:59.000000 nanoCEM-0.0.5.5/README.md
-drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2024-04-16 07:30:24.822410 nanoCEM-0.0.5.5/nanoCEM/
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    15651 2024-04-16 07:22:23.000000 nanoCEM-0.0.5.5/nanoCEM/CE_magnifier_test.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     5416 2023-12-21 04:37:40.000000 nanoCEM-0.0.5.5/nanoCEM/NEW_TRAINER.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       56 2023-06-14 11:15:11.000000 nanoCEM-0.0.5.5/nanoCEM/__init__.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     4547 2023-12-10 10:36:58.000000 nanoCEM-0.0.5.5/nanoCEM/alignment_feature_camera.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    10849 2024-04-16 04:27:47.000000 nanoCEM-0.0.5.5/nanoCEM/alignment_magnifier
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    14695 2024-04-15 10:30:11.000000 nanoCEM-0.0.5.5/nanoCEM/cem_utils.py
--rwxrwxr-x   0 zhguo     (1000) zhguo     (1000)    10801 2024-04-13 03:51:24.000000 nanoCEM-0.0.5.5/nanoCEM/current_events_magnifier
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     5903 2024-03-27 13:32:46.000000 nanoCEM-0.0.5.5/nanoCEM/de_novo.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     3137 2023-12-15 14:01:45.000000 nanoCEM-0.0.5.5/nanoCEM/density_2d.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     4083 2024-02-22 02:44:17.000000 nanoCEM-0.0.5.5/nanoCEM/extract_sub_fast5_from_bam
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1868 2023-07-24 04:48:56.000000 nanoCEM-0.0.5.5/nanoCEM/extract_sub_fastq_from_bam
-drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2024-04-16 07:30:24.822410 nanoCEM-0.0.5.5/nanoCEM/f5c_result_rna/
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)        0 2024-01-29 04:01:24.000000 nanoCEM-0.0.5.5/nanoCEM/f5c_result_rna/__init__.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      318 2024-01-29 04:02:07.000000 nanoCEM-0.0.5.5/nanoCEM/f5c_result_rna/test.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     2160 2024-03-27 13:32:46.000000 nanoCEM-0.0.5.5/nanoCEM/kmer_test.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1988 2024-02-23 07:56:30.000000 nanoCEM-0.0.5.5/nanoCEM/kmer_test_pr.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     3600 2024-03-27 13:32:45.000000 nanoCEM-0.0.5.5/nanoCEM/machine_learning_trainer.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     4427 2024-03-27 13:32:45.000000 nanoCEM-0.0.5.5/nanoCEM/normalization.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    11200 2024-02-23 10:21:22.000000 nanoCEM-0.0.5.5/nanoCEM/plot.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    10253 2024-04-16 02:28:14.000000 nanoCEM-0.0.5.5/nanoCEM/read_f5c_eventalign.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     6811 2024-04-16 02:48:18.000000 nanoCEM-0.0.5.5/nanoCEM/read_f5c_resquiggle.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     6866 2024-04-16 02:51:06.000000 nanoCEM-0.0.5.5/nanoCEM/read_move_table.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    13342 2024-02-26 08:39:30.000000 nanoCEM-0.0.5.5/nanoCEM/read_tombo_resquiggle.py
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     8548 2024-04-09 09:41:06.000000 nanoCEM-0.0.5.5/nanoCEM/squigualiser_utils.py
-drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2024-04-16 07:30:24.822410 nanoCEM-0.0.5.5/nanoCEM.egg-info/
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     2730 2024-04-16 07:30:24.000000 nanoCEM-0.0.5.5/nanoCEM.egg-info/PKG-INFO
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      821 2024-04-16 07:30:24.000000 nanoCEM-0.0.5.5/nanoCEM.egg-info/SOURCES.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)        1 2024-04-16 07:30:24.000000 nanoCEM-0.0.5.5/nanoCEM.egg-info/dependency_links.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      178 2024-04-16 07:30:24.000000 nanoCEM-0.0.5.5/nanoCEM.egg-info/requires.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)        8 2024-04-16 07:30:24.000000 nanoCEM-0.0.5.5/nanoCEM.egg-info/top_level.txt
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       38 2024-04-16 07:30:24.822410 nanoCEM-0.0.5.5/setup.cfg
--rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1295 2024-04-16 07:30:08.000000 nanoCEM-0.0.5.5/setup.py
+drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2024-04-16 08:18:55.164478 nanoCEM-0.0.5.6/
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1087 2023-05-31 12:16:43.000000 nanoCEM-0.0.5.6/LICENSE
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     2730 2024-04-16 08:18:55.164478 nanoCEM-0.0.5.6/PKG-INFO
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     2100 2024-03-07 07:08:59.000000 nanoCEM-0.0.5.6/README.md
+drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2024-04-16 08:18:55.164478 nanoCEM-0.0.5.6/nanoCEM/
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    15641 2024-04-16 08:04:15.000000 nanoCEM-0.0.5.6/nanoCEM/CE_magnifier_test.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     5416 2023-12-21 04:37:40.000000 nanoCEM-0.0.5.6/nanoCEM/NEW_TRAINER.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       56 2023-06-14 11:15:11.000000 nanoCEM-0.0.5.6/nanoCEM/__init__.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     4547 2023-12-10 10:36:58.000000 nanoCEM-0.0.5.6/nanoCEM/alignment_feature_camera.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    10849 2024-04-16 04:27:47.000000 nanoCEM-0.0.5.6/nanoCEM/alignment_magnifier
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    14691 2024-04-16 08:18:09.000000 nanoCEM-0.0.5.6/nanoCEM/cem_utils.py
+-rwxrwxr-x   0 zhguo     (1000) zhguo     (1000)    10801 2024-04-13 03:51:24.000000 nanoCEM-0.0.5.6/nanoCEM/current_events_magnifier
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     5903 2024-03-27 13:32:46.000000 nanoCEM-0.0.5.6/nanoCEM/de_novo.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     3137 2023-12-15 14:01:45.000000 nanoCEM-0.0.5.6/nanoCEM/density_2d.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     4083 2024-02-22 02:44:17.000000 nanoCEM-0.0.5.6/nanoCEM/extract_sub_fast5_from_bam
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1868 2023-07-24 04:48:56.000000 nanoCEM-0.0.5.6/nanoCEM/extract_sub_fastq_from_bam
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     2160 2024-03-27 13:32:46.000000 nanoCEM-0.0.5.6/nanoCEM/kmer_test.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1988 2024-02-23 07:56:30.000000 nanoCEM-0.0.5.6/nanoCEM/kmer_test_pr.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     3600 2024-03-27 13:32:45.000000 nanoCEM-0.0.5.6/nanoCEM/machine_learning_trainer.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     4427 2024-03-27 13:32:45.000000 nanoCEM-0.0.5.6/nanoCEM/normalization.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    11200 2024-02-23 10:21:22.000000 nanoCEM-0.0.5.6/nanoCEM/plot.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    10253 2024-04-16 02:28:14.000000 nanoCEM-0.0.5.6/nanoCEM/read_f5c_eventalign.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     6807 2024-04-16 07:47:03.000000 nanoCEM-0.0.5.6/nanoCEM/read_f5c_resquiggle.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     6866 2024-04-16 02:51:06.000000 nanoCEM-0.0.5.6/nanoCEM/read_move_table.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)    13342 2024-02-26 08:39:30.000000 nanoCEM-0.0.5.6/nanoCEM/read_tombo_resquiggle.py
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     8548 2024-04-09 09:41:06.000000 nanoCEM-0.0.5.6/nanoCEM/squigualiser_utils.py
+drwxrwxr-x   0 zhguo     (1000) zhguo     (1000)        0 2024-04-16 08:18:55.164478 nanoCEM-0.0.5.6/nanoCEM.egg-info/
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     2730 2024-04-16 08:18:55.000000 nanoCEM-0.0.5.6/nanoCEM.egg-info/PKG-INFO
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      755 2024-04-16 08:18:55.000000 nanoCEM-0.0.5.6/nanoCEM.egg-info/SOURCES.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)        1 2024-04-16 08:18:55.000000 nanoCEM-0.0.5.6/nanoCEM.egg-info/dependency_links.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)      178 2024-04-16 08:18:55.000000 nanoCEM-0.0.5.6/nanoCEM.egg-info/requires.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)        8 2024-04-16 08:18:55.000000 nanoCEM-0.0.5.6/nanoCEM.egg-info/top_level.txt
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)       38 2024-04-16 08:18:55.164478 nanoCEM-0.0.5.6/setup.cfg
+-rw-rw-r--   0 zhguo     (1000) zhguo     (1000)     1295 2024-04-16 08:18:54.000000 nanoCEM-0.0.5.6/setup.py
```

### Comparing `nanoCEM-0.0.5.5/LICENSE` & `nanoCEM-0.0.5.6/LICENSE`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.5.5/PKG-INFO` & `nanoCEM-0.0.5.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanoCEM
-Version: 0.0.5.5
+Version: 0.0.5.6
 Summary: A simple tool designed to visualize the features that distinguish between two groups of ONT data at the site level.                It supports 4 re-squiggle program(tombo resquiggle/f5c resquiggle/f5c eventalign/move_table).
 Home-page: https://github.com/lrslab/nanoCEM
 Author: GUO Zhihao
 Author-email: qhuozhihao@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nanoCEM Version: 0.0.5.5 Summary: A simple tool
+Metadata-Version: 2.1 Name: nanoCEM Version: 0.0.5.6 Summary: A simple tool
 designed to visualize the features that distinguish between two groups of ONT
 data at the site level. It supports 4 re-squiggle program(tombo resquiggle/f5c
 resquiggle/f5c eventalign/move_table). Home-page: https://github.com/lrslab/
 nanoCEM Author: GUO Zhihao Author-email: qhuozhihao@icloud.com Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python:
 >=3.7.0,<=3.11.7 Description-Content-Type: text/markdown License-File: LICENSE
```

### Comparing `nanoCEM-0.0.5.5/README.md` & `nanoCEM-0.0.5.6/README.md`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.5.5/nanoCEM/CE_magnifier_test.py` & `nanoCEM-0.0.5.6/nanoCEM/CE_magnifier_test.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,19 +98,19 @@
     #                     subsample_ratio=1,
     #                     ref="../example/data/23S_rRNA.fasta", rna=True)
     # parser.set_defaults(function='move_table', chrom="17", pos=43281378, len=10, strand='+', cpu=8,norm=True,
     #                                         input='../example/dna/hg38_chr17_43281378/WGS_r941/basecall',
     #                                         control='../example/dna/hg38_chr17_43281378/scWGA_941/basecall', output='move_result_dna',
     #                     subsample_ratio=1,sig_move_offset=4,kmer_length=5,
     #                     ref="../example/dna/hg38_17.fa", rna=False)
-    # parser.set_defaults(function='f5c_re', chrom="17", pos=43281378, len=10, strand='-', cpu=8,base_shift='auto',norm=True,
-    #                     input='../example/dna/hg38_chr17_43281378/WGS_r941/file',kmer_size=3,
-    #                     control='../example/dna/hg38_chr17_43281378/scWGA_941/file', output='f5c_result_dna_re',
-    #                     subsample_ratio=1,rna=False,
-    #                     ref="../example/dna/hg38_17.fa", pore='r9')
+    parser.set_defaults(function='f5c_re', chrom="17", pos=43281378, len=10, strand='+', cpu=8,base_shift='auto',norm=True,
+                        input='../example/dna/hg38_chr17_43281378/WGS_r941/file',kmer_size=3,
+                        control='../example/dna/hg38_chr17_43281378/scWGA_941/file', output='f5c_result_dna_re',
+                        subsample_ratio=1,rna=False,
+                        ref="../example/dna/hg38_17.fa", pore='r9')
     # parser.set_defaults(function='f5c_re', chrom="17", pos=39976063, len=10, strand='-', cpu=8, base_shift='auto',
     #                     norm=True,
     #                     input='../example/dna/hg38_chr17_43281378/WGS_r941/file', kmer_size=3,
     #                     control='../example/dna/hg38_chr17_43281378/scWGA_941/file', output='f5c_result_dna_re_re',
     #                     subsample_ratio=1, rna=False,
     #                     ref="../example/dna/hg38_17_rev.fa", pore='r9')
 
@@ -119,16 +119,16 @@
     #                     control='/hdd_data/download/23s_rRNA_A2030/ivt/file', output='f5c_result_rna_re_2524',
     #                     subsample_ratio=1,rna=True,
     #                     ref="../example/data/23S_rRNA.fasta", pore='r9')
     # parser.set_defaults(function='f5c_re', chrom="NR_103073.1", pos=875, len=10, strand='-', cpu=8,norm=True,base_shift='auto',pore='r9',
     #                     input='../example/data/wt/file', control='../example/data/ivt/file', output='f5c_result_rna_re_re',
     #                     subsample_ratio=1,kmer_size=3,
     #                     ref="../example/data/reverse/23S_rRNA_re.fasta", rna=True)
-    # parser.set_defaults(function='f5c_ev', chrom="NR_103073.1", pos=2251, len=5, strand='+', cpu=8,norm=True,base_shift='auto',pore='r9',
-    #                     input='../example/data/wt/file', control='../example/data/ivt/file', output='f5c_result_rna_ev_2251',kmer_size=3,
+    # parser.set_defaults(function='f5c_re', chrom="NR_103073.1", pos=2251, len=5, strand='+', cpu=8,norm=True,base_shift='auto',pore='r9',
+    #                     input='../example/data/wt/file', control='../example/data/ivt/file', output='f5c_result_rna_re_2030',kmer_size=3,
     #                     subsample_ratio=1,
     #                     ref="../example/data/23S_rRNA.fasta", rna=True)
     return parser
 
 if __name__ == '__main__':
     # Parse the arguments
     parser = init_parser()
```

### Comparing `nanoCEM-0.0.5.5/nanoCEM/NEW_TRAINER.py` & `nanoCEM-0.0.5.6/nanoCEM/NEW_TRAINER.py`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.5.5/nanoCEM/alignment_feature_camera.py` & `nanoCEM-0.0.5.6/nanoCEM/alignment_feature_camera.py`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.5.5/nanoCEM/alignment_magnifier` & `nanoCEM-0.0.5.6/nanoCEM/alignment_magnifier`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.5.5/nanoCEM/cem_utils.py` & `nanoCEM-0.0.5.6/nanoCEM/cem_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,32 +5,32 @@
 import numpy as np
 import pandas as pd
 from tqdm import tqdm
 import multiprocessing
 import warnings
 
 warnings.filterwarnings("ignore", category=FutureWarning)
-from scipy import stats
 import copy
 
 ker_model_size ={
-    'r9+RNA': 5,
-    'r9+DNA': 6,
-    'r10+DNA': 9,
-    'rna004+RNA': 9
+    'r9RNA': 5,
+    'r9DNA': 6,
+    'r10DNA': 9,
+    'rna004RNA': 9
 }
 
 base_shift_dict ={
     'r9RNA+': -1,
     'r9RNA-': -3,
     'r9DNA+': -2,
     'r9DNA-': -3,
-    'r10DNA+': -2,
-    'r10DNA-': -6,
-    'rna004+RNA': 9
+    'r10DNA+': -6,
+    'r10DNA-': -2,
+    'rna004RNA+': -6,
+    'rna004RNA-': -2,
 }
 
 def caculate_base_shift_size(kmer_model,strand):
     def is_odd(number):
         if number % 2 == 0:
             return False
         else:
```

### Comparing `nanoCEM-0.0.5.5/nanoCEM/current_events_magnifier` & `nanoCEM-0.0.5.6/nanoCEM/current_events_magnifier`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.5.5/nanoCEM/de_novo.py` & `nanoCEM-0.0.5.6/nanoCEM/de_novo.py`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.5.5/nanoCEM/density_2d.py` & `nanoCEM-0.0.5.6/nanoCEM/density_2d.py`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.5.5/nanoCEM/extract_sub_fast5_from_bam` & `nanoCEM-0.0.5.6/nanoCEM/extract_sub_fast5_from_bam`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.5.5/nanoCEM/extract_sub_fastq_from_bam` & `nanoCEM-0.0.5.6/nanoCEM/extract_sub_fastq_from_bam`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.5.5/nanoCEM/kmer_test.py` & `nanoCEM-0.0.5.6/nanoCEM/kmer_test.py`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.5.5/nanoCEM/kmer_test_pr.py` & `nanoCEM-0.0.5.6/nanoCEM/kmer_test_pr.py`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.5.5/nanoCEM/machine_learning_trainer.py` & `nanoCEM-0.0.5.6/nanoCEM/machine_learning_trainer.py`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.5.5/nanoCEM/normalization.py` & `nanoCEM-0.0.5.6/nanoCEM/normalization.py`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.5.5/nanoCEM/plot.py` & `nanoCEM-0.0.5.6/nanoCEM/plot.py`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.5.5/nanoCEM/read_f5c_eventalign.py` & `nanoCEM-0.0.5.6/nanoCEM/read_f5c_eventalign.py`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.5.5/nanoCEM/read_f5c_resquiggle.py` & `nanoCEM-0.0.5.6/nanoCEM/read_f5c_resquiggle.py`

 * *Files 0% similar despite different names*

```diff
@@ -123,15 +123,15 @@
     identify_file_path(fastq_file)
     identify_file_path(slow5_file)
 
     if rna:
         nucleotide_type = 'RNA'
     else:
         nucleotide_type = 'DNA'
-    kmer_model = ker_model_size[pore+'+'+nucleotide_type]
+    kmer_model = ker_model_size[pore+nucleotide_type]
     if base_shift == 'auto':
         base_shift = base_shift_dict[pore + nucleotide_type + strand]
     else:
         base_shift = base_shift
 
     fastq_file, bam_file = generate_bam_file(fastq_file, reference, cpu, subsample_ratio)
     paf_file = generate_paf_file_resquiggle(fastq_file, slow5_file, pore, rna, cpu)
```

### Comparing `nanoCEM-0.0.5.5/nanoCEM/read_move_table.py` & `nanoCEM-0.0.5.6/nanoCEM/read_move_table.py`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.5.5/nanoCEM/read_tombo_resquiggle.py` & `nanoCEM-0.0.5.6/nanoCEM/read_tombo_resquiggle.py`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.5.5/nanoCEM/squigualiser_utils.py` & `nanoCEM-0.0.5.6/nanoCEM/squigualiser_utils.py`

 * *Files identical despite different names*

### Comparing `nanoCEM-0.0.5.5/nanoCEM.egg-info/PKG-INFO` & `nanoCEM-0.0.5.6/nanoCEM.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nanoCEM
-Version: 0.0.5.5
+Version: 0.0.5.6
 Summary: A simple tool designed to visualize the features that distinguish between two groups of ONT data at the site level.                It supports 4 re-squiggle program(tombo resquiggle/f5c resquiggle/f5c eventalign/move_table).
 Home-page: https://github.com/lrslab/nanoCEM
 Author: GUO Zhihao
 Author-email: qhuozhihao@icloud.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nanoCEM Version: 0.0.5.5 Summary: A simple tool
+Metadata-Version: 2.1 Name: nanoCEM Version: 0.0.5.6 Summary: A simple tool
 designed to visualize the features that distinguish between two groups of ONT
 data at the site level. It supports 4 re-squiggle program(tombo resquiggle/f5c
 resquiggle/f5c eventalign/move_table). Home-page: https://github.com/lrslab/
 nanoCEM Author: GUO Zhihao Author-email: qhuozhihao@icloud.com Classifier:
 Programming Language :: Python :: 3 Classifier: License :: OSI Approved :: MIT
 License Classifier: Operating System :: OS Independent Requires-Python:
 >=3.7.0,<=3.11.7 Description-Content-Type: text/markdown License-File: LICENSE
```

### Comparing `nanoCEM-0.0.5.5/nanoCEM.egg-info/SOURCES.txt` & `nanoCEM-0.0.5.6/nanoCEM.egg-info/SOURCES.txt`

 * *Files 22% similar despite different names*

```diff
@@ -22,10 +22,8 @@
 nanoCEM/read_move_table.py
 nanoCEM/read_tombo_resquiggle.py
 nanoCEM/squigualiser_utils.py
 nanoCEM.egg-info/PKG-INFO
 nanoCEM.egg-info/SOURCES.txt
 nanoCEM.egg-info/dependency_links.txt
 nanoCEM.egg-info/requires.txt
-nanoCEM.egg-info/top_level.txt
-nanoCEM/f5c_result_rna/__init__.py
-nanoCEM/f5c_result_rna/test.py
+nanoCEM.egg-info/top_level.txt
```

### Comparing `nanoCEM-0.0.5.5/setup.py` & `nanoCEM-0.0.5.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="nanoCEM",
-    version="0.0.5.5",
+    version="0.0.5.6",
     author="GUO Zhihao",
     author_email="qhuozhihao@icloud.com",
     description='A simple tool designed to visualize the features that distinguish between two groups of ONT data at the site level.\
                 It supports 4 re-squiggle program(tombo resquiggle/f5c resquiggle/f5c eventalign/move_table).',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/lrslab/nanoCEM",
```

