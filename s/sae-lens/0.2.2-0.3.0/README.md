# Comparing `tmp/sae_lens-0.2.2.tar.gz` & `tmp/sae_lens-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sae_lens-0.2.2.tar", max compression
+gzip compressed data, was "sae_lens-0.3.0.tar", max compression
```

## Comparing `sae_lens-0.2.2.tar` & `sae_lens-0.3.0.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1069 2024-04-15 14:53:42.825325 sae_lens-0.2.2/LICENSE
--rw-r--r--   0        0        0     2134 2024-04-15 14:53:42.825325 sae_lens-0.2.2/README.md
--rw-r--r--   0        0        0     1585 2024-04-15 14:53:43.801319 sae_lens-0.2.2/pyproject.toml
--rw-r--r--   0        0        0      943 2024-04-15 14:53:43.801319 sae_lens-0.2.2/sae_lens/__init__.py
--rw-r--r--   0        0        0        0 2024-04-15 14:53:42.833325 sae_lens-0.2.2/sae_lens/analysis/__init__.py
--rw-r--r--   0        0        0    15355 2024-04-15 14:53:42.833325 sae_lens-0.2.2/sae_lens/analysis/dashboard_runner.py
--rw-r--r--   0        0        0     3535 2024-04-15 14:53:42.837325 sae_lens-0.2.2/sae_lens/analysis/feature_statistics.py
--rw-r--r--   0        0        0      595 2024-04-15 14:53:42.837325 sae_lens-0.2.2/sae_lens/analysis/neuronpedia_integration.py
--rw-r--r--   0        0        0    19076 2024-04-15 14:53:42.837325 sae_lens-0.2.2/sae_lens/analysis/neuronpedia_runner.py
--rw-r--r--   0        0        0    18275 2024-04-15 14:53:42.837325 sae_lens-0.2.2/sae_lens/analysis/tsea.py
--rw-r--r--   0        0        0     5562 2024-04-15 14:53:42.837325 sae_lens-0.2.2/sae_lens/toolkit/pretrained_saes.py
--rw-r--r--   0        0        0        0 2024-04-15 14:53:42.837325 sae_lens-0.2.2/sae_lens/training/__init__.py
--rw-r--r--   0        0        0    16559 2024-04-15 14:53:42.837325 sae_lens-0.2.2/sae_lens/training/activations_store.py
--rw-r--r--   0        0        0     2804 2024-04-15 14:53:42.837325 sae_lens-0.2.2/sae_lens/training/cache_activations_runner.py
--rw-r--r--   0        0        0     8793 2024-04-15 14:53:42.837325 sae_lens-0.2.2/sae_lens/training/config.py
--rw-r--r--   0        0        0     5732 2024-04-15 14:53:42.837325 sae_lens-0.2.2/sae_lens/training/evals.py
--rw-r--r--   0        0        0     3747 2024-04-15 14:53:42.837325 sae_lens-0.2.2/sae_lens/training/geometric_median.py
--rw-r--r--   0        0        0     1528 2024-04-15 14:53:42.837325 sae_lens-0.2.2/sae_lens/training/lm_runner.py
--rw-r--r--   0        0        0     3675 2024-04-15 14:53:42.837325 sae_lens-0.2.2/sae_lens/training/optim.py
--rw-r--r--   0        0        0     7187 2024-04-15 14:53:42.837325 sae_lens-0.2.2/sae_lens/training/sae_group.py
--rw-r--r--   0        0        0     2318 2024-04-15 14:53:42.837325 sae_lens-0.2.2/sae_lens/training/session_loader.py
--rw-r--r--   0        0        0    13592 2024-04-15 14:53:42.837325 sae_lens-0.2.2/sae_lens/training/sparse_autoencoder.py
--rw-r--r--   0        0        0     3276 2024-04-15 14:53:42.837325 sae_lens-0.2.2/sae_lens/training/toy_model_runner.py
--rw-r--r--   0        0        0    17362 2024-04-15 14:53:42.837325 sae_lens-0.2.2/sae_lens/training/toy_models.py
--rw-r--r--   0        0        0    17227 2024-04-15 14:53:42.837325 sae_lens-0.2.2/sae_lens/training/train_sae_on_language_model.py
--rw-r--r--   0        0        0     4888 2024-04-15 14:53:42.837325 sae_lens-0.2.2/sae_lens/training/train_sae_on_toy_model.py
--rw-r--r--   0        0        0     1628 2024-04-15 14:53:42.837325 sae_lens-0.2.2/sae_lens/training/utils.py
--rw-r--r--   0        0        0     3420 1970-01-01 00:00:00.000000 sae_lens-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2024-04-15 16:33:04.963231 sae_lens-0.3.0/LICENSE
+-rw-r--r--   0        0        0     2134 2024-04-15 16:33:04.963231 sae_lens-0.3.0/README.md
+-rw-r--r--   0        0        0     1585 2024-04-15 16:33:05.931244 sae_lens-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0      943 2024-04-15 16:33:05.931244 sae_lens-0.3.0/sae_lens/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-15 16:33:04.975231 sae_lens-0.3.0/sae_lens/analysis/__init__.py
+-rw-r--r--   0        0        0    15355 2024-04-15 16:33:04.975231 sae_lens-0.3.0/sae_lens/analysis/dashboard_runner.py
+-rw-r--r--   0        0        0     3535 2024-04-15 16:33:04.975231 sae_lens-0.3.0/sae_lens/analysis/feature_statistics.py
+-rw-r--r--   0        0        0      595 2024-04-15 16:33:04.975231 sae_lens-0.3.0/sae_lens/analysis/neuronpedia_integration.py
+-rw-r--r--   0        0        0    19076 2024-04-15 16:33:04.975231 sae_lens-0.3.0/sae_lens/analysis/neuronpedia_runner.py
+-rw-r--r--   0        0        0    18275 2024-04-15 16:33:04.975231 sae_lens-0.3.0/sae_lens/analysis/tsea.py
+-rw-r--r--   0        0        0     5562 2024-04-15 16:33:04.975231 sae_lens-0.3.0/sae_lens/toolkit/pretrained_saes.py
+-rw-r--r--   0        0        0        0 2024-04-15 16:33:04.975231 sae_lens-0.3.0/sae_lens/training/__init__.py
+-rw-r--r--   0        0        0    16559 2024-04-15 16:33:04.975231 sae_lens-0.3.0/sae_lens/training/activations_store.py
+-rw-r--r--   0        0        0     2804 2024-04-15 16:33:04.975231 sae_lens-0.3.0/sae_lens/training/cache_activations_runner.py
+-rw-r--r--   0        0        0     8793 2024-04-15 16:33:04.975231 sae_lens-0.3.0/sae_lens/training/config.py
+-rw-r--r--   0        0        0     5732 2024-04-15 16:33:04.975231 sae_lens-0.3.0/sae_lens/training/evals.py
+-rw-r--r--   0        0        0     3747 2024-04-15 16:33:04.975231 sae_lens-0.3.0/sae_lens/training/geometric_median.py
+-rw-r--r--   0        0        0     1528 2024-04-15 16:33:04.975231 sae_lens-0.3.0/sae_lens/training/lm_runner.py
+-rw-r--r--   0        0        0     3675 2024-04-15 16:33:04.975231 sae_lens-0.3.0/sae_lens/training/optim.py
+-rw-r--r--   0        0        0     7187 2024-04-15 16:33:04.975231 sae_lens-0.3.0/sae_lens/training/sae_group.py
+-rw-r--r--   0        0        0     2318 2024-04-15 16:33:04.975231 sae_lens-0.3.0/sae_lens/training/session_loader.py
+-rw-r--r--   0        0        0    13592 2024-04-15 16:33:04.975231 sae_lens-0.3.0/sae_lens/training/sparse_autoencoder.py
+-rw-r--r--   0        0        0     3276 2024-04-15 16:33:04.975231 sae_lens-0.3.0/sae_lens/training/toy_model_runner.py
+-rw-r--r--   0        0        0    17362 2024-04-15 16:33:04.975231 sae_lens-0.3.0/sae_lens/training/toy_models.py
+-rw-r--r--   0        0        0    17227 2024-04-15 16:33:04.975231 sae_lens-0.3.0/sae_lens/training/train_sae_on_language_model.py
+-rw-r--r--   0        0        0     4888 2024-04-15 16:33:04.975231 sae_lens-0.3.0/sae_lens/training/train_sae_on_toy_model.py
+-rw-r--r--   0        0        0     1628 2024-04-15 16:33:04.975231 sae_lens-0.3.0/sae_lens/training/utils.py
+-rw-r--r--   0        0        0     3420 1970-01-01 00:00:00.000000 sae_lens-0.3.0/PKG-INFO
```

### Comparing `sae_lens-0.2.2/LICENSE` & `sae_lens-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `sae_lens-0.2.2/README.md` & `sae_lens-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `sae_lens-0.2.2/pyproject.toml` & `sae_lens-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sae-lens"
-version = "0.2.2"
+version = "0.3.0"
 description = "Training and Analyzing Sparse Autoencoders (SAEs)"
 authors = ["Joseph Bloom"]
 readme = "README.md"
 packages = [{include = "sae_lens"}]
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `sae_lens-0.2.2/sae_lens/__init__.py` & `sae_lens-0.3.0/sae_lens/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.2.2"
+__version__ = "0.3.0"
 
 from .training.activations_store import ActivationsStore
 from .training.cache_activations_runner import cache_activations_runner
 from .training.config import CacheActivationsRunnerConfig, LanguageModelSAERunnerConfig
 from .training.evals import run_evals
 from .training.lm_runner import language_model_sae_runner
 from .training.sae_group import SparseAutoencoderDictionary
```

### Comparing `sae_lens-0.2.2/sae_lens/analysis/dashboard_runner.py` & `sae_lens-0.3.0/sae_lens/analysis/dashboard_runner.py`

 * *Files identical despite different names*

### Comparing `sae_lens-0.2.2/sae_lens/analysis/feature_statistics.py` & `sae_lens-0.3.0/sae_lens/analysis/feature_statistics.py`

 * *Files identical despite different names*

### Comparing `sae_lens-0.2.2/sae_lens/analysis/neuronpedia_integration.py` & `sae_lens-0.3.0/sae_lens/analysis/neuronpedia_integration.py`

 * *Files identical despite different names*

### Comparing `sae_lens-0.2.2/sae_lens/analysis/neuronpedia_runner.py` & `sae_lens-0.3.0/sae_lens/analysis/neuronpedia_runner.py`

 * *Files identical despite different names*

### Comparing `sae_lens-0.2.2/sae_lens/analysis/tsea.py` & `sae_lens-0.3.0/sae_lens/analysis/tsea.py`

 * *Files identical despite different names*

### Comparing `sae_lens-0.2.2/sae_lens/toolkit/pretrained_saes.py` & `sae_lens-0.3.0/sae_lens/toolkit/pretrained_saes.py`

 * *Files identical despite different names*

### Comparing `sae_lens-0.2.2/sae_lens/training/activations_store.py` & `sae_lens-0.3.0/sae_lens/training/activations_store.py`

 * *Files identical despite different names*

### Comparing `sae_lens-0.2.2/sae_lens/training/cache_activations_runner.py` & `sae_lens-0.3.0/sae_lens/training/cache_activations_runner.py`

 * *Files identical despite different names*

### Comparing `sae_lens-0.2.2/sae_lens/training/config.py` & `sae_lens-0.3.0/sae_lens/training/config.py`

 * *Files identical despite different names*

### Comparing `sae_lens-0.2.2/sae_lens/training/evals.py` & `sae_lens-0.3.0/sae_lens/training/evals.py`

 * *Files identical despite different names*

### Comparing `sae_lens-0.2.2/sae_lens/training/geometric_median.py` & `sae_lens-0.3.0/sae_lens/training/geometric_median.py`

 * *Files identical despite different names*

### Comparing `sae_lens-0.2.2/sae_lens/training/lm_runner.py` & `sae_lens-0.3.0/sae_lens/training/lm_runner.py`

 * *Files identical despite different names*

### Comparing `sae_lens-0.2.2/sae_lens/training/optim.py` & `sae_lens-0.3.0/sae_lens/training/optim.py`

 * *Files identical despite different names*

### Comparing `sae_lens-0.2.2/sae_lens/training/sae_group.py` & `sae_lens-0.3.0/sae_lens/training/sae_group.py`

 * *Files identical despite different names*

### Comparing `sae_lens-0.2.2/sae_lens/training/session_loader.py` & `sae_lens-0.3.0/sae_lens/training/session_loader.py`

 * *Files identical despite different names*

### Comparing `sae_lens-0.2.2/sae_lens/training/sparse_autoencoder.py` & `sae_lens-0.3.0/sae_lens/training/sparse_autoencoder.py`

 * *Files identical despite different names*

### Comparing `sae_lens-0.2.2/sae_lens/training/toy_model_runner.py` & `sae_lens-0.3.0/sae_lens/training/toy_model_runner.py`

 * *Files identical despite different names*

### Comparing `sae_lens-0.2.2/sae_lens/training/toy_models.py` & `sae_lens-0.3.0/sae_lens/training/toy_models.py`

 * *Files identical despite different names*

### Comparing `sae_lens-0.2.2/sae_lens/training/train_sae_on_language_model.py` & `sae_lens-0.3.0/sae_lens/training/train_sae_on_language_model.py`

 * *Files identical despite different names*

### Comparing `sae_lens-0.2.2/sae_lens/training/train_sae_on_toy_model.py` & `sae_lens-0.3.0/sae_lens/training/train_sae_on_toy_model.py`

 * *Files identical despite different names*

### Comparing `sae_lens-0.2.2/sae_lens/training/utils.py` & `sae_lens-0.3.0/sae_lens/training/utils.py`

 * *Files identical despite different names*

### Comparing `sae_lens-0.2.2/PKG-INFO` & `sae_lens-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sae-lens
-Version: 0.2.2
+Version: 0.3.0
 Summary: Training and Analyzing Sparse Autoencoders (SAEs)
 Author: Joseph Bloom
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

