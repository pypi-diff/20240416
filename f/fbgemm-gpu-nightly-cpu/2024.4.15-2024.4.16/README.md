# Comparing `tmp/fbgemm_gpu_nightly_cpu-2024.4.15-cp39-cp39-manylinux2014_x86_64.whl.zip` & `tmp/fbgemm_gpu_nightly_cpu-2024.4.16-cp38-cp38-manylinux2014_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,57 +1,57 @@
-Zip file size: 3099140 bytes, number of entries: 55
--rw-r--r--  2.0 unx      914 b- defN 24-Apr-15 12:59 fbgemm_gpu/__init__.py
--rw-r--r--  2.0 unx     3079 b- defN 24-Apr-15 12:59 fbgemm_gpu/batched_unary_embeddings_ops.py
--rw-r--r--  2.0 unx      789 b- defN 24-Apr-15 12:59 fbgemm_gpu/enums.py
--rwxr-xr-x  2.0 unx 10617336 b- defN 24-Apr-15 12:59 fbgemm_gpu/fbgemm_gpu_py.so
--rw-r--r--  2.0 unx     5663 b- defN 24-Apr-15 12:59 fbgemm_gpu/metrics.py
--rw-r--r--  2.0 unx     2362 b- defN 24-Apr-15 12:59 fbgemm_gpu/permute_pooled_embedding_modules.py
--rw-r--r--  2.0 unx     2752 b- defN 24-Apr-15 12:59 fbgemm_gpu/permute_pooled_embedding_modules_split.py
--rw-r--r--  2.0 unx     7885 b- defN 24-Apr-15 12:59 fbgemm_gpu/quantize_comm.py
--rw-r--r--  2.0 unx     4143 b- defN 24-Apr-15 12:59 fbgemm_gpu/quantize_utils.py
--rw-r--r--  2.0 unx     6947 b- defN 24-Apr-15 12:59 fbgemm_gpu/runtime_monitor.py
--rw-r--r--  2.0 unx    20396 b- defN 24-Apr-15 12:59 fbgemm_gpu/sparse_ops.py
--rw-r--r--  2.0 unx     5774 b- defN 24-Apr-15 12:59 fbgemm_gpu/split_embedding_configs.py
--rw-r--r--  2.0 unx     7058 b- defN 24-Apr-15 12:59 fbgemm_gpu/split_embedding_inference_converter.py
--rw-r--r--  2.0 unx      540 b- defN 24-Apr-15 12:59 fbgemm_gpu/split_embedding_optimizer_ops.py
--rw-r--r--  2.0 unx    26849 b- defN 24-Apr-15 12:59 fbgemm_gpu/split_embedding_utils.py
--rw-r--r--  2.0 unx     2339 b- defN 24-Apr-15 12:59 fbgemm_gpu/split_table_batched_embeddings_ops.py
--rw-r--r--  2.0 unx     3493 b- defN 24-Apr-15 12:59 fbgemm_gpu/split_table_batched_embeddings_ops_common.py
--rw-r--r--  2.0 unx    66517 b- defN 24-Apr-15 12:59 fbgemm_gpu/split_table_batched_embeddings_ops_inference.py
--rw-r--r--  2.0 unx    96843 b- defN 24-Apr-15 12:59 fbgemm_gpu/split_table_batched_embeddings_ops_training.py
--rw-r--r--  2.0 unx    40680 b- defN 24-Apr-15 12:59 fbgemm_gpu/ssd_split_table_batched_embeddings_ops.py
--rw-r--r--  2.0 unx      925 b- defN 24-Apr-15 12:59 fbgemm_gpu/uvm.py
--rw-r--r--  2.0 unx      383 b- defN 24-Apr-15 12:59 fbgemm_gpu/docs/__init__.py
--rw-r--r--  2.0 unx      273 b- defN 24-Apr-15 12:59 fbgemm_gpu/docs/common.py
--rw-r--r--  2.0 unx     2377 b- defN 24-Apr-15 12:59 fbgemm_gpu/docs/examples.py
--rw-r--r--  2.0 unx     7381 b- defN 24-Apr-15 12:59 fbgemm_gpu/docs/jagged_tensor_ops.py
--rw-r--r--  2.0 unx     7708 b- defN 24-Apr-15 12:59 fbgemm_gpu/docs/table_batched_embedding_ops.py
--rw-r--r--  2.0 unx      264 b- defN 24-Apr-15 12:59 fbgemm_gpu/docs/version.py
--rw-r--r--  2.0 unx     1466 b- defN 24-Apr-15 12:58 fbgemm_gpu/split_embedding_codegen_lookup_invokers/__init__.py
--rw-r--r--  2.0 unx     4180 b- defN 24-Apr-15 12:58 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adagrad.py
--rw-r--r--  2.0 unx     4180 b- defN 24-Apr-15 12:58 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adagrad_pt2.py
--rw-r--r--  2.0 unx     3395 b- defN 24-Apr-15 12:58 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adam.py
--rw-r--r--  2.0 unx     3395 b- defN 24-Apr-15 12:58 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adam_pt2.py
--rw-r--r--  2.0 unx     2147 b- defN 24-Apr-15 12:58 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_args.py
--rw-r--r--  2.0 unx     3395 b- defN 24-Apr-15 12:58 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_lamb.py
--rw-r--r--  2.0 unx     3395 b- defN 24-Apr-15 12:58 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_lamb_pt2.py
--rw-r--r--  2.0 unx     3144 b- defN 24-Apr-15 12:58 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_lars_sgd.py
--rw-r--r--  2.0 unx     3144 b- defN 24-Apr-15 12:58 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_lars_sgd_pt2.py
--rw-r--r--  2.0 unx     2420 b- defN 24-Apr-15 12:58 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_none.py
--rw-r--r--  2.0 unx     2420 b- defN 24-Apr-15 12:58 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_none_pt2.py
--rw-r--r--  2.0 unx     3100 b- defN 24-Apr-15 12:58 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_adam.py
--rw-r--r--  2.0 unx     3100 b- defN 24-Apr-15 12:58 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_adam_pt2.py
--rw-r--r--  2.0 unx     3100 b- defN 24-Apr-15 12:58 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_lamb.py
--rw-r--r--  2.0 unx     3100 b- defN 24-Apr-15 12:58 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_lamb_pt2.py
--rw-r--r--  2.0 unx     4512 b- defN 24-Apr-15 12:58 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad.py
--rw-r--r--  2.0 unx     4512 b- defN 24-Apr-15 12:58 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_pt2.py
--rw-r--r--  2.0 unx     3964 b- defN 24-Apr-15 12:58 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_with_counter.py
--rw-r--r--  2.0 unx     3964 b- defN 24-Apr-15 12:58 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_with_counter_pt2.py
--rw-r--r--  2.0 unx     3762 b- defN 24-Apr-15 12:58 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_sgd.py
--rw-r--r--  2.0 unx     3762 b- defN 24-Apr-15 12:58 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_sgd_pt2.py
--rw-r--r--  2.0 unx      649 b- defN 24-Apr-15 12:58 fbgemm_gpu/split_embedding_optimizer_codegen/optimizer_args.py
--rw-r--r--  2.0 unx     6162 b- defN 24-Apr-15 12:58 fbgemm_gpu/split_embedding_optimizer_codegen/split_embedding_optimizer_rowwise_adagrad.py
--rw-r--r--  2.0 unx     2602 b- defN 24-Apr-15 13:00 fbgemm_gpu_nightly_cpu-2024.4.15.dist-info/METADATA
--rw-r--r--  2.0 unx      105 b- defN 24-Apr-15 13:00 fbgemm_gpu_nightly_cpu-2024.4.15.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 24-Apr-15 13:00 fbgemm_gpu_nightly_cpu-2024.4.15.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     6022 b- defN 24-Apr-15 13:00 fbgemm_gpu_nightly_cpu-2024.4.15.dist-info/RECORD
-55 files, 11030778 bytes uncompressed, 3089052 bytes compressed:  72.0%
+Zip file size: 3099151 bytes, number of entries: 55
+-rw-r--r--  2.0 unx      914 b- defN 24-Apr-16 12:57 fbgemm_gpu/__init__.py
+-rw-r--r--  2.0 unx     3079 b- defN 24-Apr-16 12:57 fbgemm_gpu/batched_unary_embeddings_ops.py
+-rw-r--r--  2.0 unx      789 b- defN 24-Apr-16 12:57 fbgemm_gpu/enums.py
+-rwxr-xr-x  2.0 unx 10617336 b- defN 24-Apr-16 12:57 fbgemm_gpu/fbgemm_gpu_py.so
+-rw-r--r--  2.0 unx     5663 b- defN 24-Apr-16 12:57 fbgemm_gpu/metrics.py
+-rw-r--r--  2.0 unx     2362 b- defN 24-Apr-16 12:57 fbgemm_gpu/permute_pooled_embedding_modules.py
+-rw-r--r--  2.0 unx     2752 b- defN 24-Apr-16 12:57 fbgemm_gpu/permute_pooled_embedding_modules_split.py
+-rw-r--r--  2.0 unx     7885 b- defN 24-Apr-16 12:57 fbgemm_gpu/quantize_comm.py
+-rw-r--r--  2.0 unx     4143 b- defN 24-Apr-16 12:57 fbgemm_gpu/quantize_utils.py
+-rw-r--r--  2.0 unx     6947 b- defN 24-Apr-16 12:57 fbgemm_gpu/runtime_monitor.py
+-rw-r--r--  2.0 unx    20503 b- defN 24-Apr-16 12:57 fbgemm_gpu/sparse_ops.py
+-rw-r--r--  2.0 unx     5774 b- defN 24-Apr-16 12:57 fbgemm_gpu/split_embedding_configs.py
+-rw-r--r--  2.0 unx     7058 b- defN 24-Apr-16 12:57 fbgemm_gpu/split_embedding_inference_converter.py
+-rw-r--r--  2.0 unx      540 b- defN 24-Apr-16 12:57 fbgemm_gpu/split_embedding_optimizer_ops.py
+-rw-r--r--  2.0 unx    26849 b- defN 24-Apr-16 12:57 fbgemm_gpu/split_embedding_utils.py
+-rw-r--r--  2.0 unx     2339 b- defN 24-Apr-16 12:57 fbgemm_gpu/split_table_batched_embeddings_ops.py
+-rw-r--r--  2.0 unx     3493 b- defN 24-Apr-16 12:57 fbgemm_gpu/split_table_batched_embeddings_ops_common.py
+-rw-r--r--  2.0 unx    66517 b- defN 24-Apr-16 12:57 fbgemm_gpu/split_table_batched_embeddings_ops_inference.py
+-rw-r--r--  2.0 unx    96843 b- defN 24-Apr-16 12:57 fbgemm_gpu/split_table_batched_embeddings_ops_training.py
+-rw-r--r--  2.0 unx    40680 b- defN 24-Apr-16 12:57 fbgemm_gpu/ssd_split_table_batched_embeddings_ops.py
+-rw-r--r--  2.0 unx      925 b- defN 24-Apr-16 12:57 fbgemm_gpu/uvm.py
+-rw-r--r--  2.0 unx      383 b- defN 24-Apr-16 12:57 fbgemm_gpu/docs/__init__.py
+-rw-r--r--  2.0 unx      273 b- defN 24-Apr-16 12:57 fbgemm_gpu/docs/common.py
+-rw-r--r--  2.0 unx     2377 b- defN 24-Apr-16 12:57 fbgemm_gpu/docs/examples.py
+-rw-r--r--  2.0 unx     7381 b- defN 24-Apr-16 12:57 fbgemm_gpu/docs/jagged_tensor_ops.py
+-rw-r--r--  2.0 unx     7708 b- defN 24-Apr-16 12:57 fbgemm_gpu/docs/table_batched_embedding_ops.py
+-rw-r--r--  2.0 unx      264 b- defN 24-Apr-16 12:57 fbgemm_gpu/docs/version.py
+-rw-r--r--  2.0 unx     1466 b- defN 24-Apr-16 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/__init__.py
+-rw-r--r--  2.0 unx     4180 b- defN 24-Apr-16 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adagrad.py
+-rw-r--r--  2.0 unx     4180 b- defN 24-Apr-16 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adagrad_pt2.py
+-rw-r--r--  2.0 unx     3395 b- defN 24-Apr-16 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adam.py
+-rw-r--r--  2.0 unx     3395 b- defN 24-Apr-16 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adam_pt2.py
+-rw-r--r--  2.0 unx     2147 b- defN 24-Apr-16 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_args.py
+-rw-r--r--  2.0 unx     3395 b- defN 24-Apr-16 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_lamb.py
+-rw-r--r--  2.0 unx     3395 b- defN 24-Apr-16 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_lamb_pt2.py
+-rw-r--r--  2.0 unx     3144 b- defN 24-Apr-16 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_lars_sgd.py
+-rw-r--r--  2.0 unx     3144 b- defN 24-Apr-16 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_lars_sgd_pt2.py
+-rw-r--r--  2.0 unx     2420 b- defN 24-Apr-16 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_none.py
+-rw-r--r--  2.0 unx     2420 b- defN 24-Apr-16 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_none_pt2.py
+-rw-r--r--  2.0 unx     3100 b- defN 24-Apr-16 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_adam.py
+-rw-r--r--  2.0 unx     3100 b- defN 24-Apr-16 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_adam_pt2.py
+-rw-r--r--  2.0 unx     3100 b- defN 24-Apr-16 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_lamb.py
+-rw-r--r--  2.0 unx     3100 b- defN 24-Apr-16 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_partial_rowwise_lamb_pt2.py
+-rw-r--r--  2.0 unx     4512 b- defN 24-Apr-16 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad.py
+-rw-r--r--  2.0 unx     4512 b- defN 24-Apr-16 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_pt2.py
+-rw-r--r--  2.0 unx     3964 b- defN 24-Apr-16 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_with_counter.py
+-rw-r--r--  2.0 unx     3964 b- defN 24-Apr-16 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_with_counter_pt2.py
+-rw-r--r--  2.0 unx     3762 b- defN 24-Apr-16 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_sgd.py
+-rw-r--r--  2.0 unx     3762 b- defN 24-Apr-16 12:55 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_sgd_pt2.py
+-rw-r--r--  2.0 unx      649 b- defN 24-Apr-16 12:55 fbgemm_gpu/split_embedding_optimizer_codegen/optimizer_args.py
+-rw-r--r--  2.0 unx     6162 b- defN 24-Apr-16 12:55 fbgemm_gpu/split_embedding_optimizer_codegen/split_embedding_optimizer_rowwise_adagrad.py
+-rw-r--r--  2.0 unx     2602 b- defN 24-Apr-16 12:57 fbgemm_gpu_nightly_cpu-2024.4.16.dist-info/METADATA
+-rw-r--r--  2.0 unx      105 b- defN 24-Apr-16 12:57 fbgemm_gpu_nightly_cpu-2024.4.16.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 24-Apr-16 12:57 fbgemm_gpu_nightly_cpu-2024.4.16.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     6022 b- defN 24-Apr-16 12:57 fbgemm_gpu_nightly_cpu-2024.4.16.dist-info/RECORD
+55 files, 11030885 bytes uncompressed, 3089063 bytes compressed:  72.0%
```

## zipnote {}

```diff
@@ -147,20 +147,20 @@
 
 Filename: fbgemm_gpu/split_embedding_optimizer_codegen/optimizer_args.py
 Comment: 
 
 Filename: fbgemm_gpu/split_embedding_optimizer_codegen/split_embedding_optimizer_rowwise_adagrad.py
 Comment: 
 
-Filename: fbgemm_gpu_nightly_cpu-2024.4.15.dist-info/METADATA
+Filename: fbgemm_gpu_nightly_cpu-2024.4.16.dist-info/METADATA
 Comment: 
 
-Filename: fbgemm_gpu_nightly_cpu-2024.4.15.dist-info/WHEEL
+Filename: fbgemm_gpu_nightly_cpu-2024.4.16.dist-info/WHEEL
 Comment: 
 
-Filename: fbgemm_gpu_nightly_cpu-2024.4.15.dist-info/top_level.txt
+Filename: fbgemm_gpu_nightly_cpu-2024.4.16.dist-info/top_level.txt
 Comment: 
 
-Filename: fbgemm_gpu_nightly_cpu-2024.4.15.dist-info/RECORD
+Filename: fbgemm_gpu_nightly_cpu-2024.4.16.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fbgemm_gpu/fbgemm_gpu_py.so

### strings --all --bytes=8 {}

```diff
@@ -15595,52 +15595,52 @@
 SymFloat
 GenericList
 PyObject
 Uninitialized
 Quantizer
 Generator
 InvalidTag(
-extra_meta_ && extra_meta_->symbolic_shape_meta_ INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/c10/core/TensorImpl.h":1719, please report a bug to PyTorch. 
-/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/c10/core/TensorImpl.h
+extra_meta_ && extra_meta_->symbolic_shape_meta_ INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/c10/core/TensorImpl.h":1719, please report a bug to PyTorch. 
+/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/c10/core/TensorImpl.h
 /__w/FBGEMM/FBGEMM/fbgemm_gpu/codegen/training/forward/embedding_forward_split_cpu.cpp
 Expected !indice_weights.defined() || indice_weights.scalar_type() != at::kHalf to be true, but got false.  (Could this error message be improved?  If so, please report an enhancement request to PyTorch.)
 split_embedding_codegen_forward_cpu_meta
 split_embedding_codegen_forward_cpu(Tensor weights, Tensor weights_offsets, Tensor D_offsets, SymInt total_D, Tensor hash_size_cumsum, Tensor indices, Tensor offsets, int pooling_mode, Tensor indice_weights, int output_dtype) -> Tensor
 Expected weights.is_contiguous() to be true, but got false.  (Could this error message be improved?  If so, please report an enhancement request to PyTorch.)
 split_embedding_forward_cpu_kernel
 split_embedding_grad_indice_weights_cpu_outer
 split_embedding_grad_indice_weights_cpu
 split_embedding_codegen_grad_indice_weights_cpu(Tensor grad_output, Tensor weights, Tensor weights_offsets, Tensor D_offsets, Tensor indices, Tensor offsets, Tensor feature_requires_grad) -> Tensor
 tensor does not have a device
 device_default
 There is an error in the layout calculation logic.
-is_mkldnn() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/c10/core/TensorImpl.h":1290, please report a bug to PyTorch. 
+is_mkldnn() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/c10/core/TensorImpl.h":1290, please report a bug to PyTorch. 
 Operators taking TensorOptions cannot take a TensorOptions with options.requires_grad set as true. This isn't implemented yet.
-/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/CheckMemoryFormat.h
+/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/CheckMemoryFormat.h
 check_tensor_options_and_extract_memory_format
 Cannot set memory_format both in TensorOptions and explicit argument; please delete the redundant setter.
 basic_string::_S_construct null not valid
 basic_string::append
 IntArrayRef contains an int that cannot be represented as a SymInt: 
-/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/c10/core/SymIntArrayRef.h
+/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/c10/core/SymIntArrayRef.h
 fromIntArrayRefSlow
  dims but tensor has 
 TensorAccessor expected 
 accessor
-/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/TensorBase.h
+/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/TensorBase.h
  is out of bounds: 
 , range 
 report_embedding_error
 /__w/FBGEMM/FBGEMM/fbgemm_gpu/include/fbgemm_gpu/cpu_utils.h
 vector::_M_realloc_insert
-isInt() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/ivalue.h":642, please report a bug to PyTorch. 
-/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/ivalue.h
+isInt() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/ivalue.h":642, please report a bug to PyTorch. 
+/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/ivalue.h
 Expected SymInt or int but got 
-isSymInt() || isInt() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/ivalue_inl.h":237, please report a bug to PyTorch. 
-/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/ivalue_inl.h
+isSymInt() || isInt() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/ivalue_inl.h":237, please report a bug to PyTorch. 
+/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/ivalue_inl.h
 toSymInt
 St19bad_optional_access
 N3c1020intrusive_ptr_targetE
 N3c1014OperatorKernelE
 N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorES5_S5_S5_S5_S5_S5_S5_EXadL_Z47split_embedding_codegen_grad_indice_weights_cpuS5_S5_S5_S5_S5_S5_S5_EEEES5_NS_4guts8typelist8typelistIJS5_S5_S5_S5_S5_S5_S5_EEEEE
 FN2at6TensorES0_S0_S0_S0_S0_S0_S0_E
 N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorES5_S5_S5_NS_6SymIntES5_S5_S5_lS5_lEXadL_Z35split_embedding_codegen_forward_cpuS5_S5_S5_S6_S5_S5_S5_lS5_lEEEES5_NS_4guts8typelist8typelistIJS5_S5_S5_S6_S5_S5_S5_lS5_lEEEEE
@@ -15668,133 +15668,133 @@
 TensorQueue
 Expected GenericDict but got 
 toGenericDict
 Unknown Exception Type
  devices
 getDeviceGuardImpl
 PyTorch is not linked with support for 
-/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/c10/core/impl/DeviceGuardImplInterface.h
+/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/c10/core/impl/DeviceGuardImplInterface.h
 Event device type 
  does not match blocking stream's device type 
-/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/c10/core/impl/InlineEvent.h
+/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/c10/core/impl/InlineEvent.h
 Expected !name.empty() to be true, but got false.  (Could this error message be improved?  If so, please report an enhancement request to PyTorch.)
-/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/qualified_name.h
+/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/qualified_name.h
 Invalid name for qualified name: '
-!atom.empty() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/qualified_name.h":24, please report a bug to PyTorch. 
-!finalAtom.empty() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/qualified_name.h":32, please report a bug to PyTorch. 
-/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/c10/util/ArrayRef.h
+!atom.empty() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/qualified_name.h":24, please report a bug to PyTorch. 
+!finalAtom.empty() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/qualified_name.h":32, please report a bug to PyTorch. 
+/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/c10/util/ArrayRef.h
 QualifiedName
 basic_string::substr
 ArrayRef: invalid slice, N = 
 ; size = 
 Expected a 0-dim Tensor, but got Tensor with dimensions: 
-tensor.dim() == 0 INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/torch/csrc/api/include/torch/detail/TensorDataContainer.h":317, please report a bug to PyTorch. 
-/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/torch/csrc/api/include/torch/detail/TensorDataContainer.h
+tensor.dim() == 0 INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/torch/csrc/api/include/torch/detail/TensorDataContainer.h":317, please report a bug to PyTorch. 
+/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/torch/csrc/api/include/torch/detail/TensorDataContainer.h
  in its first dimension, but got Tensor with size 
-tensor.sizes()[0] == (int64_t)init_list_.size() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/torch/csrc/api/include/torch/detail/TensorDataContainer.h":324, please report a bug to PyTorch. 
+tensor.sizes()[0] == (int64_t)init_list_.size() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/torch/csrc/api/include/torch/detail/TensorDataContainer.h":324, please report a bug to PyTorch. 
 TensorDataContainer is already a Tensor type, `fill_tensor` should not be called
-false INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/torch/csrc/api/include/torch/detail/TensorDataContainer.h":338, please report a bug to PyTorch. 
+false INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/torch/csrc/api/include/torch/detail/TensorDataContainer.h":338, please report a bug to PyTorch. 
 Invalid TensorDataContainer type
-false INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/torch/csrc/api/include/torch/detail/TensorDataContainer.h":342, please report a bug to PyTorch. 
+false INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/torch/csrc/api/include/torch/detail/TensorDataContainer.h":342, please report a bug to PyTorch. 
 fill_tensor
 Expected a Tensor with size 
  in its first dimension
 can not do torch::tensor(complex, dtype=non-complex) because complex can not be casted to real number without loss of information
-false INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/torch/csrc/api/include/torch/detail/TensorDataContainer.h":272, please report a bug to PyTorch. 
+false INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/torch/csrc/api/include/torch/detail/TensorDataContainer.h":272, please report a bug to PyTorch. 
 convert_to_tensor
 /__w/FBGEMM/FBGEMM/fbgemm_gpu/codegen/inference/embedding_forward_quantized_host_cpu.cpp
 int_nbit_split_embedding_uvm_caching_codegen_lookup_function shouldn't be called for CPU; it is only for GPU.
-isIntList() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/ivalue_inl.h":1972, please report a bug to PyTorch. 
+isIntList() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/ivalue_inl.h":1972, please report a bug to PyTorch. 
 vector::_M_range_check: __n (which is %zu) >= this->size() (which is %zu)
 __getstate__ should take exactly one argument: self. Got: 
 self argument of __getstate__ must be the custom class type. Got 
 __getstate__ should return exactly one value for serialization. Got: 
 __getstate__'s return type should be a subtype of input argument of __setstate__. Got 
-isString() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/ivalue_inl.h":2362, please report a bug to PyTorch. 
+isString() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/ivalue_inl.h":2362, please report a bug to PyTorch. 
 //deeplearning/fbgemm/fbgemm_gpu:sparse_ops_py
 int_nbit_split_embedding_codegen_lookup_function(Tensor dev_weights, Tensor uvm_weights, Tensor weights_placements, Tensor weights_offsets, Tensor weights_tys, Tensor D_offsets, SymInt total_D, int max_int2_D, int max_int4_D, int max_int8_D, int max_float16_D, int max_float32_D, Tensor indices, Tensor offsets, int pooling_mode, Tensor? indice_weights, int output_dtype=1, Tensor? lxu_cache_weights=None, Tensor? lxu_cache_locations=None, int? row_alignment = None, int? max_float8_D=0, int? fp8_exponent_bits=-1, int? fp8_exponent_bias=-1) -> Tensor
 int_nbit_split_embedding_codegen_lookup_function
 int_nbit_split_embedding_uvm_caching_codegen_lookup_function(Tensor dev_weights, Tensor uvm_weights, Tensor weights_placements, Tensor weights_offsets, Tensor weights_tys, Tensor D_offsets, SymInt total_D, int max_int2_D, int max_int4_D, int max_int8_D, int max_float16_D, int max_float32_D, Tensor indices, Tensor offsets, int pooling_mode, Tensor? indice_weights=None, int output_dtype=1, Tensor? lxu_cache_weights=None, Tensor? lxu_cache_locations=None, int? row_alignment=-1, int? max_float8_D=0, int? fp8_exponent_bits=-1, int? fp8_exponent_bias=-1, Tensor? cache_hash_size_cumsum=None, int? total_cache_hash_size=-1, Tensor? cache_index_table_map=None, Tensor? lxu_cache_state=None, Tensor? lxu_state=None) -> Tensor
 int_nbit_split_embedding_uvm_caching_codegen_lookup_function
 pruned_hashmap_insert(Tensor indices, Tensor dense_indices, Tensor offsets, Tensor(a!) hash_table, Tensor hash_table_offsets) -> ()
 pruned_hashmap_lookup(Tensor indices, Tensor offsets, Tensor hash_table, Tensor hash_table_offsets) -> Tensor
 pruned_array_lookup(Tensor indices, Tensor offsets, Tensor index_remappings, Tensor index_remappings_offsets) -> Tensor
-isGenericDict() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/ivalue_inl.h":2088, please report a bug to PyTorch. 
-self_impl INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/torch/csrc/autograd/variable.h":305, please report a bug to PyTorch. 
-/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/torch/csrc/autograd/variable.h
+isGenericDict() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/ivalue_inl.h":2088, please report a bug to PyTorch. 
+self_impl INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/torch/csrc/autograd/variable.h":305, please report a bug to PyTorch. 
+/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/torch/csrc/autograd/variable.h
 Only Tensors of floating point and complex dtype can require gradients
 AutogradMeta
 set_requires_grad
 Expected T > 0 to be true, but got false.  (Could this error message be improved?  If so, please report an enhancement request to PyTorch.)
 Expected B > 0 to be true, but got false.  (Could this error message be improved?  If so, please report an enhancement request to PyTorch.)
 Expected maps_.size() == T to be true, but got false.  (Could this error message be improved?  If so, please report an enhancement request to PyTorch.)
 , got one on device 
 getDevicesOfStorages
 Expected all data ptrs to be on a device of type 
 vector::reserve
 Expected map.size() == (table_offsets_acc[t + 1] - table_offsets_acc[t]) to be true, but got false.  (Could this error message be improved?  If so, please report an enhancement request to PyTorch.)
 serialize
 table_offsets
 vector::_M_fill_insert
-schema_.returns().size() == 1 INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/builtin_function.h":22, please report a bug to PyTorch. 
-/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/builtin_function.h
+schema_.returns().size() == 1 INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/builtin_function.h":22, please report a bug to PyTorch. 
+/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/builtin_function.h
 BuiltinOpFunction
 defineMethod
 Default values must be specified for none or all arguments
-/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/torch/custom_class.h
+/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/torch/custom_class.h
 TensorImpl with nullptr is not supported
 vector::_M_default_append
 cannot create std::deque larger than max_size()
 *ZN5torch6class_I12PrunedMapCPUE12defineMethodIZNS2_10def_pickleINL20PrunedMapCPURegistryMUlRKN3c1013intrusive_ptrIS1_NS5_6detail34intrusive_target_default_null_typeIS1_EEEEE_ENL20PrunedMapCPURegistryMUlSsE0_EEERS2_OT_OT0_EUlNS5_14tagged_capsuleIS1_EEOSsE_EEPNS_3jit8FunctionESsSG_SsSt16initializer_listINS_3argEEEUlRSt6vectorINS5_6IValueESaISV_EEE_
 *ZN5torch6class_I13AtomicCounterE12defineMethodIZNS2_10def_pickleINL21AtomicCounterRegistryMUlRKN3c1013intrusive_ptrIS1_NS5_6detail34intrusive_target_default_null_typeIS1_EEEEE_ENL21AtomicCounterRegistryMUlSsE0_EEERS2_OT_OT0_EUlNS5_14tagged_capsuleIS1_EEOSsE_EEPNS_3jit8FunctionESsSG_SsSt16initializer_listINS_3argEEEUlRSt6vectorINS5_6IValueESaISV_EEE_
 *ZN5torch6class_I11TensorQueueE12defineMethodIZNS2_10def_pickleINL19TensorQueueRegistryMUlRKN3c1013intrusive_ptrIS1_NS5_6detail34intrusive_target_default_null_typeIS1_EEEEE_ENL19TensorQueueRegistryMUlNS5_4DictISsN2at6TensorEEEE0_EEERS2_OT_OT0_EUlNS5_14tagged_capsuleIS1_EEOSH_E_EEPNS_3jit8FunctionESsSK_SsSt16initializer_listINS_3argEEEUlRSt6vectorINS5_6IValueESaISZ_EEE_
 *ZN5torch6class_I12PrunedMapCPUE12defineMethodINL20PrunedMapCPURegistryMUlRKN3c1013intrusive_ptrIS1_NS4_6detail34intrusive_target_default_null_typeIS1_EEEEE_EEEPNS_3jit8FunctionESsT_SsSt16initializer_listINS_3argEEEUlRSt6vectorINS4_6IValueESaISL_EEE_
 *ZN5torch6class_I13AtomicCounterE12defineMethodINL21AtomicCounterRegistryMUlRKN3c1013intrusive_ptrIS1_NS4_6detail34intrusive_target_default_null_typeIS1_EEEEE_EEEPNS_3jit8FunctionESsT_SsSt16initializer_listINS_3argEEEUlRSt6vectorINS4_6IValueESaISL_EEE_
 *ZN5torch6class_I11TensorQueueE12defineMethodINL19TensorQueueRegistryMUlRKN3c1013intrusive_ptrIS1_NS4_6detail34intrusive_target_default_null_typeIS1_EEEEE_EEEPNS_3jit8FunctionESsT_SsSt16initializer_listINS_3argEEEUlRSt6vectorINS4_6IValueESaISL_EEE_
 Argument passed to at() was not in the map.
 init_tensor
 Expected Object but got 
 toObject
-isObject() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/ivalue_inl.h":133, please report a bug to PyTorch. 
+isObject() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/ivalue_inl.h":133, please report a bug to PyTorch. 
 Streams have a mix of device types: stream 0 is on 
-/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/c10/core/impl/InlineStreamGuard.h
+/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/c10/core/impl/InlineStreamGuard.h
  while stream 
  is on device 
 getDeviceTypeOfStreams
 , trying to set error: 
 setErrorInternal
 Error already set on this Future: 
 Future is already marked completed
-!completed() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/ivalue_inl.h":1221, please report a bug to PyTorch. 
+!completed() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/ivalue_inl.h":1221, please report a bug to PyTorch. 
  which are not among the expected device(s) 
 The result contained tensors residing on device(s) 
 Attempting to mark a completed Future as complete again. Note that a Future can only be marked completed once.
  does not match recording stream's device type 
 ensureIsSubsetOfDevices
 markCompleted
 constexpr c10::string_view c10::util::detail::fully_qualified_type_name_impl() [with T = c10::intrusive_ptr<TensorQueue>; c10::string_view = c10::basic_string_view<char>]
  could not be converted to any of the known types.
-/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/jit_type.h
+/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/jit_type.h
 constexpr c10::string_view c10::util::detail::fully_qualified_type_name_impl() [with T = c10::tagged_capsule<TensorQueue>; c10::string_view = c10::basic_string_view<char>]
 constexpr c10::string_view c10::util::detail::fully_qualified_type_name_impl() [with T = c10::intrusive_ptr<AtomicCounter>; c10::string_view = c10::basic_string_view<char>]
 constexpr c10::string_view c10::util::detail::fully_qualified_type_name_impl() [with T = c10::tagged_capsule<AtomicCounter>; c10::string_view = c10::basic_string_view<char>]
 constexpr c10::string_view c10::util::detail::fully_qualified_type_name_impl() [with T = c10::intrusive_ptr<PrunedMapCPU>; c10::string_view = c10::basic_string_view<char>]
 constexpr c10::string_view c10::util::detail::fully_qualified_type_name_impl() [with T = c10::tagged_capsule<PrunedMapCPU>; c10::string_view = c10::basic_string_view<char>]
 Tried to cast IValue to custom class but it did not contain a custom class!
-isCapsule() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/ivalue_inl.h":225, please report a bug to PyTorch. 
+isCapsule() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/ivalue_inl.h":225, please report a bug to PyTorch. 
 toCustomClass
 toCapsule
 Tried to cast a Dict<
 > to a Dict<
 >. Key types mismatch.
 toTypedDict
 >. Value types mismatch.
-*getTypePtr<Key>() == *dict.impl_->elementTypes.keyType INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/Dict_inl.h":26, please report a bug to PyTorch. 
-/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/Dict_inl.h
-*getTypePtr<Value>() == *dict.impl_->elementTypes.valueType INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/Dict_inl.h":27, please report a bug to PyTorch. 
+*getTypePtr<Key>() == *dict.impl_->elementTypes.keyType INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/Dict_inl.h":26, please report a bug to PyTorch. 
+/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/Dict_inl.h
+*getTypePtr<Value>() == *dict.impl_->elementTypes.valueType INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/Dict_inl.h":27, please report a bug to PyTorch. 
 N3c105ErrorE
 N3c1010ValueErrorE
 N3c1011StorageImplE
 N3c1015VariableVersion14VersionCounterE
 N3c104impl24DeviceGuardImplInterfaceE
 N3c106detail8ListImplE
 N5torch17CustomClassHolderE
@@ -15840,37 +15840,37 @@
 pooling_mode
 function 
 apply_with_saved
 missing before())
 vector<bool>::_M_insert_aux
 Please open a feature request on GitHub if you need this.
 jvp is not implemented for the c++ API of custom Function yet.
-/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/torch/csrc/autograd/custom_function.h
+/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/torch/csrc/autograd/custom_function.h
 compiled_args not implemented for non-traceable node: 
 dense_embedding_codegen_lookup_function(Tensor dev_weights, Tensor weights_offsets, Tensor D_offsets, int total_D, int max_D, Tensor hash_size_cumsum, int total_hash_size_bits, Tensor indices, Tensor offsets, int pooling_mode, Tensor? indice_weights, Tensor? feature_requires_grad, int output_dtype=0) -> Tensor
 dense_embedding_codegen_lookup_function
 Cannot update a node's topological_nr after it already has a parent. If we allow this, we can no longer guarantee that a parent's topo_nr is always greater than those of all its children
-!has_parent_ INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/torch/csrc/autograd/function.h":262, please report a bug to PyTorch. 
-/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/torch/csrc/autograd/function.h
+!has_parent_ INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/torch/csrc/autograd/function.h":262, please report a bug to PyTorch. 
+/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/torch/csrc/autograd/function.h
 /__w/FBGEMM/FBGEMM/fbgemm_gpu/codegen/training/backward/embedding_backward_dense_host_cpu.cpp
 Check failed: grad_outputs.size() == 1 (
  returned an incorrect number of gradients (expected 
  returned a gradient different that is defined at position 
 , but the corresponding forward input was not a Variable
-ctx_.non_differentiable_.empty() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/torch/csrc/autograd/custom_function.h":221, please report a bug to PyTorch. 
-ctx_.dirty_inputs_.empty() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/torch/csrc/autograd/custom_function.h":222, please report a bug to PyTorch. 
-it != _saved_variables.end() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/torch/csrc/dynamo/compiled_autograd.h":138, please report a bug to PyTorch. 
-arg.proxy_tensor.defined() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/torch/csrc/dynamo/compiled_autograd.h":561, please report a bug to PyTorch. 
-ctx_.to_save_.empty() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/torch/csrc/autograd/custom_function.h":224, please report a bug to PyTorch. 
-it != this->end() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/torch/csrc/dynamo/compiled_autograd.h":760, please report a bug to PyTorch. 
-ctx_.non_differentiable_.empty() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/torch/csrc/autograd/custom_function.h":231, please report a bug to PyTorch. 
-ctx_.dirty_inputs_.empty() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/torch/csrc/autograd/custom_function.h":232, please report a bug to PyTorch. 
-ctx_.to_save_.empty() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/torch/csrc/autograd/custom_function.h":234, please report a bug to PyTorch. 
-sym_sizes_index < sym_sizes.size() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/torch/csrc/dynamo/compiled_autograd.h":531, please report a bug to PyTorch. 
-/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/torch/csrc/dynamo/compiled_autograd.h
+ctx_.non_differentiable_.empty() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/torch/csrc/autograd/custom_function.h":221, please report a bug to PyTorch. 
+ctx_.dirty_inputs_.empty() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/torch/csrc/autograd/custom_function.h":222, please report a bug to PyTorch. 
+it != _saved_variables.end() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/torch/csrc/dynamo/compiled_autograd.h":138, please report a bug to PyTorch. 
+arg.proxy_tensor.defined() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/torch/csrc/dynamo/compiled_autograd.h":561, please report a bug to PyTorch. 
+ctx_.to_save_.empty() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/torch/csrc/autograd/custom_function.h":224, please report a bug to PyTorch. 
+it != this->end() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/torch/csrc/dynamo/compiled_autograd.h":760, please report a bug to PyTorch. 
+ctx_.non_differentiable_.empty() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/torch/csrc/autograd/custom_function.h":231, please report a bug to PyTorch. 
+ctx_.dirty_inputs_.empty() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/torch/csrc/autograd/custom_function.h":232, please report a bug to PyTorch. 
+ctx_.to_save_.empty() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/torch/csrc/autograd/custom_function.h":234, please report a bug to PyTorch. 
+sym_sizes_index < sym_sizes.size() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/torch/csrc/dynamo/compiled_autograd.h":531, please report a bug to PyTorch. 
+/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/torch/csrc/dynamo/compiled_autograd.h
 next_sym_size
 PFvPN5torch8autograd4NodeEE
 *N5torch8autograd7CppNodeIN12_GLOBAL__N_128SplitLookupFunction_Dense_OpEEE
 *ZN5torch8autograd8FunctionIN12_GLOBAL__N_128SplitLookupFunction_Dense_OpEE5applyIS3_JRN2at6TensorES8_S8_RlS9_S8_S9_S8_S8_S9_RSt8optionalIS7_ESC_EEENSt9enable_ifIX9is_same_vIT_S3_EEDTclsrSE_7forwardLDnEspcl7declvalIT0_EEEEE4typeEDpOSF_EUlRKSt6vectorIS7_SaIS7_EESP_E_
 *ZN5torch8autograd8FunctionIN12_GLOBAL__N_128SplitLookupFunction_Dense_OpEE5applyIS3_JRN2at6TensorES8_S8_RlS9_S8_S9_S8_S8_S9_RSt8optionalIS7_ESC_EEENSt9enable_ifIX9is_same_vIT_S3_EEDTclsrSE_7forwardLDnEspcl7declvalIT0_EEEEE4typeEDpOSF_EUlRKS7_E0_
 *N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorES5_S5_S5_llS5_lS5_S5_lSt8optionalIS5_ES7_lEXadL_ZN12_GLOBAL__N_145split_embedding_codegen_lookup_dense_functionES5_S5_S5_llS5_lS5_S5_lS7_S7_lEEEES5_NS_4guts8typelist8typelistIJS5_S5_S5_llS5_lS5_S5_lS7_S7_lEEEEE
 *St19_Sp_counted_deleterIPN5torch8autograd7CppNodeIN12_GLOBAL__N_128SplitLookupFunction_Dense_OpEEEPFvPNS1_4NodeEESaIvELN9__gnu_cxx12_Lock_policyE2EE
@@ -15913,35 +15913,35 @@
 sum_reduce_to_one
 merge_pooled_embeddings
 t must be a CPU tensor; it is currently on device 
 /__w/FBGEMM/FBGEMM/fbgemm_gpu/src/merge_pooled_embedding_ops/merge_pooled_embedding_ops_cpu.cpp
 Expected input_tensors.size() > 0 to be true, but got false.  (Could this error message be improved?  If so, please report an enhancement request to PyTorch.)
 input_0 must be a CPU tensor; it is currently on device 
 input_tensors[i] must be a CPU tensor; it is currently on device 
-isDevice() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/ivalue.h":916, please report a bug to PyTorch. 
-isTensorList() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/ivalue_inl.h":2040, please report a bug to PyTorch. 
-isTensorList() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/ivalue_inl.h":2044, please report a bug to PyTorch. 
+isDevice() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/ivalue.h":916, please report a bug to PyTorch. 
+isTensorList() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/ivalue_inl.h":2040, please report a bug to PyTorch. 
+isTensorList() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/ivalue_inl.h":2044, please report a bug to PyTorch. 
 toDevice
 Expected TensorList but got 
 toTensorList
 N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorESt6vectorIS5_SaIS5_EElNS_6DeviceElEXadL_ZN10fbgemm_gpu27merge_pooled_embeddings_cpuES8_lS9_lEEEES5_NS_4guts8typelist8typelistIJS8_lS9_lEEEEE
 FN2at6TensorESt6vectorIS0_SaIS0_EElN3c106DeviceElE
 N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorESt6vectorIS5_SaIS5_EENS_6DeviceEEXadL_ZN10fbgemm_gpu21sum_reduce_to_one_cpuES8_S9_EEEES5_NS_4guts8typelist8typelistIJS8_S9_EEEEE
 FN2at6TensorESt6vectorIS0_SaIS0_EEN3c106DeviceEE
 N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFSt6vectorIN2at6TensorESaIS6_EES8_NS_6DeviceEEXadL_ZN10fbgemm_gpu21all_to_one_device_cpuES8_S9_EEEES8_NS_4guts8typelist8typelistIJS8_S9_EEEEE
 FSt6vectorIN2at6TensorESaIS1_EES3_N3c106DeviceEE
 merge_pooled_embeddings(Tensor[] pooled_embeddings, SymInt uncat_dim_size, Device target_device, SymInt cat_dim=all_to_one_device(Tensor[] input_tensors, Device target_device) sum_reduce_to_onTried to access the schema for 
  which doesn't have a schema registered yet
-schema_.has_value() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/dispatch/OperatorEntry.h":80, please report a bug to PyTorch. 
-/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/dispatch/OperatorEntry.h
+schema_.has_value() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/dispatch/OperatorEntry.h":80, please report a bug to PyTorch. 
+/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/dispatch/OperatorEntry.h
 fbgemm::permute_duplicate_pooled_embs
 offset_dim_list needs to have long/int64 type
 /__w/FBGEMM/FBGEMM/fbgemm_gpu/src/permute_pooled_embedding_ops/permute_pooled_embedding_function.cpp
 permute_list needs to have long/int64 type
-isBool() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/ivalue.h":661, please report a bug to PyTorch. 
+isBool() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/ivalue.h":661, please report a bug to PyTorch. 
 permute_pooled_embs does not support allow_duplicates in backward!
 fbgemm::permute_pooled_embs
 FN2at6TensorERKS0_S2_S2_S2_S2_E
 inv_offset_dim_linv_permute_listallow_duplicatespermute_pooled_embs_cpu_impl
 permute_pooled_embs_auto_grad
 permute_duplicate_pooled_embs
 /__w/FBGEMM/FBGEMM/fbgemm_gpu/src/permute_pooled_embedding_ops/permute_pooled_embedding_ops_cpu.cpp
@@ -16001,27 +16001,27 @@
 num_output_rows
 slice_length
 fbgemm::jagged_slice_forward
 lengths is currently on 
 start should be <= len
 jagged_dense_dense_elementwise_add_jagged_output
 batched_dense_vec_jagged_2d_mul
-isList() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/ivalue_inl.h":2072, please report a bug to PyTorch. 
+isList() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/ivalue_inl.h":2072, please report a bug to PyTorch. 
 /__w/FBGEMM/FBGEMM/fbgemm_gpu/src/jagged_tensor_ops/jagged_tensor_ops_autograd.cpp
 Expected grad_outputs.size() == 1 to be true, but got false.  (Could this error message be improved?  If so, please report an enhancement request to PyTorch.)
 Expected total_L >= 0 to be true, but got false.  (Could this error message be improved?  If so, please report an enhancement request to PyTorch.)
 fbgemm::jagged_to_padded_dense_backward
 fbgemm::jagged_to_padded_dense_forward
 Expected values.dim() == 1 to be true, but got false.  (Could this error message be improved?  If so, please report an enhancement request to PyTorch.)
 Expected offsets.dim() == 1 to be true, but got false.  (Could this error message be improved?  If so, please report an enhancement request to PyTorch.)
 Expected max_L > 0 to be true, but got false.  (Could this error message be improved?  If so, please report an enhancement request to PyTorch.)
 Expected max_lengths.size() == x_offsets.size() to be true, but got false.  (Could this error message be improved?  If so, please report an enhancement request to PyTorch.)
 Expected SymIntList or IntList but got 
-isSymIntList() || isIntList() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/ivalue_inl.h":1984, please report a bug to PyTorch. 
-/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/c10/core/SymInt.h
+isSymIntList() || isIntList() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/ivalue_inl.h":1984, please report a bug to PyTorch. 
+/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/c10/core/SymInt.h
 Expected dense_values_grad.sym_sizes() == dense_shape to be true, but got false.  (Could this error message be improved?  If so, please report an enhancement request to PyTorch.)
 fbgemm::jagged_dense_dense_elementwise_add_jagged_output_forward
 fbgemm::jagged_dense_elementwise_mul_backward
 fbgemm::jagged_dense_elementwise_mul_forward
 fbgemm::batched_dense_vec_jagged_2d_mul_backward
 fbgemm::batched_dense_vec_jagged_2d_mul_forward
 fbgemm::dense_to_jagged_forward
@@ -16041,15 +16041,15 @@
 fbgemm::jagged_index_select_2d_forward_v2
 output_lengths is currently on 
 grad must be on the same device as output_lengths! grad is currently on 
 Tensor 'values' must have 1 dimension(s). Found 
 values must be on the same device as lengths! values is currently on 
 start should be always be positive
 type with contained types did not overload createWithContained: 
-/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/jit_type_base.h
+/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/jit_type_base.h
 createWithContained
 ; Length = 
 ArrayRef: invalid index Index = 
  with None type
 Can not create 
 : SymIntArrayRef expected to contain only concrete integers
 asIntArrayRefSlow
@@ -16095,22 +16095,22 @@
 *St19_Sp_counted_deleterIPN5torch8autograd7CppNodeIN10fbgemm_gpu12_GLOBAL__N_115DenseToJaggedOpEEEPFvPNS1_4NodeEESaIvELN9__gnu_cxx12_Lock_policyE2EE
 *St19_Sp_counted_deleterIPN5torch8autograd7CppNodeIN10fbgemm_gpu12_GLOBAL__N_136JaggedDenseElementwiseAddJaggedOutOpEEEPFvPNS1_4NodeEESaIvELN9__gnu_cxx12_Lock_policyE2EE
 *St19_Sp_counted_deleterIPN5torch8autograd7CppNodeIN10fbgemm_gpu12_GLOBAL__N_115JaggedSoftmaxOpEEEPFvPNS1_4NodeEESaIvELN9__gnu_cxx12_Lock_policyE2EE
 *St19_Sp_counted_deleterIPN5torch8autograd7CppNodeIN10fbgemm_gpu12_GLOBAL__N_117JaggedJaggedBmmOpEEEPFvPNS1_4NodeEESaIvELN9__gnu_cxx12_Lock_policyE2EE
 *St19_Sp_counted_deleterIPN5torch8autograd7CppNodeIN10fbgemm_gpu12_GLOBAL__N_116JaggedDenseBmmOpEEEPFvPNS1_4NodeEESaIvELN9__gnu_cxx12_Lock_policyE2EE
 *St19_Sp_counted_deleterIPN5torch8autograd7CppNodeIN10fbgemm_gpu12_GLOBAL__N_121JaggedIndexSelect2dOpEEEPFvPNS1_4NodeEESaIvELN9__gnu_cxx12_Lock_policyE2EE
 *St19_Sp_counted_deleterIPN5torch8autograd7CppNodeIN10fbgemm_gpu12_GLOBAL__N_113JaggedSliceOpEEEPFvPNS1_4NodeEESaIvELN9__gnu_cxx12_Lock_policyE2EE
-isSymInt() || isInt() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/ivalue_inl.h":245, please report a bug to PyTorch. 
+isSymInt() || isInt() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/ivalue_inl.h":245, please report a bug to PyTorch. 
 Tried to cast a List<
 > to a List<
 >. Types mismatch.
 toTypedList
-/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/List_inl.h
-/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/boxing/KernelFunction_impl.h
-isDouble() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/ivalue.h":535, please report a bug to PyTorch. 
+/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/List_inl.h
+/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/boxing/KernelFunction_impl.h
+isDouble() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/ivalue.h":535, please report a bug to PyTorch. 
 toDouble
 St23enable_shared_from_thisIN3c1010SharedTypeEE
 N3c1010SharedTypeE
 N3c1017SingleElementTypeILNS_8TypeKindE6ENS_8ListTypeEEE
 FN2at6TensorERKS0_RKSt6vectorIS0_SaIS0_EEN3c108ArrayRefINS8_6SymIntEEEdE
 FN2at6TensorERKS0_RKSt6vectorIS0_SaIS0_EEN3c108ArrayRefIlEEdE
 FN2at6TensorERKS0_RKSt6vectorIS0_SaIS0_EEN3c106SymIntEE
@@ -16304,15 +16304,15 @@
 jagged_jagged_elementwise_dense_output_kernel_
 Expected !NO_INNER_DENSE || output.size(-1) == 1 to be true, but got false.  (Could this error message be improved?  If so, please report an enhancement request to PyTorch.)
 unsupported number of jagged dim 
 jagged_2d_to_dense_forward_cpu
 jagged_2d_to_dense_backward_kernel
 fbgemm::jagged_index_select_2d_forward
 fbgemm::jagged_index_add_2d_forward
-isIntList() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/ivalue_inl.h":1968, please report a bug to PyTorch. 
+isIntList() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/ivalue_inl.h":1968, please report a bug to PyTorch. 
 FN2at6TensorERKS0_S2_S2_S2_lE
 FN2at6TensorERKS0_S2_S2_S2_llE
 N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorERKS5_RKSt6vectorIS5_SaIS5_EES7_EXadL_ZN10fbgemm_gpu28jagged_dense_elementwise_addES7_SC_S7_EEEES5_NS_4guts8typelist8typelistIJS7_SC_S7_EEEEE
 N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFSt6vectorIN2at6TensorESaIS6_EES6_S6_RKS4_IlSaIlEESC_lEXadL_ZN10fbgemm_gpu30stacked_jagged_1d_to_dense_cpuES6_S6_SC_SC_lEEEES8_NS_4guts8typelist8typelistIJS6_S6_SC_SC_lEEEEE
 FSt6vectorIN2at6TensorESaIS1_EES1_S1_RKS_IlSaIlEES7_lE
 N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFSt6vectorIN2at6TensorESaIS6_EES6_S6_RKS4_IlSaIlEESC_lEXadL_ZN10fbgemm_gpu30stacked_jagged_2d_to_dense_cpuES6_S6_SC_SC_lEEEES8_NS_4guts8typelist8typelistIJS6_S6_SC_SC_lEEEEE
 N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorERKS5_S7_S7_S7_lEXadL_ZN10fbgemm_gpu34jagged_index_select_2d_forward_cpuES7_S7_S7_S7_lEEEES5_NS_4guts8typelist8typelistIJS7_S7_S7_S7_lEEEEE
@@ -16810,15 +16810,15 @@
 FvN2at6TensorES0_lS0_S0_S0_S0_S0_S0_S0_S0_lE
 N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorES5_S5_lbSt8optionalIS5_ES7_S7_EXadL_ZN10fbgemm_gpu20lxu_cache_lookup_cpuES5_S5_lbS7_S7_S7_EEEES5_NS_4guts8typelist8typelistIJS5_S5_lbS7_S7_S7_EEEEE
 FN2at6TensorES0_S0_lbSt8optionalIS0_ES2_S2_E
 N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorES5_S5_lbSt8optionalIS5_EEXadL_ZN10fbgemm_gpu34direct_mapped_lxu_cache_lookup_cpuES5_S5_lbS7_EEEES5_NS_4guts8typelist8typelistIJS5_S5_lbS7_EEEEE
 FN2at6TensorES0_S0_lbSt8optionalIS0_EE
 linearize_cache_indices(Tensor cache_hash_size_cumsum, Tensor indices, Tensor offsets, Tensor? B_offsets=None, int max_B=-1) -> indices_from_row_idx(Tensor cache_hash_size_cumsum, Tensor update_table_indices, Tensor update_row_indices) -> Tdirect_mapped_lxu_cache_lookup(Tensor linear_cache_indices, Tensor lxu_cache_state, int invalid_index = -1, bool gather_cache_stats=False, Tensor(a!)? uvm_cache_stats=None) -> lxu_cache_slot(int h_in, int C) lxu_cache_locking_counter_decrement(Tensor(a!) lxu_cache_locking_counter, Tensor lxu_cache_locatlxu_cache_locations_update(Tensor(a!) lxu_cache_locations, Tensor lxu_cache_locations_new, Tensor? num_uniq_cache_indices=None) get_unique_indices(Tensor linear_indices, int max_indices, bool compute_count) -> (Tensor, Tensobatch_index_select_dim0
 batch_index_select_dim0_cpu
-isIntList() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.9/site-packages/torch/include/ATen/core/ivalue_inl.h":1976, please report a bug to PyTorch. 
+isIntList() INTERNAL ASSERT FAILED at "/github/home/miniconda/envs/build_binary/lib/python3.8/site-packages/torch/include/ATen/core/ivalue_inl.h":1976, please report a bug to PyTorch. 
 toIntVector
 batch_index_select_dim0(    Tensor inputs,    Tensor indices,    SymInt[] input_num_indices,    SymInt[] input_rows,    SymInt[] input_columns,    bool permute_output_dim_0_1=False) -> Tensor
 [batch_index_select_dim0] input_rows must have the same length as input_num_indices.
 /__w/FBGEMM/FBGEMM/fbgemm_gpu/codegen/training/index_select/batch_index_select_dim0_cpu_host.cpp
 [batch_index_select_dim0] input_columns must have the same length as input_num_indices.
 Currently batch_index_select only supports 16-byte align input tensors
 [batch_index_select_dim0] All input_columns must be the same.
@@ -16836,15 +16836,15 @@
 ZN5torch8autograd8FunctionI25BatchIndexSelectDim0CPUOpE5applyIS2_JRN2at6TensorES7_RSt6vectorIlSaIlEESB_SB_RKbEEENSt9enable_ifIX9is_same_vIT_S2_EEDTclsrSF_7forwardLDnEspcl7declvalIT0_EEEEE4typeEDpOSG_EUlRKS6_E0_
 N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorES5_S5_St6vectorIlSaIlEES8_S8_bEXadL_Z27batch_index_select_dim0_cpuS5_S5_S8_S8_S8_bEEEES5_NS_4guts8typelist8typelistIJS5_S5_S8_S8_S8_bEEEEE
 FN2at6TensorES0_S0_St6vectorIlSaIlEES3_S3_bE
 St19_Sp_counted_deleterIPN5torch8autograd7CppNodeI25BatchIndexSelectDim0CPUOpEEPFvPNS1_4NodeEESaIvELN9__gnu_cxx12_Lock_policyE2EE
 Unsupported SparseType: 
 pruned_array_lookup_cpu
 Expected placement != PlacementType::DEVICE to be true, but got false.  (Could this error message be improved?  If so, please report an enhancement request to PyTorch.)
-/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.9/cmake-build/gen_embedding_forward_quantized_unweighted_codegen_cpu.cpp
+/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.8/cmake-build/gen_embedding_forward_quantized_unweighted_codegen_cpu.cpp
 int8 output are only supported for int8 weights
 Expected offsets_nobag.numel() == index_size + 1 to be true, but got false.  (Could this error message be improved?  If so, please report an enhancement request to PyTorch.)
 Expected offsets_nobag_ptr[index_size] - offsets_nobag_ptr[0] == index_size to be true, but got false.  (Could this error message be improved?  If so, please report an enhancement request to PyTorch.)
 int_nbit_split_embedding_codegen_forward_unweighted_cpu
 Expected B >= 0 to be true, but got false.  (Could this error message be improved?  If so, please report an enhancement request to PyTorch.)
 Expected total_D > 0 to be true, but got false.  (Could this error message be improved?  If so, please report an enhancement request to PyTorch.)
 Enabling both CUDA and HIP in ATen is not supported, as HIP masquerades to be CUDA (e.g., when you say CUDA, on a HIP build of ATen, this actually means HIP.  Rebuild PyTorch with one or the other disabled.
@@ -16857,30 +16857,30 @@
 int_nbit_split_embedding_nobag_codegen_forward_
 "intn_split_embedding_nobag_codegen_forward_kernel"
 pruned_hashmap_lookup_unweighted_cpu
 hash_table must be a CPU tensor; it is currently on device 
 hash_table_offsets must be a CPU tensor; it is currently on device 
 pruned_hashmap_insert_unweighted_cpu
 dense_indices must be a CPU tensor; it is currently on device 
-/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.9/cmake-build/gen_embedding_forward_quantized_weighted_codegen_cpu.cpp
+/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.8/cmake-build/gen_embedding_forward_quantized_weighted_codegen_cpu.cpp
 pruned_hashmap_lookup_weighted_cpu
 pruned_hashmap_insert_weighted_cpu
 int_nbit_split_embedding_codegen_forward_weighted_cpu
 indice_weights must be empty or a CPU tensor; it is currently on device 
-/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.9/cmake-build/gen_embedding_backward_dense_split_cpu.cpp
+/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.8/cmake-build/gen_embedding_backward_dense_split_cpu.cpp
 Check failed: host_weights.dim() == 1 (
 split_embedding_backward_exact_cpu
 split_embedding_backward_codegen_dense_cpu(Tensor grad_output, Tensor(a!) host_weights, Tensor weights_offsets, Tensor D_offsets, int max_D, Tensor hash_size_cumsum, int total_hash_size_bits, Tensor indices, Tensor offsets,int pooling_mode, Tensor indice_weights, float unused = 0) -> Tensor
 split_embedding_backward_codegen_dense_cpu
 N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorES5_S5_S5_S5_lS5_lS5_S5_lS5_dEXadL_Z42split_embedding_backward_codegen_dense_cpuS5_S5_S5_S5_lS5_lS5_S5_lS5_dEEEES5_NS_4guts8typelist8typelistIJS5_S5_S5_S5_lS5_lS5_S5_lS5_dEEEEE
 FN2at6TensorES0_S0_S0_S0_lS0_lS0_S0_lS0_dE
 split_embedding_codegen_grad_indice_weights_pt2_wrapper
 split_embedding_codegen_forward_weighted_pt2_wrapper
 split_embedding_codegen_forward_unweighted_pt2_wrapper
-/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.9/cmake-build/gen_embedding_forward_split_pt2_cpu_wrapper.cpp
+/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.8/cmake-build/gen_embedding_forward_split_pt2_cpu_wrapper.cpp
 fbgemm::split_embedding_codegen_grad_indice_weights_cpu
 fbgemm::split_embedding_codegen_forward_cpu
 FN2at6TensorES0_S0_S0_lS0_S0_S0_lS0_lE
 N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorERKS5_S7_S7_S7_S7_S7_S7_S7_NS_6SymIntES7_S7_S7_S7_EXadL_Z59split_embedding_codegen_grad_indice_weights_pt2_cpu_wrapperS7_S7_S7_S7_S7_S7_S7_S7_S8_S7_S7_S7_S7_EEEES5_NS_4guts8typelist8typelistIJS7_S7_S7_S7_S7_S7_S7_S7_S8_S7_S7_S7_S7_EEEEE
 FN2at6TensorERKS0_S2_S2_S2_S2_S2_S2_S2_N3c106SymIntES2_S2_S2_S2_E
 N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorERKS5_S7_S7_S7_S7_S7_S7_NS_6SymIntES8_S7_S7_S7_lS7_S7_S7_blEXadL_Z56split_embedding_codegen_forward_weighted_pt2_cpu_wrapperS7_S7_S7_S7_S7_S7_S7_S8_S8_S7_S7_S7_lS7_S7_S7_blEEEES5_NS_4guts8typelist8typelistIJS7_S7_S7_S7_S7_S7_S7_S8_S8_S7_S7_S7_lS7_S7_S7_blEEEEE
 FN2at6TensorERKS0_S2_S2_S2_S2_S2_S2_N3c106SymIntES4_S2_S2_S2_lS2_S2_S2_blE
@@ -16888,150 +16888,150 @@
 gradient_clipping
 max_gradient
 stochastic_rounding
 output_dtype
 learning_rate
 split_embedding_codegen_lookup_adagrad_function_cpu(Tensor(a!) host_weights, Tensor weights_placements, Tensor weights_offsets, Tensor D_offsets, SymInt total_D, SymInt max_D, Tensor hash_size_cumsum, int total_hash_size_bits, Tensor indices, Tensor offsets, int pooling_mode, Tensor? indice_weights, Tensor? feature_requires_grad, bool gradient_clipping, float max_gradient, bool stochastic_rounding, Tensor momentum1_host, Tensor momentum1_placements, Tensor momentum1_offsets, float eps = 0, float learning_rate = 0, int output_dtype=0) -> Tensor
 split_embedding_codegen_lookup_adagrad_function_cpu
-/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.9/cmake-build/gen_embedding_backward_split_adagrad_cpu.cpp
+/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.8/cmake-build/gen_embedding_backward_split_adagrad_cpu.cpp
 fbgemm::split_embedding_backward_codegen_adagrad_cpu
 *N5torch8autograd7CppNodeIN12_GLOBAL__N_130SplitLookupFunction_adagrad_OpEEE
 *ZN5torch8autograd8FunctionIN12_GLOBAL__N_130SplitLookupFunction_adagrad_OpEE5applyIS3_JRN2at6TensorES8_S8_S8_RN3c106SymIntESB_S8_RlS8_S8_SC_RSt8optionalIS7_ESF_RbRdSG_S8_S8_S8_SH_SH_SC_EEENSt9enable_ifIX9is_same_vIT_S3_EEDTclsrSJ_7forwardLDnEspcl7declvalIT0_EEEEE4typeEDpOSK_EUlRKSt6vectorIS7_SaIS7_EESU_E_
 *ZN5torch8autograd8FunctionIN12_GLOBAL__N_130SplitLookupFunction_adagrad_OpEE5applyIS3_JRN2at6TensorES8_S8_S8_RN3c106SymIntESB_S8_RlS8_S8_SC_RSt8optionalIS7_ESF_RbRdSG_S8_S8_S8_SH_SH_SC_EEENSt9enable_ifIX9is_same_vIT_S3_EEDTclsrSJ_7forwardLDnEspcl7declvalIT0_EEEEE4typeEDpOSK_EUlRKS7_E0_
 *N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorES5_S5_S5_S5_NS_6SymIntES6_S5_lS5_S5_lSt8optionalIS5_ES8_bdbS5_S5_S5_ddlEXadL_ZN12_GLOBAL__N_151split_embedding_codegen_lookup_adagrad_function_cpuES5_S5_S5_S5_S6_S6_S5_lS5_S5_lS8_S8_bdbS5_S5_S5_ddlEEEES5_NS_4guts8typelist8typelistIJS5_S5_S5_S5_S6_S6_S5_lS5_S5_lS8_S8_bdbS5_S5_S5_ddlEEEEE
 *St19_Sp_counted_deleterIPN5torch8autograd7CppNodeIN12_GLOBAL__N_130SplitLookupFunction_adagrad_OpEEEPFvPNS1_4NodeEESaIvELN9__gnu_cxx12_Lock_policyE2EE
 FvN2at6TensorES0_S0_S0_S0_N3c106SymIntES0_lS0_S0_lS0_bS0_S0_S0_ddlE
 FvN2at6TensorES0_S0_S0_S0_lS0_lS0_S0_lS0_bS0_S0_S0_ddlE
 FN2at6TensorES0_S0_S0_S0_N3c106SymIntES2_S0_lS0_S0_lSt8optionalIS0_ES4_bdbS0_S0_S0_ddlE
-/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.9/cmake-build/gen_embedding_backward_split_adagrad_pt2_cpu_wrapper.cpp
+/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.8/cmake-build/gen_embedding_backward_split_adagrad_pt2_cpu_wrapper.cpp
 split_embedding_backward_codegen_adagrad_weighted_exact_pt2_wrapper
 split_embedding_backward_codegen_adagrad_unweighted_exact_pt2_wrapper
 N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorERKS5_S7_S7_S7_S7_S7_S7_S7_lS7_lS7_S7_lS7_S7_llbllbbS5_S5_S5_S5_S5_ddlEXadL_Z71split_embedding_backward_codegen_adagrad_weighted_exact_pt2_cpu_wrapperS7_S7_S7_S7_S7_S7_S7_S7_lS7_lS7_S7_lS7_S7_llbllbbS5_S5_S5_S5_S5_ddlEEEES5_NS_4guts8typelist8typelistIJS7_S7_S7_S7_S7_S7_S7_S7_lS7_lS7_S7_lS7_S7_llbllbbS5_S5_S5_S5_S5_ddlEEEEE
 FN2at6TensorERKS0_S2_S2_S2_S2_S2_S2_S2_lS2_lS2_S2_lS2_S2_llbllbbS0_S0_S0_S0_S0_ddlE
 N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorERKS5_S7_S7_S7_S7_S7_S7_S7_lS7_lS7_S7_lS7_S7_llbllbbS5_S5_S5_S5_S5_ddlEXadL_Z73split_embedding_backward_codegen_adagrad_unweighted_exact_pt2_cpu_wrapperS7_S7_S7_S7_S7_S7_S7_S7_lS7_lS7_S7_lS7_S7_llbllbbS5_S5_S5_S5_S5_ddlEEEES5_NS_4guts8typelist8typelistIJS7_S7_S7_S7_S7_S7_S7_S7_lS7_lS7_S7_lS7_S7_llbllbbS5_S5_S5_S5_S5_ddlEEEEE
 weight_decay
 weight_decay_mode
 max_norm
 split_embedding_codegen_lookup_rowwise_adagrad_function_cpu(Tensor(a!) host_weights, Tensor weights_placements, Tensor weights_offsets, Tensor D_offsets, SymInt total_D, SymInt max_D, Tensor hash_size_cumsum, int total_hash_size_bits, Tensor indices, Tensor offsets, int pooling_mode, Tensor? indice_weights, Tensor? feature_requires_grad, bool gradient_clipping, float max_gradient, bool stochastic_rounding, Tensor momentum1_host, Tensor momentum1_placements, Tensor momentum1_offsets, float eps = 0, float learning_rate = 0, float weight_decay = 0.0, int weight_decay_mode = 0, float max_norm = 0.0, int output_dtype=0) -> Tensor
 split_embedding_codegen_lookup_rowwise_adagrad_function_cpu
-/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.9/cmake-build/gen_embedding_backward_split_rowwise_adagrad_cpu.cpp
+/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.8/cmake-build/gen_embedding_backward_split_rowwise_adagrad_cpu.cpp
 fbgemm::split_embedding_backward_codegen_rowwise_adagrad_cpu
 *N5torch8autograd7CppNodeIN12_GLOBAL__N_138SplitLookupFunction_rowwise_adagrad_OpEEE
 *ZN5torch8autograd8FunctionIN12_GLOBAL__N_138SplitLookupFunction_rowwise_adagrad_OpEE5applyIS3_JRN2at6TensorES8_S8_S8_RN3c106SymIntESB_S8_RlS8_S8_SC_RSt8optionalIS7_ESF_RbRdSG_S8_S8_S8_SH_SH_SH_SC_SH_SC_EEENSt9enable_ifIX9is_same_vIT_S3_EEDTclsrSJ_7forwardLDnEspcl7declvalIT0_EEEEE4typeEDpOSK_EUlRKSt6vectorIS7_SaIS7_EESU_E_
 *ZN5torch8autograd8FunctionIN12_GLOBAL__N_138SplitLookupFunction_rowwise_adagrad_OpEE5applyIS3_JRN2at6TensorES8_S8_S8_RN3c106SymIntESB_S8_RlS8_S8_SC_RSt8optionalIS7_ESF_RbRdSG_S8_S8_S8_SH_SH_SH_SC_SH_SC_EEENSt9enable_ifIX9is_same_vIT_S3_EEDTclsrSJ_7forwardLDnEspcl7declvalIT0_EEEEE4typeEDpOSK_EUlRKS7_E0_
 *N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorES5_S5_S5_S5_NS_6SymIntES6_S5_lS5_S5_lSt8optionalIS5_ES8_bdbS5_S5_S5_dddldlEXadL_ZN12_GLOBAL__N_159split_embedding_codegen_lookup_rowwise_adagrad_function_cpuES5_S5_S5_S5_S6_S6_S5_lS5_S5_lS8_S8_bdbS5_S5_S5_dddldlEEEES5_NS_4guts8typelist8typelistIJS5_S5_S5_S5_S6_S6_S5_lS5_S5_lS8_S8_bdbS5_S5_S5_dddldlEEEEE
 *St19_Sp_counted_deleterIPN5torch8autograd7CppNodeIN12_GLOBAL__N_138SplitLookupFunction_rowwise_adagrad_OpEEEPFvPNS1_4NodeEESaIvELN9__gnu_cxx12_Lock_policyE2EE
 FvN2at6TensorES0_S0_S0_S0_N3c106SymIntES0_lS0_S0_lS0_bS0_S0_S0_dddldlE
 FvN2at6TensorES0_S0_S0_S0_lS0_lS0_S0_lS0_bS0_S0_S0_dddldlE
 FN2at6TensorES0_S0_S0_S0_N3c106SymIntES2_S0_lS0_S0_lSt8optionalIS0_ES4_bdbS0_S0_S0_dddldlE
-/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.9/cmake-build/gen_embedding_backward_split_rowwise_adagrad_pt2_cpu_wrapper.cpp
+/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.8/cmake-build/gen_embedding_backward_split_rowwise_adagrad_pt2_cpu_wrapper.cpp
 split_embedding_backward_codegen_rowwise_adagrad_weighted_exact_pt2_wrapper
 split_embedding_backward_codegen_rowwise_adagrad_unweighted_exact_pt2_wrapper
 N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorERKS5_S7_S7_S7_S7_S7_S7_S7_lS7_lS7_S7_lS7_S7_llbllbbS5_S5_S5_S5_S5_dddldlEXadL_Z79split_embedding_backward_codegen_rowwise_adagrad_weighted_exact_pt2_cpu_wrapperS7_S7_S7_S7_S7_S7_S7_S7_lS7_lS7_S7_lS7_S7_llbllbbS5_S5_S5_S5_S5_dddldlEEEES5_NS_4guts8typelist8typelistIJS7_S7_S7_S7_S7_S7_S7_S7_lS7_lS7_S7_lS7_S7_llbllbbS5_S5_S5_S5_S5_dddldlEEEEE
 FN2at6TensorERKS0_S2_S2_S2_S2_S2_S2_S2_lS2_lS2_S2_lS2_S2_llbllbbS0_S0_S0_S0_S0_dddldlE
 N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorERKS5_S7_S7_S7_S7_S7_S7_S7_lS7_lS7_S7_lS7_S7_llbllbbS5_S5_S5_S5_S5_dddldlEXadL_Z81split_embedding_backward_codegen_rowwise_adagrad_unweighted_exact_pt2_cpu_wrapperS7_S7_S7_S7_S7_S7_S7_S7_lS7_lS7_S7_lS7_S7_llbllbbS5_S5_S5_S5_S5_dddldlEEEES5_NS_4guts8typelist8typelistIJS7_S7_S7_S7_S7_S7_S7_S7_lS7_lS7_S7_lS7_S7_llbllbbS5_S5_S5_S5_S5_dddldlEEEEE
 split_embedding_codegen_lookup_sgd_function_cpu(Tensor(a!) host_weights, Tensor weights_placements, Tensor weights_offsets, Tensor D_offsets, SymInt total_D, SymInt max_D, Tensor hash_size_cumsum, int total_hash_size_bits, Tensor indices, Tensor offsets, int pooling_mode, Tensor? indice_weights, Tensor? feature_requires_grad, bool gradient_clipping, float max_gradient, bool stochastic_rounding, float learning_rate = 0, int output_dtype=0) -> Tensor
 split_embedding_codegen_lookup_sgd_function_cpu
-/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.9/cmake-build/gen_embedding_backward_split_sgd_cpu.cpp
+/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.8/cmake-build/gen_embedding_backward_split_sgd_cpu.cpp
 fbgemm::split_embedding_backward_codegen_sgd_cpu
 *N5torch8autograd7CppNodeIN12_GLOBAL__N_126SplitLookupFunction_sgd_OpEEE
 *ZN5torch8autograd8FunctionIN12_GLOBAL__N_126SplitLookupFunction_sgd_OpEE5applyIS3_JRN2at6TensorES8_S8_S8_RN3c106SymIntESB_S8_RlS8_S8_SC_RSt8optionalIS7_ESF_RbRdSG_SH_SC_EEENSt9enable_ifIX9is_same_vIT_S3_EEDTclsrSJ_7forwardLDnEspcl7declvalIT0_EEEEE4typeEDpOSK_EUlRKSt6vectorIS7_SaIS7_EESU_E_
 *ZN5torch8autograd8FunctionIN12_GLOBAL__N_126SplitLookupFunction_sgd_OpEE5applyIS3_JRN2at6TensorES8_S8_S8_RN3c106SymIntESB_S8_RlS8_S8_SC_RSt8optionalIS7_ESF_RbRdSG_SH_SC_EEENSt9enable_ifIX9is_same_vIT_S3_EEDTclsrSJ_7forwardLDnEspcl7declvalIT0_EEEEE4typeEDpOSK_EUlRKS7_E0_
 *N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorES5_S5_S5_S5_NS_6SymIntES6_S5_lS5_S5_lSt8optionalIS5_ES8_bdbdlEXadL_ZN12_GLOBAL__N_147split_embedding_codegen_lookup_sgd_function_cpuES5_S5_S5_S5_S6_S6_S5_lS5_S5_lS8_S8_bdbdlEEEES5_NS_4guts8typelist8typelistIJS5_S5_S5_S5_S6_S6_S5_lS5_S5_lS8_S8_bdbdlEEEEE
 *St19_Sp_counted_deleterIPN5torch8autograd7CppNodeIN12_GLOBAL__N_126SplitLookupFunction_sgd_OpEEEPFvPNS1_4NodeEESaIvELN9__gnu_cxx12_Lock_policyE2EE
 FvN2at6TensorES0_S0_S0_S0_N3c106SymIntES0_lS0_S0_lS0_bdlE
 FvN2at6TensorES0_S0_S0_S0_lS0_lS0_S0_lS0_bdlE
 FN2at6TensorES0_S0_S0_S0_N3c106SymIntES2_S0_lS0_S0_lSt8optionalIS0_ES4_bdbdlE
-/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.9/cmake-build/gen_embedding_backward_split_sgd_pt2_cpu_wrapper.cpp
+/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.8/cmake-build/gen_embedding_backward_split_sgd_pt2_cpu_wrapper.cpp
 split_embedding_backward_codegen_sgd_weighted_exact_pt2_wrapper
 split_embedding_backward_codegen_sgd_unweighted_exact_pt2_wrapper
 N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorERKS5_S7_S7_S7_S7_S7_S7_S7_lS7_lS7_S7_lS7_S7_llbllbbdlEXadL_Z67split_embedding_backward_codegen_sgd_weighted_exact_pt2_cpu_wrapperS7_S7_S7_S7_S7_S7_S7_S7_lS7_lS7_S7_lS7_S7_llbllbbdlEEEES5_NS_4guts8typelist8typelistIJS7_S7_S7_S7_S7_S7_S7_S7_lS7_lS7_S7_lS7_S7_llbllbbdlEEEEE
 FN2at6TensorERKS0_S2_S2_S2_S2_S2_S2_S2_lS2_lS2_S2_lS2_S2_llbllbbdlE
 N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorERKS5_S7_S7_S7_S7_S7_S7_S7_lS7_lS7_S7_lS7_S7_llbllbbdlEXadL_Z69split_embedding_backward_codegen_sgd_unweighted_exact_pt2_cpu_wrapperS7_S7_S7_S7_S7_S7_S7_S7_lS7_lS7_S7_lS7_S7_llbllbbdlEEEES5_NS_4guts8typelist8typelistIJS7_S7_S7_S7_S7_S7_S7_S7_lS7_lS7_S7_lS7_S7_llbllbbdlEEEEE
 split_embedding_codegen_lookup_adam_function_cpu is deprecated. Please see https://github.com/pytorch/FBGEMM/discussions/1727 for more detail.
-/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.9/cmake-build/gen_embedding_backward_split_adam_cpu.cpp
+/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.8/cmake-build/gen_embedding_backward_split_adam_cpu.cpp
 split_embedding_codegen_lookup_adam_function_cpu
 split_embedding_codegen_lookup_adam_function_cpu(Tensor(a!) host_weights, Tensor weights_placements, Tensor weights_offsets, Tensor D_offsets, SymInt total_D, SymInt max_D, Tensor hash_size_cumsum, int total_hash_size_bits, Tensor indices, Tensor offsets, int pooling_mode, Tensor? indice_weights, Tensor? feature_requires_grad, bool gradient_clipping, float max_gradient, bool stochastic_rounding, Tensor momentum1_host, Tensor momentum1_placements, Tensor momentum1_offsets, Tensor momentum2_host, Tensor momentum2_placements, Tensor momentum2_offsets, float learning_rate = 0, float eps = 0, float beta1 = 0, float beta2 = 0, float weight_decay = 0, int iter = 0, int output_dtype=0) -> Tensor
 *N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorES5_S5_S5_S5_NS_6SymIntES6_S5_lS5_S5_lSt8optionalIS5_ES8_bdbS5_S5_S5_S5_S5_S5_dddddllEXadL_ZN12_GLOBAL__N_148split_embedding_codegen_lookup_adam_function_cpuES5_S5_S5_S5_S6_S6_S5_lS5_S5_lS8_S8_bdbS5_S5_S5_S5_S5_S5_dddddllEEEES5_NS_4guts8typelist8typelistIJS5_S5_S5_S5_S6_S6_S5_lS5_S5_lS8_S8_bdbS5_S5_S5_S5_S5_S5_dddddllEEEEE
 FN2at6TensorES0_S0_S0_S0_N3c106SymIntES2_S0_lS0_S0_lSt8optionalIS0_ES4_bdbS0_S0_S0_S0_S0_S0_dddddllE
 split_embedding_codegen_lookup_lamb_function_cpu is deprecated. Please see https://github.com/pytorch/FBGEMM/discussions/1727 for more detail.
-/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.9/cmake-build/gen_embedding_backward_split_lamb_cpu.cpp
+/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.8/cmake-build/gen_embedding_backward_split_lamb_cpu.cpp
 split_embedding_codegen_lookup_lamb_function_cpu
 split_embedding_codegen_lookup_lamb_function_cpu(Tensor(a!) host_weights, Tensor weights_placements, Tensor weights_offsets, Tensor D_offsets, SymInt total_D, SymInt max_D, Tensor hash_size_cumsum, int total_hash_size_bits, Tensor indices, Tensor offsets, int pooling_mode, Tensor? indice_weights, Tensor? feature_requires_grad, bool gradient_clipping, float max_gradient, bool stochastic_rounding, Tensor momentum1_host, Tensor momentum1_placements, Tensor momentum1_offsets, Tensor momentum2_host, Tensor momentum2_placements, Tensor momentum2_offsets, float learning_rate = 0, float eps = 0, float beta1 = 0, float beta2 = 0, float weight_decay = 0, int iter = 0, int output_dtype=0) -> Tensor
 *N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorES5_S5_S5_S5_NS_6SymIntES6_S5_lS5_S5_lSt8optionalIS5_ES8_bdbS5_S5_S5_S5_S5_S5_dddddllEXadL_ZN12_GLOBAL__N_148split_embedding_codegen_lookup_lamb_function_cpuES5_S5_S5_S5_S6_S6_S5_lS5_S5_lS8_S8_bdbS5_S5_S5_S5_S5_S5_dddddllEEEES5_NS_4guts8typelist8typelistIJS5_S5_S5_S5_S6_S6_S5_lS5_S5_lS8_S8_bdbS5_S5_S5_S5_S5_S5_dddddllEEEEE
 split_embedding_codegen_lookup_partial_rowwise_adam_function_cpu is deprecated. Please see https://github.com/pytorch/FBGEMM/discussions/1727 for more detail.
-/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.9/cmake-build/gen_embedding_backward_split_partial_rowwise_adam_cpu.cpp
+/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.8/cmake-build/gen_embedding_backward_split_partial_rowwise_adam_cpu.cpp
 split_embedding_codegen_lookup_partial_rowwise_adam_function_cpu
 split_embedding_codegen_lookup_partial_rowwise_adam_function_cpu(Tensor(a!) host_weights, Tensor weights_placements, Tensor weights_offsets, Tensor D_offsets, SymInt total_D, SymInt max_D, Tensor hash_size_cumsum, int total_hash_size_bits, Tensor indices, Tensor offsets, int pooling_mode, Tensor? indice_weights, Tensor? feature_requires_grad, bool gradient_clipping, float max_gradient, bool stochastic_rounding, Tensor momentum1_host, Tensor momentum1_placements, Tensor momentum1_offsets, Tensor momentum2_host, Tensor momentum2_placements, Tensor momentum2_offsets, float learning_rate = 0, float eps = 0, float beta1 = 0, float beta2 = 0, float weight_decay = 0, int iter = 0, int output_dtype=0) -> Tensor
 *N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorES5_S5_S5_S5_NS_6SymIntES6_S5_lS5_S5_lSt8optionalIS5_ES8_bdbS5_S5_S5_S5_S5_S5_dddddllEXadL_ZN12_GLOBAL__N_164split_embedding_codegen_lookup_partial_rowwise_adam_function_cpuES5_S5_S5_S5_S6_S6_S5_lS5_S5_lS8_S8_bdbS5_S5_S5_S5_S5_S5_dddddllEEEES5_NS_4guts8typelist8typelistIJS5_S5_S5_S5_S6_S6_S5_lS5_S5_lS8_S8_bdbS5_S5_S5_S5_S5_S5_dddddllEEEEE
 split_embedding_codegen_lookup_partial_rowwise_lamb_function_cpu is deprecated. Please see https://github.com/pytorch/FBGEMM/discussions/1727 for more detail.
-/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.9/cmake-build/gen_embedding_backward_split_partial_rowwise_lamb_cpu.cpp
+/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.8/cmake-build/gen_embedding_backward_split_partial_rowwise_lamb_cpu.cpp
 split_embedding_codegen_lookup_partial_rowwise_lamb_function_cpu
 split_embedding_codegen_lookup_partial_rowwise_lamb_function_cpu(Tensor(a!) host_weights, Tensor weights_placements, Tensor weights_offsets, Tensor D_offsets, SymInt total_D, SymInt max_D, Tensor hash_size_cumsum, int total_hash_size_bits, Tensor indices, Tensor offsets, int pooling_mode, Tensor? indice_weights, Tensor? feature_requires_grad, bool gradient_clipping, float max_gradient, bool stochastic_rounding, Tensor momentum1_host, Tensor momentum1_placements, Tensor momentum1_offsets, Tensor momentum2_host, Tensor momentum2_placements, Tensor momentum2_offsets, float learning_rate = 0, float eps = 0, float beta1 = 0, float beta2 = 0, float weight_decay = 0, int iter = 0, int output_dtype=0) -> Tensor
 *N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorES5_S5_S5_S5_NS_6SymIntES6_S5_lS5_S5_lSt8optionalIS5_ES8_bdbS5_S5_S5_S5_S5_S5_dddddllEXadL_ZN12_GLOBAL__N_164split_embedding_codegen_lookup_partial_rowwise_lamb_function_cpuES5_S5_S5_S5_S6_S6_S5_lS5_S5_lS8_S8_bdbS5_S5_S5_S5_S5_S5_dddddllEEEES5_NS_4guts8typelist8typelistIJS5_S5_S5_S5_S6_S6_S5_lS5_S5_lS8_S8_bdbS5_S5_S5_S5_S5_S5_dddddllEEEEE
 split_embedding_codegen_lookup_lars_sgd_function_cpu is deprecated. Please see https://github.com/pytorch/FBGEMM/discussions/1727 for more detail.
-/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.9/cmake-build/gen_embedding_backward_split_lars_sgd_cpu.cpp
+/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.8/cmake-build/gen_embedding_backward_split_lars_sgd_cpu.cpp
 split_embedding_codegen_lookup_lars_sgd_function_cpu
 split_embedding_codegen_lookup_lars_sgd_function_cpu(Tensor(a!) host_weights, Tensor weights_placements, Tensor weights_offsets, Tensor D_offsets, SymInt total_D, SymInt max_D, Tensor hash_size_cumsum, int total_hash_size_bits, Tensor indices, Tensor offsets, int pooling_mode, Tensor? indice_weights, Tensor? feature_requires_grad, bool gradient_clipping, float max_gradient, bool stochastic_rounding, Tensor momentum1_host, Tensor momentum1_placements, Tensor momentum1_offsets, float learning_rate = 0, float eta = 0, float momentum = 0, float weight_decay = 0, int output_dtype=0) -> Tensor
 *N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorES5_S5_S5_S5_NS_6SymIntES6_S5_lS5_S5_lSt8optionalIS5_ES8_bdbS5_S5_S5_ddddlEXadL_ZN12_GLOBAL__N_152split_embedding_codegen_lookup_lars_sgd_function_cpuES5_S5_S5_S5_S6_S6_S5_lS5_S5_lS8_S8_bdbS5_S5_S5_ddddlEEEES5_NS_4guts8typelist8typelistIJS5_S5_S5_S5_S6_S6_S5_lS5_S5_lS8_S8_bdbS5_S5_S5_ddddlEEEEE
 FN2at6TensorES0_S0_S0_S0_N3c106SymIntES2_S0_lS0_S0_lSt8optionalIS0_ES4_bdbS0_S0_S0_ddddlE
 split_embedding_codegen_lookup_none_function_cpu is deprecated. Please see https://github.com/pytorch/FBGEMM/discussions/1727 for more detail.
-/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.9/cmake-build/gen_embedding_backward_split_none_cpu.cpp
+/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.8/cmake-build/gen_embedding_backward_split_none_cpu.cpp
 split_embedding_codegen_lookup_none_function_cpu
 split_embedding_codegen_lookup_none_function_cpu(Tensor(a!) host_weights, Tensor weights_placements, Tensor weights_offsets, Tensor D_offsets, SymInt total_D, SymInt max_D, Tensor hash_size_cumsum, int total_hash_size_bits, Tensor indices, Tensor offsets, int pooling_mode, Tensor? indice_weights, Tensor? feature_requires_grad, bool gradient_clipping, float max_gradient, bool stochastic_rounding, int total_hash_size = 0, int total_unique_indices = 0, int output_dtype=0) -> Tensor
 *N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorES5_S5_S5_S5_NS_6SymIntES6_S5_lS5_S5_lSt8optionalIS5_ES8_bdblllEXadL_ZN12_GLOBAL__N_148split_embedding_codegen_lookup_none_function_cpuES5_S5_S5_S5_S6_S6_S5_lS5_S5_lS8_S8_bdblllEEEES5_NS_4guts8typelist8typelistIJS5_S5_S5_S5_S6_S6_S5_lS5_S5_lS8_S8_bdblllEEEEE
 FN2at6TensorES0_S0_S0_S0_N3c106SymIntES2_S0_lS0_S0_lSt8optionalIS0_ES4_bdblllE
 split_embedding_codegen_lookup_rowwise_adagrad_with_counter_function_cpu is deprecated. Please see https://github.com/pytorch/FBGEMM/discussions/1727 for more detail.
-/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.9/cmake-build/gen_embedding_backward_split_rowwise_adagrad_with_counter_cpu.cpp
+/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.8/cmake-build/gen_embedding_backward_split_rowwise_adagrad_with_counter_cpu.cpp
 split_embedding_codegen_lookup_rowwise_adagrad_with_counter_function_cpu
 split_embedding_codegen_lookup_rowwise_adagrad_with_counter_function_cpu(Tensor(a!) host_weights, Tensor weights_placements, Tensor weights_offsets, Tensor D_offsets, SymInt total_D, SymInt max_D, Tensor hash_size_cumsum, int total_hash_size_bits, Tensor indices, Tensor offsets, int pooling_mode, Tensor? indice_weights, Tensor? feature_requires_grad, bool gradient_clipping, float max_gradient, bool stochastic_rounding, Tensor momentum1_host, Tensor momentum1_placements, Tensor momentum1_offsets, Tensor prev_iter_host, Tensor prev_iter_placements, Tensor prev_iter_offsets, Tensor row_counter_host, Tensor row_counter_placements, Tensor row_counter_offsets, float eps = 0, float learning_rate = 0, float weight_decay = 0.0, int iter = 0, int counter_halflife = -1, int adjustment_iter = -1, float adjustment_ub = 1.0, int learning_rate_mode = -1, int weight_decay_mode = 1, int grad_sum_decay = -1, float max_counter = 0, float tail_id_threshold = 0.0, int is_tail_id_thresh_ratio = 0, int regularization_mode = 0, float weight_norm_coefficient = 0.0, float lower_bound = 0.0, int output_dtype=0) -> Tensor
 *N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorES5_S5_S5_S5_NS_6SymIntES6_S5_lS5_S5_lSt8optionalIS5_ES8_bdbS5_S5_S5_S5_S5_S5_S5_S5_S5_dddllldlllddllddlEXadL_ZN12_GLOBAL__N_172split_embedding_codegen_lookup_rowwise_adagrad_with_counter_function_cpuES5_S5_S5_S5_S6_S6_S5_lS5_S5_lS8_S8_bdbS5_S5_S5_S5_S5_S5_S5_S5_S5_dddllldlllddllddlEEEES5_NS_4guts8typelist8typelistIJS5_S5_S5_S5_S6_S6_S5_lS5_S5_lS8_S8_bdbS5_S5_S5_S5_S5_S5_S5_S5_S5_dddllldlllddllddlEEEEE
 FN2at6TensorES0_S0_S0_S0_N3c106SymIntES2_S0_lS0_S0_lSt8optionalIS0_ES4_bdbS0_S0_S0_S0_S0_S0_S0_S0_S0_dddllldlllddllddlE
 split_embedding_codegen_lookup_approx_sgd_function_cpu is deprecated. Please see https://github.com/pytorch/FBGEMM/discussions/1727 for more detail.
-/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.9/cmake-build/gen_embedding_backward_split_approx_sgd_cpu.cpp
+/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.8/cmake-build/gen_embedding_backward_split_approx_sgd_cpu.cpp
 split_embedding_codegen_lookup_approx_sgd_function_cpu
 split_embedding_codegen_lookup_approx_sgd_function_cpu(Tensor(a!) host_weights, Tensor weights_placements, Tensor weights_offsets, Tensor D_offsets, SymInt total_D, SymInt max_D, Tensor hash_size_cumsum, int total_hash_size_bits, Tensor indices, Tensor offsets, int pooling_mode, Tensor? indice_weights, Tensor? feature_requires_grad, bool gradient_clipping, float max_gradient, bool stochastic_rounding, float learning_rate = 0, int output_dtype=0) -> Tensor
 *N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorES5_S5_S5_S5_NS_6SymIntES6_S5_lS5_S5_lSt8optionalIS5_ES8_bdbdlEXadL_ZN12_GLOBAL__N_154split_embedding_codegen_lookup_approx_sgd_function_cpuES5_S5_S5_S5_S6_S6_S5_lS5_S5_lS8_S8_bdbdlEEEES5_NS_4guts8typelist8typelistIJS5_S5_S5_S5_S6_S6_S5_lS5_S5_lS8_S8_bdbdlEEEEE
 split_embedding_codegen_lookup_approx_rowwise_adagrad_function_cpu is deprecated. Please see https://github.com/pytorch/FBGEMM/discussions/1727 for more detail.
-/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.9/cmake-build/gen_embedding_backward_split_approx_rowwise_adagrad_cpu.cpp
+/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.8/cmake-build/gen_embedding_backward_split_approx_rowwise_adagrad_cpu.cpp
 split_embedding_codegen_lookup_approx_rowwise_adagrad_function_cpu
 split_embedding_codegen_lookup_approx_rowwise_adagrad_function_cpu(Tensor(a!) host_weights, Tensor weights_placements, Tensor weights_offsets, Tensor D_offsets, SymInt total_D, SymInt max_D, Tensor hash_size_cumsum, int total_hash_size_bits, Tensor indices, Tensor offsets, int pooling_mode, Tensor? indice_weights, Tensor? feature_requires_grad, bool gradient_clipping, float max_gradient, bool stochastic_rounding, Tensor momentum1_host, Tensor momentum1_placements, Tensor momentum1_offsets, float eps = 0, float learning_rate = 0, float weight_decay = 0.0, int weight_decay_mode = 0, int output_dtype=0) -> Tensor
 *N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorES5_S5_S5_S5_NS_6SymIntES6_S5_lS5_S5_lSt8optionalIS5_ES8_bdbS5_S5_S5_dddllEXadL_ZN12_GLOBAL__N_166split_embedding_codegen_lookup_approx_rowwise_adagrad_function_cpuES5_S5_S5_S5_S6_S6_S5_lS5_S5_lS8_S8_bdbS5_S5_S5_dddllEEEES5_NS_4guts8typelist8typelistIJS5_S5_S5_S5_S6_S6_S5_lS5_S5_lS8_S8_bdbS5_S5_S5_dddllEEEEE
 FN2at6TensorES0_S0_S0_S0_N3c106SymIntES2_S0_lS0_S0_lSt8optionalIS0_ES4_bdbS0_S0_S0_dddllE
 split_embedding_codegen_lookup_approx_rowwise_adagrad_with_counter_function_cpu is deprecated. Please see https://github.com/pytorch/FBGEMM/discussions/1727 for more detail.
-/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.9/cmake-build/gen_embedding_backward_split_approx_rowwise_adagrad_with_counter_cpu.cpp
+/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.8/cmake-build/gen_embedding_backward_split_approx_rowwise_adagrad_with_counter_cpu.cpp
 split_embedding_codegen_lookup_approx_rowwise_adagrad_with_counter_function_cpu
 split_embedding_codegen_lookup_approx_rowwise_adagrad_with_counter_function_cpu(Tensor(a!) host_weights, Tensor weights_placements, Tensor weights_offsets, Tensor D_offsets, SymInt total_D, SymInt max_D, Tensor hash_size_cumsum, int total_hash_size_bits, Tensor indices, Tensor offsets, int pooling_mode, Tensor? indice_weights, Tensor? feature_requires_grad, bool gradient_clipping, float max_gradient, bool stochastic_rounding, Tensor momentum1_host, Tensor momentum1_placements, Tensor momentum1_offsets, Tensor prev_iter_host, Tensor prev_iter_placements, Tensor prev_iter_offsets, Tensor row_counter_host, Tensor row_counter_placements, Tensor row_counter_offsets, float eps = 0, float learning_rate = 0, float weight_decay = 0.0, int iter = 0, int counter_halflife = -1, int adjustment_iter = -1, float adjustment_ub = 1.0, int learning_rate_mode = -1, int weight_decay_mode = 1, int grad_sum_decay = -1, float max_counter = 0, float tail_id_threshold = 0.0, int is_tail_id_thresh_ratio = 0, int regularization_mode = 0, float weight_norm_coefficient = 0.0, float lower_bound = 0.0, int output_dtype=0) -> Tensor
 *N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorES5_S5_S5_S5_NS_6SymIntES6_S5_lS5_S5_lSt8optionalIS5_ES8_bdbS5_S5_S5_S5_S5_S5_S5_S5_S5_dddllldlllddllddlEXadL_ZN12_GLOBAL__N_179split_embedding_codegen_lookup_approx_rowwise_adagrad_with_counter_function_cpuES5_S5_S5_S5_S6_S6_S5_lS5_S5_lS8_S8_bdbS5_S5_S5_S5_S5_S5_S5_S5_S5_dddllldlllddllddlEEEES5_NS_4guts8typelist8typelistIJS5_S5_S5_S5_S6_S6_S5_lS5_S5_lS8_S8_bdbS5_S5_S5_S5_S5_S5_S5_S5_S5_dddllldlllddllddlEEEEE
 split_embedding_codegen_lookup_approx_rowwise_adagrad_with_weight_decay_function_cpu is deprecated. Please see https://github.com/pytorch/FBGEMM/discussions/1727 for more detail.
-/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.9/cmake-build/gen_embedding_backward_split_approx_rowwise_adagrad_with_weight_decay_cpu.cpp
+/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.8/cmake-build/gen_embedding_backward_split_approx_rowwise_adagrad_with_weight_decay_cpu.cpp
 split_embedding_codegen_lookup_approx_rowwise_adagrad_with_weight_decay_function_cpu
 split_embedding_codegen_lookup_approx_rowwise_adagrad_with_weight_decay_function_cpu(Tensor(a!) host_weights, Tensor weights_placements, Tensor weights_offsets, Tensor D_offsets, SymInt total_D, SymInt max_D, Tensor hash_size_cumsum, int total_hash_size_bits, Tensor indices, Tensor offsets, int pooling_mode, Tensor? indice_weights, Tensor? feature_requires_grad, bool gradient_clipping, float max_gradient, bool stochastic_rounding, Tensor momentum1_host, Tensor momentum1_placements, Tensor momentum1_offsets, float eps = 0, float learning_rate = 0, float weight_decay = 0.0, int weight_decay_mode = 0, int output_dtype=0) -> Tensor
 *N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorES5_S5_S5_S5_NS_6SymIntES6_S5_lS5_S5_lSt8optionalIS5_ES8_bdbS5_S5_S5_dddllEXadL_ZN12_GLOBAL__N_184split_embedding_codegen_lookup_approx_rowwise_adagrad_with_weight_decay_function_cpuES5_S5_S5_S5_S6_S6_S5_lS5_S5_lS8_S8_bdbS5_S5_S5_dddllEEEES5_NS_4guts8typelist8typelistIJS5_S5_S5_S5_S6_S6_S5_lS5_S5_lS8_S8_bdbS5_S5_S5_dddllEEEEE
 split_embedding_codegen_lookup_rowwise_adagrad_with_weight_decay_function_cpu is deprecated. Please see https://github.com/pytorch/FBGEMM/discussions/1727 for more detail.
-/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.9/cmake-build/gen_embedding_backward_split_rowwise_adagrad_with_weight_decay_cpu.cpp
+/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.8/cmake-build/gen_embedding_backward_split_rowwise_adagrad_with_weight_decay_cpu.cpp
 split_embedding_codegen_lookup_rowwise_adagrad_with_weight_decay_function_cpu
 split_embedding_codegen_lookup_rowwise_adagrad_with_weight_decay_function_cpu(Tensor(a!) host_weights, Tensor weights_placements, Tensor weights_offsets, Tensor D_offsets, SymInt total_D, SymInt max_D, Tensor hash_size_cumsum, int total_hash_size_bits, Tensor indices, Tensor offsets, int pooling_mode, Tensor? indice_weights, Tensor? feature_requires_grad, bool gradient_clipping, float max_gradient, bool stochastic_rounding, Tensor momentum1_host, Tensor momentum1_placements, Tensor momentum1_offsets, float eps = 0, float learning_rate = 0, float weight_decay = 0.0, int weight_decay_mode = 0, int output_dtype=0) -> Tensor
 *N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorES5_S5_S5_S5_NS_6SymIntES6_S5_lS5_S5_lSt8optionalIS5_ES8_bdbS5_S5_S5_dddllEXadL_ZN12_GLOBAL__N_177split_embedding_codegen_lookup_rowwise_adagrad_with_weight_decay_function_cpuES5_S5_S5_S5_S6_S6_S5_lS5_S5_lS8_S8_bdbS5_S5_S5_dddllEEEES5_NS_4guts8typelist8typelistIJS5_S5_S5_S5_S6_S6_S5_lS5_S5_lS8_S8_bdbS5_S5_S5_dddllEEEEE
 split_embedding_codegen_lookup_rowwise_weighted_adagrad_function_cpu is deprecated. Please see https://github.com/pytorch/FBGEMM/discussions/1727 for more detail.
-/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.9/cmake-build/gen_embedding_backward_split_rowwise_weighted_adagrad_cpu.cpp
+/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.8/cmake-build/gen_embedding_backward_split_rowwise_weighted_adagrad_cpu.cpp
 split_embedding_codegen_lookup_rowwise_weighted_adagrad_function_cpu
 split_embedding_codegen_lookup_rowwise_weighted_adagrad_function_cpu(Tensor(a!) host_weights, Tensor weights_placements, Tensor weights_offsets, Tensor D_offsets, SymInt total_D, SymInt max_D, Tensor hash_size_cumsum, int total_hash_size_bits, Tensor indices, Tensor offsets, int pooling_mode, Tensor? indice_weights, Tensor? feature_requires_grad, bool gradient_clipping, float max_gradient, bool stochastic_rounding, Tensor momentum1_host, Tensor momentum1_placements, Tensor momentum1_offsets, float eps = 0, float learning_rate = 0, float weight_decay = 0, int iter = 0, int output_dtype=0) -> Tensor
 *N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFN2at6TensorES5_S5_S5_S5_NS_6SymIntES6_S5_lS5_S5_lSt8optionalIS5_ES8_bdbS5_S5_S5_dddllEXadL_ZN12_GLOBAL__N_168split_embedding_codegen_lookup_rowwise_weighted_adagrad_function_cpuES5_S5_S5_S5_S6_S6_S5_lS5_S5_lS8_S8_bdbS5_S5_S5_dddllEEEES5_NS_4guts8typelist8typelistIJS5_S5_S5_S5_S6_S6_S5_lS5_S5_lS8_S8_bdbS5_S5_S5_dddllEEEEE
-/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.9/cmake-build/gen_embedding_backward_adagrad_split_cpu.cpp
+/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.8/cmake-build/gen_embedding_backward_adagrad_split_cpu.cpp
 split_embedding_backward_exact_cpu_outer
 CPU exact rowwise adagrad currently doesn't support embedding tables with more than 2B rows
 split_embedding_backward_codegen_adagrad_cpu(Tensor grad_output, Tensor(a!) host_weights, Tensor weights_placements, Tensor weights_offsets, Tensor D_offsets, int max_D, Tensor hash_size_cumsum, int total_hash_size_bits, Tensor indices, Tensor offsets,int pooling_mode, Tensor indice_weights, bool stochastic_rounding, Tensor(b!) momentum1_host, Tensor momentum1_placements, Tensor momentum1_offsets, float eps = 0, float learning_rate = 0, int output_dtype = 0) -> ()
 N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFvN2at6TensorES5_S5_S5_S5_lS5_lS5_S5_lS5_bS5_S5_S5_ddlEXadL_Z44split_embedding_backward_codegen_adagrad_cpuS5_S5_S5_S5_S5_lS5_lS5_S5_lS5_bS5_S5_S5_ddlEEEEvNS_4guts8typelist8typelistIJS5_S5_S5_S5_S5_lS5_lS5_S5_lS5_bS5_S5_S5_ddlEEEEE
 does not match c_block size: 
 num of rows processed by adagrad: 
-/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.9/cmake-build/gen_embedding_backward_rowwise_adagrad_split_cpu.cpp
+/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.8/cmake-build/gen_embedding_backward_rowwise_adagrad_split_cpu.cpp
 split_embedding_backward_codegen_rowwise_adagrad_cpu(Tensor grad_output, Tensor(a!) host_weights, Tensor weights_placements, Tensor weights_offsets, Tensor D_offsets, int max_D, Tensor hash_size_cumsum, int total_hash_size_bits, Tensor indices, Tensor offsets,int pooling_mode, Tensor indice_weights, bool stochastic_rounding, Tensor(b!) momentum1_host, Tensor momentum1_placements, Tensor momentum1_offsets, float eps = 0, float learning_rate = 0, float weight_decay = 0.0, int weight_decay_mode = 0, float max_norm = 0.0, int output_dtype = 0) -> ()
 N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFvN2at6TensorES5_S5_S5_S5_lS5_lS5_S5_lS5_bS5_S5_S5_dddldlEXadL_Z52split_embedding_backward_codegen_rowwise_adagrad_cpuS5_S5_S5_S5_S5_lS5_lS5_S5_lS5_bS5_S5_S5_dddldlEEEEvNS_4guts8typelist8typelistIJS5_S5_S5_S5_S5_lS5_lS5_S5_lS5_bS5_S5_S5_dddldlEEEEE
-/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.9/cmake-build/gen_embedding_backward_sgd_split_cpu.cpp
+/__w/FBGEMM/FBGEMM/fbgemm_gpu/_skbuild/linux-x86_64-3.8/cmake-build/gen_embedding_backward_sgd_split_cpu.cpp
 split_embedding_backward_codegen_sgd_cpu(Tensor grad_output, Tensor(a!) host_weights, Tensor weights_placements, Tensor weights_offsets, Tensor D_offsets, int max_D, Tensor hash_size_cumsum, int total_hash_size_bits, Tensor indices, Tensor offsets,int pooling_mode, Tensor indice_weights, bool stochastic_rounding, float learning_rate = 0, int output_dtype = 0) -> ()
 N3c104impl6detail24WrapFunctionIntoFunctor_INS_26CompileTimeFunctionPointerIFvN2at6TensorES5_S5_S5_S5_lS5_lS5_S5_lS5_bdlEXadL_Z40split_embedding_backward_codegen_sgd_cpuS5_S5_S5_S5_S5_lS5_lS5_S5_lS5_bdlEEEEvNS_4guts8typelist8typelistIJS5_S5_S5_S5_S5_lS5_lS5_S5_lS5_bdlEEEEE
 GCC: (conda-forge gcc 10.4.0-19) 10.4.0
 .shstrtab
 .gnu.hash
 .gnu.version
 .gnu.version_r
```

### readelf --wide --decompress --hex-dump=.rodata {}

```diff
@@ -10695,24 +10695,24 @@
   0x00945c40 78747261 5f6d6574 615f2d3e 73796d62 xtra_meta_->symb
   0x00945c50 6f6c6963 5f736861 70655f6d 6574615f olic_shape_meta_
   0x00945c60 20494e54 45524e41 4c204153 53455254  INTERNAL ASSERT
   0x00945c70 20464149 4c454420 61742022 2f676974  FAILED at "/git
   0x00945c80 6875622f 686f6d65 2f6d696e 69636f6e hub/home/minicon
   0x00945c90 64612f65 6e76732f 6275696c 645f6269 da/envs/build_bi
   0x00945ca0 6e617279 2f6c6962 2f707974 686f6e33 nary/lib/python3
-  0x00945cb0 2e392f73 6974652d 7061636b 61676573 .9/site-packages
+  0x00945cb0 2e382f73 6974652d 7061636b 61676573 .8/site-packages
   0x00945cc0 2f746f72 63682f69 6e636c75 64652f63 /torch/include/c
   0x00945cd0 31302f63 6f72652f 54656e73 6f72496d 10/core/TensorIm
   0x00945ce0 706c2e68 223a3137 31392c20 706c6561 pl.h":1719, plea
   0x00945cf0 73652072 65706f72 74206120 62756720 se report a bug 
   0x00945d00 746f2050 79546f72 63682e20 00000000 to PyTorch. ....
   0x00945d10 2f676974 6875622f 686f6d65 2f6d696e /github/home/min
   0x00945d20 69636f6e 64612f65 6e76732f 6275696c iconda/envs/buil
   0x00945d30 645f6269 6e617279 2f6c6962 2f707974 d_binary/lib/pyt
-  0x00945d40 686f6e33 2e392f73 6974652d 7061636b hon3.9/site-pack
+  0x00945d40 686f6e33 2e382f73 6974652d 7061636b hon3.8/site-pack
   0x00945d50 61676573 2f746f72 63682f69 6e636c75 ages/torch/inclu
   0x00945d60 64652f63 31302f63 6f72652f 54656e73 de/c10/core/Tens
   0x00945d70 6f72496d 706c2e68 00000000 00000000 orImpl.h........
   0x00945d80 2f5f5f77 2f464247 454d4d2f 46424745 /__w/FBGEMM/FBGE
   0x00945d90 4d4d2f66 6267656d 6d5f6770 752f636f MM/fbgemm_gpu/co
   0x00945da0 64656765 6e2f7472 61696e69 6e672f66 degen/training/f
   0x00945db0 6f727761 72642f65 6d626564 64696e67 orward/embedding
@@ -10787,15 +10787,15 @@
   0x00946200 206c6179 6f757420 63616c63 756c6174  layout calculat
   0x00946210 696f6e20 6c6f6769 632e0000 00000000 ion logic.......
   0x00946220 69735f6d 6b6c646e 6e282920 494e5445 is_mkldnn() INTE
   0x00946230 524e414c 20415353 45525420 4641494c RNAL ASSERT FAIL
   0x00946240 45442061 7420222f 67697468 75622f68 ED at "/github/h
   0x00946250 6f6d652f 6d696e69 636f6e64 612f656e ome/miniconda/en
   0x00946260 76732f62 75696c64 5f62696e 6172792f vs/build_binary/
-  0x00946270 6c69622f 70797468 6f6e332e 392f7369 lib/python3.9/si
+  0x00946270 6c69622f 70797468 6f6e332e 382f7369 lib/python3.8/si
   0x00946280 74652d70 61636b61 6765732f 746f7263 te-packages/torc
   0x00946290 682f696e 636c7564 652f6331 302f636f h/include/c10/co
   0x009462a0 72652f54 656e736f 72496d70 6c2e6822 re/TensorImpl.h"
   0x009462b0 3a313239 302c2070 6c656173 65207265 :1290, please re
   0x009462c0 706f7274 20612062 75672074 6f205079 port a bug to Py
   0x009462d0 546f7263 682e2000 4f706572 61746f72 Torch. .Operator
   0x009462e0 73207461 6b696e67 2054656e 736f724f s taking TensorO
@@ -10804,15 +10804,15 @@
   0x00946310 6e732077 69746820 6f707469 6f6e732e ns with options.
   0x00946320 72657175 69726573 5f677261 64207365 requires_grad se
   0x00946330 74206173 20747275 652e2054 68697320 t as true. This 
   0x00946340 69736e27 7420696d 706c656d 656e7465 isn't implemente
   0x00946350 64207965 742e0000 2f676974 6875622f d yet.../github/
   0x00946360 686f6d65 2f6d696e 69636f6e 64612f65 home/miniconda/e
   0x00946370 6e76732f 6275696c 645f6269 6e617279 nvs/build_binary
-  0x00946380 2f6c6962 2f707974 686f6e33 2e392f73 /lib/python3.9/s
+  0x00946380 2f6c6962 2f707974 686f6e33 2e382f73 /lib/python3.8/s
   0x00946390 6974652d 7061636b 61676573 2f746f72 ite-packages/tor
   0x009463a0 63682f69 6e636c75 64652f41 54656e2f ch/include/ATen/
   0x009463b0 636f7265 2f436865 636b4d65 6d6f7279 core/CheckMemory
   0x009463c0 466f726d 61742e68 00000000 00000000 Format.h........
   0x009463d0 63686563 6b5f7465 6e736f72 5f6f7074 check_tensor_opt
   0x009463e0 696f6e73 5f616e64 5f657874 72616374 ions_and_extract
   0x009463f0 5f6d656d 6f72795f 666f726d 61740000 _memory_format..
@@ -10830,27 +10830,27 @@
   0x009464b0 496e7441 72726179 52656620 636f6e74 IntArrayRef cont
   0x009464c0 61696e73 20616e20 696e7420 74686174 ains an int that
   0x009464d0 2063616e 6e6f7420 62652072 65707265  cannot be repre
   0x009464e0 73656e74 65642061 73206120 53796d49 sented as a SymI
   0x009464f0 6e743a20 00000000 2f676974 6875622f nt: ..../github/
   0x00946500 686f6d65 2f6d696e 69636f6e 64612f65 home/miniconda/e
   0x00946510 6e76732f 6275696c 645f6269 6e617279 nvs/build_binary
-  0x00946520 2f6c6962 2f707974 686f6e33 2e392f73 /lib/python3.9/s
+  0x00946520 2f6c6962 2f707974 686f6e33 2e382f73 /lib/python3.8/s
   0x00946530 6974652d 7061636b 61676573 2f746f72 ite-packages/tor
   0x00946540 63682f69 6e636c75 64652f63 31302f63 ch/include/c10/c
   0x00946550 6f72652f 53796d49 6e744172 72617952 ore/SymIntArrayR
   0x00946560 65662e68 0066726f 6d496e74 41727261 ef.h.fromIntArra
   0x00946570 79526566 536c6f77 00206469 6d732062 yRefSlow. dims b
   0x00946580 75742074 656e736f 72206861 73200054 ut tensor has .T
   0x00946590 656e736f 72416363 6573736f 72206578 ensorAccessor ex
   0x009465a0 70656374 65642000 61636365 73736f72 pected .accessor
   0x009465b0 00000000 00000000 2f676974 6875622f ......../github/
   0x009465c0 686f6d65 2f6d696e 69636f6e 64612f65 home/miniconda/e
   0x009465d0 6e76732f 6275696c 645f6269 6e617279 nvs/build_binary
-  0x009465e0 2f6c6962 2f707974 686f6e33 2e392f73 /lib/python3.9/s
+  0x009465e0 2f6c6962 2f707974 686f6e33 2e382f73 /lib/python3.8/s
   0x009465f0 6974652d 7061636b 61676573 2f746f72 ite-packages/tor
   0x00946600 63682f69 6e636c75 64652f41 54656e2f ch/include/ATen/
   0x00946610 636f7265 2f54656e 736f7242 6173652e core/TensorBase.
   0x00946620 68002d31 00496e64 65782000 20697320 h.-1.Index . is 
   0x00946630 6f757420 6f662062 6f756e64 733a2000 out of bounds: .
   0x00946640 2c207261 6e676520 0020746f 20007265 , range . to .re
   0x00946650 706f7274 5f656d62 65646469 6e675f65 port_embedding_e
@@ -10861,45 +10861,45 @@
   0x009466a0 6c732e68 00766563 746f723a 3a5f4d5f ls.h.vector::_M_
   0x009466b0 7265616c 6c6f635f 696e7365 72740000 realloc_insert..
   0x009466c0 6973496e 74282920 494e5445 524e414c isInt() INTERNAL
   0x009466d0 20415353 45525420 4641494c 45442061  ASSERT FAILED a
   0x009466e0 7420222f 67697468 75622f68 6f6d652f t "/github/home/
   0x009466f0 6d696e69 636f6e64 612f656e 76732f62 miniconda/envs/b
   0x00946700 75696c64 5f62696e 6172792f 6c69622f uild_binary/lib/
-  0x00946710 70797468 6f6e332e 392f7369 74652d70 python3.9/site-p
+  0x00946710 70797468 6f6e332e 382f7369 74652d70 python3.8/site-p
   0x00946720 61636b61 6765732f 746f7263 682f696e ackages/torch/in
   0x00946730 636c7564 652f4154 656e2f63 6f72652f clude/ATen/core/
   0x00946740 6976616c 75652e68 223a3634 322c2070 ivalue.h":642, p
   0x00946750 6c656173 65207265 706f7274 20612062 lease report a b
   0x00946760 75672074 6f205079 546f7263 682e2000 ug to PyTorch. .
   0x00946770 2f676974 6875622f 686f6d65 2f6d696e /github/home/min
   0x00946780 69636f6e 64612f65 6e76732f 6275696c iconda/envs/buil
   0x00946790 645f6269 6e617279 2f6c6962 2f707974 d_binary/lib/pyt
-  0x009467a0 686f6e33 2e392f73 6974652d 7061636b hon3.9/site-pack
+  0x009467a0 686f6e33 2e382f73 6974652d 7061636b hon3.8/site-pack
   0x009467b0 61676573 2f746f72 63682f69 6e636c75 ages/torch/inclu
   0x009467c0 64652f41 54656e2f 636f7265 2f697661 de/ATen/core/iva
   0x009467d0 6c75652e 68000000 45787065 63746564 lue.h...Expected
   0x009467e0 2053796d 496e7420 6f722069 6e742062  SymInt or int b
   0x009467f0 75742067 6f742000 69735379 6d496e74 ut got .isSymInt
   0x00946800 2829207c 7c206973 496e7428 2920494e () || isInt() IN
   0x00946810 5445524e 414c2041 53534552 54204641 TERNAL ASSERT FA
   0x00946820 494c4544 20617420 222f6769 74687562 ILED at "/github
   0x00946830 2f686f6d 652f6d69 6e69636f 6e64612f /home/miniconda/
   0x00946840 656e7673 2f627569 6c645f62 696e6172 envs/build_binar
-  0x00946850 792f6c69 622f7079 74686f6e 332e392f y/lib/python3.9/
+  0x00946850 792f6c69 622f7079 74686f6e 332e382f y/lib/python3.8/
   0x00946860 73697465 2d706163 6b616765 732f746f site-packages/to
   0x00946870 7263682f 696e636c 7564652f 4154656e rch/include/ATen
   0x00946880 2f636f72 652f6976 616c7565 5f696e6c /core/ivalue_inl
   0x00946890 2e68223a 3233372c 20706c65 61736520 .h":237, please 
   0x009468a0 7265706f 72742061 20627567 20746f20 report a bug to 
   0x009468b0 5079546f 7263682e 20000000 00000000 PyTorch. .......
   0x009468c0 2f676974 6875622f 686f6d65 2f6d696e /github/home/min
   0x009468d0 69636f6e 64612f65 6e76732f 6275696c iconda/envs/buil
   0x009468e0 645f6269 6e617279 2f6c6962 2f707974 d_binary/lib/pyt
-  0x009468f0 686f6e33 2e392f73 6974652d 7061636b hon3.9/site-pack
+  0x009468f0 686f6e33 2e382f73 6974652d 7061636b hon3.8/site-pack
   0x00946900 61676573 2f746f72 63682f69 6e636c75 ages/torch/inclu
   0x00946910 64652f41 54656e2f 636f7265 2f697661 de/ATen/core/iva
   0x00946920 6c75655f 696e6c2e 6800746f 496e7400 lue_inl.h.toInt.
   0x00946930 746f5379 6d496e74 00000000 00000000 toSymInt........
   0x00946940 53743139 6261645f 6f707469 6f6e616c St19bad_optional
   0x00946950 5f616363 65737300 00000000 00000000 _access.........
   0x00946960 4e336331 30323069 6e747275 73697665 N3c1020intrusive
@@ -11030,28 +11030,28 @@
   0x00947130 6e642000 20646576 69636573 00676574 nd . devices.get
   0x00947140 44657669 63654775 61726449 6d706c00 DeviceGuardImpl.
   0x00947150 5079546f 72636820 6973206e 6f74206c PyTorch is not l
   0x00947160 696e6b65 64207769 74682073 7570706f inked with suppo
   0x00947170 72742066 6f722000 2f676974 6875622f rt for ./github/
   0x00947180 686f6d65 2f6d696e 69636f6e 64612f65 home/miniconda/e
   0x00947190 6e76732f 6275696c 645f6269 6e617279 nvs/build_binary
-  0x009471a0 2f6c6962 2f707974 686f6e33 2e392f73 /lib/python3.9/s
+  0x009471a0 2f6c6962 2f707974 686f6e33 2e382f73 /lib/python3.8/s
   0x009471b0 6974652d 7061636b 61676573 2f746f72 ite-packages/tor
   0x009471c0 63682f69 6e636c75 64652f63 31302f63 ch/include/c10/c
   0x009471d0 6f72652f 696d706c 2f446576 69636547 ore/impl/DeviceG
   0x009471e0 75617264 496d706c 496e7465 72666163 uardImplInterfac
   0x009471f0 652e6800 4576656e 74206465 76696365 e.h.Event device
   0x00947200 20747970 65200062 6c6f636b 00000000  type .block....
   0x00947210 20646f65 73206e6f 74206d61 74636820  does not match 
   0x00947220 626c6f63 6b696e67 20737472 65616d27 blocking stream'
   0x00947230 73206465 76696365 20747970 65200000 s device type ..
   0x00947240 2f676974 6875622f 686f6d65 2f6d696e /github/home/min
   0x00947250 69636f6e 64612f65 6e76732f 6275696c iconda/envs/buil
   0x00947260 645f6269 6e617279 2f6c6962 2f707974 d_binary/lib/pyt
-  0x00947270 686f6e33 2e392f73 6974652d 7061636b hon3.9/site-pack
+  0x00947270 686f6e33 2e382f73 6974652d 7061636b hon3.8/site-pack
   0x00947280 61676573 2f746f72 63682f69 6e636c75 ages/torch/inclu
   0x00947290 64652f63 31302f63 6f72652f 696d706c de/c10/core/impl
   0x009472a0 2f496e6c 696e6545 76656e74 2e680000 /InlineEvent.h..
   0x009472b0 45787065 63746564 20216e61 6d652e65 Expected !name.e
   0x009472c0 6d707479 28292074 6f206265 20747275 mpty() to be tru
   0x009472d0 652c2062 75742067 6f742066 616c7365 e, but got false
   0x009472e0 2e202028 436f756c 64207468 69732065 .  (Could this e
@@ -11059,49 +11059,49 @@
   0x00947300 696d7072 6f766564 3f202049 6620736f improved?  If so
   0x00947310 2c20706c 65617365 20726570 6f727420 , please report 
   0x00947320 616e2065 6e68616e 63656d65 6e742072 an enhancement r
   0x00947330 65717565 73742074 6f205079 546f7263 equest to PyTorc
   0x00947340 682e2900 00000000 2f676974 6875622f h.)...../github/
   0x00947350 686f6d65 2f6d696e 69636f6e 64612f65 home/miniconda/e
   0x00947360 6e76732f 6275696c 645f6269 6e617279 nvs/build_binary
-  0x00947370 2f6c6962 2f707974 686f6e33 2e392f73 /lib/python3.9/s
+  0x00947370 2f6c6962 2f707974 686f6e33 2e382f73 /lib/python3.8/s
   0x00947380 6974652d 7061636b 61676573 2f746f72 ite-packages/tor
   0x00947390 63682f69 6e636c75 64652f41 54656e2f ch/include/ATen/
   0x009473a0 636f7265 2f717561 6c696669 65645f6e core/qualified_n
   0x009473b0 616d652e 68000000 496e7661 6c696420 ame.h...Invalid 
   0x009473c0 6e616d65 20666f72 20717561 6c696669 name for qualifi
   0x009473d0 6564206e 616d653a 20270000 00000000 ed name: '......
   0x009473e0 2161746f 6d2e656d 70747928 2920494e !atom.empty() IN
   0x009473f0 5445524e 414c2041 53534552 54204641 TERNAL ASSERT FA
   0x00947400 494c4544 20617420 222f6769 74687562 ILED at "/github
   0x00947410 2f686f6d 652f6d69 6e69636f 6e64612f /home/miniconda/
   0x00947420 656e7673 2f627569 6c645f62 696e6172 envs/build_binar
-  0x00947430 792f6c69 622f7079 74686f6e 332e392f y/lib/python3.9/
+  0x00947430 792f6c69 622f7079 74686f6e 332e382f y/lib/python3.8/
   0x00947440 73697465 2d706163 6b616765 732f746f site-packages/to
   0x00947450 7263682f 696e636c 7564652f 4154656e rch/include/ATen
   0x00947460 2f636f72 652f7175 616c6966 6965645f /core/qualified_
   0x00947470 6e616d65 2e68223a 32342c20 706c6561 name.h":24, plea
   0x00947480 73652072 65706f72 74206120 62756720 se report a bug 
   0x00947490 746f2050 79546f72 63682e20 00000000 to PyTorch. ....
   0x009474a0 2166696e 616c4174 6f6d2e65 6d707479 !finalAtom.empty
   0x009474b0 28292049 4e544552 4e414c20 41535345 () INTERNAL ASSE
   0x009474c0 52542046 41494c45 44206174 20222f67 RT FAILED at "/g
   0x009474d0 69746875 622f686f 6d652f6d 696e6963 ithub/home/minic
   0x009474e0 6f6e6461 2f656e76 732f6275 696c645f onda/envs/build_
   0x009474f0 62696e61 72792f6c 69622f70 7974686f binary/lib/pytho
-  0x00947500 6e332e39 2f736974 652d7061 636b6167 n3.9/site-packag
+  0x00947500 6e332e38 2f736974 652d7061 636b6167 n3.8/site-packag
   0x00947510 65732f74 6f726368 2f696e63 6c756465 es/torch/include
   0x00947520 2f415465 6e2f636f 72652f71 75616c69 /ATen/core/quali
   0x00947530 66696564 5f6e616d 652e6822 3a33322c fied_name.h":32,
   0x00947540 20706c65 61736520 7265706f 72742061  please report a
   0x00947550 20627567 20746f20 5079546f 7263682e  bug to PyTorch.
   0x00947560 20000000 00000000 2f676974 6875622f  ......./github/
   0x00947570 686f6d65 2f6d696e 69636f6e 64612f65 home/miniconda/e
   0x00947580 6e76732f 6275696c 645f6269 6e617279 nvs/build_binary
-  0x00947590 2f6c6962 2f707974 686f6e33 2e392f73 /lib/python3.9/s
+  0x00947590 2f6c6962 2f707974 686f6e33 2e382f73 /lib/python3.8/s
   0x009475a0 6974652d 7061636b 61676573 2f746f72 ite-packages/tor
   0x009475b0 63682f69 6e636c75 64652f63 31302f75 ch/include/c10/u
   0x009475c0 74696c2f 41727261 79526566 2e680051 til/ArrayRef.h.Q
   0x009475d0 75616c69 66696564 4e616d65 00626173 ualifiedName.bas
   0x009475e0 69635f73 7472696e 673a3a73 75627374 ic_string::subst
   0x009475f0 72004172 72617952 65663a20 696e7661 r.ArrayRef: inva
   0x00947600 6c696420 736c6963 652c204e 203d2000 lid slice, N = .
@@ -11112,27 +11112,27 @@
   0x00947650 77697468 2064696d 656e7369 6f6e733a with dimensions:
   0x00947660 20000000 00000000 74656e73 6f722e64  .......tensor.d
   0x00947670 696d2829 203d3d20 3020494e 5445524e im() == 0 INTERN
   0x00947680 414c2041 53534552 54204641 494c4544 AL ASSERT FAILED
   0x00947690 20617420 222f6769 74687562 2f686f6d  at "/github/hom
   0x009476a0 652f6d69 6e69636f 6e64612f 656e7673 e/miniconda/envs
   0x009476b0 2f627569 6c645f62 696e6172 792f6c69 /build_binary/li
-  0x009476c0 622f7079 74686f6e 332e392f 73697465 b/python3.9/site
+  0x009476c0 622f7079 74686f6e 332e382f 73697465 b/python3.8/site
   0x009476d0 2d706163 6b616765 732f746f 7263682f -packages/torch/
   0x009476e0 696e636c 7564652f 746f7263 682f6373 include/torch/cs
   0x009476f0 72632f61 70692f69 6e636c75 64652f74 rc/api/include/t
   0x00947700 6f726368 2f646574 61696c2f 54656e73 orch/detail/Tens
   0x00947710 6f724461 7461436f 6e746169 6e65722e orDataContainer.
   0x00947720 68223a33 31372c20 706c6561 73652072 h":317, please r
   0x00947730 65706f72 74206120 62756720 746f2050 eport a bug to P
   0x00947740 79546f72 63682e20 00000000 00000000 yTorch. ........
   0x00947750 2f676974 6875622f 686f6d65 2f6d696e /github/home/min
   0x00947760 69636f6e 64612f65 6e76732f 6275696c iconda/envs/buil
   0x00947770 645f6269 6e617279 2f6c6962 2f707974 d_binary/lib/pyt
-  0x00947780 686f6e33 2e392f73 6974652d 7061636b hon3.9/site-pack
+  0x00947780 686f6e33 2e382f73 6974652d 7061636b hon3.8/site-pack
   0x00947790 61676573 2f746f72 63682f69 6e636c75 ages/torch/inclu
   0x009477a0 64652f74 6f726368 2f637372 632f6170 de/torch/csrc/ap
   0x009477b0 692f696e 636c7564 652f746f 7263682f i/include/torch/
   0x009477c0 64657461 696c2f54 656e736f 72446174 detail/TensorDat
   0x009477d0 61436f6e 7461696e 65722e68 00000000 aContainer.h....
   0x009477e0 20696e20 69747320 66697273 74206469  in its first di
   0x009477f0 6d656e73 696f6e2c 20627574 20676f74 mension, but got
@@ -11141,15 +11141,15 @@
   0x00947820 697a6573 28295b30 5d203d3d 2028696e izes()[0] == (in
   0x00947830 7436345f 7429696e 69745f6c 6973745f t64_t)init_list_
   0x00947840 2e73697a 65282920 494e5445 524e414c .size() INTERNAL
   0x00947850 20415353 45525420 4641494c 45442061  ASSERT FAILED a
   0x00947860 7420222f 67697468 75622f68 6f6d652f t "/github/home/
   0x00947870 6d696e69 636f6e64 612f656e 76732f62 miniconda/envs/b
   0x00947880 75696c64 5f62696e 6172792f 6c69622f uild_binary/lib/
-  0x00947890 70797468 6f6e332e 392f7369 74652d70 python3.9/site-p
+  0x00947890 70797468 6f6e332e 382f7369 74652d70 python3.8/site-p
   0x009478a0 61636b61 6765732f 746f7263 682f696e ackages/torch/in
   0x009478b0 636c7564 652f746f 7263682f 63737263 clude/torch/csrc
   0x009478c0 2f617069 2f696e63 6c756465 2f746f72 /api/include/tor
   0x009478d0 63682f64 65746169 6c2f5465 6e736f72 ch/detail/Tensor
   0x009478e0 44617461 436f6e74 61696e65 722e6822 DataContainer.h"
   0x009478f0 3a333234 2c20706c 65617365 20726570 :324, please rep
   0x00947900 6f727420 61206275 6720746f 20507954 ort a bug to PyT
@@ -11160,15 +11160,15 @@
   0x00947950 6f726020 73686f75 6c64206e 6f742062 or` should not b
   0x00947960 65206361 6c6c6564 00000000 00000000 e called........
   0x00947970 66616c73 6520494e 5445524e 414c2041 false INTERNAL A
   0x00947980 53534552 54204641 494c4544 20617420 SSERT FAILED at 
   0x00947990 222f6769 74687562 2f686f6d 652f6d69 "/github/home/mi
   0x009479a0 6e69636f 6e64612f 656e7673 2f627569 niconda/envs/bui
   0x009479b0 6c645f62 696e6172 792f6c69 622f7079 ld_binary/lib/py
-  0x009479c0 74686f6e 332e392f 73697465 2d706163 thon3.9/site-pac
+  0x009479c0 74686f6e 332e382f 73697465 2d706163 thon3.8/site-pac
   0x009479d0 6b616765 732f746f 7263682f 696e636c kages/torch/incl
   0x009479e0 7564652f 746f7263 682f6373 72632f61 ude/torch/csrc/a
   0x009479f0 70692f69 6e636c75 64652f74 6f726368 pi/include/torch
   0x00947a00 2f646574 61696c2f 54656e73 6f724461 /detail/TensorDa
   0x00947a10 7461436f 6e746169 6e65722e 68223a33 taContainer.h":3
   0x00947a20 33382c20 706c6561 73652072 65706f72 38, please repor
   0x00947a30 74206120 62756720 746f2050 79546f72 t a bug to PyTor
@@ -11176,15 +11176,15 @@
   0x00947a50 54656e73 6f724461 7461436f 6e746169 TensorDataContai
   0x00947a60 6e657220 74797065 00000000 00000000 ner type........
   0x00947a70 66616c73 6520494e 5445524e 414c2041 false INTERNAL A
   0x00947a80 53534552 54204641 494c4544 20617420 SSERT FAILED at 
   0x00947a90 222f6769 74687562 2f686f6d 652f6d69 "/github/home/mi
   0x00947aa0 6e69636f 6e64612f 656e7673 2f627569 niconda/envs/bui
   0x00947ab0 6c645f62 696e6172 792f6c69 622f7079 ld_binary/lib/py
-  0x00947ac0 74686f6e 332e392f 73697465 2d706163 thon3.9/site-pac
+  0x00947ac0 74686f6e 332e382f 73697465 2d706163 thon3.8/site-pac
   0x00947ad0 6b616765 732f746f 7263682f 696e636c kages/torch/incl
   0x00947ae0 7564652f 746f7263 682f6373 72632f61 ude/torch/csrc/a
   0x00947af0 70692f69 6e636c75 64652f74 6f726368 pi/include/torch
   0x00947b00 2f646574 61696c2f 54656e73 6f724461 /detail/TensorDa
   0x00947b10 7461436f 6e746169 6e65722e 68223a33 taContainer.h":3
   0x00947b20 34322c20 706c6561 73652072 65706f72 42, please repor
   0x00947b30 74206120 62756720 746f2050 79546f72 t a bug to PyTor
@@ -11202,15 +11202,15 @@
   0x00947bf0 74686f75 74206c6f 7373206f 6620696e thout loss of in
   0x00947c00 666f726d 6174696f 6e000000 00000000 formation.......
   0x00947c10 66616c73 6520494e 5445524e 414c2041 false INTERNAL A
   0x00947c20 53534552 54204641 494c4544 20617420 SSERT FAILED at 
   0x00947c30 222f6769 74687562 2f686f6d 652f6d69 "/github/home/mi
   0x00947c40 6e69636f 6e64612f 656e7673 2f627569 niconda/envs/bui
   0x00947c50 6c645f62 696e6172 792f6c69 622f7079 ld_binary/lib/py
-  0x00947c60 74686f6e 332e392f 73697465 2d706163 thon3.9/site-pac
+  0x00947c60 74686f6e 332e382f 73697465 2d706163 thon3.8/site-pac
   0x00947c70 6b616765 732f746f 7263682f 696e636c kages/torch/incl
   0x00947c80 7564652f 746f7263 682f6373 72632f61 ude/torch/csrc/a
   0x00947c90 70692f69 6e636c75 64652f74 6f726368 pi/include/torch
   0x00947ca0 2f646574 61696c2f 54656e73 6f724461 /detail/TensorDa
   0x00947cb0 7461436f 6e746169 6e65722e 68223a32 taContainer.h":2
   0x00947cc0 37322c20 706c6561 73652072 65706f72 72, please repor
   0x00947cd0 74206120 62756720 746f2050 79546f72 t a bug to PyTor
@@ -11230,15 +11230,15 @@
   0x00947db0 3b206974 20697320 6f6e6c79 20666f72 ; it is only for
   0x00947dc0 20475055 2e000000 6973496e 744c6973  GPU....isIntLis
   0x00947dd0 74282920 494e5445 524e414c 20415353 t() INTERNAL ASS
   0x00947de0 45525420 4641494c 45442061 7420222f ERT FAILED at "/
   0x00947df0 67697468 75622f68 6f6d652f 6d696e69 github/home/mini
   0x00947e00 636f6e64 612f656e 76732f62 75696c64 conda/envs/build
   0x00947e10 5f62696e 6172792f 6c69622f 70797468 _binary/lib/pyth
-  0x00947e20 6f6e332e 392f7369 74652d70 61636b61 on3.9/site-packa
+  0x00947e20 6f6e332e 382f7369 74652d70 61636b61 on3.8/site-packa
   0x00947e30 6765732f 746f7263 682f696e 636c7564 ges/torch/includ
   0x00947e40 652f4154 656e2f63 6f72652f 6976616c e/ATen/core/ival
   0x00947e50 75655f69 6e6c2e68 223a3139 37322c20 ue_inl.h":1972, 
   0x00947e60 706c6561 73652072 65706f72 74206120 please report a 
   0x00947e70 62756720 746f2050 79546f72 63682e20 bug to PyTorch. 
   0x00947e80 00000000 00000000 76656374 6f723a3a ........vector::
   0x00947e90 5f4d5f72 616e6765 5f636865 636b3a20 _M_range_check: 
@@ -11265,15 +11265,15 @@
   0x00947fe0 61726775 6d656e74 206f6620 5f5f7365 argument of __se
   0x00947ff0 74737461 74655f5f 2e20476f 74200000 tstate__. Got ..
   0x00948000 69735374 72696e67 28292049 4e544552 isString() INTER
   0x00948010 4e414c20 41535345 52542046 41494c45 NAL ASSERT FAILE
   0x00948020 44206174 20222f67 69746875 622f686f D at "/github/ho
   0x00948030 6d652f6d 696e6963 6f6e6461 2f656e76 me/miniconda/env
   0x00948040 732f6275 696c645f 62696e61 72792f6c s/build_binary/l
-  0x00948050 69622f70 7974686f 6e332e39 2f736974 ib/python3.9/sit
+  0x00948050 69622f70 7974686f 6e332e38 2f736974 ib/python3.8/sit
   0x00948060 652d7061 636b6167 65732f74 6f726368 e-packages/torch
   0x00948070 2f696e63 6c756465 2f415465 6e2f636f /include/ATen/co
   0x00948080 72652f69 76616c75 655f696e 6c2e6822 re/ivalue_inl.h"
   0x00948090 3a323336 322c2070 6c656173 65207265 :2362, please re
   0x009480a0 706f7274 20612062 75672074 6f205079 port a bug to Py
   0x009480b0 546f7263 682e2000 2f2f6465 65706c65 Torch. .//deeple
   0x009480c0 61726e69 6e672f66 6267656d 6d2f6662 arning/fbgemm/fb
@@ -11391,36 +11391,36 @@
   0x009487c0 73657473 29202d3e 2054656e 736f7200 sets) -> Tensor.
   0x009487d0 69734765 6e657269 63446963 74282920 isGenericDict() 
   0x009487e0 494e5445 524e414c 20415353 45525420 INTERNAL ASSERT 
   0x009487f0 4641494c 45442061 7420222f 67697468 FAILED at "/gith
   0x00948800 75622f68 6f6d652f 6d696e69 636f6e64 ub/home/minicond
   0x00948810 612f656e 76732f62 75696c64 5f62696e a/envs/build_bin
   0x00948820 6172792f 6c69622f 70797468 6f6e332e ary/lib/python3.
-  0x00948830 392f7369 74652d70 61636b61 6765732f 9/site-packages/
+  0x00948830 382f7369 74652d70 61636b61 6765732f 8/site-packages/
   0x00948840 746f7263 682f696e 636c7564 652f4154 torch/include/AT
   0x00948850 656e2f63 6f72652f 6976616c 75655f69 en/core/ivalue_i
   0x00948860 6e6c2e68 223a3230 38382c20 706c6561 nl.h":2088, plea
   0x00948870 73652072 65706f72 74206120 62756720 se report a bug 
   0x00948880 746f2050 79546f72 63682e20 00000000 to PyTorch. ....
   0x00948890 73656c66 5f696d70 6c20494e 5445524e self_impl INTERN
   0x009488a0 414c2041 53534552 54204641 494c4544 AL ASSERT FAILED
   0x009488b0 20617420 222f6769 74687562 2f686f6d  at "/github/hom
   0x009488c0 652f6d69 6e69636f 6e64612f 656e7673 e/miniconda/envs
   0x009488d0 2f627569 6c645f62 696e6172 792f6c69 /build_binary/li
-  0x009488e0 622f7079 74686f6e 332e392f 73697465 b/python3.9/site
+  0x009488e0 622f7079 74686f6e 332e382f 73697465 b/python3.8/site
   0x009488f0 2d706163 6b616765 732f746f 7263682f -packages/torch/
   0x00948900 696e636c 7564652f 746f7263 682f6373 include/torch/cs
   0x00948910 72632f61 75746f67 7261642f 76617269 rc/autograd/vari
   0x00948920 61626c65 2e68223a 3330352c 20706c65 able.h":305, ple
   0x00948930 61736520 7265706f 72742061 20627567 ase report a bug
   0x00948940 20746f20 5079546f 7263682e 20000000  to PyTorch. ...
   0x00948950 2f676974 6875622f 686f6d65 2f6d696e /github/home/min
   0x00948960 69636f6e 64612f65 6e76732f 6275696c iconda/envs/buil
   0x00948970 645f6269 6e617279 2f6c6962 2f707974 d_binary/lib/pyt
-  0x00948980 686f6e33 2e392f73 6974652d 7061636b hon3.9/site-pack
+  0x00948980 686f6e33 2e382f73 6974652d 7061636b hon3.8/site-pack
   0x00948990 61676573 2f746f72 63682f69 6e636c75 ages/torch/inclu
   0x009489a0 64652f74 6f726368 2f637372 632f6175 de/torch/csrc/au
   0x009489b0 746f6772 61642f76 61726961 626c652e tograd/variable.
   0x009489c0 68000000 00000000 4f6e6c79 2054656e h.......Only Ten
   0x009489d0 736f7273 206f6620 666c6f61 74696e67 sors of floating
   0x009489e0 20706f69 6e742061 6e642063 6f6d706c  point and compl
   0x009489f0 65782064 74797065 2063616e 20726571 ex dtype can req
@@ -11480,37 +11480,37 @@
   0x00948d50 73657274 00000000 73636865 6d615f2e sert....schema_.
   0x00948d60 72657475 726e7328 292e7369 7a652829 returns().size()
   0x00948d70 203d3d20 3120494e 5445524e 414c2041  == 1 INTERNAL A
   0x00948d80 53534552 54204641 494c4544 20617420 SSERT FAILED at 
   0x00948d90 222f6769 74687562 2f686f6d 652f6d69 "/github/home/mi
   0x00948da0 6e69636f 6e64612f 656e7673 2f627569 niconda/envs/bui
   0x00948db0 6c645f62 696e6172 792f6c69 622f7079 ld_binary/lib/py
-  0x00948dc0 74686f6e 332e392f 73697465 2d706163 thon3.9/site-pac
+  0x00948dc0 74686f6e 332e382f 73697465 2d706163 thon3.8/site-pac
   0x00948dd0 6b616765 732f746f 7263682f 696e636c kages/torch/incl
   0x00948de0 7564652f 4154656e 2f636f72 652f6275 ude/ATen/core/bu
   0x00948df0 696c7469 6e5f6675 6e637469 6f6e2e68 iltin_function.h
   0x00948e00 223a3232 2c20706c 65617365 20726570 ":22, please rep
   0x00948e10 6f727420 61206275 6720746f 20507954 ort a bug to PyT
   0x00948e20 6f726368 2e200000 2f676974 6875622f orch. ../github/
   0x00948e30 686f6d65 2f6d696e 69636f6e 64612f65 home/miniconda/e
   0x00948e40 6e76732f 6275696c 645f6269 6e617279 nvs/build_binary
-  0x00948e50 2f6c6962 2f707974 686f6e33 2e392f73 /lib/python3.9/s
+  0x00948e50 2f6c6962 2f707974 686f6e33 2e382f73 /lib/python3.8/s
   0x00948e60 6974652d 7061636b 61676573 2f746f72 ite-packages/tor
   0x00948e70 63682f69 6e636c75 64652f41 54656e2f ch/include/ATen/
   0x00948e80 636f7265 2f627569 6c74696e 5f66756e core/builtin_fun
   0x00948e90 6374696f 6e2e6800 4275696c 74696e4f ction.h.BuiltinO
   0x00948ea0 7046756e 6374696f 6e006465 66696e65 pFunction.define
   0x00948eb0 4d657468 6f640000 44656661 756c7420 Method..Default 
   0x00948ec0 76616c75 6573206d 75737420 62652073 values must be s
   0x00948ed0 70656369 66696564 20666f72 206e6f6e pecified for non
   0x00948ee0 65206f72 20616c6c 20617267 756d656e e or all argumen
   0x00948ef0 74730000 00000000 2f676974 6875622f ts....../github/
   0x00948f00 686f6d65 2f6d696e 69636f6e 64612f65 home/miniconda/e
   0x00948f10 6e76732f 6275696c 645f6269 6e617279 nvs/build_binary
-  0x00948f20 2f6c6962 2f707974 686f6e33 2e392f73 /lib/python3.9/s
+  0x00948f20 2f6c6962 2f707974 686f6e33 2e382f73 /lib/python3.8/s
   0x00948f30 6974652d 7061636b 61676573 2f746f72 ite-packages/tor
   0x00948f40 63682f69 6e636c75 64652f74 6f726368 ch/include/torch
   0x00948f50 2f637573 746f6d5f 636c6173 732e6800 /custom_class.h.
   0x00948f60 54656e73 6f72496d 706c2077 69746820 TensorImpl with 
   0x00948f70 6e756c6c 70747220 6973206e 6f742073 nullptr is not s
   0x00948f80 7570706f 72746564 00766563 746f723a upported.vector:
   0x00948f90 3a5f4d5f 64656661 756c745f 61707065 :_M_default_appe
@@ -11652,28 +11652,28 @@
   0x00949810 70656374 6564204f 626a6563 74206275 pected Object bu
   0x00949820 7420676f 74200074 6f4f626a 65637400 t got .toObject.
   0x00949830 69734f62 6a656374 28292049 4e544552 isObject() INTER
   0x00949840 4e414c20 41535345 52542046 41494c45 NAL ASSERT FAILE
   0x00949850 44206174 20222f67 69746875 622f686f D at "/github/ho
   0x00949860 6d652f6d 696e6963 6f6e6461 2f656e76 me/miniconda/env
   0x00949870 732f6275 696c645f 62696e61 72792f6c s/build_binary/l
-  0x00949880 69622f70 7974686f 6e332e39 2f736974 ib/python3.9/sit
+  0x00949880 69622f70 7974686f 6e332e38 2f736974 ib/python3.8/sit
   0x00949890 652d7061 636b6167 65732f74 6f726368 e-packages/torch
   0x009498a0 2f696e63 6c756465 2f415465 6e2f636f /include/ATen/co
   0x009498b0 72652f69 76616c75 655f696e 6c2e6822 re/ivalue_inl.h"
   0x009498c0 3a313333 2c20706c 65617365 20726570 :133, please rep
   0x009498d0 6f727420 61206275 6720746f 20507954 ort a bug to PyT
   0x009498e0 6f726368 2e200000 53747265 616d7320 orch. ..Streams 
   0x009498f0 68617665 2061206d 6978206f 66206465 have a mix of de
   0x00949900 76696365 20747970 65733a20 73747265 vice types: stre
   0x00949910 616d2030 20697320 6f6e2000 00000000 am 0 is on .....
   0x00949920 2f676974 6875622f 686f6d65 2f6d696e /github/home/min
   0x00949930 69636f6e 64612f65 6e76732f 6275696c iconda/envs/buil
   0x00949940 645f6269 6e617279 2f6c6962 2f707974 d_binary/lib/pyt
-  0x00949950 686f6e33 2e392f73 6974652d 7061636b hon3.9/site-pack
+  0x00949950 686f6e33 2e382f73 6974652d 7061636b hon3.8/site-pack
   0x00949960 61676573 2f746f72 63682f69 6e636c75 ages/torch/inclu
   0x00949970 64652f63 31302f63 6f72652f 696d706c de/c10/core/impl
   0x00949980 2f496e6c 696e6553 74726561 6d477561 /InlineStreamGua
   0x00949990 72642e68 00207768 696c6520 73747265 rd.h. while stre
   0x009499a0 616d2000 20697320 6f6e2064 65766963 am . is on devic
   0x009499b0 65200067 65744465 76696365 54797065 e .getDeviceType
   0x009499c0 4f665374 7265616d 73002c20 74727969 OfStreams., tryi
@@ -11686,15 +11686,15 @@
   0x00949a30 79206d61 726b6564 20636f6d 706c6574 y marked complet
   0x00949a40 65640000 00000000 21636f6d 706c6574 ed......!complet
   0x00949a50 65642829 20494e54 45524e41 4c204153 ed() INTERNAL AS
   0x00949a60 53455254 20464149 4c454420 61742022 SERT FAILED at "
   0x00949a70 2f676974 6875622f 686f6d65 2f6d696e /github/home/min
   0x00949a80 69636f6e 64612f65 6e76732f 6275696c iconda/envs/buil
   0x00949a90 645f6269 6e617279 2f6c6962 2f707974 d_binary/lib/pyt
-  0x00949aa0 686f6e33 2e392f73 6974652d 7061636b hon3.9/site-pack
+  0x00949aa0 686f6e33 2e382f73 6974652d 7061636b hon3.8/site-pack
   0x00949ab0 61676573 2f746f72 63682f69 6e636c75 ages/torch/inclu
   0x00949ac0 64652f41 54656e2f 636f7265 2f697661 de/ATen/core/iva
   0x00949ad0 6c75655f 696e6c2e 68223a31 3232312c lue_inl.h":1221,
   0x00949ae0 20706c65 61736520 7265706f 72742061  please report a
   0x00949af0 20627567 20746f20 5079546f 7263682e  bug to PyTorch.
   0x00949b00 20000000 00000000 20776869 63682061  ....... which a
   0x00949b10 7265206e 6f742061 6d6f6e67 20746865 re not among the
@@ -11729,15 +11729,15 @@
   0x00949ce0 6965773c 63686172 3e5d0000 00000000 iew<char>]......
   0x00949cf0 20636f75 6c64206e 6f742062 6520636f  could not be co
   0x00949d00 6e766572 74656420 746f2061 6e79206f nverted to any o
   0x00949d10 66207468 65206b6e 6f776e20 74797065 f the known type
   0x00949d20 732e0000 00000000 2f676974 6875622f s......./github/
   0x00949d30 686f6d65 2f6d696e 69636f6e 64612f65 home/miniconda/e
   0x00949d40 6e76732f 6275696c 645f6269 6e617279 nvs/build_binary
-  0x00949d50 2f6c6962 2f707974 686f6e33 2e392f73 /lib/python3.9/s
+  0x00949d50 2f6c6962 2f707974 686f6e33 2e382f73 /lib/python3.8/s
   0x00949d60 6974652d 7061636b 61676573 2f746f72 ite-packages/tor
   0x00949d70 63682f69 6e636c75 64652f41 54656e2f ch/include/ATen/
   0x00949d80 636f7265 2f6a6974 5f747970 652e6800 core/jit_type.h.
   0x00949d90 54797065 20000000 636f6e73 74657870 Type ...constexp
   0x00949da0 72206331 303a3a73 7472696e 675f7669 r c10::string_vi
   0x00949db0 65772063 31303a3a 7574696c 3a3a6465 ew c10::util::de
   0x00949dc0 7461696c 3a3a6675 6c6c795f 7175616c tail::fully_qual
@@ -11799,15 +11799,15 @@
   0x0094a140 61696e20 61206375 73746f6d 20636c61 ain a custom cla
   0x0094a150 73732100 00000000 69734361 7073756c ss!.....isCapsul
   0x0094a160 65282920 494e5445 524e414c 20415353 e() INTERNAL ASS
   0x0094a170 45525420 4641494c 45442061 7420222f ERT FAILED at "/
   0x0094a180 67697468 75622f68 6f6d652f 6d696e69 github/home/mini
   0x0094a190 636f6e64 612f656e 76732f62 75696c64 conda/envs/build
   0x0094a1a0 5f62696e 6172792f 6c69622f 70797468 _binary/lib/pyth
-  0x0094a1b0 6f6e332e 392f7369 74652d70 61636b61 on3.9/site-packa
+  0x0094a1b0 6f6e332e 382f7369 74652d70 61636b61 on3.8/site-packa
   0x0094a1c0 6765732f 746f7263 682f696e 636c7564 ges/torch/includ
   0x0094a1d0 652f4154 656e2f63 6f72652f 6976616c e/ATen/core/ival
   0x0094a1e0 75655f69 6e6c2e68 223a3232 352c2070 ue_inl.h":225, p
   0x0094a1f0 6c656173 65207265 706f7274 20612062 lease report a b
   0x0094a200 75672074 6f205079 546f7263 682e2000 ug to PyTorch. .
   0x0094a210 746f4375 73746f6d 436c6173 7300746f toCustomClass.to
   0x0094a220 43617073 756c6500 54726965 6420746f Capsule.Tried to
@@ -11821,36 +11821,36 @@
   0x0094a2a0 6963742e 696d706c 5f2d3e65 6c656d65 ict.impl_->eleme
   0x0094a2b0 6e745479 7065732e 6b657954 79706520 ntTypes.keyType 
   0x0094a2c0 494e5445 524e414c 20415353 45525420 INTERNAL ASSERT 
   0x0094a2d0 4641494c 45442061 7420222f 67697468 FAILED at "/gith
   0x0094a2e0 75622f68 6f6d652f 6d696e69 636f6e64 ub/home/minicond
   0x0094a2f0 612f656e 76732f62 75696c64 5f62696e a/envs/build_bin
   0x0094a300 6172792f 6c69622f 70797468 6f6e332e ary/lib/python3.
-  0x0094a310 392f7369 74652d70 61636b61 6765732f 9/site-packages/
+  0x0094a310 382f7369 74652d70 61636b61 6765732f 8/site-packages/
   0x0094a320 746f7263 682f696e 636c7564 652f4154 torch/include/AT
   0x0094a330 656e2f63 6f72652f 44696374 5f696e6c en/core/Dict_inl
   0x0094a340 2e68223a 32362c20 706c6561 73652072 .h":26, please r
   0x0094a350 65706f72 74206120 62756720 746f2050 eport a bug to P
   0x0094a360 79546f72 63682e20 00000000 00000000 yTorch. ........
   0x0094a370 2f676974 6875622f 686f6d65 2f6d696e /github/home/min
   0x0094a380 69636f6e 64612f65 6e76732f 6275696c iconda/envs/buil
   0x0094a390 645f6269 6e617279 2f6c6962 2f707974 d_binary/lib/pyt
-  0x0094a3a0 686f6e33 2e392f73 6974652d 7061636b hon3.9/site-pack
+  0x0094a3a0 686f6e33 2e382f73 6974652d 7061636b hon3.8/site-pack
   0x0094a3b0 61676573 2f746f72 63682f69 6e636c75 ages/torch/inclu
   0x0094a3c0 64652f41 54656e2f 636f7265 2f446963 de/ATen/core/Dic
   0x0094a3d0 745f696e 6c2e6800 2a676574 54797065 t_inl.h.*getType
   0x0094a3e0 5074723c 56616c75 653e2829 203d3d20 Ptr<Value>() == 
   0x0094a3f0 2a646963 742e696d 706c5f2d 3e656c65 *dict.impl_->ele
   0x0094a400 6d656e74 54797065 732e7661 6c756554 mentTypes.valueT
   0x0094a410 79706520 494e5445 524e414c 20415353 ype INTERNAL ASS
   0x0094a420 45525420 4641494c 45442061 7420222f ERT FAILED at "/
   0x0094a430 67697468 75622f68 6f6d652f 6d696e69 github/home/mini
   0x0094a440 636f6e64 612f656e 76732f62 75696c64 conda/envs/build
   0x0094a450 5f62696e 6172792f 6c69622f 70797468 _binary/lib/pyth
-  0x0094a460 6f6e332e 392f7369 74652d70 61636b61 on3.9/site-packa
+  0x0094a460 6f6e332e 382f7369 74652d70 61636b61 on3.8/site-packa
   0x0094a470 6765732f 746f7263 682f696e 636c7564 ges/torch/includ
   0x0094a480 652f4154 656e2f63 6f72652f 44696374 e/ATen/core/Dict
   0x0094a490 5f696e6c 2e68223a 32372c20 706c6561 _inl.h":27, plea
   0x0094a4a0 73652072 65706f72 74206120 62756720 se report a bug 
   0x0094a4b0 746f2050 79546f72 63682e20 00000000 to PyTorch. ....
   0x0094a4c0 4e336331 30354572 726f7245 00000000 N3c105ErrorE....
   0x0094a4d0 4e336331 30313056 616c7565 4572726f N3c1010ValueErro
@@ -12210,15 +12210,15 @@
   0x0094baf0 6a767020 6973206e 6f742069 6d706c65 jvp is not imple
   0x0094bb00 6d656e74 65642066 6f722074 68652063 mented for the c
   0x0094bb10 2b2b2041 5049206f 66206375 73746f6d ++ API of custom
   0x0094bb20 2046756e 6374696f 6e207965 742e0000  Function yet...
   0x0094bb30 2f676974 6875622f 686f6d65 2f6d696e /github/home/min
   0x0094bb40 69636f6e 64612f65 6e76732f 6275696c iconda/envs/buil
   0x0094bb50 645f6269 6e617279 2f6c6962 2f707974 d_binary/lib/pyt
-  0x0094bb60 686f6e33 2e392f73 6974652d 7061636b hon3.9/site-pack
+  0x0094bb60 686f6e33 2e382f73 6974652d 7061636b hon3.8/site-pack
   0x0094bb70 61676573 2f746f72 63682f69 6e636c75 ages/torch/inclu
   0x0094bb80 64652f74 6f726368 2f637372 632f6175 de/torch/csrc/au
   0x0094bb90 746f6772 61642f63 7573746f 6d5f6675 tograd/custom_fu
   0x0094bba0 6e637469 6f6e2e68 00000000 00000000 nction.h........
   0x0094bbb0 636f6d70 696c6564 5f617267 73206e6f compiled_args no
   0x0094bbc0 7420696d 706c656d 656e7465 6420666f t implemented fo
   0x0094bbd0 72206e6f 6e2d7472 61636561 626c6520 r non-traceable 
@@ -12258,25 +12258,25 @@
   0x0094bdf0 6620616c 6c206974 73206368 696c6472 f all its childr
   0x0094be00 656e0000 00000000 21686173 5f706172 en......!has_par
   0x0094be10 656e745f 20494e54 45524e41 4c204153 ent_ INTERNAL AS
   0x0094be20 53455254 20464149 4c454420 61742022 SERT FAILED at "
   0x0094be30 2f676974 6875622f 686f6d65 2f6d696e /github/home/min
   0x0094be40 69636f6e 64612f65 6e76732f 6275696c iconda/envs/buil
   0x0094be50 645f6269 6e617279 2f6c6962 2f707974 d_binary/lib/pyt
-  0x0094be60 686f6e33 2e392f73 6974652d 7061636b hon3.9/site-pack
+  0x0094be60 686f6e33 2e382f73 6974652d 7061636b hon3.8/site-pack
   0x0094be70 61676573 2f746f72 63682f69 6e636c75 ages/torch/inclu
   0x0094be80 64652f74 6f726368 2f637372 632f6175 de/torch/csrc/au
   0x0094be90 746f6772 61642f66 756e6374 696f6e2e tograd/function.
   0x0094bea0 68223a32 36322c20 706c6561 73652072 h":262, please r
   0x0094beb0 65706f72 74206120 62756720 746f2050 eport a bug to P
   0x0094bec0 79546f72 63682e20 00000000 00000000 yTorch. ........
   0x0094bed0 2f676974 6875622f 686f6d65 2f6d696e /github/home/min
   0x0094bee0 69636f6e 64612f65 6e76732f 6275696c iconda/envs/buil
   0x0094bef0 645f6269 6e617279 2f6c6962 2f707974 d_binary/lib/pyt
-  0x0094bf00 686f6e33 2e392f73 6974652d 7061636b hon3.9/site-pack
+  0x0094bf00 686f6e33 2e382f73 6974652d 7061636b hon3.8/site-pack
   0x0094bf10 61676573 2f746f72 63682f69 6e636c75 ages/torch/inclu
   0x0094bf20 64652f74 6f726368 2f637372 632f6175 de/torch/csrc/au
   0x0094bf30 746f6772 61642f66 756e6374 696f6e2e tograd/function.
   0x0094bf40 68000000 00000000 2f5f5f77 2f464247 h......./__w/FBG
   0x0094bf50 454d4d2f 46424745 4d4d2f66 6267656d EMM/FBGEMM/fbgem
   0x0094bf60 6d5f6770 752f636f 64656765 6e2f7472 m_gpu/codegen/tr
   0x0094bf70 61696e69 6e672f62 61636b77 6172642f aining/backward/
@@ -12300,147 +12300,147 @@
   0x0094c090 6374785f 2e6e6f6e 5f646966 66657265 ctx_.non_differe
   0x0094c0a0 6e746961 626c655f 2e656d70 74792829 ntiable_.empty()
   0x0094c0b0 20494e54 45524e41 4c204153 53455254  INTERNAL ASSERT
   0x0094c0c0 20464149 4c454420 61742022 2f676974  FAILED at "/git
   0x0094c0d0 6875622f 686f6d65 2f6d696e 69636f6e hub/home/minicon
   0x0094c0e0 64612f65 6e76732f 6275696c 645f6269 da/envs/build_bi
   0x0094c0f0 6e617279 2f6c6962 2f707974 686f6e33 nary/lib/python3
-  0x0094c100 2e392f73 6974652d 7061636b 61676573 .9/site-packages
+  0x0094c100 2e382f73 6974652d 7061636b 61676573 .8/site-packages
   0x0094c110 2f746f72 63682f69 6e636c75 64652f74 /torch/include/t
   0x0094c120 6f726368 2f637372 632f6175 746f6772 orch/csrc/autogr
   0x0094c130 61642f63 7573746f 6d5f6675 6e637469 ad/custom_functi
   0x0094c140 6f6e2e68 223a3232 312c2070 6c656173 on.h":221, pleas
   0x0094c150 65207265 706f7274 20612062 75672074 e report a bug t
   0x0094c160 6f205079 546f7263 682e2000 00000000 o PyTorch. .....
   0x0094c170 6374785f 2e646972 74795f69 6e707574 ctx_.dirty_input
   0x0094c180 735f2e65 6d707479 28292049 4e544552 s_.empty() INTER
   0x0094c190 4e414c20 41535345 52542046 41494c45 NAL ASSERT FAILE
   0x0094c1a0 44206174 20222f67 69746875 622f686f D at "/github/ho
   0x0094c1b0 6d652f6d 696e6963 6f6e6461 2f656e76 me/miniconda/env
   0x0094c1c0 732f6275 696c645f 62696e61 72792f6c s/build_binary/l
-  0x0094c1d0 69622f70 7974686f 6e332e39 2f736974 ib/python3.9/sit
+  0x0094c1d0 69622f70 7974686f 6e332e38 2f736974 ib/python3.8/sit
   0x0094c1e0 652d7061 636b6167 65732f74 6f726368 e-packages/torch
   0x0094c1f0 2f696e63 6c756465 2f746f72 63682f63 /include/torch/c
   0x0094c200 7372632f 6175746f 67726164 2f637573 src/autograd/cus
   0x0094c210 746f6d5f 66756e63 74696f6e 2e68223a tom_function.h":
   0x0094c220 3232322c 20706c65 61736520 7265706f 222, please repo
   0x0094c230 72742061 20627567 20746f20 5079546f rt a bug to PyTo
   0x0094c240 7263682e 20000000 69742021 3d205f73 rch. ...it != _s
   0x0094c250 61766564 5f766172 6961626c 65732e65 aved_variables.e
   0x0094c260 6e642829 20494e54 45524e41 4c204153 nd() INTERNAL AS
   0x0094c270 53455254 20464149 4c454420 61742022 SERT FAILED at "
   0x0094c280 2f676974 6875622f 686f6d65 2f6d696e /github/home/min
   0x0094c290 69636f6e 64612f65 6e76732f 6275696c iconda/envs/buil
   0x0094c2a0 645f6269 6e617279 2f6c6962 2f707974 d_binary/lib/pyt
-  0x0094c2b0 686f6e33 2e392f73 6974652d 7061636b hon3.9/site-pack
+  0x0094c2b0 686f6e33 2e382f73 6974652d 7061636b hon3.8/site-pack
   0x0094c2c0 61676573 2f746f72 63682f69 6e636c75 ages/torch/inclu
   0x0094c2d0 64652f74 6f726368 2f637372 632f6479 de/torch/csrc/dy
   0x0094c2e0 6e616d6f 2f636f6d 70696c65 645f6175 namo/compiled_au
   0x0094c2f0 746f6772 61642e68 223a3133 382c2070 tograd.h":138, p
   0x0094c300 6c656173 65207265 706f7274 20612062 lease report a b
   0x0094c310 75672074 6f205079 546f7263 682e2000 ug to PyTorch. .
   0x0094c320 6172672e 70726f78 795f7465 6e736f72 arg.proxy_tensor
   0x0094c330 2e646566 696e6564 28292049 4e544552 .defined() INTER
   0x0094c340 4e414c20 41535345 52542046 41494c45 NAL ASSERT FAILE
   0x0094c350 44206174 20222f67 69746875 622f686f D at "/github/ho
   0x0094c360 6d652f6d 696e6963 6f6e6461 2f656e76 me/miniconda/env
   0x0094c370 732f6275 696c645f 62696e61 72792f6c s/build_binary/l
-  0x0094c380 69622f70 7974686f 6e332e39 2f736974 ib/python3.9/sit
+  0x0094c380 69622f70 7974686f 6e332e38 2f736974 ib/python3.8/sit
   0x0094c390 652d7061 636b6167 65732f74 6f726368 e-packages/torch
   0x0094c3a0 2f696e63 6c756465 2f746f72 63682f63 /include/torch/c
   0x0094c3b0 7372632f 64796e61 6d6f2f63 6f6d7069 src/dynamo/compi
   0x0094c3c0 6c65645f 6175746f 67726164 2e68223a led_autograd.h":
   0x0094c3d0 3536312c 20706c65 61736520 7265706f 561, please repo
   0x0094c3e0 72742061 20627567 20746f20 5079546f rt a bug to PyTo
   0x0094c3f0 7263682e 20000000 6374785f 2e746f5f rch. ...ctx_.to_
   0x0094c400 73617665 5f2e656d 70747928 2920494e save_.empty() IN
   0x0094c410 5445524e 414c2041 53534552 54204641 TERNAL ASSERT FA
   0x0094c420 494c4544 20617420 222f6769 74687562 ILED at "/github
   0x0094c430 2f686f6d 652f6d69 6e69636f 6e64612f /home/miniconda/
   0x0094c440 656e7673 2f627569 6c645f62 696e6172 envs/build_binar
-  0x0094c450 792f6c69 622f7079 74686f6e 332e392f y/lib/python3.9/
+  0x0094c450 792f6c69 622f7079 74686f6e 332e382f y/lib/python3.8/
   0x0094c460 73697465 2d706163 6b616765 732f746f site-packages/to
   0x0094c470 7263682f 696e636c 7564652f 746f7263 rch/include/torc
   0x0094c480 682f6373 72632f61 75746f67 7261642f h/csrc/autograd/
   0x0094c490 63757374 6f6d5f66 756e6374 696f6e2e custom_function.
   0x0094c4a0 68223a32 32342c20 706c6561 73652072 h":224, please r
   0x0094c4b0 65706f72 74206120 62756720 746f2050 eport a bug to P
   0x0094c4c0 79546f72 63682e20 00000000 00000000 yTorch. ........
   0x0094c4d0 69742021 3d207468 69732d3e 656e6428 it != this->end(
   0x0094c4e0 2920494e 5445524e 414c2041 53534552 ) INTERNAL ASSER
   0x0094c4f0 54204641 494c4544 20617420 222f6769 T FAILED at "/gi
   0x0094c500 74687562 2f686f6d 652f6d69 6e69636f thub/home/minico
   0x0094c510 6e64612f 656e7673 2f627569 6c645f62 nda/envs/build_b
   0x0094c520 696e6172 792f6c69 622f7079 74686f6e inary/lib/python
-  0x0094c530 332e392f 73697465 2d706163 6b616765 3.9/site-package
+  0x0094c530 332e382f 73697465 2d706163 6b616765 3.8/site-package
   0x0094c540 732f746f 7263682f 696e636c 7564652f s/torch/include/
   0x0094c550 746f7263 682f6373 72632f64 796e616d torch/csrc/dynam
   0x0094c560 6f2f636f 6d70696c 65645f61 75746f67 o/compiled_autog
   0x0094c570 7261642e 68223a37 36302c20 706c6561 rad.h":760, plea
   0x0094c580 73652072 65706f72 74206120 62756720 se report a bug 
   0x0094c590 746f2050 79546f72 63682e20 00000000 to PyTorch. ....
   0x0094c5a0 6374785f 2e6e6f6e 5f646966 66657265 ctx_.non_differe
   0x0094c5b0 6e746961 626c655f 2e656d70 74792829 ntiable_.empty()
   0x0094c5c0 20494e54 45524e41 4c204153 53455254  INTERNAL ASSERT
   0x0094c5d0 20464149 4c454420 61742022 2f676974  FAILED at "/git
   0x0094c5e0 6875622f 686f6d65 2f6d696e 69636f6e hub/home/minicon
   0x0094c5f0 64612f65 6e76732f 6275696c 645f6269 da/envs/build_bi
   0x0094c600 6e617279 2f6c6962 2f707974 686f6e33 nary/lib/python3
-  0x0094c610 2e392f73 6974652d 7061636b 61676573 .9/site-packages
+  0x0094c610 2e382f73 6974652d 7061636b 61676573 .8/site-packages
   0x0094c620 2f746f72 63682f69 6e636c75 64652f74 /torch/include/t
   0x0094c630 6f726368 2f637372 632f6175 746f6772 orch/csrc/autogr
   0x0094c640 61642f63 7573746f 6d5f6675 6e637469 ad/custom_functi
   0x0094c650 6f6e2e68 223a3233 312c2070 6c656173 on.h":231, pleas
   0x0094c660 65207265 706f7274 20612062 75672074 e report a bug t
   0x0094c670 6f205079 546f7263 682e2000 00000000 o PyTorch. .....
   0x0094c680 6374785f 2e646972 74795f69 6e707574 ctx_.dirty_input
   0x0094c690 735f2e65 6d707479 28292049 4e544552 s_.empty() INTER
   0x0094c6a0 4e414c20 41535345 52542046 41494c45 NAL ASSERT FAILE
   0x0094c6b0 44206174 20222f67 69746875 622f686f D at "/github/ho
   0x0094c6c0 6d652f6d 696e6963 6f6e6461 2f656e76 me/miniconda/env
   0x0094c6d0 732f6275 696c645f 62696e61 72792f6c s/build_binary/l
-  0x0094c6e0 69622f70 7974686f 6e332e39 2f736974 ib/python3.9/sit
+  0x0094c6e0 69622f70 7974686f 6e332e38 2f736974 ib/python3.8/sit
   0x0094c6f0 652d7061 636b6167 65732f74 6f726368 e-packages/torch
   0x0094c700 2f696e63 6c756465 2f746f72 63682f63 /include/torch/c
   0x0094c710 7372632f 6175746f 67726164 2f637573 src/autograd/cus
   0x0094c720 746f6d5f 66756e63 74696f6e 2e68223a tom_function.h":
   0x0094c730 3233322c 20706c65 61736520 7265706f 232, please repo
   0x0094c740 72742061 20627567 20746f20 5079546f rt a bug to PyTo
   0x0094c750 7263682e 20000000 6374785f 2e746f5f rch. ...ctx_.to_
   0x0094c760 73617665 5f2e656d 70747928 2920494e save_.empty() IN
   0x0094c770 5445524e 414c2041 53534552 54204641 TERNAL ASSERT FA
   0x0094c780 494c4544 20617420 222f6769 74687562 ILED at "/github
   0x0094c790 2f686f6d 652f6d69 6e69636f 6e64612f /home/miniconda/
   0x0094c7a0 656e7673 2f627569 6c645f62 696e6172 envs/build_binar
-  0x0094c7b0 792f6c69 622f7079 74686f6e 332e392f y/lib/python3.9/
+  0x0094c7b0 792f6c69 622f7079 74686f6e 332e382f y/lib/python3.8/
   0x0094c7c0 73697465 2d706163 6b616765 732f746f site-packages/to
   0x0094c7d0 7263682f 696e636c 7564652f 746f7263 rch/include/torc
   0x0094c7e0 682f6373 72632f61 75746f67 7261642f h/csrc/autograd/
   0x0094c7f0 63757374 6f6d5f66 756e6374 696f6e2e custom_function.
   0x0094c800 68223a32 33342c20 706c6561 73652072 h":234, please r
   0x0094c810 65706f72 74206120 62756720 746f2050 eport a bug to P
   0x0094c820 79546f72 63682e20 00000000 00000000 yTorch. ........
   0x0094c830 73796d5f 73697a65 735f696e 64657820 sym_sizes_index 
   0x0094c840 3c207379 6d5f7369 7a65732e 73697a65 < sym_sizes.size
   0x0094c850 28292049 4e544552 4e414c20 41535345 () INTERNAL ASSE
   0x0094c860 52542046 41494c45 44206174 20222f67 RT FAILED at "/g
   0x0094c870 69746875 622f686f 6d652f6d 696e6963 ithub/home/minic
   0x0094c880 6f6e6461 2f656e76 732f6275 696c645f onda/envs/build_
   0x0094c890 62696e61 72792f6c 69622f70 7974686f binary/lib/pytho
-  0x0094c8a0 6e332e39 2f736974 652d7061 636b6167 n3.9/site-packag
+  0x0094c8a0 6e332e38 2f736974 652d7061 636b6167 n3.8/site-packag
   0x0094c8b0 65732f74 6f726368 2f696e63 6c756465 es/torch/include
   0x0094c8c0 2f746f72 63682f63 7372632f 64796e61 /torch/csrc/dyna
   0x0094c8d0 6d6f2f63 6f6d7069 6c65645f 6175746f mo/compiled_auto
   0x0094c8e0 67726164 2e68223a 3533312c 20706c65 grad.h":531, ple
   0x0094c8f0 61736520 7265706f 72742061 20627567 ase report a bug
   0x0094c900 20746f20 5079546f 7263682e 20000000  to PyTorch. ...
   0x0094c910 2f676974 6875622f 686f6d65 2f6d696e /github/home/min
   0x0094c920 69636f6e 64612f65 6e76732f 6275696c iconda/envs/buil
   0x0094c930 645f6269 6e617279 2f6c6962 2f707974 d_binary/lib/pyt
-  0x0094c940 686f6e33 2e392f73 6974652d 7061636b hon3.9/site-pack
+  0x0094c940 686f6e33 2e382f73 6974652d 7061636b hon3.8/site-pack
   0x0094c950 61676573 2f746f72 63682f69 6e636c75 ages/torch/inclu
   0x0094c960 64652f74 6f726368 2f637372 632f6479 de/torch/csrc/dy
   0x0094c970 6e616d6f 2f636f6d 70696c65 645f6175 namo/compiled_au
   0x0094c980 746f6772 61642e68 006e6578 745f7379 tograd.h.next_sy
   0x0094c990 6d5f7369 7a650000 00000000 00000000 m_size..........
   0x0094c9a0 50467650 4e35746f 72636838 6175746f PFvPN5torch8auto
   0x0094c9b0 67726164 344e6f64 65454500 00000000 grad4NodeEE.....
@@ -12714,38 +12714,38 @@
   0x0094da70 6444ccff 1444ccff cc43ccff 8443ccff dD...D...C...C..
   0x0094da80 2443ccff 944accff 69734465 76696365 $C...J..isDevice
   0x0094da90 28292049 4e544552 4e414c20 41535345 () INTERNAL ASSE
   0x0094daa0 52542046 41494c45 44206174 20222f67 RT FAILED at "/g
   0x0094dab0 69746875 622f686f 6d652f6d 696e6963 ithub/home/minic
   0x0094dac0 6f6e6461 2f656e76 732f6275 696c645f onda/envs/build_
   0x0094dad0 62696e61 72792f6c 69622f70 7974686f binary/lib/pytho
-  0x0094dae0 6e332e39 2f736974 652d7061 636b6167 n3.9/site-packag
+  0x0094dae0 6e332e38 2f736974 652d7061 636b6167 n3.8/site-packag
   0x0094daf0 65732f74 6f726368 2f696e63 6c756465 es/torch/include
   0x0094db00 2f415465 6e2f636f 72652f69 76616c75 /ATen/core/ivalu
   0x0094db10 652e6822 3a393136 2c20706c 65617365 e.h":916, please
   0x0094db20 20726570 6f727420 61206275 6720746f  report a bug to
   0x0094db30 20507954 6f726368 2e200000 00000000  PyTorch. ......
   0x0094db40 69735465 6e736f72 4c697374 28292049 isTensorList() I
   0x0094db50 4e544552 4e414c20 41535345 52542046 NTERNAL ASSERT F
   0x0094db60 41494c45 44206174 20222f67 69746875 AILED at "/githu
   0x0094db70 622f686f 6d652f6d 696e6963 6f6e6461 b/home/miniconda
   0x0094db80 2f656e76 732f6275 696c645f 62696e61 /envs/build_bina
-  0x0094db90 72792f6c 69622f70 7974686f 6e332e39 ry/lib/python3.9
+  0x0094db90 72792f6c 69622f70 7974686f 6e332e38 ry/lib/python3.8
   0x0094dba0 2f736974 652d7061 636b6167 65732f74 /site-packages/t
   0x0094dbb0 6f726368 2f696e63 6c756465 2f415465 orch/include/ATe
   0x0094dbc0 6e2f636f 72652f69 76616c75 655f696e n/core/ivalue_in
   0x0094dbd0 6c2e6822 3a323034 302c2070 6c656173 l.h":2040, pleas
   0x0094dbe0 65207265 706f7274 20612062 75672074 e report a bug t
   0x0094dbf0 6f205079 546f7263 682e2000 00000000 o PyTorch. .....
   0x0094dc00 69735465 6e736f72 4c697374 28292049 isTensorList() I
   0x0094dc10 4e544552 4e414c20 41535345 52542046 NTERNAL ASSERT F
   0x0094dc20 41494c45 44206174 20222f67 69746875 AILED at "/githu
   0x0094dc30 622f686f 6d652f6d 696e6963 6f6e6461 b/home/miniconda
   0x0094dc40 2f656e76 732f6275 696c645f 62696e61 /envs/build_bina
-  0x0094dc50 72792f6c 69622f70 7974686f 6e332e39 ry/lib/python3.9
+  0x0094dc50 72792f6c 69622f70 7974686f 6e332e38 ry/lib/python3.8
   0x0094dc60 2f736974 652d7061 636b6167 65732f74 /site-packages/t
   0x0094dc70 6f726368 2f696e63 6c756465 2f415465 orch/include/ATe
   0x0094dc80 6e2f636f 72652f69 76616c75 655f696e n/core/ivalue_in
   0x0094dc90 6c2e6822 3a323034 342c2070 6c656173 l.h":2044, pleas
   0x0094dca0 65207265 706f7274 20612062 75672074 e report a bug t
   0x0094dcb0 6f205079 546f7263 682e2000 746f4465 o PyTorch. .toDe
   0x0094dcc0 76696365 00457870 65637465 64205465 vice.Expected Te
@@ -12827,25 +12827,25 @@
   0x0094e180 69737465 72656420 79657400 00000000 istered yet.....
   0x0094e190 73636865 6d615f2e 6861735f 76616c75 schema_.has_valu
   0x0094e1a0 65282920 494e5445 524e414c 20415353 e() INTERNAL ASS
   0x0094e1b0 45525420 4641494c 45442061 7420222f ERT FAILED at "/
   0x0094e1c0 67697468 75622f68 6f6d652f 6d696e69 github/home/mini
   0x0094e1d0 636f6e64 612f656e 76732f62 75696c64 conda/envs/build
   0x0094e1e0 5f62696e 6172792f 6c69622f 70797468 _binary/lib/pyth
-  0x0094e1f0 6f6e332e 392f7369 74652d70 61636b61 on3.9/site-packa
+  0x0094e1f0 6f6e332e 382f7369 74652d70 61636b61 on3.8/site-packa
   0x0094e200 6765732f 746f7263 682f696e 636c7564 ges/torch/includ
   0x0094e210 652f4154 656e2f63 6f72652f 64697370 e/ATen/core/disp
   0x0094e220 61746368 2f4f7065 7261746f 72456e74 atch/OperatorEnt
   0x0094e230 72792e68 223a3830 2c20706c 65617365 ry.h":80, please
   0x0094e240 20726570 6f727420 61206275 6720746f  report a bug to
   0x0094e250 20507954 6f726368 2e200000 00000000  PyTorch. ......
   0x0094e260 2f676974 6875622f 686f6d65 2f6d696e /github/home/min
   0x0094e270 69636f6e 64612f65 6e76732f 6275696c iconda/envs/buil
   0x0094e280 645f6269 6e617279 2f6c6962 2f707974 d_binary/lib/pyt
-  0x0094e290 686f6e33 2e392f73 6974652d 7061636b hon3.9/site-pack
+  0x0094e290 686f6e33 2e382f73 6974652d 7061636b hon3.8/site-pack
   0x0094e2a0 61676573 2f746f72 63682f69 6e636c75 ages/torch/inclu
   0x0094e2b0 64652f41 54656e2f 636f7265 2f646973 de/ATen/core/dis
   0x0094e2c0 70617463 682f4f70 65726174 6f72456e patch/OperatorEn
   0x0094e2d0 7472792e 68007363 68656d61 00000000 try.h.schema....
   0x0094e2e0 66626765 6d6d3a3a 7065726d 7574655f fbgemm::permute_
   0x0094e2f0 6475706c 69636174 655f706f 6f6c6564 duplicate_pooled
   0x0094e300 5f656d62 73000000 6f666673 65745f64 _embs...offset_d
@@ -12862,15 +12862,15 @@
   0x0094e3b0 64732074 6f206861 7665206c 6f6e672f ds to have long/
   0x0094e3c0 696e7436 34207479 70650000 00000000 int64 type......
   0x0094e3d0 6973426f 6f6c2829 20494e54 45524e41 isBool() INTERNA
   0x0094e3e0 4c204153 53455254 20464149 4c454420 L ASSERT FAILED 
   0x0094e3f0 61742022 2f676974 6875622f 686f6d65 at "/github/home
   0x0094e400 2f6d696e 69636f6e 64612f65 6e76732f /miniconda/envs/
   0x0094e410 6275696c 645f6269 6e617279 2f6c6962 build_binary/lib
-  0x0094e420 2f707974 686f6e33 2e392f73 6974652d /python3.9/site-
+  0x0094e420 2f707974 686f6e33 2e382f73 6974652d /python3.8/site-
   0x0094e430 7061636b 61676573 2f746f72 63682f69 packages/torch/i
   0x0094e440 6e636c75 64652f41 54656e2f 636f7265 nclude/ATen/core
   0x0094e450 2f697661 6c75652e 68223a36 36312c20 /ivalue.h":661, 
   0x0094e460 706c6561 73652072 65706f72 74206120 please report a 
   0x0094e470 62756720 746f2050 79546f72 63682e20 bug to PyTorch. 
   0x0094e480 00000000 00000000 7065726d 7574655f ........permute_
   0x0094e490 706f6f6c 65645f65 6d627320 646f6573 pooled_embs does
@@ -13374,15 +13374,15 @@
   0x009503b0 64656e73 655f7665 635f6a61 67676564 dense_vec_jagged
   0x009503c0 5f32645f 6d756c00 69734c69 73742829 _2d_mul.isList()
   0x009503d0 20494e54 45524e41 4c204153 53455254  INTERNAL ASSERT
   0x009503e0 20464149 4c454420 61742022 2f676974  FAILED at "/git
   0x009503f0 6875622f 686f6d65 2f6d696e 69636f6e hub/home/minicon
   0x00950400 64612f65 6e76732f 6275696c 645f6269 da/envs/build_bi
   0x00950410 6e617279 2f6c6962 2f707974 686f6e33 nary/lib/python3
-  0x00950420 2e392f73 6974652d 7061636b 61676573 .9/site-packages
+  0x00950420 2e382f73 6974652d 7061636b 61676573 .8/site-packages
   0x00950430 2f746f72 63682f69 6e636c75 64652f41 /torch/include/A
   0x00950440 54656e2f 636f7265 2f697661 6c75655f Ten/core/ivalue_
   0x00950450 696e6c2e 68223a32 3037322c 20706c65 inl.h":2072, ple
   0x00950460 61736520 7265706f 72742061 20627567 ase report a bug
   0x00950470 20746f20 5079546f 7263682e 20000000  to PyTorch. ...
   0x00950480 2f5f5f77 2f464247 454d4d2f 46424745 /__w/FBGEMM/FBGE
   0x00950490 4d4d2f66 6267656d 6d5f6770 752f7372 MM/fbgemm_gpu/sr
@@ -13458,25 +13458,25 @@
   0x009508f0 6e744c69 73742062 75742067 6f742000 ntList but got .
   0x00950900 69735379 6d496e74 4c697374 2829207c isSymIntList() |
   0x00950910 7c206973 496e744c 69737428 2920494e | isIntList() IN
   0x00950920 5445524e 414c2041 53534552 54204641 TERNAL ASSERT FA
   0x00950930 494c4544 20617420 222f6769 74687562 ILED at "/github
   0x00950940 2f686f6d 652f6d69 6e69636f 6e64612f /home/miniconda/
   0x00950950 656e7673 2f627569 6c645f62 696e6172 envs/build_binar
-  0x00950960 792f6c69 622f7079 74686f6e 332e392f y/lib/python3.9/
+  0x00950960 792f6c69 622f7079 74686f6e 332e382f y/lib/python3.8/
   0x00950970 73697465 2d706163 6b616765 732f746f site-packages/to
   0x00950980 7263682f 696e636c 7564652f 4154656e rch/include/ATen
   0x00950990 2f636f72 652f6976 616c7565 5f696e6c /core/ivalue_inl
   0x009509a0 2e68223a 31393834 2c20706c 65617365 .h":1984, please
   0x009509b0 20726570 6f727420 61206275 6720746f  report a bug to
   0x009509c0 20507954 6f726368 2e200000 00000000  PyTorch. ......
   0x009509d0 2f676974 6875622f 686f6d65 2f6d696e /github/home/min
   0x009509e0 69636f6e 64612f65 6e76732f 6275696c iconda/envs/buil
   0x009509f0 645f6269 6e617279 2f6c6962 2f707974 d_binary/lib/pyt
-  0x00950a00 686f6e33 2e392f73 6974652d 7061636b hon3.9/site-pack
+  0x00950a00 686f6e33 2e382f73 6974652d 7061636b hon3.8/site-pack
   0x00950a10 61676573 2f746f72 63682f69 6e636c75 ages/torch/inclu
   0x00950a20 64652f63 31302f63 6f72652f 53796d49 de/c10/core/SymI
   0x00950a30 6e742e68 00000000 45787065 63746564 nt.h....Expected
   0x00950a40 2064656e 73655f76 616c7565 735f6772  dense_values_gr
   0x00950a50 61642e73 796d5f73 697a6573 2829203d ad.sym_sizes() =
   0x00950a60 3d206465 6e73655f 73686170 6520746f = dense_shape to
   0x00950a70 20626520 74727565 2c206275 7420676f  be true, but go
@@ -13585,15 +13585,15 @@
   0x009510e0 6820636f 6e746169 6e656420 74797065 h contained type
   0x009510f0 73206469 64206e6f 74206f76 65726c6f s did not overlo
   0x00951100 61642063 72656174 65576974 68436f6e ad createWithCon
   0x00951110 7461696e 65643a20 00000000 00000000 tained: ........
   0x00951120 2f676974 6875622f 686f6d65 2f6d696e /github/home/min
   0x00951130 69636f6e 64612f65 6e76732f 6275696c iconda/envs/buil
   0x00951140 645f6269 6e617279 2f6c6962 2f707974 d_binary/lib/pyt
-  0x00951150 686f6e33 2e392f73 6974652d 7061636b hon3.9/site-pack
+  0x00951150 686f6e33 2e382f73 6974652d 7061636b hon3.8/site-pack
   0x00951160 61676573 2f746f72 63682f69 6e636c75 ages/torch/inclu
   0x00951170 64652f41 54656e2f 636f7265 2f6a6974 de/ATen/core/jit
   0x00951180 5f747970 655f6261 73652e68 00637265 _type_base.h.cre
   0x00951190 61746557 69746843 6f6e7461 696e6564 ateWithContained
   0x009511a0 003b204c 656e6774 68203d20 00000000 .; Length = ....
   0x009511b0 41727261 79526566 3a20696e 76616c69 ArrayRef: invali
   0x009511c0 6420696e 64657820 496e6465 78203d20 d index Index = 
@@ -14178,45 +14178,45 @@
   0x009535f0 45450000 00000000 00000000 78000000 EE..........x...
   0x00953600 69735379 6d496e74 2829207c 7c206973 isSymInt() || is
   0x00953610 496e7428 2920494e 5445524e 414c2041 Int() INTERNAL A
   0x00953620 53534552 54204641 494c4544 20617420 SSERT FAILED at 
   0x00953630 222f6769 74687562 2f686f6d 652f6d69 "/github/home/mi
   0x00953640 6e69636f 6e64612f 656e7673 2f627569 niconda/envs/bui
   0x00953650 6c645f62 696e6172 792f6c69 622f7079 ld_binary/lib/py
-  0x00953660 74686f6e 332e392f 73697465 2d706163 thon3.9/site-pac
+  0x00953660 74686f6e 332e382f 73697465 2d706163 thon3.8/site-pac
   0x00953670 6b616765 732f746f 7263682f 696e636c kages/torch/incl
   0x00953680 7564652f 4154656e 2f636f72 652f6976 ude/ATen/core/iv
   0x00953690 616c7565 5f696e6c 2e68223a 3234352c alue_inl.h":245,
   0x009536a0 20706c65 61736520 7265706f 72742061  please report a
   0x009536b0 20627567 20746f20 5079546f 7263682e  bug to PyTorch.
   0x009536c0 20005472 69656420 746f2063 61737420  .Tried to cast 
   0x009536d0 61204c69 73743c00 3e20746f 2061204c a List<.> to a L
   0x009536e0 6973743c 003e2e20 54797065 73206d69 ist<.>. Types mi
   0x009536f0 736d6174 63682e00 746f5479 7065644c smatch..toTypedL
   0x00953700 69737400 00000000 2f676974 6875622f ist...../github/
   0x00953710 686f6d65 2f6d696e 69636f6e 64612f65 home/miniconda/e
   0x00953720 6e76732f 6275696c 645f6269 6e617279 nvs/build_binary
-  0x00953730 2f6c6962 2f707974 686f6e33 2e392f73 /lib/python3.9/s
+  0x00953730 2f6c6962 2f707974 686f6e33 2e382f73 /lib/python3.8/s
   0x00953740 6974652d 7061636b 61676573 2f746f72 ite-packages/tor
   0x00953750 63682f69 6e636c75 64652f41 54656e2f ch/include/ATen/
   0x00953760 636f7265 2f4c6973 745f696e 6c2e6800 core/List_inl.h.
   0x00953770 2f676974 6875622f 686f6d65 2f6d696e /github/home/min
   0x00953780 69636f6e 64612f65 6e76732f 6275696c iconda/envs/buil
   0x00953790 645f6269 6e617279 2f6c6962 2f707974 d_binary/lib/pyt
-  0x009537a0 686f6e33 2e392f73 6974652d 7061636b hon3.9/site-pack
+  0x009537a0 686f6e33 2e382f73 6974652d 7061636b hon3.8/site-pack
   0x009537b0 61676573 2f746f72 63682f69 6e636c75 ages/torch/inclu
   0x009537c0 64652f41 54656e2f 636f7265 2f626f78 de/ATen/core/box
   0x009537d0 696e672f 4b65726e 656c4675 6e637469 ing/KernelFuncti
   0x009537e0 6f6e5f69 6d706c2e 68000000 00000000 on_impl.h.......
   0x009537f0 6973446f 75626c65 28292049 4e544552 isDouble() INTER
   0x00953800 4e414c20 41535345 52542046 41494c45 NAL ASSERT FAILE
   0x00953810 44206174 20222f67 69746875 622f686f D at "/github/ho
   0x00953820 6d652f6d 696e6963 6f6e6461 2f656e76 me/miniconda/env
   0x00953830 732f6275 696c645f 62696e61 72792f6c s/build_binary/l
-  0x00953840 69622f70 7974686f 6e332e39 2f736974 ib/python3.9/sit
+  0x00953840 69622f70 7974686f 6e332e38 2f736974 ib/python3.8/sit
   0x00953850 652d7061 636b6167 65732f74 6f726368 e-packages/torch
   0x00953860 2f696e63 6c756465 2f415465 6e2f636f /include/ATen/co
   0x00953870 72652f69 76616c75 652e6822 3a353335 re/ivalue.h":535
   0x00953880 2c20706c 65617365 20726570 6f727420 , please report 
   0x00953890 61206275 6720746f 20507954 6f726368 a bug to PyTorch
   0x009538a0 2e200074 6f446f75 626c6500 00000000 . .toDouble.....
   0x009538b0 00000000 00000000 00000000 00000000 ................
@@ -15662,15 +15662,15 @@
   0x009592b0 5f32645f 666f7277 61726400 76656374 _2d_forward.vect
   0x009592c0 6f720000 00000000 6973496e 744c6973 or......isIntLis
   0x009592d0 74282920 494e5445 524e414c 20415353 t() INTERNAL ASS
   0x009592e0 45525420 4641494c 45442061 7420222f ERT FAILED at "/
   0x009592f0 67697468 75622f68 6f6d652f 6d696e69 github/home/mini
   0x00959300 636f6e64 612f656e 76732f62 75696c64 conda/envs/build
   0x00959310 5f62696e 6172792f 6c69622f 70797468 _binary/lib/pyth
-  0x00959320 6f6e332e 392f7369 74652d70 61636b61 on3.9/site-packa
+  0x00959320 6f6e332e 382f7369 74652d70 61636b61 on3.8/site-packa
   0x00959330 6765732f 746f7263 682f696e 636c7564 ges/torch/includ
   0x00959340 652f4154 656e2f63 6f72652f 6976616c e/ATen/core/ival
   0x00959350 75655f69 6e6c2e68 223a3139 36382c20 ue_inl.h":1968, 
   0x00959360 706c6561 73652072 65706f72 74206120 please report a 
   0x00959370 62756720 746f2050 79546f72 63682e20 bug to PyTorch. 
   0x00959380 00000000 00000000 00000000 00000000 ................
   0x00959390 464e3261 74365465 6e736f72 45524b53 FN2at6TensorERKS
@@ -19196,15 +19196,15 @@
   0x00966f90 01010101 01010201 01010102 04080101 ................
   0x00966fa0 01010101 01000000 00000000 70000000 ............p...
   0x00966fb0 6973496e 744c6973 74282920 494e5445 isIntList() INTE
   0x00966fc0 524e414c 20415353 45525420 4641494c RNAL ASSERT FAIL
   0x00966fd0 45442061 7420222f 67697468 75622f68 ED at "/github/h
   0x00966fe0 6f6d652f 6d696e69 636f6e64 612f656e ome/miniconda/en
   0x00966ff0 76732f62 75696c64 5f62696e 6172792f vs/build_binary/
-  0x00967000 6c69622f 70797468 6f6e332e 392f7369 lib/python3.9/si
+  0x00967000 6c69622f 70797468 6f6e332e 382f7369 lib/python3.8/si
   0x00967010 74652d70 61636b61 6765732f 746f7263 te-packages/torc
   0x00967020 682f696e 636c7564 652f4154 656e2f63 h/include/ATen/c
   0x00967030 6f72652f 6976616c 75655f69 6e6c2e68 ore/ivalue_inl.h
   0x00967040 223a3139 37362c20 706c6561 73652072 ":1976, please r
   0x00967050 65706f72 74206120 62756720 746f2050 eport a bug to P
   0x00967060 79546f72 63682e20 00746f49 6e745665 yTorch. .toIntVe
   0x00967070 63746f72 00000000 62617463 685f696e ctor....batch_in
@@ -19361,15 +19361,15 @@
   0x009679e0 49662073 6f2c2070 6c656173 65207265 If so, please re
   0x009679f0 706f7274 20616e20 656e6861 6e63656d port an enhancem
   0x00967a00 656e7420 72657175 65737420 746f2050 ent request to P
   0x00967a10 79546f72 63682e29 00000000 00000000 yTorch.)........
   0x00967a20 2f5f5f77 2f464247 454d4d2f 46424745 /__w/FBGEMM/FBGE
   0x00967a30 4d4d2f66 6267656d 6d5f6770 752f5f73 MM/fbgemm_gpu/_s
   0x00967a40 6b627569 6c642f6c 696e7578 2d783836 kbuild/linux-x86
-  0x00967a50 5f36342d 332e392f 636d616b 652d6275 _64-3.9/cmake-bu
+  0x00967a50 5f36342d 332e382f 636d616b 652d6275 _64-3.8/cmake-bu
   0x00967a60 696c642f 67656e5f 656d6265 6464696e ild/gen_embeddin
   0x00967a70 675f666f 72776172 645f7175 616e7469 g_forward_quanti
   0x00967a80 7a65645f 756e7765 69676874 65645f63 zed_unweighted_c
   0x00967a90 6f646567 656e5f63 70752e63 70700000 odegen_cpu.cpp..
   0x00967aa0 696e7438 206f7574 70757420 61726520 int8 output are 
   0x00967ab0 6f6e6c79 20737570 706f7274 65642066 only supported f
   0x00967ac0 6f722069 6e743820 77656967 68747300 or int8 weights.
@@ -19502,15 +19502,15 @@
   0x009682b0 8057f3ff 7057f3ff e058f3ff d058f3ff .W..pW...X...X..
   0x009682c0 c058f3ff b058f3ff e057f3ff d057f3ff .X...X...W...W..
   0x009682d0 c057f3ff b057f3ff 4057f3ff 3057f3ff .W...W..@W..0W..
   0x009682e0 5057f3ff 06050010 110f0000 00000000 PW..............
   0x009682f0 2f5f5f77 2f464247 454d4d2f 46424745 /__w/FBGEMM/FBGE
   0x00968300 4d4d2f66 6267656d 6d5f6770 752f5f73 MM/fbgemm_gpu/_s
   0x00968310 6b627569 6c642f6c 696e7578 2d783836 kbuild/linux-x86
-  0x00968320 5f36342d 332e392f 636d616b 652d6275 _64-3.9/cmake-bu
+  0x00968320 5f36342d 332e382f 636d616b 652d6275 _64-3.8/cmake-bu
   0x00968330 696c642f 67656e5f 656d6265 6464696e ild/gen_embeddin
   0x00968340 675f666f 72776172 645f7175 616e7469 g_forward_quanti
   0x00968350 7a65645f 77656967 68746564 5f636f64 zed_weighted_cod
   0x00968360 6567656e 5f637075 2e637070 00000000 egen_cpu.cpp....
   0x00968370 7072756e 65645f68 6173686d 61705f6c pruned_hashmap_l
   0x00968380 6f6f6b75 705f7765 69676874 65645f63 ookup_weighted_c
   0x00968390 70750000 00000000 7072756e 65645f68 pu......pruned_h
@@ -19523,15 +19523,15 @@
   0x00968400 65696768 7473206d 75737420 62652065 eights must be e
   0x00968410 6d707479 206f7220 61204350 55207465 mpty or a CPU te
   0x00968420 6e736f72 3b206974 20697320 63757272 nsor; it is curr
   0x00968430 656e746c 79206f6e 20646576 69636520 ently on device 
   0x00968440 00000000 00000000 2f5f5f77 2f464247 ......../__w/FBG
   0x00968450 454d4d2f 46424745 4d4d2f66 6267656d EMM/FBGEMM/fbgem
   0x00968460 6d5f6770 752f5f73 6b627569 6c642f6c m_gpu/_skbuild/l
-  0x00968470 696e7578 2d783836 5f36342d 332e392f inux-x86_64-3.9/
+  0x00968470 696e7578 2d783836 5f36342d 332e382f inux-x86_64-3.8/
   0x00968480 636d616b 652d6275 696c642f 67656e5f cmake-build/gen_
   0x00968490 656d6265 6464696e 675f6261 636b7761 embedding_backwa
   0x009684a0 72645f64 656e7365 5f73706c 69745f63 rd_dense_split_c
   0x009684b0 70752e63 70700000 43686563 6b206661 pu.cpp..Check fa
   0x009684c0 696c6564 3a20686f 73745f77 65696768 iled: host_weigh
   0x009684d0 74732e64 696d2829 203d3d20 31202800 ts.dim() == 1 (.
   0x009684e0 73706c69 745f656d 62656464 696e675f split_embedding_
@@ -19598,15 +19598,15 @@
   0x009688b0 5f707432 5f777261 70706572 00000000 _pt2_wrapper....
   0x009688c0 73706c69 745f656d 62656464 696e675f split_embedding_
   0x009688d0 636f6465 67656e5f 666f7277 6172645f codegen_forward_
   0x009688e0 756e7765 69676874 65645f70 74325f77 unweighted_pt2_w
   0x009688f0 72617070 65720000 2f5f5f77 2f464247 rapper../__w/FBG
   0x00968900 454d4d2f 46424745 4d4d2f66 6267656d EMM/FBGEMM/fbgem
   0x00968910 6d5f6770 752f5f73 6b627569 6c642f6c m_gpu/_skbuild/l
-  0x00968920 696e7578 2d783836 5f36342d 332e392f inux-x86_64-3.9/
+  0x00968920 696e7578 2d783836 5f36342d 332e382f inux-x86_64-3.8/
   0x00968930 636d616b 652d6275 696c642f 67656e5f cmake-build/gen_
   0x00968940 656d6265 6464696e 675f666f 72776172 embedding_forwar
   0x00968950 645f7370 6c69745f 7074325f 6370755f d_split_pt2_cpu_
   0x00968960 77726170 7065722e 63707000 00000000 wrapper.cpp.....
   0x00968970 66626765 6d6d3a3a 73706c69 745f656d fbgemm::split_em
   0x00968980 62656464 696e675f 636f6465 67656e5f bedding_codegen_
   0x00968990 67726164 5f696e64 6963655f 77656967 grad_indice_weig
@@ -19738,15 +19738,15 @@
   0x00969170 3d302920 2d3e2054 656e736f 72000000 =0) -> Tensor...
   0x00969180 73706c69 745f656d 62656464 696e675f split_embedding_
   0x00969190 636f6465 67656e5f 6c6f6f6b 75705f61 codegen_lookup_a
   0x009691a0 64616772 61645f66 756e6374 696f6e5f dagrad_function_
   0x009691b0 63707500 00000000 2f5f5f77 2f464247 cpu...../__w/FBG
   0x009691c0 454d4d2f 46424745 4d4d2f66 6267656d EMM/FBGEMM/fbgem
   0x009691d0 6d5f6770 752f5f73 6b627569 6c642f6c m_gpu/_skbuild/l
-  0x009691e0 696e7578 2d783836 5f36342d 332e392f inux-x86_64-3.9/
+  0x009691e0 696e7578 2d783836 5f36342d 332e382f inux-x86_64-3.8/
   0x009691f0 636d616b 652d6275 696c642f 67656e5f cmake-build/gen_
   0x00969200 656d6265 6464696e 675f6261 636b7761 embedding_backwa
   0x00969210 72645f73 706c6974 5f616461 67726164 rd_split_adagrad
   0x00969220 5f637075 2e637070 00000000 00000000 _cpu.cpp........
   0x00969230 66626765 6d6d3a3a 73706c69 745f656d fbgemm::split_em
   0x00969240 62656464 696e675f 6261636b 77617264 bedding_backward
   0x00969250 5f636f64 6567656e 5f616461 67726164 _codegen_adagrad
@@ -19854,15 +19854,15 @@
   0x009698b0 53305f6c 5374386f 7074696f 6e616c49 S0_lSt8optionalI
   0x009698c0 53305f45 53345f62 64625330 5f53305f S0_ES4_bdbS0_S0_
   0x009698d0 53305f64 646c4500 00000000 00000000 S0_ddlE.........
   0x009698e0 00000000 00000080 00000000 00000000 ................
   0x009698f0 2f5f5f77 2f464247 454d4d2f 46424745 /__w/FBGEMM/FBGE
   0x00969900 4d4d2f66 6267656d 6d5f6770 752f5f73 MM/fbgemm_gpu/_s
   0x00969910 6b627569 6c642f6c 696e7578 2d783836 kbuild/linux-x86
-  0x00969920 5f36342d 332e392f 636d616b 652d6275 _64-3.9/cmake-bu
+  0x00969920 5f36342d 332e382f 636d616b 652d6275 _64-3.8/cmake-bu
   0x00969930 696c642f 67656e5f 656d6265 6464696e ild/gen_embeddin
   0x00969940 675f6261 636b7761 72645f73 706c6974 g_backward_split
   0x00969950 5f616461 67726164 5f707432 5f637075 _adagrad_pt2_cpu
   0x00969960 5f777261 70706572 2e637070 00000000 _wrapper.cpp....
   0x00969970 73706c69 745f656d 62656464 696e675f split_embedding_
   0x00969980 6261636b 77617264 5f636f64 6567656e backward_codegen
   0x00969990 5f616461 67726164 5f776569 67687465 _adagrad_weighte
@@ -19975,15 +19975,15 @@
   0x0096a040 00000000 00000000 73706c69 745f656d ........split_em
   0x0096a050 62656464 696e675f 636f6465 67656e5f bedding_codegen_
   0x0096a060 6c6f6f6b 75705f72 6f777769 73655f61 lookup_rowwise_a
   0x0096a070 64616772 61645f66 756e6374 696f6e5f dagrad_function_
   0x0096a080 63707500 00000000 2f5f5f77 2f464247 cpu...../__w/FBG
   0x0096a090 454d4d2f 46424745 4d4d2f66 6267656d EMM/FBGEMM/fbgem
   0x0096a0a0 6d5f6770 752f5f73 6b627569 6c642f6c m_gpu/_skbuild/l
-  0x0096a0b0 696e7578 2d783836 5f36342d 332e392f inux-x86_64-3.9/
+  0x0096a0b0 696e7578 2d783836 5f36342d 332e382f inux-x86_64-3.8/
   0x0096a0c0 636d616b 652d6275 696c642f 67656e5f cmake-build/gen_
   0x0096a0d0 656d6265 6464696e 675f6261 636b7761 embedding_backwa
   0x0096a0e0 72645f73 706c6974 5f726f77 77697365 rd_split_rowwise
   0x0096a0f0 5f616461 67726164 5f637075 2e637070 _adagrad_cpu.cpp
   0x0096a100 00000000 00000000 66626765 6d6d3a3a ........fbgemm::
   0x0096a110 73706c69 745f656d 62656464 696e675f split_embedding_
   0x0096a120 6261636b 77617264 5f636f64 6567656e backward_codegen
@@ -20097,15 +20097,15 @@
   0x0096a7e0 796d496e 74455332 5f53305f 6c53305f ymIntES2_S0_lS0_
   0x0096a7f0 53305f6c 5374386f 7074696f 6e616c49 S0_lSt8optionalI
   0x0096a800 53305f45 53345f62 64625330 5f53305f S0_ES4_bdbS0_S0_
   0x0096a810 53305f64 64646c64 6c450000 00000000 S0_dddldlE......
   0x0096a820 2f5f5f77 2f464247 454d4d2f 46424745 /__w/FBGEMM/FBGE
   0x0096a830 4d4d2f66 6267656d 6d5f6770 752f5f73 MM/fbgemm_gpu/_s
   0x0096a840 6b627569 6c642f6c 696e7578 2d783836 kbuild/linux-x86
-  0x0096a850 5f36342d 332e392f 636d616b 652d6275 _64-3.9/cmake-bu
+  0x0096a850 5f36342d 332e382f 636d616b 652d6275 _64-3.8/cmake-bu
   0x0096a860 696c642f 67656e5f 656d6265 6464696e ild/gen_embeddin
   0x0096a870 675f6261 636b7761 72645f73 706c6974 g_backward_split
   0x0096a880 5f726f77 77697365 5f616461 67726164 _rowwise_adagrad
   0x0096a890 5f707432 5f637075 5f777261 70706572 _pt2_cpu_wrapper
   0x0096a8a0 2e637070 00000000 73706c69 745f656d .cpp....split_em
   0x0096a8b0 62656464 696e675f 6261636b 77617264 bedding_backward
   0x0096a8c0 5f636f64 6567656e 5f726f77 77697365 _codegen_rowwise
@@ -20209,15 +20209,15 @@
   0x0096aee0 745f6474 7970653d 3029202d 3e205465 t_dtype=0) -> Te
   0x0096aef0 6e736f72 00000000 73706c69 745f656d nsor....split_em
   0x0096af00 62656464 696e675f 636f6465 67656e5f bedding_codegen_
   0x0096af10 6c6f6f6b 75705f73 67645f66 756e6374 lookup_sgd_funct
   0x0096af20 696f6e5f 63707500 2f5f5f77 2f464247 ion_cpu./__w/FBG
   0x0096af30 454d4d2f 46424745 4d4d2f66 6267656d EMM/FBGEMM/fbgem
   0x0096af40 6d5f6770 752f5f73 6b627569 6c642f6c m_gpu/_skbuild/l
-  0x0096af50 696e7578 2d783836 5f36342d 332e392f inux-x86_64-3.9/
+  0x0096af50 696e7578 2d783836 5f36342d 332e382f inux-x86_64-3.8/
   0x0096af60 636d616b 652d6275 696c642f 67656e5f cmake-build/gen_
   0x0096af70 656d6265 6464696e 675f6261 636b7761 embedding_backwa
   0x0096af80 72645f73 706c6974 5f736764 5f637075 rd_split_sgd_cpu
   0x0096af90 2e637070 00000000 66626765 6d6d3a3a .cpp....fbgemm::
   0x0096afa0 73706c69 745f656d 62656464 696e675f split_embedding_
   0x0096afb0 6261636b 77617264 5f636f64 6567656e backward_codegen
   0x0096afc0 5f736764 5f637075 00000000 00000000 _sgd_cpu........
@@ -20318,15 +20318,15 @@
   0x0096b5b0 53305f53 305f5330 5f4e3363 31303653 S0_S0_S0_N3c106S
   0x0096b5c0 796d496e 74455332 5f53305f 6c53305f ymIntES2_S0_lS0_
   0x0096b5d0 53305f6c 5374386f 7074696f 6e616c49 S0_lSt8optionalI
   0x0096b5e0 53305f45 53345f62 6462646c 45000000 S0_ES4_bdbdlE...
   0x0096b5f0 2f5f5f77 2f464247 454d4d2f 46424745 /__w/FBGEMM/FBGE
   0x0096b600 4d4d2f66 6267656d 6d5f6770 752f5f73 MM/fbgemm_gpu/_s
   0x0096b610 6b627569 6c642f6c 696e7578 2d783836 kbuild/linux-x86
-  0x0096b620 5f36342d 332e392f 636d616b 652d6275 _64-3.9/cmake-bu
+  0x0096b620 5f36342d 332e382f 636d616b 652d6275 _64-3.8/cmake-bu
   0x0096b630 696c642f 67656e5f 656d6265 6464696e ild/gen_embeddin
   0x0096b640 675f6261 636b7761 72645f73 706c6974 g_backward_split
   0x0096b650 5f736764 5f707432 5f637075 5f777261 _sgd_pt2_cpu_wra
   0x0096b660 70706572 2e637070 00000000 00000000 pper.cpp........
   0x0096b670 73706c69 745f656d 62656464 696e675f split_embedding_
   0x0096b680 6261636b 77617264 5f636f64 6567656e backward_codegen
   0x0096b690 5f736764 5f776569 67687465 645f6578 _sgd_weighted_ex
@@ -20397,15 +20397,15 @@
   0x0096baa0 3a2f2f67 69746875 622e636f 6d2f7079 ://github.com/py
   0x0096bab0 746f7263 682f4642 47454d4d 2f646973 torch/FBGEMM/dis
   0x0096bac0 63757373 696f6e73 2f313732 3720666f cussions/1727 fo
   0x0096bad0 72206d6f 72652064 65746169 6c2e0000 r more detail...
   0x0096bae0 2f5f5f77 2f464247 454d4d2f 46424745 /__w/FBGEMM/FBGE
   0x0096baf0 4d4d2f66 6267656d 6d5f6770 752f5f73 MM/fbgemm_gpu/_s
   0x0096bb00 6b627569 6c642f6c 696e7578 2d783836 kbuild/linux-x86
-  0x0096bb10 5f36342d 332e392f 636d616b 652d6275 _64-3.9/cmake-bu
+  0x0096bb10 5f36342d 332e382f 636d616b 652d6275 _64-3.8/cmake-bu
   0x0096bb20 696c642f 67656e5f 656d6265 6464696e ild/gen_embeddin
   0x0096bb30 675f6261 636b7761 72645f73 706c6974 g_backward_split
   0x0096bb40 5f616461 6d5f6370 752e6370 70000000 _adam_cpu.cpp...
   0x0096bb50 73706c69 745f656d 62656464 696e675f split_embedding_
   0x0096bb60 636f6465 67656e5f 6c6f6f6b 75705f61 codegen_lookup_a
   0x0096bb70 64616d5f 66756e63 74696f6e 5f637075 dam_function_cpu
   0x0096bb80 00000000 00000000 73706c69 745f656d ........split_em
@@ -20494,15 +20494,15 @@
   0x0096c0b0 65652068 74747073 3a2f2f67 69746875 ee https://githu
   0x0096c0c0 622e636f 6d2f7079 746f7263 682f4642 b.com/pytorch/FB
   0x0096c0d0 47454d4d 2f646973 63757373 696f6e73 GEMM/discussions
   0x0096c0e0 2f313732 3720666f 72206d6f 72652064 /1727 for more d
   0x0096c0f0 65746169 6c2e0000 2f5f5f77 2f464247 etail.../__w/FBG
   0x0096c100 454d4d2f 46424745 4d4d2f66 6267656d EMM/FBGEMM/fbgem
   0x0096c110 6d5f6770 752f5f73 6b627569 6c642f6c m_gpu/_skbuild/l
-  0x0096c120 696e7578 2d783836 5f36342d 332e392f inux-x86_64-3.9/
+  0x0096c120 696e7578 2d783836 5f36342d 332e382f inux-x86_64-3.8/
   0x0096c130 636d616b 652d6275 696c642f 67656e5f cmake-build/gen_
   0x0096c140 656d6265 6464696e 675f6261 636b7761 embedding_backwa
   0x0096c150 72645f73 706c6974 5f6c616d 625f6370 rd_split_lamb_cp
   0x0096c160 752e6370 70000000 73706c69 745f656d u.cpp...split_em
   0x0096c170 62656464 696e675f 636f6465 67656e5f bedding_codegen_
   0x0096c180 6c6f6f6b 75705f6c 616d625f 66756e63 lookup_lamb_func
   0x0096c190 74696f6e 5f637075 00000000 00000000 tion_cpu........
@@ -20585,15 +20585,15 @@
   0x0096c660 3a2f2f67 69746875 622e636f 6d2f7079 ://github.com/py
   0x0096c670 746f7263 682f4642 47454d4d 2f646973 torch/FBGEMM/dis
   0x0096c680 63757373 696f6e73 2f313732 3720666f cussions/1727 fo
   0x0096c690 72206d6f 72652064 65746169 6c2e0000 r more detail...
   0x0096c6a0 2f5f5f77 2f464247 454d4d2f 46424745 /__w/FBGEMM/FBGE
   0x0096c6b0 4d4d2f66 6267656d 6d5f6770 752f5f73 MM/fbgemm_gpu/_s
   0x0096c6c0 6b627569 6c642f6c 696e7578 2d783836 kbuild/linux-x86
-  0x0096c6d0 5f36342d 332e392f 636d616b 652d6275 _64-3.9/cmake-bu
+  0x0096c6d0 5f36342d 332e382f 636d616b 652d6275 _64-3.8/cmake-bu
   0x0096c6e0 696c642f 67656e5f 656d6265 6464696e ild/gen_embeddin
   0x0096c6f0 675f6261 636b7761 72645f73 706c6974 g_backward_split
   0x0096c700 5f706172 7469616c 5f726f77 77697365 _partial_rowwise
   0x0096c710 5f616461 6d5f6370 752e6370 70000000 _adam_cpu.cpp...
   0x0096c720 73706c69 745f656d 62656464 696e675f split_embedding_
   0x0096c730 636f6465 67656e5f 6c6f6f6b 75705f70 codegen_lookup_p
   0x0096c740 61727469 616c5f72 6f777769 73655f61 artial_rowwise_a
@@ -20680,15 +20680,15 @@
   0x0096cc50 3a2f2f67 69746875 622e636f 6d2f7079 ://github.com/py
   0x0096cc60 746f7263 682f4642 47454d4d 2f646973 torch/FBGEMM/dis
   0x0096cc70 63757373 696f6e73 2f313732 3720666f cussions/1727 fo
   0x0096cc80 72206d6f 72652064 65746169 6c2e0000 r more detail...
   0x0096cc90 2f5f5f77 2f464247 454d4d2f 46424745 /__w/FBGEMM/FBGE
   0x0096cca0 4d4d2f66 6267656d 6d5f6770 752f5f73 MM/fbgemm_gpu/_s
   0x0096ccb0 6b627569 6c642f6c 696e7578 2d783836 kbuild/linux-x86
-  0x0096ccc0 5f36342d 332e392f 636d616b 652d6275 _64-3.9/cmake-bu
+  0x0096ccc0 5f36342d 332e382f 636d616b 652d6275 _64-3.8/cmake-bu
   0x0096ccd0 696c642f 67656e5f 656d6265 6464696e ild/gen_embeddin
   0x0096cce0 675f6261 636b7761 72645f73 706c6974 g_backward_split
   0x0096ccf0 5f706172 7469616c 5f726f77 77697365 _partial_rowwise
   0x0096cd00 5f6c616d 625f6370 752e6370 70000000 _lamb_cpu.cpp...
   0x0096cd10 73706c69 745f656d 62656464 696e675f split_embedding_
   0x0096cd20 636f6465 67656e5f 6c6f6f6b 75705f70 codegen_lookup_p
   0x0096cd30 61727469 616c5f72 6f777769 73655f6c artial_rowwise_l
@@ -20775,15 +20775,15 @@
   0x0096d240 74747073 3a2f2f67 69746875 622e636f ttps://github.co
   0x0096d250 6d2f7079 746f7263 682f4642 47454d4d m/pytorch/FBGEMM
   0x0096d260 2f646973 63757373 696f6e73 2f313732 /discussions/172
   0x0096d270 3720666f 72206d6f 72652064 65746169 7 for more detai
   0x0096d280 6c2e0000 00000000 2f5f5f77 2f464247 l......./__w/FBG
   0x0096d290 454d4d2f 46424745 4d4d2f66 6267656d EMM/FBGEMM/fbgem
   0x0096d2a0 6d5f6770 752f5f73 6b627569 6c642f6c m_gpu/_skbuild/l
-  0x0096d2b0 696e7578 2d783836 5f36342d 332e392f inux-x86_64-3.9/
+  0x0096d2b0 696e7578 2d783836 5f36342d 332e382f inux-x86_64-3.8/
   0x0096d2c0 636d616b 652d6275 696c642f 67656e5f cmake-build/gen_
   0x0096d2d0 656d6265 6464696e 675f6261 636b7761 embedding_backwa
   0x0096d2e0 72645f73 706c6974 5f6c6172 735f7367 rd_split_lars_sg
   0x0096d2f0 645f6370 752e6370 70000000 00000000 d_cpu.cpp.......
   0x0096d300 73706c69 745f656d 62656464 696e675f split_embedding_
   0x0096d310 636f6465 67656e5f 6c6f6f6b 75705f6c codegen_lookup_l
   0x0096d320 6172735f 7367645f 66756e63 74696f6e ars_sgd_function
@@ -20866,15 +20866,15 @@
   0x0096d7f0 3a2f2f67 69746875 622e636f 6d2f7079 ://github.com/py
   0x0096d800 746f7263 682f4642 47454d4d 2f646973 torch/FBGEMM/dis
   0x0096d810 63757373 696f6e73 2f313732 3720666f cussions/1727 fo
   0x0096d820 72206d6f 72652064 65746169 6c2e0000 r more detail...
   0x0096d830 2f5f5f77 2f464247 454d4d2f 46424745 /__w/FBGEMM/FBGE
   0x0096d840 4d4d2f66 6267656d 6d5f6770 752f5f73 MM/fbgemm_gpu/_s
   0x0096d850 6b627569 6c642f6c 696e7578 2d783836 kbuild/linux-x86
-  0x0096d860 5f36342d 332e392f 636d616b 652d6275 _64-3.9/cmake-bu
+  0x0096d860 5f36342d 332e382f 636d616b 652d6275 _64-3.8/cmake-bu
   0x0096d870 696c642f 67656e5f 656d6265 6464696e ild/gen_embeddin
   0x0096d880 675f6261 636b7761 72645f73 706c6974 g_backward_split
   0x0096d890 5f6e6f6e 655f6370 752e6370 70000000 _none_cpu.cpp...
   0x0096d8a0 73706c69 745f656d 62656464 696e675f split_embedding_
   0x0096d8b0 636f6465 67656e5f 6c6f6f6b 75705f6e codegen_lookup_n
   0x0096d8c0 6f6e655f 66756e63 74696f6e 5f637075 one_function_cpu
   0x0096d8d0 00000000 00000000 73706c69 745f656d ........split_em
@@ -20944,15 +20944,15 @@
   0x0096dcd0 65652068 74747073 3a2f2f67 69746875 ee https://githu
   0x0096dce0 622e636f 6d2f7079 746f7263 682f4642 b.com/pytorch/FB
   0x0096dcf0 47454d4d 2f646973 63757373 696f6e73 GEMM/discussions
   0x0096dd00 2f313732 3720666f 72206d6f 72652064 /1727 for more d
   0x0096dd10 65746169 6c2e0000 2f5f5f77 2f464247 etail.../__w/FBG
   0x0096dd20 454d4d2f 46424745 4d4d2f66 6267656d EMM/FBGEMM/fbgem
   0x0096dd30 6d5f6770 752f5f73 6b627569 6c642f6c m_gpu/_skbuild/l
-  0x0096dd40 696e7578 2d783836 5f36342d 332e392f inux-x86_64-3.9/
+  0x0096dd40 696e7578 2d783836 5f36342d 332e382f inux-x86_64-3.8/
   0x0096dd50 636d616b 652d6275 696c642f 67656e5f cmake-build/gen_
   0x0096dd60 656d6265 6464696e 675f6261 636b7761 embedding_backwa
   0x0096dd70 72645f73 706c6974 5f726f77 77697365 rd_split_rowwise
   0x0096dd80 5f616461 67726164 5f776974 685f636f _adagrad_with_co
   0x0096dd90 756e7465 725f6370 752e6370 70000000 unter_cpu.cpp...
   0x0096dda0 73706c69 745f656d 62656464 696e675f split_embedding_
   0x0096ddb0 636f6465 67656e5f 6c6f6f6b 75705f72 codegen_lookup_r
@@ -21078,15 +21078,15 @@
   0x0096e530 2f676974 6875622e 636f6d2f 7079746f /github.com/pyto
   0x0096e540 7263682f 46424745 4d4d2f64 69736375 rch/FBGEMM/discu
   0x0096e550 7373696f 6e732f31 37323720 666f7220 ssions/1727 for 
   0x0096e560 6d6f7265 20646574 61696c2e 00000000 more detail.....
   0x0096e570 2f5f5f77 2f464247 454d4d2f 46424745 /__w/FBGEMM/FBGE
   0x0096e580 4d4d2f66 6267656d 6d5f6770 752f5f73 MM/fbgemm_gpu/_s
   0x0096e590 6b627569 6c642f6c 696e7578 2d783836 kbuild/linux-x86
-  0x0096e5a0 5f36342d 332e392f 636d616b 652d6275 _64-3.9/cmake-bu
+  0x0096e5a0 5f36342d 332e382f 636d616b 652d6275 _64-3.8/cmake-bu
   0x0096e5b0 696c642f 67656e5f 656d6265 6464696e ild/gen_embeddin
   0x0096e5c0 675f6261 636b7761 72645f73 706c6974 g_backward_split
   0x0096e5d0 5f617070 726f785f 7367645f 6370752e _approx_sgd_cpu.
   0x0096e5e0 63707000 00000000 73706c69 745f656d cpp.....split_em
   0x0096e5f0 62656464 696e675f 636f6465 67656e5f bedding_codegen_
   0x0096e600 6c6f6f6b 75705f61 7070726f 785f7367 lookup_approx_sg
   0x0096e610 645f6675 6e637469 6f6e5f63 70750000 d_function_cpu..
@@ -21151,15 +21151,15 @@
   0x0096e9c0 70733a2f 2f676974 6875622e 636f6d2f ps://github.com/
   0x0096e9d0 7079746f 7263682f 46424745 4d4d2f64 pytorch/FBGEMM/d
   0x0096e9e0 69736375 7373696f 6e732f31 37323720 iscussions/1727 
   0x0096e9f0 666f7220 6d6f7265 20646574 61696c2e for more detail.
   0x0096ea00 00000000 00000000 2f5f5f77 2f464247 ......../__w/FBG
   0x0096ea10 454d4d2f 46424745 4d4d2f66 6267656d EMM/FBGEMM/fbgem
   0x0096ea20 6d5f6770 752f5f73 6b627569 6c642f6c m_gpu/_skbuild/l
-  0x0096ea30 696e7578 2d783836 5f36342d 332e392f inux-x86_64-3.9/
+  0x0096ea30 696e7578 2d783836 5f36342d 332e382f inux-x86_64-3.8/
   0x0096ea40 636d616b 652d6275 696c642f 67656e5f cmake-build/gen_
   0x0096ea50 656d6265 6464696e 675f6261 636b7761 embedding_backwa
   0x0096ea60 72645f73 706c6974 5f617070 726f785f rd_split_approx_
   0x0096ea70 726f7777 6973655f 61646167 7261645f rowwise_adagrad_
   0x0096ea80 6370752e 63707000 73706c69 745f656d cpu.cpp.split_em
   0x0096ea90 62656464 696e675f 636f6465 67656e5f bedding_codegen_
   0x0096eaa0 6c6f6f6b 75705f61 7070726f 785f726f lookup_approx_ro
@@ -21246,15 +21246,15 @@
   0x0096efb0 2f2f6769 74687562 2e636f6d 2f707974 //github.com/pyt
   0x0096efc0 6f726368 2f464247 454d4d2f 64697363 orch/FBGEMM/disc
   0x0096efd0 75737369 6f6e732f 31373237 20666f72 ussions/1727 for
   0x0096efe0 206d6f72 65206465 7461696c 2e000000  more detail....
   0x0096eff0 2f5f5f77 2f464247 454d4d2f 46424745 /__w/FBGEMM/FBGE
   0x0096f000 4d4d2f66 6267656d 6d5f6770 752f5f73 MM/fbgemm_gpu/_s
   0x0096f010 6b627569 6c642f6c 696e7578 2d783836 kbuild/linux-x86
-  0x0096f020 5f36342d 332e392f 636d616b 652d6275 _64-3.9/cmake-bu
+  0x0096f020 5f36342d 332e382f 636d616b 652d6275 _64-3.8/cmake-bu
   0x0096f030 696c642f 67656e5f 656d6265 6464696e ild/gen_embeddin
   0x0096f040 675f6261 636b7761 72645f73 706c6974 g_backward_split
   0x0096f050 5f617070 726f785f 726f7777 6973655f _approx_rowwise_
   0x0096f060 61646167 7261645f 77697468 5f636f75 adagrad_with_cou
   0x0096f070 6e746572 5f637075 2e637070 00000000 nter_cpu.cpp....
   0x0096f080 73706c69 745f656d 62656464 696e675f split_embedding_
   0x0096f090 636f6465 67656e5f 6c6f6f6b 75705f61 codegen_lookup_a
@@ -21374,15 +21374,15 @@
   0x0096f7b0 69746875 622e636f 6d2f7079 746f7263 ithub.com/pytorc
   0x0096f7c0 682f4642 47454d4d 2f646973 63757373 h/FBGEMM/discuss
   0x0096f7d0 696f6e73 2f313732 3720666f 72206d6f ions/1727 for mo
   0x0096f7e0 72652064 65746169 6c2e0000 00000000 re detail.......
   0x0096f7f0 2f5f5f77 2f464247 454d4d2f 46424745 /__w/FBGEMM/FBGE
   0x0096f800 4d4d2f66 6267656d 6d5f6770 752f5f73 MM/fbgemm_gpu/_s
   0x0096f810 6b627569 6c642f6c 696e7578 2d783836 kbuild/linux-x86
-  0x0096f820 5f36342d 332e392f 636d616b 652d6275 _64-3.9/cmake-bu
+  0x0096f820 5f36342d 332e382f 636d616b 652d6275 _64-3.8/cmake-bu
   0x0096f830 696c642f 67656e5f 656d6265 6464696e ild/gen_embeddin
   0x0096f840 675f6261 636b7761 72645f73 706c6974 g_backward_split
   0x0096f850 5f617070 726f785f 726f7777 6973655f _approx_rowwise_
   0x0096f860 61646167 7261645f 77697468 5f776569 adagrad_with_wei
   0x0096f870 6768745f 64656361 795f6370 752e6370 ght_decay_cpu.cp
   0x0096f880 70000000 00000000 73706c69 745f656d p.......split_em
   0x0096f890 62656464 696e675f 636f6465 67656e5f bedding_codegen_
@@ -21466,15 +21466,15 @@
   0x0096fd70 68747470 733a2f2f 67697468 75622e63 https://github.c
   0x0096fd80 6f6d2f70 79746f72 63682f46 4247454d om/pytorch/FBGEM
   0x0096fd90 4d2f6469 73637573 73696f6e 732f3137 M/discussions/17
   0x0096fda0 32372066 6f72206d 6f726520 64657461 27 for more deta
   0x0096fdb0 696c2e00 00000000 2f5f5f77 2f464247 il....../__w/FBG
   0x0096fdc0 454d4d2f 46424745 4d4d2f66 6267656d EMM/FBGEMM/fbgem
   0x0096fdd0 6d5f6770 752f5f73 6b627569 6c642f6c m_gpu/_skbuild/l
-  0x0096fde0 696e7578 2d783836 5f36342d 332e392f inux-x86_64-3.9/
+  0x0096fde0 696e7578 2d783836 5f36342d 332e382f inux-x86_64-3.8/
   0x0096fdf0 636d616b 652d6275 696c642f 67656e5f cmake-build/gen_
   0x0096fe00 656d6265 6464696e 675f6261 636b7761 embedding_backwa
   0x0096fe10 72645f73 706c6974 5f726f77 77697365 rd_split_rowwise
   0x0096fe20 5f616461 67726164 5f776974 685f7765 _adagrad_with_we
   0x0096fe30 69676874 5f646563 61795f63 70752e63 ight_decay_cpu.c
   0x0096fe40 70700000 00000000 73706c69 745f656d pp......split_em
   0x0096fe50 62656464 696e675f 636f6465 67656e5f bedding_codegen_
@@ -21557,15 +21557,15 @@
   0x00970320 74747073 3a2f2f67 69746875 622e636f ttps://github.co
   0x00970330 6d2f7079 746f7263 682f4642 47454d4d m/pytorch/FBGEMM
   0x00970340 2f646973 63757373 696f6e73 2f313732 /discussions/172
   0x00970350 3720666f 72206d6f 72652064 65746169 7 for more detai
   0x00970360 6c2e0000 00000000 2f5f5f77 2f464247 l......./__w/FBG
   0x00970370 454d4d2f 46424745 4d4d2f66 6267656d EMM/FBGEMM/fbgem
   0x00970380 6d5f6770 752f5f73 6b627569 6c642f6c m_gpu/_skbuild/l
-  0x00970390 696e7578 2d783836 5f36342d 332e392f inux-x86_64-3.9/
+  0x00970390 696e7578 2d783836 5f36342d 332e382f inux-x86_64-3.8/
   0x009703a0 636d616b 652d6275 696c642f 67656e5f cmake-build/gen_
   0x009703b0 656d6265 6464696e 675f6261 636b7761 embedding_backwa
   0x009703c0 72645f73 706c6974 5f726f77 77697365 rd_split_rowwise
   0x009703d0 5f776569 67687465 645f6164 61677261 _weighted_adagra
   0x009703e0 645f6370 752e6370 70000000 00000000 d_cpu.cpp.......
   0x009703f0 73706c69 745f656d 62656464 696e675f split_embedding_
   0x00970400 636f6465 67656e5f 6c6f6f6b 75705f72 codegen_lookup_r
@@ -21643,15 +21643,15 @@
   0x00970880 3c6df9ff 2c6df9ff 1c6df9ff fc6df9ff <m..,m...m...m..
   0x00970890 ec6df9ff dc6df9ff cc6df9ff 3c6ff9ff .m...m...m..<o..
   0x009708a0 2c6ff9ff 1c6ff9ff 0c6ff9ff 3c6ef9ff ,o...o...o..<n..
   0x009708b0 2c6ef9ff 1c6ef9ff 0c6ef9ff 9c6df9ff ,n...n...n...m..
   0x009708c0 8c6df9ff ac6df9ff 2f5f5f77 2f464247 .m...m../__w/FBG
   0x009708d0 454d4d2f 46424745 4d4d2f66 6267656d EMM/FBGEMM/fbgem
   0x009708e0 6d5f6770 752f5f73 6b627569 6c642f6c m_gpu/_skbuild/l
-  0x009708f0 696e7578 2d783836 5f36342d 332e392f inux-x86_64-3.9/
+  0x009708f0 696e7578 2d783836 5f36342d 332e382f inux-x86_64-3.8/
   0x00970900 636d616b 652d6275 696c642f 67656e5f cmake-build/gen_
   0x00970910 656d6265 6464696e 675f6261 636b7761 embedding_backwa
   0x00970920 72645f61 64616772 61645f73 706c6974 rd_adagrad_split
   0x00970930 5f637075 2e637070 00000000 00000000 _cpu.cpp........
   0x00970940 73706c69 745f656d 62656464 696e675f split_embedding_
   0x00970950 6261636b 77617264 5f657861 63745f63 backward_exact_c
   0x00970960 70755f6f 75746572 00000000 00000000 pu_outer........
@@ -21724,15 +21724,15 @@
   0x00970d90 6ccbf9ff 5ccbf9ff 4ccbf9ff dccaf9ff l...\...L.......
   0x00970da0 cccaf9ff eccaf9ff 6e756d20 6f662072 ........num of r
   0x00970db0 6f777320 70726f63 65737365 64206279 ows processed by
   0x00970dc0 20616461 67726164 3a200000 00000000  adagrad: ......
   0x00970dd0 2f5f5f77 2f464247 454d4d2f 46424745 /__w/FBGEMM/FBGE
   0x00970de0 4d4d2f66 6267656d 6d5f6770 752f5f73 MM/fbgemm_gpu/_s
   0x00970df0 6b627569 6c642f6c 696e7578 2d783836 kbuild/linux-x86
-  0x00970e00 5f36342d 332e392f 636d616b 652d6275 _64-3.9/cmake-bu
+  0x00970e00 5f36342d 332e382f 636d616b 652d6275 _64-3.8/cmake-bu
   0x00970e10 696c642f 67656e5f 656d6265 6464696e ild/gen_embeddin
   0x00970e20 675f6261 636b7761 72645f72 6f777769 g_backward_rowwi
   0x00970e30 73655f61 64616772 61645f73 706c6974 se_adagrad_split
   0x00970e40 5f637075 2e637070 00000000 00000000 _cpu.cpp........
   0x00970e50 73706c69 745f656d 62656464 696e675f split_embedding_
   0x00970e60 6261636b 77617264 5f636f64 6567656e backward_codegen
   0x00970e70 5f726f77 77697365 5f616461 67726164 _rowwise_adagrad
@@ -21797,15 +21797,15 @@
   0x00971220 684afaff 584afaff 484afaff 384afaff hJ..XJ..HJ..8J..
   0x00971230 a84bfaff 984bfaff 884bfaff 784bfaff .K...K...K..xK..
   0x00971240 a84afaff 984afaff 884afaff 784afaff .J...J...J..xJ..
   0x00971250 084afaff f849faff 184afaff 00000000 .J...I...J......
   0x00971260 2f5f5f77 2f464247 454d4d2f 46424745 /__w/FBGEMM/FBGE
   0x00971270 4d4d2f66 6267656d 6d5f6770 752f5f73 MM/fbgemm_gpu/_s
   0x00971280 6b627569 6c642f6c 696e7578 2d783836 kbuild/linux-x86
-  0x00971290 5f36342d 332e392f 636d616b 652d6275 _64-3.9/cmake-bu
+  0x00971290 5f36342d 332e382f 636d616b 652d6275 _64-3.8/cmake-bu
   0x009712a0 696c642f 67656e5f 656d6265 6464696e ild/gen_embeddin
   0x009712b0 675f6261 636b7761 72645f73 67645f73 g_backward_sgd_s
   0x009712c0 706c6974 5f637075 2e637070 00000000 plit_cpu.cpp....
   0x009712d0 73706c69 745f656d 62656464 696e675f split_embedding_
   0x009712e0 6261636b 77617264 5f636f64 6567656e backward_codegen
   0x009712f0 5f736764 5f637075 2854656e 736f7220 _sgd_cpu(Tensor 
   0x00971300 67726164 5f6f7574 7075742c 2054656e grad_output, Ten
```

## fbgemm_gpu/sparse_ops.py

```diff
@@ -8,14 +8,15 @@
 
 from typing import Callable, List, Optional, Tuple
 
 import torch
 
 from fbgemm_gpu.split_embedding_configs import SparseType
 from fbgemm_gpu.split_table_batched_embeddings_ops_common import PoolingMode
+from torch import SymInt
 
 try:
     # pyre-ignore
     from fbgemm_gpu import open_source  # noqa: F401
 except Exception:
     if torch.version.hip:
         torch.ops.load_library("//deeplearning/fbgemm/fbgemm_gpu:sparse_ops_hip")
@@ -564,13 +565,15 @@
 def bounds_check_indices_abstract(
     rows_per_table: torch.Tensor,
     indices: torch.Tensor,
     offsets: torch.Tensor,
     bounds_check_mode_int: int,
     bounds_check_warning: torch.Tensor,
     per_sample_weights: Optional[torch.Tensor] = None,
+    B_offsets: Optional[torch.Tensor] = None,
+    max_B: Optional[SymInt] = None,
 ) -> None:
     """
     This meta function is used to fake the bounds checking
     from the original function `fbgemm::bounds_check_indices`
     """
     return
```

## fbgemm_gpu/docs/version.py

```diff
@@ -2,8 +2,8 @@
 #!/usr/bin/env python3
 # Copyright (c) Meta Platforms, Inc. and affiliates.
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
-__version__: str = "2024.4.15"
+__version__: str = "2024.4.16"
```

## Comparing `fbgemm_gpu_nightly_cpu-2024.4.15.dist-info/METADATA` & `fbgemm_gpu_nightly_cpu-2024.4.16.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fbgemm-gpu-nightly-cpu
-Version: 2024.4.15
+Version: 2024.4.16
 Home-page: https://github.com/pytorch/fbgemm
 Author: FBGEMM Team
 Author-email: packages@pytorch.org
 License: BSD-3
 Keywords: PyTorch,Recommendation Models,High Performance Computing,GPU,CUDA
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

## Comparing `fbgemm_gpu_nightly_cpu-2024.4.15.dist-info/RECORD` & `fbgemm_gpu_nightly_cpu-2024.4.16.dist-info/RECORD`

 * *Files 5% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 fbgemm_gpu/__init__.py,sha256=ZPy0iaSSHb6-eT6lz8MSpr-5Ircj9SLmVpL0o0ejcNQ,914
 fbgemm_gpu/batched_unary_embeddings_ops.py,sha256=dpxZAueNsadJVuK7Dwo8GbOlho9r67Lfh8kesqRKJNI,3079
 fbgemm_gpu/enums.py,sha256=GVuzF5cFTLzttkvlH1SdcGrxrppMhDSbQj_Vm_4zmEo,789
-fbgemm_gpu/fbgemm_gpu_py.so,sha256=QMHmQUL1JE8KyHBSoZ1bJIBcnyrbw4ojizd8Ak0V-No,10617336
+fbgemm_gpu/fbgemm_gpu_py.so,sha256=lC1RTDFrCea4JSUUHWTdvVdmRcyKoD3dLeaf6r-lHKQ,10617336
 fbgemm_gpu/metrics.py,sha256=TsurFLJf0nJvPDN7urWb4LMQlf5RgdWPTTTDO7S4wtI,5663
 fbgemm_gpu/permute_pooled_embedding_modules.py,sha256=4mHJ2fo3SeG25iSwdm2YsM8q_oWsF1LxRguYmxSnuDI,2362
 fbgemm_gpu/permute_pooled_embedding_modules_split.py,sha256=cUrEbRIvLFW_3Zmh07QkN4S1Cfvvge6TYO1VXBFCpz8,2752
 fbgemm_gpu/quantize_comm.py,sha256=UZcVSC2JQ0oSkwsJQnjaZ2k8mm2p3hvVzpyg7X5xFXM,7885
 fbgemm_gpu/quantize_utils.py,sha256=-vwHIEkyStDo1TWoYfwmC5U6DvR6iRMHXyjFc9lO_p8,4143
 fbgemm_gpu/runtime_monitor.py,sha256=tIdxkJIWkJ8705btxs9NqzEXC7QprFh3sA8Q4LpvtJ8,6947
-fbgemm_gpu/sparse_ops.py,sha256=CuLIWJUMXnjqTVdpU38TsgGy7XcBv59e7nyr9cv2Yrc,20396
+fbgemm_gpu/sparse_ops.py,sha256=9BVsV5yXbbSrwTPrWHzr1S8MBX5AlUBoH5gc9efBhxA,20503
 fbgemm_gpu/split_embedding_configs.py,sha256=cJ5zuKHrN16-9ptEOIsDbWMhVnjUQha5zMnGRo06-aU,5774
 fbgemm_gpu/split_embedding_inference_converter.py,sha256=W61ps3tyNQYv__V3vNnAjEK9Q_LKNUqDB2cLtDNvEyE,7058
 fbgemm_gpu/split_embedding_optimizer_ops.py,sha256=qIf00N56cFF5AX0zSoB8k1v60HnDBoq8JniSDFhdPC0,540
 fbgemm_gpu/split_embedding_utils.py,sha256=LNJOeDmLCmcdvbSpVIa_q8kWVfV9-sdnRP-NNaMSawg,26849
 fbgemm_gpu/split_table_batched_embeddings_ops.py,sha256=_MIp6uHYHLn4GxGdrGsfddfSsZ2Z9mjsYIrih3ncI1I,2339
 fbgemm_gpu/split_table_batched_embeddings_ops_common.py,sha256=NEZmejyAkAWDAfNQupAyFQQ4QuqqiDq1l_I244wbZs4,3493
 fbgemm_gpu/split_table_batched_embeddings_ops_inference.py,sha256=bNSvTr17ThTer8ZSEusZXCmg-FxdqN14XQFUPb5dBZI,66517
@@ -20,15 +20,15 @@
 fbgemm_gpu/ssd_split_table_batched_embeddings_ops.py,sha256=S6qWfFzpqNIB8l9N3LAsYfaXSExg53f_b3fl47d1b1U,40680
 fbgemm_gpu/uvm.py,sha256=-cZunsuvnAKUEQptIwdYVar_3hUE99FbQUsyfBVeXPE,925
 fbgemm_gpu/docs/__init__.py,sha256=BbAfYbNZsBhO7L5Am4wyBLet4mTY2aXFucyGTxF9IlI,383
 fbgemm_gpu/docs/common.py,sha256=8ipXTwVb222X-aZ71O6n8fhxHCHPNhJEHMFiO7epcIs,273
 fbgemm_gpu/docs/examples.py,sha256=ZMN_6sL74LH_hrp2bF_hmg8gi29GhcgvwV3kCMjxkoE,2377
 fbgemm_gpu/docs/jagged_tensor_ops.py,sha256=Bsx-ZxvvdMv5CaldSvuw9GPR-HRcLbRR2IEXCOCm9r0,7381
 fbgemm_gpu/docs/table_batched_embedding_ops.py,sha256=h_EQOIMsdVlr-Pygul-fDGxx7JqLRjaBMI_z0PFrGAE,7708
-fbgemm_gpu/docs/version.py,sha256=eucgVR8_8VRNzLjD44LfrgkJ72NyQztNd1WBlMDg9-4,264
+fbgemm_gpu/docs/version.py,sha256=A5XP13gG_RN3BZv3j5tTxamJ-o5EkhppJF4nrdcL-xs,264
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/__init__.py,sha256=lfob_IDNeAs2FjS2WCldKlw0gm_qUZdp043fngI8sGE,1466
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adagrad.py,sha256=x17z36WrjIloP-pLVzyxpxjats7XjxJZv8OysT9JxD4,4180
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adagrad_pt2.py,sha256=x17z36WrjIloP-pLVzyxpxjats7XjxJZv8OysT9JxD4,4180
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adam.py,sha256=EBR6BEDV_SOuJM_yGq4IEfdL8umYkAmCWekcAwpHpNQ,3395
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_adam_pt2.py,sha256=EBR6BEDV_SOuJM_yGq4IEfdL8umYkAmCWekcAwpHpNQ,3395
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_args.py,sha256=ibfUa6H9BY85_e9VgbKujKi4nuR7Mgyw77VbFMkLKCs,2147
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_lamb.py,sha256=xhDnYR0vVDSK96nbcNSs5NbGXqFF3FGIs3DPDBJYt08,3395
@@ -45,11 +45,11 @@
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_pt2.py,sha256=Aljkdf4GB0zetL2j5YIhTZaOqiIMIlQ9iTDM421lbiM,4512
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_with_counter.py,sha256=Qr3xtASUsgNbPJD46__jyKkR3xy0n-n2IZSa5QPD-NA,3964
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_rowwise_adagrad_with_counter_pt2.py,sha256=Qr3xtASUsgNbPJD46__jyKkR3xy0n-n2IZSa5QPD-NA,3964
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_sgd.py,sha256=fOgbq-u3VtbtKFqLTGQJiCwoHpa_xP-rBIvj98S78F4,3762
 fbgemm_gpu/split_embedding_codegen_lookup_invokers/lookup_sgd_pt2.py,sha256=fOgbq-u3VtbtKFqLTGQJiCwoHpa_xP-rBIvj98S78F4,3762
 fbgemm_gpu/split_embedding_optimizer_codegen/optimizer_args.py,sha256=yiD3_bG5yT5VXLoGw4eeRKQ2Nj087DRq0qKCVPb52SY,649
 fbgemm_gpu/split_embedding_optimizer_codegen/split_embedding_optimizer_rowwise_adagrad.py,sha256=OFw5PM2YDiKvr6T9ZW7BKiq58gB7txcKfuJkBUROxdI,6162
-fbgemm_gpu_nightly_cpu-2024.4.15.dist-info/METADATA,sha256=FaTDZZZpFx2Ip6Zc3SUkAbq3kjeyCMnGkg8SBrYqsMw,2602
-fbgemm_gpu_nightly_cpu-2024.4.15.dist-info/WHEEL,sha256=AdAOsf8BL1uIBxiEcIdcPDjJWWb0G5USb4X4msVaesE,105
-fbgemm_gpu_nightly_cpu-2024.4.15.dist-info/top_level.txt,sha256=2tlbTWLkPjhqvLF_6BbqKzkcPluSE-oPRVjI8axK76I,11
-fbgemm_gpu_nightly_cpu-2024.4.15.dist-info/RECORD,,
+fbgemm_gpu_nightly_cpu-2024.4.16.dist-info/METADATA,sha256=6ayEXNzFw9wO0Vd2-gFtE6XQuxLsKpri6lHNQ4AQSOw,2602
+fbgemm_gpu_nightly_cpu-2024.4.16.dist-info/WHEEL,sha256=OEmkRrFcnutAqrz0YyBUaC3hh1288y58dKLCWma58N0,105
+fbgemm_gpu_nightly_cpu-2024.4.16.dist-info/top_level.txt,sha256=2tlbTWLkPjhqvLF_6BbqKzkcPluSE-oPRVjI8axK76I,11
+fbgemm_gpu_nightly_cpu-2024.4.16.dist-info/RECORD,,
```

