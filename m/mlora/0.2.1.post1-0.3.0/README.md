# Comparing `tmp/mlora-0.2.1.post1.tar.gz` & `tmp/mlora-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlora-0.2.1.post1.tar", last modified: Sun Apr  7 07:39:47 2024, max compression
+gzip compressed data, was "mlora-0.3.0.tar", last modified: Tue Apr 16 13:15:56 2024, max compression
```

## Comparing `mlora-0.2.1.post1.tar` & `mlora-0.3.0.tar`

### file list

```diff
@@ -1,37 +1,50 @@
-drwxr-xr-x   0 mikecovlee   (501) staff       (20)        0 2024-04-07 07:39:47.302902 mlora-0.2.1.post1/
--rw-r--r--   0 mikecovlee   (501) staff       (20)    11357 2024-01-06 04:20:01.000000 mlora-0.2.1.post1/LICENSE
--rw-r--r--   0 mikecovlee   (501) staff       (20)    10793 2024-04-07 07:39:47.302660 mlora-0.2.1.post1/PKG-INFO
--rw-r--r--   0 mikecovlee   (501) staff       (20)    10026 2024-04-07 05:32:43.000000 mlora-0.2.1.post1/README.md
-drwxr-xr-x   0 mikecovlee   (501) staff       (20)        0 2024-04-07 07:39:47.300875 mlora-0.2.1.post1/mlora/
--rw-r--r--   0 mikecovlee   (501) staff       (20)     1292 2024-04-07 07:38:52.000000 mlora-0.2.1.post1/mlora/__init__.py
--rw-r--r--   0 mikecovlee   (501) staff       (20)    22069 2024-04-06 16:30:59.000000 mlora-0.2.1.post1/mlora/attention.py
--rw-r--r--   0 mikecovlee   (501) staff       (20)     5068 2024-04-06 16:30:36.000000 mlora-0.2.1.post1/mlora/backends.py
--rw-r--r--   0 mikecovlee   (501) staff       (20)     4955 2024-04-05 15:46:05.000000 mlora-0.2.1.post1/mlora/checkpoint.py
--rw-r--r--   0 mikecovlee   (501) staff       (20)    13130 2024-04-03 07:55:06.000000 mlora-0.2.1.post1/mlora/dispatcher.py
--rw-r--r--   0 mikecovlee   (501) staff       (20)     3865 2024-04-06 16:30:59.000000 mlora-0.2.1.post1/mlora/feed_forward.py
--rw-r--r--   0 mikecovlee   (501) staff       (20)     7872 2024-04-03 07:55:06.000000 mlora-0.2.1.post1/mlora/generate.py
--rw-r--r--   0 mikecovlee   (501) staff       (20)    14342 2024-04-06 16:30:59.000000 mlora-0.2.1.post1/mlora/lora_linear.py
--rw-r--r--   0 mikecovlee   (501) staff       (20)    11045 2024-04-06 08:47:07.000000 mlora-0.2.1.post1/mlora/mix_lora.py
--rw-r--r--   0 mikecovlee   (501) staff       (20)     1277 2024-04-03 07:55:06.000000 mlora-0.2.1.post1/mlora/model.py
--rw-r--r--   0 mikecovlee   (501) staff       (20)    28382 2024-04-07 07:28:45.000000 mlora-0.2.1.post1/mlora/model_llama.py
--rw-r--r--   0 mikecovlee   (501) staff       (20)     9490 2024-04-03 16:46:28.000000 mlora-0.2.1.post1/mlora/modelargs.py
--rw-r--r--   0 mikecovlee   (501) staff       (20)     1764 2024-04-03 07:55:06.000000 mlora-0.2.1.post1/mlora/prompter.py
-drwxr-xr-x   0 mikecovlee   (501) staff       (20)        0 2024-04-07 07:39:47.302085 mlora-0.2.1.post1/mlora/tasks/
--rw-r--r--   0 mikecovlee   (501) staff       (20)      602 2024-04-07 07:38:50.000000 mlora-0.2.1.post1/mlora/tasks/__init__.py
--rw-r--r--   0 mikecovlee   (501) staff       (20)     6564 2024-04-03 07:55:06.000000 mlora-0.2.1.post1/mlora/tasks/common.py
--rw-r--r--   0 mikecovlee   (501) staff       (20)     9766 2024-04-06 09:10:39.000000 mlora-0.2.1.post1/mlora/tasks/evaluator.py
--rw-r--r--   0 mikecovlee   (501) staff       (20)     3544 2024-04-03 07:55:06.000000 mlora-0.2.1.post1/mlora/tasks/glue_tasks.py
--rw-r--r--   0 mikecovlee   (501) staff       (20)     5978 2024-04-03 07:55:06.000000 mlora-0.2.1.post1/mlora/tasks/qa_tasks.py
--rw-r--r--   0 mikecovlee   (501) staff       (20)     1516 2024-04-03 07:55:06.000000 mlora-0.2.1.post1/mlora/tokenizer.py
--rw-r--r--   0 mikecovlee   (501) staff       (20)     7885 2024-04-06 09:10:39.000000 mlora-0.2.1.post1/mlora/train.py
--rw-r--r--   0 mikecovlee   (501) staff       (20)     1864 2024-04-06 03:11:46.000000 mlora-0.2.1.post1/mlora/utils.py
-drwxr-xr-x   0 mikecovlee   (501) staff       (20)        0 2024-04-07 07:39:47.302400 mlora-0.2.1.post1/mlora.egg-info/
--rw-r--r--   0 mikecovlee   (501) staff       (20)    10793 2024-04-07 07:39:47.000000 mlora-0.2.1.post1/mlora.egg-info/PKG-INFO
--rw-r--r--   0 mikecovlee   (501) staff       (20)      612 2024-04-07 07:39:47.000000 mlora-0.2.1.post1/mlora.egg-info/SOURCES.txt
--rw-r--r--   0 mikecovlee   (501) staff       (20)        1 2024-04-07 07:39:47.000000 mlora-0.2.1.post1/mlora.egg-info/dependency_links.txt
--rw-r--r--   0 mikecovlee   (501) staff       (20)      106 2024-04-07 07:39:47.000000 mlora-0.2.1.post1/mlora.egg-info/requires.txt
--rw-r--r--   0 mikecovlee   (501) staff       (20)        6 2024-04-07 07:39:47.000000 mlora-0.2.1.post1/mlora.egg-info/top_level.txt
--rw-r--r--   0 mikecovlee   (501) staff       (20)      823 2024-04-07 07:39:27.000000 mlora-0.2.1.post1/pyproject.toml
--rw-r--r--   0 mikecovlee   (501) staff       (20)       38 2024-04-07 07:39:47.302943 mlora-0.2.1.post1/setup.cfg
-drwxr-xr-x   0 mikecovlee   (501) staff       (20)        0 2024-04-07 07:39:47.302212 mlora-0.2.1.post1/tests/
--rw-r--r--   0 mikecovlee   (501) staff       (20)      166 2024-04-03 07:54:48.000000 mlora-0.2.1.post1/tests/test_demo.py
+drwxr-xr-x   0 mikecovlee   (501) staff       (20)        0 2024-04-16 13:15:56.567340 mlora-0.3.0/
+-rw-r--r--   0 mikecovlee   (501) staff       (20)    11357 2024-01-06 04:20:01.000000 mlora-0.3.0/LICENSE
+-rw-r--r--   0 mikecovlee   (501) staff       (20)    11715 2024-04-16 13:15:56.567151 mlora-0.3.0/PKG-INFO
+-rw-r--r--   0 mikecovlee   (501) staff       (20)    10954 2024-04-10 06:30:53.000000 mlora-0.3.0/README.md
+drwxr-xr-x   0 mikecovlee   (501) staff       (20)        0 2024-04-16 13:15:56.560441 mlora-0.3.0/mlora/
+-rw-r--r--   0 mikecovlee   (501) staff       (20)     1195 2024-04-09 15:43:19.000000 mlora-0.3.0/mlora/__init__.py
+drwxr-xr-x   0 mikecovlee   (501) staff       (20)        0 2024-04-16 13:15:56.562734 mlora-0.3.0/mlora/backends/
+-rw-r--r--   0 mikecovlee   (501) staff       (20)      987 2024-04-09 13:04:56.000000 mlora-0.3.0/mlora/backends/__init__.py
+-rw-r--r--   0 mikecovlee   (501) staff       (20)     1324 2024-04-09 13:09:12.000000 mlora-0.3.0/mlora/backends/common.py
+-rw-r--r--   0 mikecovlee   (501) staff       (20)     1571 2024-04-09 13:03:52.000000 mlora-0.3.0/mlora/backends/cpu.py
+-rw-r--r--   0 mikecovlee   (501) staff       (20)     1343 2024-04-09 12:41:19.000000 mlora-0.3.0/mlora/backends/cuda.py
+-rw-r--r--   0 mikecovlee   (501) staff       (20)     2044 2024-04-09 12:41:19.000000 mlora-0.3.0/mlora/backends/mps.py
+drwxr-xr-x   0 mikecovlee   (501) staff       (20)        0 2024-04-16 13:15:56.564374 mlora-0.3.0/mlora/common/
+-rw-r--r--   0 mikecovlee   (501) staff       (20)     2171 2024-04-09 12:41:19.000000 mlora-0.3.0/mlora/common/__init__.py
+-rw-r--r--   0 mikecovlee   (501) staff       (20)     5197 2024-04-09 12:41:19.000000 mlora-0.3.0/mlora/common/attention.py
+-rw-r--r--   0 mikecovlee   (501) staff       (20)     5040 2024-04-09 12:44:14.000000 mlora-0.3.0/mlora/common/checkpoint.py
+-rw-r--r--   0 mikecovlee   (501) staff       (20)     2859 2024-04-16 13:15:44.000000 mlora-0.3.0/mlora/common/feed_forward.py
+-rw-r--r--   0 mikecovlee   (501) staff       (20)    14330 2024-04-09 12:41:19.000000 mlora-0.3.0/mlora/common/lora_linear.py
+-rw-r--r--   0 mikecovlee   (501) staff       (20)    11145 2024-04-16 13:15:44.000000 mlora-0.3.0/mlora/common/mix_lora.py
+-rw-r--r--   0 mikecovlee   (501) staff       (20)     2266 2024-04-09 12:41:19.000000 mlora-0.3.0/mlora/common/model.py
+-rw-r--r--   0 mikecovlee   (501) staff       (20)     9628 2024-04-16 13:15:44.000000 mlora-0.3.0/mlora/common/modelargs.py
+-rw-r--r--   0 mikecovlee   (501) staff       (20)    13118 2024-04-09 12:41:19.000000 mlora-0.3.0/mlora/dispatcher.py
+-rw-r--r--   0 mikecovlee   (501) staff       (20)     9770 2024-04-11 14:44:51.000000 mlora-0.3.0/mlora/evaluator.py
+-rw-r--r--   0 mikecovlee   (501) staff       (20)     7872 2024-04-11 14:44:51.000000 mlora-0.3.0/mlora/generator.py
+-rw-r--r--   0 mikecovlee   (501) staff       (20)    18206 2024-04-16 13:15:44.000000 mlora-0.3.0/mlora/model.py
+drwxr-xr-x   0 mikecovlee   (501) staff       (20)        0 2024-04-16 13:15:56.565658 mlora-0.3.0/mlora/models/
+-rw-r--r--   0 mikecovlee   (501) staff       (20)      872 2024-04-09 12:41:19.000000 mlora-0.3.0/mlora/models/__init__.py
+-rw-r--r--   0 mikecovlee   (501) staff       (20)     6308 2024-04-09 13:56:23.000000 mlora-0.3.0/mlora/models/modeling_gemma.py
+-rw-r--r--   0 mikecovlee   (501) staff       (20)    20566 2024-04-09 13:56:23.000000 mlora-0.3.0/mlora/models/modeling_llama.py
+-rw-r--r--   0 mikecovlee   (501) staff       (20)    12070 2024-04-09 13:56:23.000000 mlora-0.3.0/mlora/models/modeling_mistral.py
+-rw-r--r--   0 mikecovlee   (501) staff       (20)    22465 2024-04-09 13:56:23.000000 mlora-0.3.0/mlora/models/modeling_phi.py
+-rw-r--r--   0 mikecovlee   (501) staff       (20)     1764 2024-04-03 07:55:06.000000 mlora-0.3.0/mlora/prompter.py
+drwxr-xr-x   0 mikecovlee   (501) staff       (20)        0 2024-04-16 13:15:56.566451 mlora-0.3.0/mlora/tasks/
+-rw-r--r--   0 mikecovlee   (501) staff       (20)      528 2024-04-16 13:15:44.000000 mlora-0.3.0/mlora/tasks/__init__.py
+-rw-r--r--   0 mikecovlee   (501) staff       (20)     6439 2024-04-11 14:44:51.000000 mlora-0.3.0/mlora/tasks/common.py
+-rw-r--r--   0 mikecovlee   (501) staff       (20)     3182 2024-04-11 14:44:51.000000 mlora-0.3.0/mlora/tasks/glue_tasks.py
+-rw-r--r--   0 mikecovlee   (501) staff       (20)     5850 2024-04-11 14:44:51.000000 mlora-0.3.0/mlora/tasks/qa_tasks.py
+-rw-r--r--   0 mikecovlee   (501) staff       (20)     1370 2024-04-11 14:44:51.000000 mlora-0.3.0/mlora/tokenizer.py
+-rw-r--r--   0 mikecovlee   (501) staff       (20)     7862 2024-04-09 12:41:19.000000 mlora-0.3.0/mlora/trainer.py
+-rw-r--r--   0 mikecovlee   (501) staff       (20)     2125 2024-04-09 15:43:44.000000 mlora-0.3.0/mlora/utils.py
+drwxr-xr-x   0 mikecovlee   (501) staff       (20)        0 2024-04-16 13:15:56.566873 mlora-0.3.0/mlora.egg-info/
+-rw-r--r--   0 mikecovlee   (501) staff       (20)    11715 2024-04-16 13:15:56.000000 mlora-0.3.0/mlora.egg-info/PKG-INFO
+-rw-r--r--   0 mikecovlee   (501) staff       (20)      927 2024-04-16 13:15:56.000000 mlora-0.3.0/mlora.egg-info/SOURCES.txt
+-rw-r--r--   0 mikecovlee   (501) staff       (20)        1 2024-04-16 13:15:56.000000 mlora-0.3.0/mlora.egg-info/dependency_links.txt
+-rw-r--r--   0 mikecovlee   (501) staff       (20)      106 2024-04-16 13:15:56.000000 mlora-0.3.0/mlora.egg-info/requires.txt
+-rw-r--r--   0 mikecovlee   (501) staff       (20)        6 2024-04-16 13:15:56.000000 mlora-0.3.0/mlora.egg-info/top_level.txt
+-rw-r--r--   0 mikecovlee   (501) staff       (20)      817 2024-04-16 13:15:44.000000 mlora-0.3.0/pyproject.toml
+-rw-r--r--   0 mikecovlee   (501) staff       (20)       38 2024-04-16 13:15:56.567373 mlora-0.3.0/setup.cfg
+drwxr-xr-x   0 mikecovlee   (501) staff       (20)        0 2024-04-16 13:15:56.566621 mlora-0.3.0/tests/
+-rw-r--r--   0 mikecovlee   (501) staff       (20)      166 2024-04-03 07:54:48.000000 mlora-0.3.0/tests/test_demo.py
```

### Comparing `mlora-0.2.1.post1/LICENSE` & `mlora-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mlora-0.2.1.post1/PKG-INFO` & `mlora-0.3.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlora
-Version: 0.2.1.post1
+Version: 0.3.0
 Summary: A tool for fine-tuning large language models (LLMs) using the LoRA or QLoRA methods more efficiently.
 Project-URL: Homepage, https://github.com/scukdde-llm/mlora
 Project-URL: Bug Tracker, https://github.com/scukdde-llm/mlora/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
@@ -44,25 +44,31 @@
 ## Supported Platform
 
 | OS      | Backend | Model Precision        | Quantization  | xFormers | Flash Attention |
 |---------|---------|------------------------|---------------|----------|-----------------|
 | Linux   | CUDA    | FP32, FP16, TF32, BF16 | 8bit and 4bit | &check;  | &check;         |
 | Windows | CUDA    | FP32, FP16, TF32, BF16 | &cross;       | &cross;  | &cross;         |
 | macOS   | MPS     | FP32, FP16             | &cross;       | &cross;  | &cross;         |
+| All     | CPU     | FP32, FP16, BF16       | &cross;       | &cross;  | &cross;         |
+
+You can use the `MLORA_BACKEND_TYPE` environment variable to force m-LoRA to use a specific backend. For example, if you want m-LoRA to run only on CPU, you can set `MLORA_BACKEND_TYPE=CPU` before importing `mlora`.
 
 **Note**: Windows and macOS support are experimental feature.
 
 ## Supported Pre-trained Models
 
-|         | Model                                                    | # Parameters    |
-|---------|----------------------------------------------------------|-----------------|
-| &check; | [LLaMA](https://github.com/facebookresearch/llama)       | 7B/13B/33B/65B  |
-| &check; | [LLaMA-2](https://huggingface.co/meta-llama)             | 7B/13B/70B      |
-| &check; | [Qwen-2](https://qwenlm.github.io)                       | 4B/7B/14B/72B   |
-| &check; | [Mistral](https://mistral.ai)                            | 7B              |
+|         | Model                                                    | # Parameters       |
+|---------|----------------------------------------------------------|--------------------|
+| &check; | [LLaMA](https://github.com/facebookresearch/llama)       | 7B/13B/33B/65B     |
+| &check; | [LLaMA-2](https://huggingface.co/meta-llama)             | 7B/13B/70B         |
+| &check; | [Qwen-2](https://qwenlm.github.io)                       | 1.8B/4B/7B/14B/72B |
+| &check; | [Mistral](https://mistral.ai)                            | 7B                 |
+| &check; | [Gemma](https://ai.google.dev/gemma/docs)                | 2B/7B              |
+| &check; | [Phi-2](https://huggingface.co/microsoft/phi-2)          | 2.7B               |
+
 
 ## Supported LoRA Variants
 
 |         | LoRA Variants                                            | Arguments*                       |
 |---------|----------------------------------------------------------|----------------------------------|
 | &check; | [QLoRA](https://arxiv.org/abs/2402.12354)                | See *Quantize Methods*           |
 | &check; | [LoRA+](https://arxiv.org/abs/2402.12354)                | `loraplus_lr_ratio: 20.0`        |
@@ -123,47 +129,52 @@
 
 It's crucial to note that regardless of the settings, **LoRA weights are always calculated and stored at full precision**. For maintaining calculation accuracy, m-LoRA framework mandates the use of full precision for calculations when accuracy is imperative.
 
 For users with NVIDIA Ampere or newer GPU architectures, the `--tf32` option can be utilized to enable full-precision calculation acceleration.
 
 ## Known issues
 
- + DoRA with Quantization on Qwen2
- + Half Precision with Qwen2
+ + Applying quantization to Qwen2 in DoRA will result in an error
+ + Employing half precision models on MPS may occasionally result in challenges, such as encountering 'nan' values or experiencing convergence difficulties.
 
 ## Installation
 
 Please refer to [Install Guide](./docs/Install.md).
 
 ## Quickstart
 
-You can use m-LoRA via `launch.py` conveniently:
+You can conveniently utilize m-LoRA via `launch.py`. The following example demonstrates a streamlined approach to training a dummy model with m-LoRA.
 
 ```bash
 # Generating configuration
-python launch.py gen --template lora --tasks yahma/alpaca-cleaned
+python launch.py gen --template lora_phi --tasks ./data/dummy_data.json
 # Running the training task
-python launch.py run --base_model yahma/llama-7b-hf
+python launch.py run --base_model microsoft/phi-2
+# Try with gradio web ui
+python inference.py \
+  --base_model microsoft/phi-2 \
+  --template ./template/alpaca.json \
+  --lora_weights ./casual_0
 ```
 
-For further detailed usage information, please use the `help` command:
+For further detailed usage information, please refer to the `help` command:
 
 ```bash
 python launch.py help
 ```
 
 ## m-LoRA
 
 The `mlora.py` code is a starting point for finetuning on various datasets.
 Basic command for finetuning a baseline model on the [Alpaca Cleaned](https://github.com/gururise/AlpacaDataCleaned) dataset:
 ```bash
 python mlora.py \
-  --base_model yahma/llama-7b-hf \
+  --base_model meta-llama/Llama-2-7b-hf \
   --config ./config/alpaca.json \
-  --load_16bit
+  --bf16
 ```
 
 You can check the template finetune configuration in [template](./template/) folder.
 
 For further detailed usage information, please use `--help` option:
 ```bash
 python mlora.py --help
```

### Comparing `mlora-0.2.1.post1/README.md` & `mlora-0.3.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -23,25 +23,31 @@
 ## Supported Platform
 
 | OS      | Backend | Model Precision        | Quantization  | xFormers | Flash Attention |
 |---------|---------|------------------------|---------------|----------|-----------------|
 | Linux   | CUDA    | FP32, FP16, TF32, BF16 | 8bit and 4bit | &check;  | &check;         |
 | Windows | CUDA    | FP32, FP16, TF32, BF16 | &cross;       | &cross;  | &cross;         |
 | macOS   | MPS     | FP32, FP16             | &cross;       | &cross;  | &cross;         |
+| All     | CPU     | FP32, FP16, BF16       | &cross;       | &cross;  | &cross;         |
+
+You can use the `MLORA_BACKEND_TYPE` environment variable to force m-LoRA to use a specific backend. For example, if you want m-LoRA to run only on CPU, you can set `MLORA_BACKEND_TYPE=CPU` before importing `mlora`.
 
 **Note**: Windows and macOS support are experimental feature.
 
 ## Supported Pre-trained Models
 
-|         | Model                                                    | # Parameters    |
-|---------|----------------------------------------------------------|-----------------|
-| &check; | [LLaMA](https://github.com/facebookresearch/llama)       | 7B/13B/33B/65B  |
-| &check; | [LLaMA-2](https://huggingface.co/meta-llama)             | 7B/13B/70B      |
-| &check; | [Qwen-2](https://qwenlm.github.io)                       | 4B/7B/14B/72B   |
-| &check; | [Mistral](https://mistral.ai)                            | 7B              |
+|         | Model                                                    | # Parameters       |
+|---------|----------------------------------------------------------|--------------------|
+| &check; | [LLaMA](https://github.com/facebookresearch/llama)       | 7B/13B/33B/65B     |
+| &check; | [LLaMA-2](https://huggingface.co/meta-llama)             | 7B/13B/70B         |
+| &check; | [Qwen-2](https://qwenlm.github.io)                       | 1.8B/4B/7B/14B/72B |
+| &check; | [Mistral](https://mistral.ai)                            | 7B                 |
+| &check; | [Gemma](https://ai.google.dev/gemma/docs)                | 2B/7B              |
+| &check; | [Phi-2](https://huggingface.co/microsoft/phi-2)          | 2.7B               |
+
 
 ## Supported LoRA Variants
 
 |         | LoRA Variants                                            | Arguments*                       |
 |---------|----------------------------------------------------------|----------------------------------|
 | &check; | [QLoRA](https://arxiv.org/abs/2402.12354)                | See *Quantize Methods*           |
 | &check; | [LoRA+](https://arxiv.org/abs/2402.12354)                | `loraplus_lr_ratio: 20.0`        |
@@ -102,47 +108,52 @@
 
 It's crucial to note that regardless of the settings, **LoRA weights are always calculated and stored at full precision**. For maintaining calculation accuracy, m-LoRA framework mandates the use of full precision for calculations when accuracy is imperative.
 
 For users with NVIDIA Ampere or newer GPU architectures, the `--tf32` option can be utilized to enable full-precision calculation acceleration.
 
 ## Known issues
 
- + DoRA with Quantization on Qwen2
- + Half Precision with Qwen2
+ + Applying quantization to Qwen2 in DoRA will result in an error
+ + Employing half precision models on MPS may occasionally result in challenges, such as encountering 'nan' values or experiencing convergence difficulties.
 
 ## Installation
 
 Please refer to [Install Guide](./docs/Install.md).
 
 ## Quickstart
 
-You can use m-LoRA via `launch.py` conveniently:
+You can conveniently utilize m-LoRA via `launch.py`. The following example demonstrates a streamlined approach to training a dummy model with m-LoRA.
 
 ```bash
 # Generating configuration
-python launch.py gen --template lora --tasks yahma/alpaca-cleaned
+python launch.py gen --template lora_phi --tasks ./data/dummy_data.json
 # Running the training task
-python launch.py run --base_model yahma/llama-7b-hf
+python launch.py run --base_model microsoft/phi-2
+# Try with gradio web ui
+python inference.py \
+  --base_model microsoft/phi-2 \
+  --template ./template/alpaca.json \
+  --lora_weights ./casual_0
 ```
 
-For further detailed usage information, please use the `help` command:
+For further detailed usage information, please refer to the `help` command:
 
 ```bash
 python launch.py help
 ```
 
 ## m-LoRA
 
 The `mlora.py` code is a starting point for finetuning on various datasets.
 Basic command for finetuning a baseline model on the [Alpaca Cleaned](https://github.com/gururise/AlpacaDataCleaned) dataset:
 ```bash
 python mlora.py \
-  --base_model yahma/llama-7b-hf \
+  --base_model meta-llama/Llama-2-7b-hf \
   --config ./config/alpaca.json \
-  --load_16bit
+  --bf16
 ```
 
 You can check the template finetune configuration in [template](./template/) folder.
 
 For further detailed usage information, please use `--help` option:
 ```bash
 python mlora.py --help
```

### Comparing `mlora-0.2.1.post1/mlora/checkpoint.py` & `mlora-0.3.0/mlora/common/checkpoint.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,17 @@
 def check_backward_validity(inputs: Iterable[Any]) -> None:
     if not any(inp.requires_grad for inp in inputs if isinstance(inp, torch.Tensor)):
         raise RuntimeError("Input need grad")
 
 
 def get_device_states(*args) -> Tuple[List[int], List[torch.Tensor]]:
     fwd_gpu_devices = list({arg.device.index for arg in args
-                            if isinstance(arg, torch.Tensor) and arg.device.type == _backend.device_name()})
+                            if isinstance(arg, torch.Tensor)
+                            and arg.device.type != 'cpu'
+                            and arg.device.type == _backend.device_name()})
 
     fwd_gpu_states = []
     for device in fwd_gpu_devices:
         fwd_gpu_states.append(_backend.get_rng_state(device))
 
     return fwd_gpu_devices, fwd_gpu_states
```

### Comparing `mlora-0.2.1.post1/mlora/dispatcher.py` & `mlora-0.3.0/mlora/dispatcher.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,15 @@
-from mlora import Tokenizer
-from mlora import MultiLoraBatchData
-from mlora import LoraBatchDataConfig
-from mlora.modelargs import Tokens, Masks, DataClass
+from .tokenizer import Tokenizer
+from .common import (
+    Tokens,
+    Masks,
+    DataClass,
+    MultiLoraBatchData,
+    LoraBatchDataConfig,
+)
 
 import sys
 import math
 import random
 import logging
 import datasets
 from typing import Dict, List, Union, Callable
```

### Comparing `mlora-0.2.1.post1/mlora/generate.py` & `mlora-0.3.0/mlora/generator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
-from mlora.modelargs import LoraBatchDataConfig, MultiLoraBatchData
-from mlora.tokenizer import Tokenizer, Tokens
+from mlora.common import Tokens, LoraBatchDataConfig, MultiLoraBatchData
+from mlora.tokenizer import Tokenizer
 from mlora.prompter import Prompter
 from mlora.model import LLMModel
 
-from typing import List, Union, Tuple
 from dataclasses import dataclass
+from typing import List, Tuple, Union
 import logging
 import torch
 
 
 @dataclass
 class GenerateConfig:
     adapter_name: str = None
@@ -152,27 +152,27 @@
 
     device = torch.device(model.device_)
     raw_prompts: List[Tokens] = []
     batch_data_config: List[LoraBatchDataConfig] = []
     config_dict = {}
     for config in configs:
         config_dict[config.adapter_name] = config
-        tokens = [tokenizer.encode(prompt, True, False)
+        tokens = [tokenizer.encode(prompt)
                   for prompt in config.get_prompts()]
         config.batch_start_idx_ = len(raw_prompts)
         config.batch_end_idx_ = config.batch_start_idx_ + len(tokens)
         batch_data_config.append(LoraBatchDataConfig(
             config.adapter_name, config.batch_start_idx_, config.batch_end_idx_))
         raw_prompts.extend(tokens)
 
     batch_size = len(raw_prompts)
     min_tokens_len = min(len(t) for t in raw_prompts)
     max_tokens_len = max(len(t) for t in raw_prompts)
-    assert max_tokens_len <= model.max_seq_len_
-    total_len = min(model.max_seq_len_, max_gen_len + max_tokens_len)
+    assert max_tokens_len <= model.config_.max_seq_len_
+    total_len = min(model.config_.max_seq_len_, max_gen_len + max_tokens_len)
 
     tokens = torch.full((batch_size, total_len),
                         tokenizer.pad_id_, dtype=torch.int64, device=device)
     for k, t in enumerate(raw_prompts):
         tokens[k, : len(t)] = torch.tensor(t, dtype=torch.int64, device=device)
 
     prev_pos = 0
```

### Comparing `mlora-0.2.1.post1/mlora/lora_linear.py` & `mlora-0.3.0/mlora/common/lora_linear.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-from mlora.modelargs import MultiLoraBatchData
-from mlora.modelargs import LoraConfig
-from mlora.utils import _is_package_available
+from .modelargs import MultiLoraBatchData
+from .modelargs import LoraConfig
+from mlora.utils import is_package_available
 
 import math
 import torch
 import torch.nn as nn
 import torch.nn.functional as F
 
-if _is_package_available("bitsandbytes"):
+if is_package_available("bitsandbytes"):
     from bitsandbytes.nn import Linear8bitLt, Linear4bit
     import bitsandbytes as bnb
 else:
     from mlora.utils import Linear8bitLt, Linear4bit
 
 from typing import Dict, Tuple, List
```

### Comparing `mlora-0.2.1.post1/mlora/mix_lora.py` & `mlora-0.3.0/mlora/common/mix_lora.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from mlora.modelargs import MixConfig
+from .modelargs import LLMModelArgs, MixConfig
 
 import torch
 import torch.nn.functional as F
 
 from typing import List, Tuple
 from transformers.activations import ACT2FN
 
@@ -35,22 +35,22 @@
         self.topk = config.top_k_
 
     def forward(self, gate_logits) -> torch.Tensor:
         return self.aux_loss_coef * _mixtral_load_balancing_loss_func(gate_logits, self.experts, self.topk)
 
 
 class MixtralSparseMoe(torch.nn.Module):
-    def __init__(self, in_features: int, config: MixConfig) -> None:
+    def __init__(self, args: LLMModelArgs, config: MixConfig) -> None:
         super().__init__()
 
         self.adapter_name_: str = config.adapter_name
         self.dtype_: torch.dtype = torch.float32
         self.gate_ = torch.nn.Linear(
-            in_features, config.num_experts_, bias=False, device=config.device, dtype=self.dtype_)
-        self.act_ = ACT2FN[config.act_fn_]
+            args.dim_, config.num_experts_, bias=False, device=config.device, dtype=self.dtype_)
+        self.act_ = ACT2FN[args.hidden_act_ if config.act_fn_ is None else config.act_fn_]
         self.experts_ = config.num_experts_
         self.topk_ = config.top_k_
         self.router_profile_: bool = False
         self.profiler_: List[int] = None
 
     def _profiling(self,
                    batch_size: int,
@@ -183,22 +183,22 @@
         router_probs = F.softmax(router_logits, dim=-1)
         aux_loss = _switch_load_balancing_loss_func(
             router_probs, expert_indexes)
         return self.z_loss_coef * z_loss + self.aux_loss_coef * aux_loss
 
 
 class SwitchSparseMoe(torch.nn.Module):
-    def __init__(self, in_features: int, config: MixConfig) -> None:
+    def __init__(self, args: LLMModelArgs, config: MixConfig) -> None:
         super().__init__()
 
         self.adapter_name_: str = config.adapter_name
         self.dtype_: torch.dtype = torch.float32
         self.gate_ = torch.nn.Linear(
-            in_features, config.num_experts_, bias=False, device=config.device, dtype=self.dtype_)
-        self.act_ = ACT2FN[config.act_fn_]
+            args.dim_, config.num_experts_, bias=False, device=config.device, dtype=self.dtype_)
+        self.act_ = ACT2FN[args.hidden_act_ if config.act_fn_ is None else config.act_fn_]
         self.experts_: int = config.num_experts_
         self.dropout_ = torch.nn.Dropout(
             config.ffn_dropout_) if config.ffn_dropout_ > 0 else torch.nn.Identity()
         self.expert_capacity_: int = config.expert_capacity_
         self.jitter_noise_: float = config.jitter_noise_
 
     def route(self, hidden_states: torch.Tensor) -> Tuple:
@@ -259,12 +259,12 @@
 
 moe_layer_dict = {
     "mixtral": MixtralSparseMoe,
     "switch": SwitchSparseMoe
 }
 
 
-def moe_layer_factory(in_features: int, config: MixConfig) -> torch.nn.Module:
+def moe_layer_factory(args: LLMModelArgs, config: MixConfig) -> torch.nn.Module:
     if config.routing_strategy_ not in router_loss_dict:
         raise ValueError(
             f"Unknown routing strategy {config.routing_strategy_}")
-    return moe_layer_dict[config.routing_strategy_](in_features, config)
+    return moe_layer_dict[config.routing_strategy_](args, config)
```

### Comparing `mlora-0.2.1.post1/mlora/model_llama.py` & `mlora-0.3.0/mlora/model.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,100 +1,40 @@
-from mlora.modelargs import LLMModelArgs, LLMModelOutput, MultiLoraBatchData
-from mlora.modelargs import Masks, LoraConfig, MixConfig, lora_config_factory
-from mlora.attention import LlamaAttention, llama_attention_factory
-from mlora.checkpoint import CheckpointRecomputeFunction
-from mlora.model import LLMOutput, LLMModel
-from mlora.feed_forward import FeedForward
-from mlora.lora_linear import Linear
-from mlora.generate import GenerateConfig
-from mlora.mix_lora import router_loss_factory
+from mlora.common import (
+    LLMOutput,
+    LLMDecoder,
+    LLMForCausalLM,
+    LLMModelArgs,
+    LLMModelOutput,
+    MultiLoraBatchData,
+    LoraConfig,
+    MixConfig,
+    router_loss_factory,
+    lora_config_factory,
+)
 from mlora.tasks import SequenceClassificationTask, task_dict
+from mlora.utils import is_package_available
+from mlora.models import from_pretrained
 from mlora.backends import get_backend
-from mlora.utils import _is_package_available
 
-import torch
-import torch.nn.functional as F
-import torch.utils.checkpoint
-from typing import List, Dict, Tuple, Optional
 from huggingface_hub import snapshot_download
 from transformers import AutoModelForCausalLM
-from collections import OrderedDict
+from typing import Tuple, List, Dict, Optional
+
 import logging
+import torch
 import json
 import math
 import os
 
-if _is_package_available("bitsandbytes"):
+if is_package_available("bitsandbytes"):
     from transformers import BitsAndBytesConfig
 else:
     from mlora.utils import BitsAndBytesConfig
 
 
-# input_tokens shape is: batch_size * seq_len
-#   default: upper triangular matrix like below, i.e. diagonal = 1
-#            0 -inf -inf
-#            0    0 -inf
-#            0    0    0
-# additional_mask: batch_size * seq_len
-#   default: is None the matrix like default, if set true, the mask metric will be -inf
-#   example: [[True, False, False]]
-#           -inf -inf -inf
-#           -inf    0 -inf
-#           -inf    0    0
-def precompute_mask(input_tokens: torch.Tensor,
-                    n_heads: int,
-                    device: str,
-                    additional_mask: List[Masks] = None,
-                    diagonal: int = 1,
-                    dtype: torch.dtype = torch.float32) -> torch.Tensor:
-    batch_size, seq_len = input_tokens.shape
-
-    TORCH_MIN_VALUE = torch.finfo(torch.float32).min
-    mask = torch.full((batch_size, n_heads, seq_len, seq_len),
-                      TORCH_MIN_VALUE, device=device, dtype=torch.float32)
-    mask = torch.triu(mask, diagonal=diagonal)
-
-    if additional_mask is not None:
-        masks_metric = ~torch.tensor(
-            additional_mask, dtype=torch.bool, device=device)
-        masks_metric = masks_metric.view(batch_size, 1, 1, seq_len)
-        masks_metric = masks_metric.expand(-1, n_heads, seq_len, -1)
-        mask = torch.masked_fill(mask, masks_metric, TORCH_MIN_VALUE)
-
-    mask.requires_grad_(False)
-
-    return mask.to(device=device, dtype=dtype)
-
-
-class LlamaRMSNorm(torch.nn.Module):
-    def __init__(self, weight: torch.Tensor, eps: float = 1e-6):
-        super().__init__()
-        self.norm_eps_ = eps
-        self.weight_ = weight
-
-    def forward(self, data: torch.Tensor) -> torch.Tensor:
-        input_dtype = data.dtype
-        v = data.to(torch.float32).pow(2).mean(-1, keepdim=True)
-        data = data * torch.rsqrt(v + self.norm_eps_)
-
-        return (self.weight_ * data).to(input_dtype)
-
-
-class LlamaEmbedding(torch.nn.Module):
-    def __init__(self, embedding: torch.Tensor, pad_token: int):
-        super().__init__()
-        self.token_embedding_: torch.Tensor = embedding
-        self.padding_idx_: int = pad_token
-
-    def forward(self, tokens: torch.Tensor) -> torch.Tensor:
-        data = F.embedding(tokens, self.token_embedding_,
-                           padding_idx=self.padding_idx_)
-        return data
-
-
 class CasualOutputLayer(LLMOutput):
     def __init__(self, vocab_size: int, weight: torch.nn.Linear):
         super().__init__()
         self.vocab_size_: int = vocab_size
         self.lm_head_: torch.nn.Linear = weight
 
     def forward(self, data: torch.Tensor) -> torch.Tensor:
@@ -157,15 +97,15 @@
         elif self.task_type_ == "multi_label_classification":
             loss_fn = torch.nn.BCEWithLogitsLoss()
             return loss_fn(pooled_logits, labels)
         else:
             raise ValueError(f"unknown task type {self.task_type_}")
 
 
-class LlamaOutputLayer(torch.nn.Module):
+class OutputLayer(torch.nn.Module):
     def __init__(self):
         super().__init__()
         self.layers_: torch.ModuleDict = {}
 
     def forward(self, data: torch.Tensor,
                 input_args: MultiLoraBatchData) -> List[LLMModelOutput]:
         outputs = []
@@ -180,196 +120,128 @@
                                           logits=layer.forward(
                                               data[start_idx:end_idx]),
                                           loss_fn_=layer.loss))
 
         return outputs
 
 
-class LlamaDecoderLayer(torch.nn.Module):
-    def __init__(self, layer_idx: int, args: LLMModelArgs):
-        super().__init__()
-        # attention
-        self.attn_norm_: LlamaRMSNorm = None  # dim
-        self.attn_: LlamaAttention = None
-        # feed forward
-        self.ffn_norm_: LlamaRMSNorm = None  # dim
-        self.ffn_: FeedForward = None
-        # other arg
-        self.layer_id_ = layer_idx
-        self.dim_ = args.dim_
-        self.norm_eps_ = args.norm_eps_
-        self.dtype_ = args.dtype_
-
-    def init_lora_layer_weight(self, config: LoraConfig, weight: Optional[Dict[str, torch.Tensor]]):
-        target = config.target_modules_
-        linear_layer_list = [self.attn_.wk_, self.attn_.wq_, self.attn_.wv_,
-                             self.attn_.wo_, self.ffn_.w1_, self.ffn_.w2_, self.ffn_.w3_]
-        linear_layer_name_list = [
-            "k_proj", "q_proj", "v_proj", "o_proj", "w1_proj", "w2_proj", "w3_proj"]
-
-        if isinstance(config, MixConfig):
-            # Inject LoRA configs into FFN layer
-            gate_layer_name = f"mixlora.layers.{self.layer_id_}.gate.weight"
-            self.ffn_.init_moe_weight(in_features=self.dim_, config=config,
-                                      gate=weight if weight is None else weight[gate_layer_name])
-
-            moe_layer_name_list = ["w1_proj", "w2_proj", "w3_proj"]
-            init_moe = True
-        else:
-            moe_layer_name_list = []
-            init_moe = False
-
-        for idx, layer_name in enumerate(linear_layer_name_list):
-            if layer_name in target and target[layer_name]:
-                if init_moe and layer_name in moe_layer_name_list:
-                    for expert_idx in range(config.num_experts_):
-                        lora_a = None
-                        lora_b = None
-                        if weight is not None:
-                            lora_a_name = f"mixlora.layers.{self.layer_id_}.experts.{expert_idx}.{layer_name}.lora_A.weight"
-                            lora_b_name = f"mixlora.layers.{self.layer_id_}.experts.{expert_idx}.{layer_name}.lora_B.weight"
-                            if lora_a_name not in weight:
-                                raise f"can not found the layer {lora_a_name} in model"
-                            if lora_b_name not in weight:
-                                raise f"can not found the layer {lora_b_name} in model"
-                            lora_a = weight[lora_a_name]
-                            lora_b = weight[lora_b_name]
-
-                        linear_layer_list[idx].init_lora_weight(
-                            config.expert_config(expert_idx), (lora_a, lora_b))
-                else:
+def init_lora_layer_weight(
+        layer: LLMDecoder, args: LLMModelArgs, config: LoraConfig, weight: Optional[Dict[str, torch.Tensor]]):
+    target = config.target_modules_
+    linear_layer_list = []
+    linear_layer_name_list = []
+    for name, module in layer.state_dict().items():
+        linear_layer_list.append(module)
+        linear_layer_name_list.append(name)
+
+    if isinstance(config, MixConfig):
+        # Inject LoRA configs into FFN layer
+        gate_layer_name = f"mixlora.layers.{layer.layer_id_}.gate.weight"
+        layer.mlp_.init_moe_weight(args=args, config=config,
+                                   gate=None if weight is None else weight[gate_layer_name])
+
+        moe_layer_name_list = list(layer.mlp_.state_dict().keys())
+        init_moe = True
+    else:
+        moe_layer_name_list = []
+        init_moe = False
+
+    for idx, layer_name in enumerate(linear_layer_name_list):
+        if layer_name in target and target[layer_name]:
+            if init_moe and layer_name in moe_layer_name_list:
+                for expert_idx in range(config.num_experts_):
                     lora_a = None
                     lora_b = None
                     if weight is not None:
-                        name_prefix = "mixlora.layers" if init_moe else "base_model.model.model.layers"
-                        lora_a_name = f"{name_prefix}.{self.layer_id_}.self_attn.{layer_name}.lora_A.weight"
-                        lora_b_name = f"{name_prefix}.{self.layer_id_}.self_attn.{layer_name}.lora_B.weight"
-
+                        lora_a_name = f"mixlora.layers.{layer.layer_id_}.experts.{expert_idx}.{layer_name}.lora_A.weight"
+                        lora_b_name = f"mixlora.layers.{layer.layer_id_}.experts.{expert_idx}.{layer_name}.lora_B.weight"
                         if lora_a_name not in weight:
                             raise f"can not found the layer {lora_a_name} in model"
                         if lora_b_name not in weight:
                             raise f"can not found the layer {lora_b_name} in model"
                         lora_a = weight[lora_a_name]
                         lora_b = weight[lora_b_name]
 
                     linear_layer_list[idx].init_lora_weight(
-                        config, (lora_a, lora_b))
-
-    def forward(self,
-                hidden_states: torch.Tensor,
-                input_args: MultiLoraBatchData,
-                attention_mask: Optional[torch.Tensor] = None,
-                router_logits: Optional[List[List]] = None):
-        # Self Attention
-        residual = hidden_states
-        hidden_states = self.attn_norm_(hidden_states)
-        hidden_states = self.attn_(hidden_states, input_args, attention_mask)
-        hidden_states = residual + hidden_states
-        # Fully Connected
-        residual = hidden_states
-        hidden_states = self.ffn_norm_(hidden_states)
-        hidden_states = self.ffn_(hidden_states, input_args, router_logits)
-        hidden_states = residual + hidden_states
+                        config.expert_config(expert_idx), (lora_a, lora_b))
+            else:
+                lora_a = None
+                lora_b = None
+                if weight is not None:
+                    name_prefix = "mixlora.layers" if init_moe else "base_model.model.model.layers"
+                    lora_a_name = f"{name_prefix}.{layer.layer_id_}.self_attn.{layer_name}.lora_A.weight"
+                    lora_b_name = f"{name_prefix}.{layer.layer_id_}.self_attn.{layer_name}.lora_B.weight"
+
+                    if lora_a_name not in weight:
+                        raise f"can not found the layer {lora_a_name} in model"
+                    if lora_b_name not in weight:
+                        raise f"can not found the layer {lora_b_name} in model"
+                    lora_a = weight[lora_a_name]
+                    lora_b = weight[lora_b_name]
 
-        return hidden_states
+                linear_layer_list[idx].init_lora_weight(
+                    config, (lora_a, lora_b))
 
 
-class LlamaSequentialWrapper(torch.nn.Module):
+class LLMSequentialWrapper(torch.nn.Module):
     def __init__(self, module: torch.nn.Module):
         super().__init__()
         self.wrapper_module_ = module
 
     def name(self) -> str:
         return type(self.wrapper_module_).__name__
 
     def forward(self, input: Tuple) -> Tuple:
-        module_name = self.name()
-
-        if module_name == "LlamaEmbedding":
-            output = self.wrapper_module_.forward(input[0])
-            if input[-1]:
-                output = output.requires_grad_(True)
-            return (output, ) + input[1:]
-        elif module_name == "LlamaRMSNorm":
-            output = self.wrapper_module_.forward(input[0])
-            return (output, ) + input[1:]
-        elif module_name == "LlamaOutputLayer":
-            output = self.wrapper_module_.forward(*input[:2])
-            return (output, ) + input[1:]
-        elif module_name == "LlamaDecoderLayer":
-            if input[-1]:
-                output = CheckpointRecomputeFunction.apply(
-                    self.wrapper_module_.forward, *input[:-1])
-            else:
-                output = self.wrapper_module_.forward(*input[:-1])
-            return (output, ) + input[1:]
-        else:
-            raise f"module invalid: {module_name}"
+        output = self.wrapper_module_.forward(*input[:2])
+        return (output, ) + input[1:]
 
 
-LlamaCompatibleModelTypes = ["mistral", "qwen2"]
-
-
-class LlamaModel(LLMModel):
-    def __init__(self, args: LLMModelArgs):
-        self.name_or_path_ = args.name_or_path_
-        # weight
-        self.token_embedding_: LlamaEmbedding = None
-
-        self.layers_: List[LlamaDecoderLayer] = []
-        for layer_id in range(args.n_layers_):
-            self.layers_.append(LlamaDecoderLayer(layer_id, args))
-
-        self.norm_: LlamaRMSNorm = None
-        self.lm_head_ = torch.nn.Linear(
-            args.dim_, args.vocab_size_, bias=False, device=args.device_, dtype=args.dtype_)
-        self.output_: LlamaOutputLayer = LlamaOutputLayer()
-        self.seq_module_: torch.nn.Sequential = None
-
+class LLMModel(torch.nn.Module):
+    def __init__(self, model: LLMForCausalLM):
+        super().__init__()
+        args: LLMModelArgs = model.config_
         if args.vocab_size_ >= torch.finfo(args.dtype_).max:
             logging.warn(
                 f"vocab_size >= max({args.dtype_}), consider load model with higher precision.")
-
+        self.model_ = model
+        self.config_ = args
         # configs
-        self.attn_implementation_ = args.attn_implementation_
-        self.norm_eps_ = args.norm_eps_
-        self.device_ = args.device_
-        self.n_heads_ = args.n_heads_
-        self.n_kv_heads_ = args.n_kv_heads_
+        self.name_or_path_ = args.name_or_path_
         self.vocab_size_ = args.vocab_size_
-        self.pad_token_id_ = args.pad_token_id_
-        self.max_seq_len_ = args.max_seq_len_
-        self.dim_ = args.dim_
+        self.device_ = args.device_
         self.dtype_ = args.dtype_
 
+        self.output_ = OutputLayer()
+        seq_module = model.sequential_module()
+        seq_module.update({"output": LLMSequentialWrapper(self.output_)})
+        seq_module.move_to_end("output")
+        self.seq_module_ = torch.nn.Sequential(seq_module)
         # adapter configs
         self.adapter_configs_: Dict[str, LoraConfig] = {}
 
     # train model or inference model: output is probs
     def forward(self, input: MultiLoraBatchData,
                 labels: List[List[int]] = None) -> List[LLMModelOutput]:
         tokens = torch.tensor(input.batch_tokens_,
                               dtype=torch.int64, device=self.device_)
 
         # prepare mask
-        if self.attn_implementation_ == "flash_attn":
+        if self.config_.attn_implementation_ == "flash_attn":
             if input.attention_masks_ is not None and 0 in input.attention_masks_:
                 # 2d mask is passed through the layers
                 mask = torch.tensor(input.attention_masks_,
                                     dtype=torch.int64, device=self.device_)
             else:
                 mask = None
         else:
-            mask = precompute_mask(
+            mask = self.model_.causal_mask(
                 input_tokens=tokens,
-                n_heads=1 if input.inference_mode_ else self.n_heads_,
-                device=self.device_,
                 additional_mask=input.attention_masks_,
-                diagonal=input.inference_seq_pos_ + 1 if input.inference_mode_ else 1,
-                dtype=self.dtype_)
+                multi_head=(self.config_.attn_implementation_ == "xformers"),
+                diagonal=input.inference_seq_pos_ + 1 if input.inference_mode_ else 1)
 
         # routing data
         router_logits: List[List] = list(
             [] for _ in range(len(input.lora_batch_data_config_)))
 
         if input.inference_mode_:
             input.gradient_checkpoint_ = False
@@ -406,40 +278,40 @@
 
     def init_lora_layer_weight(self, config: LoraConfig, weight: Optional[Dict[str, torch.Tensor]]):
         self.adapter_configs_[config.adapter_name] = config
         # init output layer
         if config.task_name in task_dict and isinstance(task_dict[config.task_name], SequenceClassificationTask):
             output_layer = ClassificationOutputLayer(
                 **task_dict[config.task_name].init_kwargs(),
-                hidden_size=self.dim_,
-                pad_token_id=self.pad_token_id_,
+                hidden_size=self.config_.dim_,
+                pad_token_id=self.config_.pad_token_id_,
                 device=self.device_,
                 weight=weight)
         else:
             output_layer = CasualOutputLayer(
-                vocab_size=self.vocab_size_,
-                weight=self.lm_head_)
+                vocab_size=self.config_.vocab_size_,
+                weight=self.model_.lm_head_)
 
         self.output_.layers_[config.adapter_name] = output_layer
         if config.adapter_name == "default" and weight is None:
             return
         # init transformer layers
-        for transformer_layer in self.layers_:
-            transformer_layer.init_lora_layer_weight(config, weight)
+        for transformer_layer in self.model_.layers_:
+            init_lora_layer_weight(
+                transformer_layer, self.config_, config, weight)
 
     def from_pretrained(path: str,
                         device: str,
                         bits: int = None,
                         attn_impl: str = "eager",
                         use_sliding_window: bool = False,
                         load_dtype: torch.dtype = torch.bfloat16,
                         compute_dtype: torch.dtype = torch.bfloat16,
                         double_quant: bool = True,
-                        quant_type: str = 'nf4',
-                        ) -> LLMModel:
+                        quant_type: str = 'nf4'):
         # load_dtype will change the precision of LLaMA pre-trained model
         # when loading with quantization (bits = 8 or bits = 4), load_dtype will only influence the actual computing precision
         if load_dtype not in [torch.bfloat16, torch.float16, torch.float32]:
             raise ValueError(f"unsupported load dtype {load_dtype}")
 
         if compute_dtype not in [torch.bfloat16, torch.float16, torch.float32]:
             raise ValueError(f"unsupported compute dtype {compute_dtype}")
@@ -455,141 +327,67 @@
 
             if bits in [4, 8] and compute_dtype == torch.bfloat16:
                 logging.warning("bf16 is not available. deprecated to fp16.")
                 compute_dtype = torch.float16
 
         if bits in [4, 8]:
             logging.info(f"Loading model with quantization, bits = {bits}.")
-            llama_model = AutoModelForCausalLM.from_pretrained(
+            llm_model = AutoModelForCausalLM.from_pretrained(
                 path,
                 device_map=device,
                 quantization_config=BitsAndBytesConfig(
                     load_in_4bit=bits == 4,
                     load_in_8bit=bits == 8,
                     llm_int8_threshold=6.0,
                     llm_int8_has_fp16_weight=False,
                     bnb_4bit_compute_dtype=compute_dtype,
                     bnb_4bit_use_double_quant=double_quant,
                     bnb_4bit_quant_type=quant_type,
                 ),
                 torch_dtype=load_dtype)
         else:
-            llama_model = AutoModelForCausalLM.from_pretrained(
+            llm_model = AutoModelForCausalLM.from_pretrained(
                 path,
                 device_map=device,
                 torch_dtype=load_dtype)
 
-        if llama_model.config.model_type != "llama":
-            if llama_model.config.model_type in LlamaCompatibleModelTypes:
-                logging.info(
-                    f"Loading {llama_model.config.model_type} model with llama compatible mode.")
-            else:
-                logging.warning(
-                    f"Unsupported model type {llama_model.config.model_type}, loading with llama compatible mode.")
+        llm_model.requires_grad_(False)
 
-        llama_model.requires_grad_(False)
+        model = from_pretrained(llm_model, attn_impl=attn_impl,
+                                use_sliding_window=use_sliding_window, device=device)
 
-        llama_args = LLMModelArgs()
-        llama_args.attn_implementation_ = attn_impl
         logging.info(f"Use {attn_impl} as attention implementation.")
-        llama_args.name_or_path_ = llama_model.config.name_or_path
-        llama_args.dim_ = llama_model.config.hidden_size
-        llama_args.n_heads_ = llama_model.config.num_attention_heads
-        llama_args.n_kv_heads_ = llama_args.n_heads_ if not hasattr(
-            llama_model.config, "num_key_value_heads") else llama_model.config.num_key_value_heads
-        llama_args.n_layers_ = llama_model.config.num_hidden_layers
-        llama_args.norm_eps_ = llama_model.config.rms_norm_eps
-        llama_args.vocab_size_ = llama_model.config.vocab_size
-        llama_args.max_seq_len_ = 4096 if not use_sliding_window and not hasattr(
-            llama_model.config, "max_position_embeddings") else llama_model.config.max_position_embeddings
-        if hasattr(llama_model.config, "use_sliding_window"):
-            llama_args.use_sliding_window_ = use_sliding_window or llama_model.config.use_sliding_window
-        else:
-            llama_args.use_sliding_window_ = use_sliding_window
-        if hasattr(llama_model.config, "max_window_layers"):
-            llama_args.max_window_layers_ = llama_model.config.max_window_layers
-        if hasattr(llama_model.config, "sliding_window"):
-            llama_args.sliding_window_ = llama_model.config.sliding_window
-        llama_args.pad_token_id_ = llama_model.config.pad_token_id
-        llama_args.rope_theta_ = llama_model.config.rope_theta
-        if llama_args.pad_token_id_ is None:
-            llama_args.pad_token_id_ = -1
-        llama_args.dtype_ = llama_model.dtype
-
-        llama_args.device_ = device
-
-        model = LlamaModel(llama_args)
-
-        model.token_embedding_ = LlamaEmbedding(
-            llama_model.model.embed_tokens.weight, llama_args.pad_token_id_)
-
-        model.norm_ = LlamaRMSNorm(
-            llama_model.model.norm.weight, model.norm_eps_)
-
-        with torch.no_grad():
-            model.lm_head_.weight.copy_(llama_model.lm_head.weight)
-
-        for idx, layer in enumerate(llama_model.model.layers):
-            model.layers_[idx].attn_norm_ = LlamaRMSNorm(
-                layer.input_layernorm.weight, model.norm_eps_)
-            model.layers_[idx].attn_ = llama_attention_factory(
-                model_type=llama_model.config.model_type,
-                wq=Linear(layer.self_attn.q_proj, device=device),
-                wk=Linear(layer.self_attn.k_proj, device=device),
-                wv=Linear(layer.self_attn.v_proj, device=device),
-                wo=Linear(layer.self_attn.o_proj, device=device),
-                args=llama_args,
-                layer_idx=idx
-            )
-            model.layers_[idx].ffn_norm_ = LlamaRMSNorm(
-                layer.post_attention_layernorm.weight, model.norm_eps_)
-            model.layers_[idx].ffn_ = FeedForward(
-                w1=Linear(layer.mlp.gate_proj, device=device),
-                w2=Linear(layer.mlp.down_proj, device=device),
-                w3=Linear(layer.mlp.up_proj, device=device),
-                args=llama_args
-            )
-
-        # convert to sequential module for use
-        model.seq_module_ = model.sequential_module()
-
-        return model
-
-    def get_generate_paramas(self) -> Dict[str, GenerateConfig]:
-        generate_paramas = {}
-        for adapter_name in self.adapter_configs_.keys():
-            generate_paramas[adapter_name] = GenerateConfig(
-                adapter_name=adapter_name)
-        return generate_paramas
+
+        return LLMModel(model)
 
     def get_lora_weight_dict(self, lora_name: str) -> Dict[str, torch.Tensor]:
         # return the lora weight and target_module's name
         lora_weight_dict = self.output_.layers_[lora_name].state_dict()
-        for idx, transformer_layer in enumerate(self.layers_):
+        for idx, transformer_layer in enumerate(self.model_.layers_):
             if isinstance(self.adapter_configs_[lora_name], MixConfig):
                 layer_prefix_name = f"mixlora.layers.{idx}.self_attn."
             else:
                 layer_prefix_name = f"base_model.model.model.layers.{idx}.self_attn."
 
-            lora_layer_list = [transformer_layer.attn_.wq_, transformer_layer.attn_.wk_,
-                               transformer_layer.attn_.wv_, transformer_layer.attn_.wo_,
-                               transformer_layer.ffn_.w1_, transformer_layer.ffn_.w2_,
-                               transformer_layer.ffn_.w3_]
-            lora_layer_name_list = [
-                "q_proj", "k_proj", "v_proj", "o_proj", "w1_proj", "w2_proj", "w3_proj"]
+            lora_layer_list = []
+            lora_layer_name_list = []
+            for name, layer in transformer_layer.state_dict().items():
+                lora_layer_list.append(layer)
+                lora_layer_name_list.append(name)
+
             for idx, lora_layer in enumerate(lora_layer_list):
                 if lora_name in lora_layer.loras_:
                     prefix_name = layer_prefix_name + lora_layer_name_list[idx]
                     lora_weight_dict[f"{prefix_name}.lora_A.weight"] = lora_layer.loras_[
                         lora_name].lora_a_.weight
                     lora_weight_dict[f"{prefix_name}.lora_B.weight"] = lora_layer.loras_[
                         lora_name].lora_b_.weight
-                elif lora_name in transformer_layer.ffn_.moes_:
+                elif lora_name in transformer_layer.mlp_.moes_:
                     moe_layer_prefix_name = f"mixlora.layers.{transformer_layer.layer_id_}."
-                    for expert_idx in range(transformer_layer.ffn_.moes_[lora_name].experts_):
+                    for expert_idx in range(transformer_layer.mlp_.moes_[lora_name].experts_):
                         moe_lora_name = f"moe.{lora_name}.experts.{expert_idx}"
                         if moe_lora_name in lora_layer.loras_:
                             lora_weight_dict[
                                 moe_layer_prefix_name
                                 + f"experts.{expert_idx}."
                                 + f"{lora_layer_name_list[idx]}.lora_A.weight"
                             ] = lora_layer.loras_[moe_lora_name].lora_a_.weight
@@ -597,38 +395,18 @@
                                 moe_layer_prefix_name
                                 + f"experts.{expert_idx}."
                                 + f"{lora_layer_name_list[idx]}.lora_B.weight"
                             ] = lora_layer.loras_[moe_lora_name].lora_b_.weight
 
                     lora_weight_dict[
                         moe_layer_prefix_name + "gate.weight"
-                    ] = transformer_layer.ffn_.moes_[lora_name].gate_.weight
+                    ] = transformer_layer.mlp_.moes_[lora_name].gate_.weight
 
         return lora_weight_dict
 
-    def sequential_module(self) -> torch.nn.Sequential:
-        seq_module = OrderedDict()
-
-        seq_module.update(
-            {"embedding": LlamaSequentialWrapper(self.token_embedding_)})
-        seq_module.move_to_end("embedding")
-
-        for index, layer in enumerate(self.layers_):
-            layer_name = f"layer{index}"
-            seq_module.update({layer_name: LlamaSequentialWrapper(layer)})
-            seq_module.move_to_end(layer_name)
-
-        seq_module.update({"norm": LlamaSequentialWrapper(self.norm_)})
-        seq_module.move_to_end("norm")
-
-        seq_module.update({"output": LlamaSequentialWrapper(self.output_)})
-        seq_module.move_to_end("output")
-
-        return torch.nn.Sequential(seq_module)
-
     def load_adapter_weight(self, path: str, adapter_name: str = None):
         if adapter_name is None:
             adapter_name = path
         if path != "default":
             if not os.path.exists(path):
                 path = snapshot_download(repo_id=path, repo_type="model")
             with open(path + os.sep + "adapter_config.json", 'r', encoding='utf8') as fp:
```

### Comparing `mlora-0.2.1.post1/mlora/modelargs.py` & `mlora-0.3.0/mlora/common/modelargs.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,11 @@
-from transformers.activations import ACT2FN
 from typing import Any, List, Dict, Callable
+from transformers.activations import ACT2FN
 from mlora.backends import get_backend
+
 from dataclasses import dataclass
 
 import torch
 import copy
 
 
 Tokens = List[int]
@@ -31,24 +32,20 @@
     name_or_path_: str = ""
     device_: str = ""
     dim_: int = 4096
     multiple_of_: int = 256
     n_heads_: int = 32
     n_kv_heads_: int = 32
     n_layers_: int = 32
-    norm_eps_: float = 1e-06
+    hidden_act_: str = "silu"
     hidden_dropout_: float = 0.0
     vocab_size_: int = -1
     pad_token_id_: int = -1
     rope_theta_: float = 10000.0
     max_seq_len_: int = 2048
-    # swa
-    use_sliding_window_: bool = False
-    max_window_layers_: int = None
-    sliding_window_: int = None
     # eager, xformers, flash_attn
     attn_implementation_: str = "eager"
     # data type
     dtype_: torch.dtype = None
 
 
 @dataclass
@@ -130,14 +127,18 @@
             "q_proj": False,
             "k_proj": False,
             "v_proj": False,
             "o_proj": False,
             "w1_proj": False,
             "w2_proj": False,
             "w3_proj": False,
+            # Phi names
+            "dense": False,
+            "fc1": False,
+            "fc2": False,
         }
         if isinstance(config["target_modules"], List):
             for target in config["target_modules"]:
                 if target in self.target_modules_:
                     self.target_modules_[target] = True
         elif isinstance(config["target_modules"], Dict):
             for target, value in config["target_modules"].items():
@@ -196,15 +197,16 @@
         assert isinstance(self.router_aux_loss_coef_,
                           float) and self.router_aux_loss_coef_ >= 0
         assert isinstance(self.router_init_range_,
                           float) and self.router_init_range_ >= 0
         assert isinstance(self.routing_strategy_,
                           str) and self.routing_strategy_ in available_routing_strategies
         assert isinstance(self.num_experts_, int) and self.num_experts_ > 0
-        assert isinstance(self.act_fn_, str) and self.act_fn_ in ACT2FN
+        assert self.act_fn_ is None or (isinstance(
+            self.act_fn_, str) and self.act_fn_ in ACT2FN)
         if self.routing_strategy_ == "mixtral":
             assert isinstance(self.top_k_, int) and self.top_k_ > 0
         elif self.routing_strategy_ == "switch":
             assert isinstance(self.router_z_loss_coef_,
                               float) and self.router_z_loss_coef_ >= 0
             assert isinstance(self.expert_capacity_,
                               int) and self.expert_capacity_ > 0
@@ -223,15 +225,16 @@
             self.expert_config_ = LoraConfig().from_config(expert_config)
         self.router_aux_loss_coef_ = config.get(
             "router_aux_loss_coef", 0.001)  # for training
         self.router_init_range_ = config.get("router_init_range", 0.02)
         self.routing_strategy_ = config["routing_strategy"]
         self.num_experts_ = config["num_experts"]
         # silu for mixtral or gelu_new for switch transformers
-        self.act_fn_ = config.get("act_fn", "silu")
+        # left blank to automatically use the original act_fn of FFN
+        self.act_fn_ = config.get("act_fn", None)
         if self.routing_strategy_ == "mixtral":
             self.top_k_ = config.get("top_k", 2)
         elif self.routing_strategy_ == "switch":
             self.router_z_loss_coef_ = config.get(
                 "router_z_loss_coef", 0.001)  # for training
             # expert_capacity = (max_sequence_length / num_experts) * capacity_factor
             # common values of capacity_factor: 1.0, 1.25, 2.0
@@ -247,15 +250,16 @@
         if self.expert_config_ is not None:
             expert_config = self.expert_config_.export()
             expert_config.pop("peft_type")
             expert_config.pop("target_modules")
             config["expert_lora"] = expert_config
         config["routing_strategy"] = self.routing_strategy_
         config["num_experts"] = self.num_experts_
-        config["act_fn"] = self.act_fn_
+        if self.act_fn_ is not None:
+            config["act_fn"] = self.act_fn_
         if self.routing_strategy_ == "mixtral":
             config["top_k"] = self.top_k_
         elif self.routing_strategy_ == "switch":
             config["expert_capacity"] = self.expert_capacity_
 
         return config
```

### Comparing `mlora-0.2.1.post1/mlora/prompter.py` & `mlora-0.3.0/mlora/prompter.py`

 * *Files identical despite different names*

### Comparing `mlora-0.2.1.post1/mlora/tasks/common.py` & `mlora-0.3.0/mlora/tasks/common.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from mlora.modelargs import DataClass
 from mlora.tokenizer import Tokenizer
 from mlora.prompter import Prompter
+from mlora.common import DataClass
 
 from typing import Any, Dict, List, Tuple, Optional, Callable
 import datasets as hf_datasets
 import evaluate as hf_evaluate
 import logging
 import torch
 
@@ -90,15 +90,15 @@
         data = self.dataset_["train" if is_train else "test"]
         ret: List[DataClass] = []
         for idx, data_point in enumerate(data):
             prompt = self.prompter_.generate_prompt(
                 data_point["instruction"],
                 data_point.get("input", None),
                 data_point.get("output", None))
-            tokens = tokenizer.encode(data=prompt, bos=True, eos=False)
+            tokens = tokenizer.encode(data=prompt)
             ret.append(DataClass(tokens_=tokens, labels_=None))
             if idx % 10000 == 0:
                 logging.info(f"Encode text data: {idx}/{len(data)}")
 
         return ret
 
 
@@ -140,19 +140,17 @@
             data = hf_datasets.load_dataset(split[0], split[1])
         else:
             data = hf_datasets.load_dataset(self.task_name_)
         data = data[self.subset_map_[0] if is_train else self.subset_map_[1]]
         logging.info(f"Preparing data for {self.task_name_.upper()}")
         ret: List[DataClass] = []
         for idx, data_point in enumerate(data):
-            inputs, labels, flags = self.dataload_function_(data_point)
+            inputs, labels = self.dataload_function_(data_point)
             assert isinstance(labels, List)
-            if "eos" in flags and not is_train:
-                flags["eos"] = False
-            tokens = tokenizer.encode(data=inputs, **flags)
+            tokens = tokenizer.encode(data=inputs)
             ret.append(DataClass(tokens_=tokens, labels_=labels))
             if idx % 10000 == 0:
                 logging.info(f"Encode text data: {idx}/{len(data)}")
 
         return ret
 
     def loading_metric(self) -> BasicMetric:
```

### Comparing `mlora-0.2.1.post1/mlora/tasks/evaluator.py` & `mlora-0.3.0/mlora/evaluator.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,21 @@
-from mlora.modelargs import DataClass, LoraBatchDataConfig, MultiLoraBatchData, MixConfig
-from mlora.tasks.common import BasicTask, BasicMetric
-from mlora.tasks.common import CommonSenseTask, task_dict
-from mlora.tokenizer import Tokenizer
-from mlora.model import LLMModel
+from .common import (
+    DataClass,
+    LoraBatchDataConfig,
+    MultiLoraBatchData,
+    MixConfig,
+)
+from .tasks import (
+    BasicTask,
+    BasicMetric,
+    CommonSenseTask,
+    task_dict,
+)
+from .tokenizer import Tokenizer
+from .model import LLMModel
 
 
 from dataclasses import dataclass
 from typing import List, Dict
 
 import logging
 import torch
@@ -33,29 +42,29 @@
         self.task_ = task_dict[self.task_name]
         self.data_ = self.task_.loading_data(tokenizer, False)
         self.metric_ = self.task_.loading_metric()
         if isinstance(self.task_, CommonSenseTask):
             labels = self.task_.label_list()
             label_indices = [0] * len(labels)
             for idx, label in enumerate(labels):
-                ids = tokenizer.encode(" " + label, False, False)
+                ids = tokenizer.encode(" " + label)
                 label_indices[idx] = ids[-1]
             self.label_indices_ = torch.tensor(
                 label_indices, dtype=torch.int64, device=device)
         else:
             self.label_indices_ = None
 
 
 def _prepare_tasks(model, tokenizer, configs):
     for config in configs:
-        config.prepare(tokenizer)
+        config.prepare(tokenizer, model.device_)
         if not isinstance(model.adapter_configs_[config.adapter_name], MixConfig):
             continue
-        for layer in model.layers_:
-            layer.ffn_.moes_[
+        for layer in model.model_.layers_:
+            layer.mlp_.moes_[
                 config.adapter_name].router_profile_ = config.router_profile
 
 
 def _dispatch_task_in(tokenizer, configs, concurrent_jobs, max_seq_len):
     batch_data_config = []
     sequence_lengths = []
     current_configs = []
@@ -121,16 +130,16 @@
 
         if config.router_profile:
             adapter_config = model.adapter_configs_[
                 config.adapter_name]
             if isinstance(adapter_config, MixConfig):
                 router_statistic_ = list(
                     0 for _ in range(adapter_config.num_experts_))
-                for layer in model.layers_:
-                    for idx, val in enumerate(layer.ffn_.moes_[config.adapter_name].profiler_):
+                for layer in model.model_.layers_:
+                    for idx, val in enumerate(layer.mlp_.moes_[config.adapter_name].profiler_):
                         router_statistic_[idx] += val
                 for idx, val in enumerate(router_statistic_):
                     logging.info(
                         f"{config.adapter_name}: expert {idx}, load = {val/32}")
 
         batch_size = logits.shape[0]
         pooled_logits = logits[torch.arange(
@@ -166,18 +175,18 @@
         compute_results = config.metric_.compute()
         result["metrics"] = compute_results
         if config.router_profile:
             adapter_config = model.adapter_configs_[config.adapter_name]
             if isinstance(adapter_config, MixConfig):
                 router_statistic_ = list(
                     0 for _ in range(adapter_config.num_experts_))
-                for layer in model.layers_:
-                    for idx, val in enumerate(layer.ffn_.moes_[config.adapter_name].profiler_):
+                for layer in model.model_.layers_:
+                    for idx, val in enumerate(layer.mlp_.moes_[config.adapter_name].profiler_):
                         router_statistic_[idx] += val
-                    layer.ffn_.moes_[config.adapter_name].profiler_ = None
+                    layer.mlp_.moes_[config.adapter_name].profiler_ = None
                 result["router_profile"] = list(
                     val / 32 for val in router_statistic_)
 
         results.append(result)
 
     if save_file is not None:
         with open(save_file, "w") as f:
```

### Comparing `mlora-0.2.1.post1/mlora/tasks/glue_tasks.py` & `mlora-0.3.0/mlora/tasks/glue_tasks.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,95 +1,87 @@
-from mlora.tasks.common import SequenceClassificationTask
+from .common import SequenceClassificationTask
 import torch
 
 
 def update_task_dict(task_dict):
     task_dict.update({
         "glue:cola": SequenceClassificationTask(
             task_name="glue:cola",
             task_type="single_label_classification",
             num_labels=2,
             label_dtype=torch.long,
             dataload_function=lambda data_point: (
                 [data_point["sentence"]],
                 [int(data_point["label"])],
-                {"bos": True, "eos": True}
             ),
         ),
         "glue:mnli": SequenceClassificationTask(
             task_name="glue:mnli",
             task_type="single_label_classification",
             num_labels=3,
             label_dtype=torch.long,
             dataload_function=lambda data_point: (
                 [data_point["premise"], data_point["hypothesis"]],
                 [int(data_point["label"])],
-                {"bos": True, "eos": True},
             ),
         ),
         "glue:mrpc": SequenceClassificationTask(
             task_name="glue:mrpc",
             task_type="single_label_classification",
             num_labels=2,
             label_dtype=torch.long,
             dataload_function=lambda data_point: (
                 [data_point["sentence1"], data_point["sentence2"]],
                 [int(data_point["label"])],
-                {"bos": True, "eos": True},
             ),
         ),
         "glue:qnli": SequenceClassificationTask(
             task_name="glue:qnli",
             task_type="single_label_classification",
             num_labels=2,
             label_dtype=torch.long,
             dataload_function=lambda data_point: (
                 [data_point["question"], data_point["sentence"]],
                 [int(data_point["label"])],
-                {"bos": True, "eos": True},
             ),
         ),
         "glue:qqp": SequenceClassificationTask(
             task_name="glue:qqp",
             task_type="single_label_classification",
             num_labels=2,
             label_dtype=torch.long,
             dataload_function=lambda data_point: (
                 [data_point["question1"], data_point["question2"]],
                 [int(data_point["label"])],
-                {"bos": True, "eos": True},
             ),
         ),
         "glue:rte": SequenceClassificationTask(
             task_name="glue:rte",
             task_type="single_label_classification",
             num_labels=2,
             label_dtype=torch.long,
             dataload_function=lambda data_point: (
                 [data_point["sentence1"], data_point["sentence2"]],
                 [int(data_point["label"])],
-                {"bos": True, "eos": True},
             ),
         ),
         "glue:sst2": SequenceClassificationTask(
             task_name="glue:sst2",
             task_type="single_label_classification",
             num_labels=2,
             label_dtype=torch.long,
             dataload_function=lambda data_point: (
                 [data_point["sentence"]],
                 [int(data_point["label"])],
-                {"bos": True, "eos": True},
             ),
         ),
         "glue:wnli": SequenceClassificationTask(
             task_name="glue:wnli",
             task_type="single_label_classification",
             num_labels=2,
             label_dtype=torch.long,
             dataload_function=lambda data_point: (
                 [data_point["sentence1"] + " </s> " + data_point["sentence2"]],
                 [int(data_point["label"])],
-                {"bos": True, "eos": True},
             ),
         ),
     })
```

### Comparing `mlora-0.2.1.post1/mlora/tasks/qa_tasks.py` & `mlora-0.3.0/mlora/tasks/qa_tasks.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,11 +1,10 @@
-from mlora.tasks.common import BasicMetric, AutoMetric
-from mlora.tasks.common import CommonSenseTask
-from mlora.modelargs import DataClass
+from .common import BasicMetric, AutoMetric, CommonSenseTask
 from mlora.tokenizer import Tokenizer
+from mlora.common import DataClass
 from typing import List
 
 import datasets as hf_datasets
 import logging
 import torch
 
 
@@ -44,15 +43,15 @@
                 prompt += f" ({label}) {text}"
             prompt += "\nAnswer:"
             if is_train:
                 prompt += " " + data_point["answerKey"]
                 labels = None
             else:
                 labels = [self.labels2id_[data_point["answerKey"]]]
-            tokens = tokenizer.encode(data=prompt, bos=True, eos=False)
+            tokens = tokenizer.encode(data=prompt)
             ret.append(DataClass(tokens_=tokens, labels_=labels))
             if idx % 10000 == 0:
                 logging.info(f"Encode text data: {idx}/{len(data)}")
 
         return ret
 
 
@@ -72,15 +71,15 @@
                 f"{data_point['question']}?\nAnswer:"
             answer = "true" if data_point["answer"] else "false"
             if is_train:
                 prompt += f" {answer}"
                 labels = None
             else:
                 labels = [self.labels2id_[answer]]
-            tokens = tokenizer.encode(data=prompt, bos=True, eos=False)
+            tokens = tokenizer.encode(data=prompt)
             ret.append(DataClass(tokens_=tokens, labels_=labels))
             if idx % 10000 == 0:
                 logging.info(f"Encode text data: {idx}/{len(data)}")
 
         return ret
 
 
@@ -103,15 +102,15 @@
                 prompt += f" ({label}) {text}"
             prompt += "\nAnswer:"
             if is_train:
                 prompt += " " + data_point["answerKey"]
                 labels = None
             else:
                 labels = [self.labels2id_[data_point["answerKey"]]]
-            tokens = tokenizer.encode(data=prompt, bos=True, eos=False)
+            tokens = tokenizer.encode(data=prompt)
             ret.append(DataClass(tokens_=tokens, labels_=labels))
             if idx % 10000 == 0:
                 logging.info(f"Encode text data: {idx}/{len(data)}")
 
         return ret
 
 
@@ -133,15 +132,15 @@
             prompt += "\nCorrect solution:"
             answer = self.labels_[data_point["label"]]
             if is_train:
                 prompt += f" {answer}"
                 labels = None
             else:
                 labels = [data_point["label"]]
-            tokens = tokenizer.encode(data=prompt, bos=True, eos=False)
+            tokens = tokenizer.encode(data=prompt)
             ret.append(DataClass(tokens_=tokens, labels_=labels))
             if idx % 10000 == 0:
                 logging.info(f"Encode text data: {idx}/{len(data)}")
 
         return ret
```

### Comparing `mlora-0.2.1.post1/mlora/tokenizer.py` & `mlora-0.3.0/mlora/tokenizer.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,38 +1,34 @@
-from mlora.modelargs import Tokens, Masks
+from .common import Tokens, Masks
 
 from transformers import AutoTokenizer
 from typing import List, Union
 
 
 class Tokenizer:
     def __init__(self, model_path: str):
-        self.tokenizer = AutoTokenizer.from_pretrained(
-            model_path, trust_remote_code=True)
-        self.n_words_ = self.tokenizer.vocab_size
+        self.tokenizer = AutoTokenizer.from_pretrained(model_path)
+        self.vocab_size_ = self.tokenizer.vocab_size
         self.bos_id_ = self.tokenizer.bos_token_id
         self.eos_id_ = self.tokenizer.eos_token_id
         self.pad_id_ = self.tokenizer.pad_token_id
         self.unk_id_ = self.tokenizer.unk_token_id
         # maybe pad id is unk
         if self.pad_id_ is None and self.unk_id_ is not None:
             self.pad_id_ = self.unk_id_
 
-    def encode(self, data: Union[str, List[str]],
-               bos: bool = True, eos: bool = False) -> Tokens:
+    def encode(self, data: Union[str, List[str]], add_special_tokens: bool = True) -> Tokens:
         if isinstance(data, str):
             data = [data]
-        ret = []
-        for dat in data:
-            if bos and self.bos_id_ is not None:
-                ret.append(self.bos_id_)
-            ret.extend(self.tokenizer.encode(dat, add_special_tokens=False))
-        if eos and self.eos_id_ is not None:
-            ret.append(self.eos_id_)
-        return ret
+        tokens = []
+        ret = self.tokenizer(
+            data, add_special_tokens=add_special_tokens, return_attention_mask=False).input_ids
+        for toks in ret:
+            tokens.extend(toks)
+        return tokens
 
     def decode(self, data: Tokens) -> str:
         return self.tokenizer.decode(data)
 
     # get the mask from tokens
     #   example: tokens is [2, 3, pad, pad, 4, 5]
     #            output is [1, 1, 0,   0,   1, 1]
```

### Comparing `mlora-0.2.1.post1/mlora/train.py` & `mlora-0.3.0/mlora/trainer.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from mlora.modelargs import LoraConfig
-from mlora.dispatcher import TrainTask, Dispatcher
-from mlora.tasks import CasualTask, MultiTask, task_dict
-from mlora.model import LLMModel
+from .tasks import CasualTask, MultiTask, task_dict
+from .dispatcher import TrainTask, Dispatcher
+from .common import LoraConfig
+from .model import LLMModel
 
 from transformers import get_scheduler
 from typing import Dict, List, Union
 import logging
 import torch
 import json
 import os
```

### Comparing `mlora-0.2.1.post1/mlora.egg-info/PKG-INFO` & `mlora-0.3.0/mlora.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlora
-Version: 0.2.1.post1
+Version: 0.3.0
 Summary: A tool for fine-tuning large language models (LLMs) using the LoRA or QLoRA methods more efficiently.
 Project-URL: Homepage, https://github.com/scukdde-llm/mlora
 Project-URL: Bug Tracker, https://github.com/scukdde-llm/mlora/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
@@ -44,25 +44,31 @@
 ## Supported Platform
 
 | OS      | Backend | Model Precision        | Quantization  | xFormers | Flash Attention |
 |---------|---------|------------------------|---------------|----------|-----------------|
 | Linux   | CUDA    | FP32, FP16, TF32, BF16 | 8bit and 4bit | &check;  | &check;         |
 | Windows | CUDA    | FP32, FP16, TF32, BF16 | &cross;       | &cross;  | &cross;         |
 | macOS   | MPS     | FP32, FP16             | &cross;       | &cross;  | &cross;         |
+| All     | CPU     | FP32, FP16, BF16       | &cross;       | &cross;  | &cross;         |
+
+You can use the `MLORA_BACKEND_TYPE` environment variable to force m-LoRA to use a specific backend. For example, if you want m-LoRA to run only on CPU, you can set `MLORA_BACKEND_TYPE=CPU` before importing `mlora`.
 
 **Note**: Windows and macOS support are experimental feature.
 
 ## Supported Pre-trained Models
 
-|         | Model                                                    | # Parameters    |
-|---------|----------------------------------------------------------|-----------------|
-| &check; | [LLaMA](https://github.com/facebookresearch/llama)       | 7B/13B/33B/65B  |
-| &check; | [LLaMA-2](https://huggingface.co/meta-llama)             | 7B/13B/70B      |
-| &check; | [Qwen-2](https://qwenlm.github.io)                       | 4B/7B/14B/72B   |
-| &check; | [Mistral](https://mistral.ai)                            | 7B              |
+|         | Model                                                    | # Parameters       |
+|---------|----------------------------------------------------------|--------------------|
+| &check; | [LLaMA](https://github.com/facebookresearch/llama)       | 7B/13B/33B/65B     |
+| &check; | [LLaMA-2](https://huggingface.co/meta-llama)             | 7B/13B/70B         |
+| &check; | [Qwen-2](https://qwenlm.github.io)                       | 1.8B/4B/7B/14B/72B |
+| &check; | [Mistral](https://mistral.ai)                            | 7B                 |
+| &check; | [Gemma](https://ai.google.dev/gemma/docs)                | 2B/7B              |
+| &check; | [Phi-2](https://huggingface.co/microsoft/phi-2)          | 2.7B               |
+
 
 ## Supported LoRA Variants
 
 |         | LoRA Variants                                            | Arguments*                       |
 |---------|----------------------------------------------------------|----------------------------------|
 | &check; | [QLoRA](https://arxiv.org/abs/2402.12354)                | See *Quantize Methods*           |
 | &check; | [LoRA+](https://arxiv.org/abs/2402.12354)                | `loraplus_lr_ratio: 20.0`        |
@@ -123,47 +129,52 @@
 
 It's crucial to note that regardless of the settings, **LoRA weights are always calculated and stored at full precision**. For maintaining calculation accuracy, m-LoRA framework mandates the use of full precision for calculations when accuracy is imperative.
 
 For users with NVIDIA Ampere or newer GPU architectures, the `--tf32` option can be utilized to enable full-precision calculation acceleration.
 
 ## Known issues
 
- + DoRA with Quantization on Qwen2
- + Half Precision with Qwen2
+ + Applying quantization to Qwen2 in DoRA will result in an error
+ + Employing half precision models on MPS may occasionally result in challenges, such as encountering 'nan' values or experiencing convergence difficulties.
 
 ## Installation
 
 Please refer to [Install Guide](./docs/Install.md).
 
 ## Quickstart
 
-You can use m-LoRA via `launch.py` conveniently:
+You can conveniently utilize m-LoRA via `launch.py`. The following example demonstrates a streamlined approach to training a dummy model with m-LoRA.
 
 ```bash
 # Generating configuration
-python launch.py gen --template lora --tasks yahma/alpaca-cleaned
+python launch.py gen --template lora_phi --tasks ./data/dummy_data.json
 # Running the training task
-python launch.py run --base_model yahma/llama-7b-hf
+python launch.py run --base_model microsoft/phi-2
+# Try with gradio web ui
+python inference.py \
+  --base_model microsoft/phi-2 \
+  --template ./template/alpaca.json \
+  --lora_weights ./casual_0
 ```
 
-For further detailed usage information, please use the `help` command:
+For further detailed usage information, please refer to the `help` command:
 
 ```bash
 python launch.py help
 ```
 
 ## m-LoRA
 
 The `mlora.py` code is a starting point for finetuning on various datasets.
 Basic command for finetuning a baseline model on the [Alpaca Cleaned](https://github.com/gururise/AlpacaDataCleaned) dataset:
 ```bash
 python mlora.py \
-  --base_model yahma/llama-7b-hf \
+  --base_model meta-llama/Llama-2-7b-hf \
   --config ./config/alpaca.json \
-  --load_16bit
+  --bf16
 ```
 
 You can check the template finetune configuration in [template](./template/) folder.
 
 For further detailed usage information, please use `--help` option:
 ```bash
 python mlora.py --help
```

### Comparing `mlora-0.2.1.post1/pyproject.toml` & `mlora-0.3.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mlora"
-version = "0.2.1.post1"
+version = "0.3.0"
 description = "A tool for fine-tuning large language models (LLMs) using the LoRA or QLoRA methods more efficiently."
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
```

