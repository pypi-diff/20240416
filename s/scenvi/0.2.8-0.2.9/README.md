# Comparing `tmp/scenvi-0.2.8.tar.gz` & `tmp/scenvi-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scenvi-0.2.8.tar", max compression
+gzip compressed data, was "scenvi-0.2.9.tar", max compression
```

## Comparing `scenvi-0.2.8.tar` & `scenvi-0.2.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1073 2024-02-20 21:59:17.777592 scenvi-0.2.8/LICENSE
--rw-r--r--   0        0        0     1715 2024-03-10 00:09:43.192347 scenvi-0.2.8/README.md
--rw-r--r--   0        0        0      394 2024-03-15 17:25:09.419983 scenvi-0.2.8/pyproject.toml
--rw-r--r--   0        0        0    20883 2024-03-09 23:06:56.188302 scenvi-0.2.8/scenvi/.ipynb_checkpoints/ENVI-checkpoint.py
--rw-r--r--   0        0        0       67 2024-03-09 23:08:20.592790 scenvi-0.2.8/scenvi/.ipynb_checkpoints/__init__-checkpoint.py
--rw-r--r--   0        0        0     1379 2024-03-09 21:43:54.336812 scenvi-0.2.8/scenvi/.ipynb_checkpoints/dists-checkpoint.py
--rw-r--r--   0        0        0     8180 2024-03-15 17:25:38.829484 scenvi-0.2.8/scenvi/.ipynb_checkpoints/utils-checkpoint.py
--rw-r--r--   0        0        0    20883 2024-03-09 23:06:56.188302 scenvi-0.2.8/scenvi/ENVI.py
--rw-r--r--   0        0        0       67 2024-03-09 23:08:20.592790 scenvi-0.2.8/scenvi/__init__.py
--rw-r--r--   0        0        0     1379 2024-03-09 21:43:54.360992 scenvi-0.2.8/scenvi/dists.py
--rw-r--r--   0        0        0     8180 2024-03-15 17:25:38.829484 scenvi-0.2.8/scenvi/utils.py
--rw-r--r--   0        0        0     2383 1970-01-01 00:00:00.000000 scenvi-0.2.8/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-02-20 21:59:17.777592 scenvi-0.2.9/LICENSE
+-rw-r--r--   0        0        0     1603 2024-03-15 17:34:51.240675 scenvi-0.2.9/README.md
+-rw-r--r--   0        0        0      395 2024-03-15 18:04:33.552469 scenvi-0.2.9/pyproject.toml
+-rw-r--r--   0        0        0    20883 2024-03-15 17:41:34.112047 scenvi-0.2.9/scenvi/.ipynb_checkpoints/ENVI-checkpoint.py
+-rw-r--r--   0        0        0       67 2024-03-09 23:08:20.592790 scenvi-0.2.9/scenvi/.ipynb_checkpoints/__init__-checkpoint.py
+-rw-r--r--   0        0        0     1379 2024-03-09 21:43:54.336812 scenvi-0.2.9/scenvi/.ipynb_checkpoints/dists-checkpoint.py
+-rw-r--r--   0        0        0     8180 2024-03-15 17:41:57.516346 scenvi-0.2.9/scenvi/.ipynb_checkpoints/utils-checkpoint.py
+-rw-r--r--   0        0        0    20883 2024-03-15 17:41:34.112047 scenvi-0.2.9/scenvi/ENVI.py
+-rw-r--r--   0        0        0       67 2024-03-09 23:08:20.592790 scenvi-0.2.9/scenvi/__init__.py
+-rw-r--r--   0        0        0     1379 2024-03-09 21:43:54.360992 scenvi-0.2.9/scenvi/dists.py
+-rw-r--r--   0        0        0     8180 2024-03-15 17:41:57.516346 scenvi-0.2.9/scenvi/utils.py
+-rw-r--r--   0        0        0     2272 1970-01-01 00:00:00.000000 scenvi-0.2.9/PKG-INFO
```

### Comparing `scenvi-0.2.8/LICENSE` & `scenvi-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `scenvi-0.2.8/README.md` & `scenvi-0.2.9/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,12 @@
 ENVI & COVET
 ======================
 
 
-ENVI is a deep learnining based variational inference method to integrate scRNAseq with spatial sequencing data. 
-It creates a combined latent space for both data modalities, from which missing gene can be imputed from spatial data, cell types labels can be transfered
-and the spatial niche can be reconstructed for the dissociated scRNAseq data
+ENVI is a deep learnining based variational inference method to integrate scRNA-seq with spatial transcriptomics data. ENVI learns to reconstruct spatial onto for dissociated scRNA-seq data and impute unimagd genes onto spatial data.
 
 This implementation is written in Python3 and relies on jax, flax, sklearn, scipy and scanpy.  
 
 
 To install JAX, simply run the command:
 
     pip install --upgrade "jax[cuda11_pip]" -f https://storage.googleapis.com/jax-releases/jax_cuda_releases.html
```

### Comparing `scenvi-0.2.8/scenvi/.ipynb_checkpoints/ENVI-checkpoint.py` & `scenvi-0.2.9/scenvi/.ipynb_checkpoints/ENVI-checkpoint.py`

 * *Files identical despite different names*

### Comparing `scenvi-0.2.8/scenvi/.ipynb_checkpoints/dists-checkpoint.py` & `scenvi-0.2.9/scenvi/.ipynb_checkpoints/dists-checkpoint.py`

 * *Files identical despite different names*

### Comparing `scenvi-0.2.8/scenvi/.ipynb_checkpoints/utils-checkpoint.py` & `scenvi-0.2.9/scenvi/.ipynb_checkpoints/utils-checkpoint.py`

 * *Files identical despite different names*

### Comparing `scenvi-0.2.8/scenvi/ENVI.py` & `scenvi-0.2.9/scenvi/ENVI.py`

 * *Files identical despite different names*

### Comparing `scenvi-0.2.8/scenvi/dists.py` & `scenvi-0.2.9/scenvi/dists.py`

 * *Files identical despite different names*

### Comparing `scenvi-0.2.8/scenvi/utils.py` & `scenvi-0.2.9/scenvi/utils.py`

 * *Files identical despite different names*

### Comparing `scenvi-0.2.8/PKG-INFO` & `scenvi-0.2.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,33 +1,31 @@
 Metadata-Version: 2.1
 Name: scenvi
-Version: 0.2.8
+Version: 0.2.9
 Summary: Integration of scRNA-seq and spatial transcriptomics data
 License: MIT
 Author: Doron Haviv
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: clu (==0.0.10)
 Requires-Dist: flax (==0.7.5)
-Requires-Dist: tensorfow_probability (==0.22.0)
+Requires-Dist: tensorflow_probability (==0.22.0)
 Requires-Dist: tqdm (>=4.66.1,<5.0.0)
 Description-Content-Type: text/markdown
 
 ENVI & COVET
 ======================
 
 
-ENVI is a deep learnining based variational inference method to integrate scRNAseq with spatial sequencing data. 
-It creates a combined latent space for both data modalities, from which missing gene can be imputed from spatial data, cell types labels can be transfered
-and the spatial niche can be reconstructed for the dissociated scRNAseq data
+ENVI is a deep learnining based variational inference method to integrate scRNA-seq with spatial transcriptomics data. ENVI learns to reconstruct spatial onto for dissociated scRNA-seq data and impute unimagd genes onto spatial data.
 
 This implementation is written in Python3 and relies on jax, flax, sklearn, scipy and scanpy.  
 
 
 To install JAX, simply run the command:
 
     pip install --upgrade "jax[cuda11_pip]" -f https://storage.googleapis.com/jax-releases/jax_cuda_releases.html
```

