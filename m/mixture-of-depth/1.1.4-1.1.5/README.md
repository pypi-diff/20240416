# Comparing `tmp/mixture-of-depth-1.1.4.tar.gz` & `tmp/mixture-of-depth-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mixture-of-depth-1.1.4.tar", last modified: Mon Apr 15 20:05:08 2024, max compression
+gzip compressed data, was "mixture-of-depth-1.1.5.tar", last modified: Mon Apr 15 20:42:58 2024, max compression
```

## Comparing `mixture-of-depth-1.1.4.tar` & `mixture-of-depth-1.1.5.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-15 20:05:08.178667 mixture-of-depth-1.1.4/
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-15 20:05:08.174667 mixture-of-depth-1.1.4/MoD/
--rw-rw-r--   0 marco     (1000) marco     (1000)     5265 2024-04-15 20:03:15.000000 mixture-of-depth-1.1.4/MoD/MoD.py
--rw-rw-r--   0 marco     (1000) marco     (1000)       83 2024-04-12 14:14:41.000000 mixture-of-depth-1.1.4/MoD/__init__.py
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-15 20:05:08.174667 mixture-of-depth-1.1.4/MoD/modeling/
--rw-rw-r--   0 marco     (1000) marco     (1000)       49 2024-04-12 13:59:17.000000 mixture-of-depth-1.1.4/MoD/modeling/__init__.py
--rw-rw-r--   0 marco     (1000) marco     (1000)     1556 2024-04-12 16:22:14.000000 mixture-of-depth-1.1.4/MoD/modeling/automodeling.py
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-15 20:05:08.178667 mixture-of-depth-1.1.4/MoD/modeling/models/
--rw-rw-r--   0 marco     (1000) marco     (1000)    55049 2024-04-13 10:23:41.000000 mixture-of-depth-1.1.4/MoD/modeling/models/BloomMoD.py
--rw-rw-r--   0 marco     (1000) marco     (1000)    75771 2024-04-13 11:04:53.000000 mixture-of-depth-1.1.4/MoD/modeling/models/FalconMoD.py
--rw-rw-r--   0 marco     (1000) marco     (1000)    63538 2024-04-13 10:23:41.000000 mixture-of-depth-1.1.4/MoD/modeling/models/GemmaMoD.py
--rw-rw-r--   0 marco     (1000) marco     (1000)    72912 2024-04-13 10:23:41.000000 mixture-of-depth-1.1.4/MoD/modeling/models/LlamaMoD.py
--rw-rw-r--   0 marco     (1000) marco     (1000)    63678 2024-04-13 10:23:41.000000 mixture-of-depth-1.1.4/MoD/modeling/models/MistralMoD.py
--rw-rw-r--   0 marco     (1000) marco     (1000)    73861 2024-04-13 10:23:41.000000 mixture-of-depth-1.1.4/MoD/modeling/models/MixtralMoD.py
--rw-rw-r--   0 marco     (1000) marco     (1000)    68490 2024-04-13 11:05:11.000000 mixture-of-depth-1.1.4/MoD/modeling/models/PhiMoD.py
--rw-rw-r--   0 marco     (1000) marco     (1000)    64007 2024-04-13 10:30:29.000000 mixture-of-depth-1.1.4/MoD/modeling/models/QwenMoD.py
--rw-rw-r--   0 marco     (1000) marco     (1000)    73663 2024-04-13 11:06:21.000000 mixture-of-depth-1.1.4/MoD/modeling/models/QwenMoEMoD.py
--rw-rw-r--   0 marco     (1000) marco     (1000)    64125 2024-04-13 10:47:31.000000 mixture-of-depth-1.1.4/MoD/modeling/models/StarCoderMoD.py
--rw-rw-r--   0 marco     (1000) marco     (1000)      439 2024-04-13 10:53:25.000000 mixture-of-depth-1.1.4/MoD/modeling/models/__init__.py
--rw-r--r--   0 marco     (1000) marco     (1000)     2978 2024-04-15 20:05:08.178667 mixture-of-depth-1.1.4/PKG-INFO
--rw-rw-r--   0 marco     (1000) marco     (1000)     2415 2024-04-13 10:55:20.000000 mixture-of-depth-1.1.4/README.md
-drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-15 20:05:08.178667 mixture-of-depth-1.1.4/mixture_of_depth.egg-info/
--rw-r--r--   0 marco     (1000) marco     (1000)     2978 2024-04-15 20:05:08.000000 mixture-of-depth-1.1.4/mixture_of_depth.egg-info/PKG-INFO
--rw-rw-r--   0 marco     (1000) marco     (1000)      658 2024-04-15 20:05:08.000000 mixture-of-depth-1.1.4/mixture_of_depth.egg-info/SOURCES.txt
--rw-rw-r--   0 marco     (1000) marco     (1000)        1 2024-04-15 20:05:08.000000 mixture-of-depth-1.1.4/mixture_of_depth.egg-info/dependency_links.txt
--rw-rw-r--   0 marco     (1000) marco     (1000)        6 2024-04-15 20:05:08.000000 mixture-of-depth-1.1.4/mixture_of_depth.egg-info/requires.txt
--rw-rw-r--   0 marco     (1000) marco     (1000)        4 2024-04-15 20:05:08.000000 mixture-of-depth-1.1.4/mixture_of_depth.egg-info/top_level.txt
--rw-rw-r--   0 marco     (1000) marco     (1000)       38 2024-04-15 20:05:08.178667 mixture-of-depth-1.1.4/setup.cfg
--rw-rw-r--   0 marco     (1000) marco     (1000)      769 2024-04-15 20:04:53.000000 mixture-of-depth-1.1.4/setup.py
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-15 20:42:58.765328 mixture-of-depth-1.1.5/
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-15 20:42:58.761328 mixture-of-depth-1.1.5/MoD/
+-rw-rw-r--   0 marco     (1000) marco     (1000)     5253 2024-04-15 20:42:35.000000 mixture-of-depth-1.1.5/MoD/MoD.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)       83 2024-04-12 14:14:41.000000 mixture-of-depth-1.1.5/MoD/__init__.py
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-15 20:42:58.761328 mixture-of-depth-1.1.5/MoD/modeling/
+-rw-rw-r--   0 marco     (1000) marco     (1000)       49 2024-04-12 13:59:17.000000 mixture-of-depth-1.1.5/MoD/modeling/__init__.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)     1556 2024-04-12 16:22:14.000000 mixture-of-depth-1.1.5/MoD/modeling/automodeling.py
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-15 20:42:58.765328 mixture-of-depth-1.1.5/MoD/modeling/models/
+-rw-rw-r--   0 marco     (1000) marco     (1000)    55049 2024-04-13 10:23:41.000000 mixture-of-depth-1.1.5/MoD/modeling/models/BloomMoD.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)    75771 2024-04-13 11:04:53.000000 mixture-of-depth-1.1.5/MoD/modeling/models/FalconMoD.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)    63538 2024-04-13 10:23:41.000000 mixture-of-depth-1.1.5/MoD/modeling/models/GemmaMoD.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)    72912 2024-04-13 10:23:41.000000 mixture-of-depth-1.1.5/MoD/modeling/models/LlamaMoD.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)    63678 2024-04-13 10:23:41.000000 mixture-of-depth-1.1.5/MoD/modeling/models/MistralMoD.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)    73861 2024-04-13 10:23:41.000000 mixture-of-depth-1.1.5/MoD/modeling/models/MixtralMoD.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)    68490 2024-04-13 11:05:11.000000 mixture-of-depth-1.1.5/MoD/modeling/models/PhiMoD.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)    64007 2024-04-13 10:30:29.000000 mixture-of-depth-1.1.5/MoD/modeling/models/QwenMoD.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)    73663 2024-04-13 11:06:21.000000 mixture-of-depth-1.1.5/MoD/modeling/models/QwenMoEMoD.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)    64125 2024-04-13 10:47:31.000000 mixture-of-depth-1.1.5/MoD/modeling/models/StarCoderMoD.py
+-rw-rw-r--   0 marco     (1000) marco     (1000)      439 2024-04-13 10:53:25.000000 mixture-of-depth-1.1.5/MoD/modeling/models/__init__.py
+-rw-r--r--   0 marco     (1000) marco     (1000)     2978 2024-04-15 20:42:58.765328 mixture-of-depth-1.1.5/PKG-INFO
+-rw-rw-r--   0 marco     (1000) marco     (1000)     2415 2024-04-13 10:55:20.000000 mixture-of-depth-1.1.5/README.md
+drwxrwxr-x   0 marco     (1000) marco     (1000)        0 2024-04-15 20:42:58.765328 mixture-of-depth-1.1.5/mixture_of_depth.egg-info/
+-rw-r--r--   0 marco     (1000) marco     (1000)     2978 2024-04-15 20:42:58.000000 mixture-of-depth-1.1.5/mixture_of_depth.egg-info/PKG-INFO
+-rw-rw-r--   0 marco     (1000) marco     (1000)      658 2024-04-15 20:42:58.000000 mixture-of-depth-1.1.5/mixture_of_depth.egg-info/SOURCES.txt
+-rw-rw-r--   0 marco     (1000) marco     (1000)        1 2024-04-15 20:42:58.000000 mixture-of-depth-1.1.5/mixture_of_depth.egg-info/dependency_links.txt
+-rw-rw-r--   0 marco     (1000) marco     (1000)        6 2024-04-15 20:42:58.000000 mixture-of-depth-1.1.5/mixture_of_depth.egg-info/requires.txt
+-rw-rw-r--   0 marco     (1000) marco     (1000)        4 2024-04-15 20:42:58.000000 mixture-of-depth-1.1.5/mixture_of_depth.egg-info/top_level.txt
+-rw-rw-r--   0 marco     (1000) marco     (1000)       38 2024-04-15 20:42:58.765328 mixture-of-depth-1.1.5/setup.cfg
+-rw-rw-r--   0 marco     (1000) marco     (1000)      769 2024-04-15 20:42:56.000000 mixture-of-depth-1.1.5/setup.py
```

### Comparing `mixture-of-depth-1.1.4/MoD/MoD.py` & `mixture-of-depth-1.1.5/MoD/MoD.py`

 * *Files 0% similar despite different names*

```diff
@@ -46,23 +46,26 @@
 
         k = int(self.capacity * s)
         top_k_values, _ = torch.topk(weights, k, dim=1, sorted=True)
         threshold = top_k_values[:, -1]
         selected_mask = weights > threshold.unsqueeze(-1)
 
         processed_tokens = torch.zeros_like(x)
+        cache = None
+
         for i in range(b):
             current_selected_mask = selected_mask[i]
             selected_tokens = x[i][current_selected_mask]
             selected_position_ids = position_ids[i][current_selected_mask].unsqueeze(0)
             if attention_mask is not None:
                 current_causal_mask = attention_mask[i, 0]
                 current_causal_mask = current_causal_mask[current_selected_mask][:, current_selected_mask].unsqueeze(0).unsqueeze(0) #first if for the one second is for the bs
             else:
                 current_causal_mask = None
+
             if selected_tokens.size(0) > 0:
                 # Dynamic cache management
                 if cache_position is not None:
                     selected_cache_position = cache_position[selected_mask[i]]
                     block_output = self.block(
                         selected_tokens.unsqueeze(0),
                         attention_mask=current_causal_mask,
@@ -73,29 +76,29 @@
                         cache_position=selected_cache_position,
                         **kwargs
                     )
                     if len(block_output) == 2:
                         processed_tokens[i][selected_mask[i]], cache = block_output
                     else:
                         processed_tokens[i][selected_mask[i]] = block_output[0]
-                        cache = None
+
                     processed_tokens[i][selected_mask[i]] = processed_tokens[i][selected_mask[i]] * weights[i][selected_mask[i]].unsqueeze(-1)
                 else:
                     processed_tokens[i][selected_mask[i]] = self.block(
                         selected_tokens.unsqueeze(0),
                         attention_mask=current_causal_mask,
                         position_ids=selected_position_ids,
                         past_key_value=past_key_value,
                         output_attentions=output_attentions,
                         use_cache=use_cache,
                         **kwargs
                     )[0] * weights[i][selected_mask[i]].unsqueeze(-1)
 
         output = processed_tokens + (x * (~selected_mask).unsqueeze(-1).to(x.dtype))
-        return (output,cache) if cache is not None else (output,)
+        return (output, cache) if cache is not None else (output,)
 
 
 def apply_mod_to_hf(model: PreTrainedModel, enabled: bool = True) -> PreTrainedModel:
     if not enabled:
         return model
 
     new_layers = nn.ModuleList()
```

### Comparing `mixture-of-depth-1.1.4/MoD/modeling/automodeling.py` & `mixture-of-depth-1.1.5/MoD/modeling/automodeling.py`

 * *Files identical despite different names*

### Comparing `mixture-of-depth-1.1.4/MoD/modeling/models/BloomMoD.py` & `mixture-of-depth-1.1.5/MoD/modeling/models/BloomMoD.py`

 * *Files identical despite different names*

### Comparing `mixture-of-depth-1.1.4/MoD/modeling/models/FalconMoD.py` & `mixture-of-depth-1.1.5/MoD/modeling/models/FalconMoD.py`

 * *Files identical despite different names*

### Comparing `mixture-of-depth-1.1.4/MoD/modeling/models/GemmaMoD.py` & `mixture-of-depth-1.1.5/MoD/modeling/models/GemmaMoD.py`

 * *Files identical despite different names*

### Comparing `mixture-of-depth-1.1.4/MoD/modeling/models/LlamaMoD.py` & `mixture-of-depth-1.1.5/MoD/modeling/models/LlamaMoD.py`

 * *Files identical despite different names*

### Comparing `mixture-of-depth-1.1.4/MoD/modeling/models/MistralMoD.py` & `mixture-of-depth-1.1.5/MoD/modeling/models/MistralMoD.py`

 * *Files identical despite different names*

### Comparing `mixture-of-depth-1.1.4/MoD/modeling/models/MixtralMoD.py` & `mixture-of-depth-1.1.5/MoD/modeling/models/MixtralMoD.py`

 * *Files identical despite different names*

### Comparing `mixture-of-depth-1.1.4/MoD/modeling/models/PhiMoD.py` & `mixture-of-depth-1.1.5/MoD/modeling/models/PhiMoD.py`

 * *Files identical despite different names*

### Comparing `mixture-of-depth-1.1.4/MoD/modeling/models/QwenMoD.py` & `mixture-of-depth-1.1.5/MoD/modeling/models/QwenMoD.py`

 * *Files identical despite different names*

### Comparing `mixture-of-depth-1.1.4/MoD/modeling/models/QwenMoEMoD.py` & `mixture-of-depth-1.1.5/MoD/modeling/models/QwenMoEMoD.py`

 * *Files identical despite different names*

### Comparing `mixture-of-depth-1.1.4/MoD/modeling/models/StarCoderMoD.py` & `mixture-of-depth-1.1.5/MoD/modeling/models/StarCoderMoD.py`

 * *Files identical despite different names*

### Comparing `mixture-of-depth-1.1.4/PKG-INFO` & `mixture-of-depth-1.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mixture-of-depth
-Version: 1.1.4
+Version: 1.1.5
 Summary: Unofficial implementation for the paper "Mixture-of-Depths: Dynamically allocating compute in transformer-based language models"
 Home-page: https://github.com/astramind-ai/Mixture-of-depths
 Author: Marco Lironi
 Author-email: marcolironi@astramind.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `mixture-of-depth-1.1.4/README.md` & `mixture-of-depth-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `mixture-of-depth-1.1.4/mixture_of_depth.egg-info/PKG-INFO` & `mixture-of-depth-1.1.5/mixture_of_depth.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mixture-of-depth
-Version: 1.1.4
+Version: 1.1.5
 Summary: Unofficial implementation for the paper "Mixture-of-Depths: Dynamically allocating compute in transformer-based language models"
 Home-page: https://github.com/astramind-ai/Mixture-of-depths
 Author: Marco Lironi
 Author-email: marcolironi@astramind.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `mixture-of-depth-1.1.4/mixture_of_depth.egg-info/SOURCES.txt` & `mixture-of-depth-1.1.5/mixture_of_depth.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mixture-of-depth-1.1.4/setup.py` & `mixture-of-depth-1.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='mixture-of-depth',
-    version='1.1.4',
+    version='1.1.5',
     author='Marco Lironi',
     author_email='marcolironi@astramind.ai',
     description='Unofficial implementation for the paper "Mixture-of-Depths: Dynamically allocating compute in transformer-based language models"',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/astramind-ai/Mixture-of-depths',
     packages=find_packages(),
```

