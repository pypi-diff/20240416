# Comparing `tmp/bitmat_tl-0.3.4.tar.gz` & `tmp/bitmat_tl-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bitmat_tl-0.3.4.tar", last modified: Mon Apr 15 11:13:08 2024, max compression
+gzip compressed data, was "bitmat_tl-0.3.5.tar", last modified: Tue Apr 16 14:53:18 2024, max compression
```

## Comparing `bitmat_tl-0.3.4.tar` & `bitmat_tl-0.3.5.tar`

### file list

```diff
@@ -1,41 +1,36 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:13:08.452710 bitmat_tl-0.3.4/
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-15 11:12:59.000000 bitmat_tl-0.3.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4879 2024-04-15 11:13:08.452710 bitmat_tl-0.3.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4247 2024-04-15 11:12:59.000000 bitmat_tl-0.3.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:13:08.444710 bitmat_tl-0.3.4/bitmat/
--rw-r--r--   0 runner    (1001) docker     (127)      489 2024-04-15 11:12:59.000000 bitmat_tl-0.3.4/bitmat/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3594 2024-04-15 11:12:59.000000 bitmat_tl-0.3.4/bitmat/bitlinear.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:13:08.448710 bitmat_tl-0.3.4/bitmat/triton_kernels/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 11:12:59.000000 bitmat_tl-0.3.4/bitmat/triton_kernels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5641 2024-04-15 11:12:59.000000 bitmat_tl-0.3.4/bitmat/triton_kernels/bitmat_kernel.py
--rw-r--r--   0 runner    (1001) docker     (127)     5241 2024-04-15 11:12:59.000000 bitmat_tl-0.3.4/bitmat/triton_kernels/rmsnorm_kernel.py
--rw-r--r--   0 runner    (1001) docker     (127)     7037 2024-04-15 11:12:59.000000 bitmat_tl-0.3.4/bitmat/triton_kernels/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:13:08.448710 bitmat_tl-0.3.4/bitmat/utils/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 11:12:59.000000 bitmat_tl-0.3.4/bitmat/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-04-15 11:12:59.000000 bitmat_tl-0.3.4/bitmat/utils/bitmat.py
--rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-04-15 11:12:59.000000 bitmat_tl-0.3.4/bitmat/utils/convert_hf_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     7547 2024-04-15 11:12:59.000000 bitmat_tl-0.3.4/bitmat/utils/custom_autotune.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:13:08.448710 bitmat_tl-0.3.4/bitmat/utils/model_hijacks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 11:12:59.000000 bitmat_tl-0.3.4/bitmat/utils/model_hijacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    61141 2024-04-15 11:12:59.000000 bitmat_tl-0.3.4/bitmat/utils/model_hijacks/gemma_1_58b.py
--rw-r--r--   0 runner    (1001) docker     (127)    73359 2024-04-15 11:12:59.000000 bitmat_tl-0.3.4/bitmat/utils/model_hijacks/llama_1_58b.py
--rw-r--r--   0 runner    (1001) docker     (127)    64378 2024-04-15 11:12:59.000000 bitmat_tl-0.3.4/bitmat/utils/model_hijacks/mistral_1_58b.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:13:08.448710 bitmat_tl-0.3.4/bitmat/utils/modeling/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-15 11:12:59.000000 bitmat_tl-0.3.4/bitmat/utils/modeling/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-04-15 11:12:59.000000 bitmat_tl-0.3.4/bitmat/utils/modeling/automodel.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:13:08.448710 bitmat_tl-0.3.4/bitmat/utils/modeling/model_hijacks/
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-15 11:12:59.000000 bitmat_tl-0.3.4/bitmat/utils/modeling/model_hijacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    61145 2024-04-15 11:12:59.000000 bitmat_tl-0.3.4/bitmat/utils/modeling/model_hijacks/gemma_1_58b.py
--rw-r--r--   0 runner    (1001) docker     (127)    73363 2024-04-15 11:12:59.000000 bitmat_tl-0.3.4/bitmat/utils/modeling/model_hijacks/llama_1_58b.py
--rw-r--r--   0 runner    (1001) docker     (127)    64382 2024-04-15 11:12:59.000000 bitmat_tl-0.3.4/bitmat/utils/modeling/model_hijacks/mistral_1_58b.py
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-15 11:12:59.000000 bitmat_tl-0.3.4/bitmat/utils/pack_model_before_save.py
--rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-04-15 11:12:59.000000 bitmat_tl-0.3.4/bitmat/utils/packing.py
--rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-15 11:12:59.000000 bitmat_tl-0.3.4/bitmat/utils/rmsnorm.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 11:13:08.452710 bitmat_tl-0.3.4/bitmat_tl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4879 2024-04-15 11:13:08.000000 bitmat_tl-0.3.4/bitmat_tl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1012 2024-04-15 11:13:08.000000 bitmat_tl-0.3.4/bitmat_tl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 11:13:08.000000 bitmat_tl-0.3.4/bitmat_tl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-15 11:13:08.000000 bitmat_tl-0.3.4/bitmat_tl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-15 11:13:08.000000 bitmat_tl-0.3.4/bitmat_tl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 11:13:08.452710 bitmat_tl-0.3.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-15 11:13:08.000000 bitmat_tl-0.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:53:18.997576 bitmat_tl-0.3.5/
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-16 14:53:08.000000 bitmat_tl-0.3.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5035 2024-04-16 14:53:18.997576 bitmat_tl-0.3.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4403 2024-04-16 14:53:08.000000 bitmat_tl-0.3.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:53:18.993576 bitmat_tl-0.3.5/bitmat/
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-16 14:53:08.000000 bitmat_tl-0.3.5/bitmat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3594 2024-04-16 14:53:08.000000 bitmat_tl-0.3.5/bitmat/bitlinear.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:53:18.993576 bitmat_tl-0.3.5/bitmat/triton_kernels/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 14:53:08.000000 bitmat_tl-0.3.5/bitmat/triton_kernels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5641 2024-04-16 14:53:08.000000 bitmat_tl-0.3.5/bitmat/triton_kernels/bitmat_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5241 2024-04-16 14:53:08.000000 bitmat_tl-0.3.5/bitmat/triton_kernels/rmsnorm_kernel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7037 2024-04-16 14:53:08.000000 bitmat_tl-0.3.5/bitmat/triton_kernels/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:53:18.993576 bitmat_tl-0.3.5/bitmat/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 14:53:08.000000 bitmat_tl-0.3.5/bitmat/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-04-16 14:53:08.000000 bitmat_tl-0.3.5/bitmat/utils/bitmat.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2978 2024-04-16 14:53:08.000000 bitmat_tl-0.3.5/bitmat/utils/convert_hf_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7547 2024-04-16 14:53:08.000000 bitmat_tl-0.3.5/bitmat/utils/custom_autotune.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:53:18.993576 bitmat_tl-0.3.5/bitmat/utils/modeling/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-04-16 14:53:08.000000 bitmat_tl-0.3.5/bitmat/utils/modeling/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1740 2024-04-16 14:53:08.000000 bitmat_tl-0.3.5/bitmat/utils/modeling/automodel.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:53:18.993576 bitmat_tl-0.3.5/bitmat/utils/modeling/model_hijacks/
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-16 14:53:08.000000 bitmat_tl-0.3.5/bitmat/utils/modeling/model_hijacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    61145 2024-04-16 14:53:08.000000 bitmat_tl-0.3.5/bitmat/utils/modeling/model_hijacks/gemma_1_58b.py
+-rw-r--r--   0 runner    (1001) docker     (127)    73363 2024-04-16 14:53:08.000000 bitmat_tl-0.3.5/bitmat/utils/modeling/model_hijacks/llama_1_58b.py
+-rw-r--r--   0 runner    (1001) docker     (127)    64382 2024-04-16 14:53:08.000000 bitmat_tl-0.3.5/bitmat/utils/modeling/model_hijacks/mistral_1_58b.py
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-16 14:53:08.000000 bitmat_tl-0.3.5/bitmat/utils/pack_model_before_save.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2106 2024-04-16 14:53:08.000000 bitmat_tl-0.3.5/bitmat/utils/packing.py
+-rw-r--r--   0 runner    (1001) docker     (127)      384 2024-04-16 14:53:08.000000 bitmat_tl-0.3.5/bitmat/utils/rmsnorm.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:53:18.997576 bitmat_tl-0.3.5/bitmat_tl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5035 2024-04-16 14:53:18.000000 bitmat_tl-0.3.5/bitmat_tl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-04-16 14:53:18.000000 bitmat_tl-0.3.5/bitmat_tl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 14:53:18.000000 bitmat_tl-0.3.5/bitmat_tl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-16 14:53:18.000000 bitmat_tl-0.3.5/bitmat_tl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-16 14:53:18.000000 bitmat_tl-0.3.5/bitmat_tl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 14:53:18.997576 bitmat_tl-0.3.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      796 2024-04-16 14:53:18.000000 bitmat_tl-0.3.5/setup.py
```

### Comparing `bitmat_tl-0.3.4/LICENSE` & `bitmat_tl-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `bitmat_tl-0.3.4/PKG-INFO` & `bitmat_tl-0.3.5/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bitmat-tl
-Version: 0.3.4
+Version: 0.3.5
 Summary: An efficent implementation for the paper: "The Era of 1-bit LLMs"
 Home-page: https://github.com/astramind-ai/BitMat/tree/main
 Author: Marco Lironi
 Author-email: marcolironi@astramind.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -90,15 +90,15 @@
 It can be observed that the performance of the custom matmul to 
 handle the multiplication of ternary matrices is better for higher precision. 
 This may be due to the optimized process within the GPU.
 
 
 **(left) 16-bit precision, (right) 32-bit precision**
 
-<img src="img/fp16.png" width="300" alt="Local Image"> <img src="img/fp32.png" width="300" alt="Local Image">
+ <img src="https://github.com/astramind-ai/BitMat/assets/121761685/5f768ce3-c947-4be6-82f0-5346f78d6645)" width="400" alt="Graph #1"> <img src="https://github.com/astramind-ai/BitMat/assets/121761685/5f768ce3-c947-4be6-82f0-5346f78d6645" width="400" alt="Graph #2">
 
 
 ## 🫱🏼‍🫲🏽 Contributing
 We welcome contributions from the community, whether it's adding new features, improving documentation, or reporting bugs. Please refer to our contribution guidelines before making a pull request.
 
 ## 📜 License
 BitMat is open-sourced under the Apache-2.0 license.
```

### Comparing `bitmat_tl-0.3.4/README.md` & `bitmat_tl-0.3.5/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -70,15 +70,15 @@
 It can be observed that the performance of the custom matmul to 
 handle the multiplication of ternary matrices is better for higher precision. 
 This may be due to the optimized process within the GPU.
 
 
 **(left) 16-bit precision, (right) 32-bit precision**
 
-<img src="img/fp16.png" width="300" alt="Local Image"> <img src="img/fp32.png" width="300" alt="Local Image">
+ <img src="https://github.com/astramind-ai/BitMat/assets/121761685/5f768ce3-c947-4be6-82f0-5346f78d6645)" width="400" alt="Graph #1"> <img src="https://github.com/astramind-ai/BitMat/assets/121761685/5f768ce3-c947-4be6-82f0-5346f78d6645" width="400" alt="Graph #2">
 
 
 ## 🫱🏼‍🫲🏽 Contributing
 We welcome contributions from the community, whether it's adding new features, improving documentation, or reporting bugs. Please refer to our contribution guidelines before making a pull request.
 
 ## 📜 License
 BitMat is open-sourced under the Apache-2.0 license.
```

### Comparing `bitmat_tl-0.3.4/bitmat/bitlinear.py` & `bitmat_tl-0.3.5/bitmat/bitlinear.py`

 * *Files identical despite different names*

### Comparing `bitmat_tl-0.3.4/bitmat/triton_kernels/bitmat_kernel.py` & `bitmat_tl-0.3.5/bitmat/triton_kernels/bitmat_kernel.py`

 * *Files identical despite different names*

### Comparing `bitmat_tl-0.3.4/bitmat/triton_kernels/rmsnorm_kernel.py` & `bitmat_tl-0.3.5/bitmat/triton_kernels/rmsnorm_kernel.py`

 * *Files identical despite different names*

### Comparing `bitmat_tl-0.3.4/bitmat/triton_kernels/utils.py` & `bitmat_tl-0.3.5/bitmat/triton_kernels/utils.py`

 * *Files identical despite different names*

### Comparing `bitmat_tl-0.3.4/bitmat/utils/bitmat.py` & `bitmat_tl-0.3.5/bitmat/utils/bitmat.py`

 * *Files identical despite different names*

### Comparing `bitmat_tl-0.3.4/bitmat/utils/convert_hf_model.py` & `bitmat_tl-0.3.5/bitmat/utils/convert_hf_model.py`

 * *Files identical despite different names*

### Comparing `bitmat_tl-0.3.4/bitmat/utils/custom_autotune.py` & `bitmat_tl-0.3.5/bitmat/utils/custom_autotune.py`

 * *Files identical despite different names*

### Comparing `bitmat_tl-0.3.4/bitmat/utils/model_hijacks/gemma_1_58b.py` & `bitmat_tl-0.3.5/bitmat/utils/modeling/model_hijacks/gemma_1_58b.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 import torch
 import torch.nn.functional as F
 import torch.utils.checkpoint
 from bitmat.utils.pack_model_before_save import pack_ternary_model
 from transformers import PretrainedConfig
 
-from ...bitlinear import BitLinear
+from bitmat.bitlinear import BitLinear
 from torch import nn
 from torch.nn import BCEWithLogitsLoss, CrossEntropyLoss, MSELoss
 
 from transformers.activations import ACT2FN
 from transformers.cache_utils import Cache, DynamicCache, StaticCache
 from transformers.modeling_attn_mask_utils import (
     _prepare_4d_causal_attention_mask,
```

### Comparing `bitmat_tl-0.3.4/bitmat/utils/model_hijacks/llama_1_58b.py` & `bitmat_tl-0.3.5/bitmat/utils/modeling/model_hijacks/llama_1_58b.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 import os
 import warnings
 from typing import List, Optional, Tuple, Union, Callable
 
 import torch
 import torch.nn.functional as F
 import torch.utils.checkpoint
-from ...bitlinear import BitLinear
+from bitmat.bitlinear import BitLinear
 from bitmat.utils.pack_model_before_save import pack_ternary_model
 from torch import nn
 from torch.nn import BCEWithLogitsLoss, CrossEntropyLoss, MSELoss
 
 from transformers.activations import ACT2FN
 from transformers.cache_utils import Cache, DynamicCache, StaticCache
 from transformers.modeling_attn_mask_utils import AttentionMaskConverter
```

### Comparing `bitmat_tl-0.3.4/bitmat/utils/model_hijacks/mistral_1_58b.py` & `bitmat_tl-0.3.5/bitmat/utils/modeling/model_hijacks/mistral_1_58b.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 import os
 import warnings
 from typing import List, Optional, Tuple, Union, Callable
 
 import torch
 import torch.nn.functional as F
 import torch.utils.checkpoint
-from ...bitlinear import BitLinear
+from bitmat.bitlinear import BitLinear
 from bitmat.utils.pack_model_before_save import pack_ternary_model
 from torch import nn
 from torch.nn import BCEWithLogitsLoss, CrossEntropyLoss, MSELoss
 
 from transformers.activations import ACT2FN
 from transformers.cache_utils import Cache, DynamicCache
 from transformers.modeling_attn_mask_utils import _prepare_4d_causal_attention_mask, \
```

### Comparing `bitmat_tl-0.3.4/bitmat/utils/modeling/automodel.py` & `bitmat_tl-0.3.5/bitmat/utils/modeling/automodel.py`

 * *Files identical despite different names*

### Comparing `bitmat_tl-0.3.4/bitmat/utils/packing.py` & `bitmat_tl-0.3.5/bitmat/utils/packing.py`

 * *Files identical despite different names*

### Comparing `bitmat_tl-0.3.4/bitmat_tl.egg-info/PKG-INFO` & `bitmat_tl-0.3.5/bitmat_tl.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bitmat-tl
-Version: 0.3.4
+Version: 0.3.5
 Summary: An efficent implementation for the paper: "The Era of 1-bit LLMs"
 Home-page: https://github.com/astramind-ai/BitMat/tree/main
 Author: Marco Lironi
 Author-email: marcolironi@astramind.ai
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -90,15 +90,15 @@
 It can be observed that the performance of the custom matmul to 
 handle the multiplication of ternary matrices is better for higher precision. 
 This may be due to the optimized process within the GPU.
 
 
 **(left) 16-bit precision, (right) 32-bit precision**
 
-<img src="img/fp16.png" width="300" alt="Local Image"> <img src="img/fp32.png" width="300" alt="Local Image">
+ <img src="https://github.com/astramind-ai/BitMat/assets/121761685/5f768ce3-c947-4be6-82f0-5346f78d6645)" width="400" alt="Graph #1"> <img src="https://github.com/astramind-ai/BitMat/assets/121761685/5f768ce3-c947-4be6-82f0-5346f78d6645" width="400" alt="Graph #2">
 
 
 ## 🫱🏼‍🫲🏽 Contributing
 We welcome contributions from the community, whether it's adding new features, improving documentation, or reporting bugs. Please refer to our contribution guidelines before making a pull request.
 
 ## 📜 License
 BitMat is open-sourced under the Apache-2.0 license.
```

### Comparing `bitmat_tl-0.3.4/bitmat_tl.egg-info/SOURCES.txt` & `bitmat_tl-0.3.5/bitmat_tl.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -10,18 +10,14 @@
 bitmat/utils/__init__.py
 bitmat/utils/bitmat.py
 bitmat/utils/convert_hf_model.py
 bitmat/utils/custom_autotune.py
 bitmat/utils/pack_model_before_save.py
 bitmat/utils/packing.py
 bitmat/utils/rmsnorm.py
-bitmat/utils/model_hijacks/__init__.py
-bitmat/utils/model_hijacks/gemma_1_58b.py
-bitmat/utils/model_hijacks/llama_1_58b.py
-bitmat/utils/model_hijacks/mistral_1_58b.py
 bitmat/utils/modeling/__init__.py
 bitmat/utils/modeling/automodel.py
 bitmat/utils/modeling/model_hijacks/__init__.py
 bitmat/utils/modeling/model_hijacks/gemma_1_58b.py
 bitmat/utils/modeling/model_hijacks/llama_1_58b.py
 bitmat/utils/modeling/model_hijacks/mistral_1_58b.py
 bitmat_tl.egg-info/PKG-INFO
```

### Comparing `bitmat_tl-0.3.4/setup.py` & `bitmat_tl-0.3.5/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='bitmat-tl',
-    version='0.3.4',
+    version='0.3.5',
     author='Marco Lironi',
     author_email='marcolironi@astramind.ai',
     description='An efficent implementation for the paper: "The Era of 1-bit LLMs"',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/astramind-ai/BitMat/tree/main',
     packages=find_packages(),
```

