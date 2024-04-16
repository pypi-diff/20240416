# Comparing `tmp/textwiz-0.5.0.tar.gz` & `tmp/textwiz-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "textwiz-0.5.0.tar", last modified: Mon Mar 25 16:15:35 2024, max compression
+gzip compressed data, was "textwiz-0.6.0.tar", last modified: Tue Apr 16 11:38:48 2024, max compression
```

## Comparing `textwiz-0.5.0.tar` & `textwiz-0.6.0.tar`

### file list

```diff
@@ -1,178 +1,180 @@
-drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-03-25 16:15:35.392323 textwiz-0.5.0/
--rw-r--r--   0 cyrilvallez   (501) staff       (20)    11357 2023-12-04 15:22:38.000000 textwiz-0.5.0/LICENSE
--rw-r--r--   0 cyrilvallez   (501) staff       (20)       55 2023-12-04 17:23:04.000000 textwiz-0.5.0/MANIFEST.in
--rw-r--r--   0 cyrilvallez   (501) staff       (20)    18685 2024-03-25 16:15:35.391866 textwiz-0.5.0/PKG-INFO
--rw-r--r--   0 cyrilvallez   (501) staff       (20)     4690 2024-03-20 17:39:43.000000 textwiz-0.5.0/README.md
--rw-r--r--   0 cyrilvallez   (501) staff       (20)     1257 2024-03-05 16:26:57.000000 textwiz-0.5.0/pyproject.toml
--rw-r--r--   0 cyrilvallez   (501) staff       (20)       38 2024-03-25 16:15:35.392399 textwiz-0.5.0/setup.cfg
-drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-03-25 16:15:35.336948 textwiz-0.5.0/textwiz/
--rw-r--r--   0 cyrilvallez   (501) staff       (20)     5091 2024-03-25 16:12:50.000000 textwiz-0.5.0/textwiz/__init__.py
-drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-03-25 16:15:35.339174 textwiz-0.5.0/textwiz/configs/
--rw-r--r--   0 cyrilvallez   (501) staff       (20)     3208 2024-03-20 16:54:16.000000 textwiz-0.5.0/textwiz/configs/__init__.py
-drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-03-25 16:15:35.345389 textwiz-0.5.0/textwiz/configs/causal/
--rw-r--r--   0 cyrilvallez   (501) staff       (20)     1746 2024-03-20 16:54:53.000000 textwiz-0.5.0/textwiz/configs/causal/__init__.py
--rw-r--r--   0 cyrilvallez   (501) staff       (20)      671 2024-03-20 10:17:49.000000 textwiz-0.5.0/textwiz/configs/causal/bloom.py
--rw-r--r--   0 cyrilvallez   (501) staff       (20)     1637 2024-03-20 10:18:21.000000 textwiz-0.5.0/textwiz/configs/causal/code_llama.py
--rw-r--r--   0 cyrilvallez   (501) staff       (20)      561 2024-03-20 10:18:42.000000 textwiz-0.5.0/textwiz/configs/causal/codegen.py
--rw-r--r--   0 cyrilvallez   (501) staff       (20)     1464 2024-03-20 10:19:09.000000 textwiz-0.5.0/textwiz/configs/causal/codegen2.py
--rw-r--r--   0 cyrilvallez   (501) staff       (20)      546 2024-03-20 10:19:29.000000 textwiz-0.5.0/textwiz/configs/causal/dialo_gpt.py
--rw-r--r--   0 cyrilvallez   (501) staff       (20)      459 2024-03-20 10:20:21.000000 textwiz-0.5.0/textwiz/configs/causal/gpt2.py
--rw-r--r--   0 cyrilvallez   (501) staff       (20)      816 2024-03-20 10:19:52.000000 textwiz-0.5.0/textwiz/configs/causal/gpt_j_neo.py
--rw-r--r--   0 cyrilvallez   (501) staff       (20)      912 2024-03-20 10:20:47.000000 textwiz-0.5.0/textwiz/configs/causal/llama2.py
--rw-r--r--   0 cyrilvallez   (501) staff       (20)      685 2024-03-20 11:11:45.000000 textwiz-0.5.0/textwiz/configs/causal/mistral.py
--rw-r--r--   0 cyrilvallez   (501) staff       (20)      645 2024-03-20 10:21:49.000000 textwiz-0.5.0/textwiz/configs/causal/opt.py
--rw-r--r--   0 cyrilvallez   (501) staff       (20)      482 2024-03-20 10:22:16.000000 textwiz-0.5.0/textwiz/configs/causal/stable_lm.py
--rw-r--r--   0 cyrilvallez   (501) staff       (20)      476 2024-03-20 10:22:36.000000 textwiz-0.5.0/textwiz/configs/causal/star_chat.py
--rw-r--r--   0 cyrilvallez   (501) staff       (20)      572 2024-03-20 10:22:58.000000 textwiz-0.5.0/textwiz/configs/causal/star_coder.py
--rw-r--r--   0 cyrilvallez   (501) staff       (20)      696 2024-03-20 10:23:24.000000 textwiz-0.5.0/textwiz/configs/causal/vicuna.py
--rw-r--r--   0 cyrilvallez   (501) staff       (20)      742 2024-03-20 10:23:49.000000 textwiz-0.5.0/textwiz/configs/causal/zephyr.py
-drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-03-25 16:15:35.346066 textwiz-0.5.0/textwiz/configs/embedding/
--rw-r--r--   0 cyrilvallez   (501) staff       (20)     1749 2024-03-20 16:54:36.000000 textwiz-0.5.0/textwiz/configs/embedding/__init__.py
--rw-r--r--   0 cyrilvallez   (501) staff       (20)      716 2024-03-22 10:32:24.000000 textwiz-0.5.0/textwiz/configs/embedding/mistral.py
-drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-03-25 16:15:35.319062 textwiz-0.5.0/textwiz/data/
-drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-03-25 16:15:35.331942 textwiz-0.5.0/textwiz/data/memory_estimator/
-drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-03-25 16:15:35.346414 textwiz-0.5.0/textwiz/data/memory_estimator/bloom-1.7B/
--rw-r--r--   0 cyrilvallez   (501) staff       (20)     2350 2023-10-03 06:55:37.000000 textwiz-0.5.0/textwiz/data/memory_estimator/bloom-1.7B/float16.json
-drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-03-25 16:15:35.346738 textwiz-0.5.0/textwiz/data/memory_estimator/bloom-3B/
--rw-r--r--   0 cyrilvallez   (501) staff       (20)     2339 2023-10-03 06:55:37.000000 textwiz-0.5.0/textwiz/data/memory_estimator/bloom-3B/float16.json
-drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-03-25 16:15:35.347010 textwiz-0.5.0/textwiz/data/memory_estimator/bloom-560M/
--rw-r--r--   0 cyrilvallez   (501) staff       (20)     2356 2023-10-03 06:55:37.000000 textwiz-0.5.0/textwiz/data/memory_estimator/bloom-560M/float16.json
-drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-03-25 16:15:35.347348 textwiz-0.5.0/textwiz/data/memory_estimator/bloom-7.1B/
--rw-r--r--   0 cyrilvallez   (501) staff       (20)     2332 2023-10-03 06:55:38.000000 textwiz-0.5.0/textwiz/data/memory_estimator/bloom-7.1B/float16.json
-drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-03-25 16:15:35.347859 textwiz-0.5.0/textwiz/data/memory_estimator/code-llama-13B/
--rw-r--r--   0 cyrilvallez   (501) staff       (20)     2338 2023-10-03 06:55:40.000000 textwiz-0.5.0/textwiz/data/memory_estimator/code-llama-13B/bfloat16.json
-drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-03-25 16:15:35.348353 textwiz-0.5.0/textwiz/data/memory_estimator/code-llama-13B-instruct/
--rw-r--r--   0 cyrilvallez   (501) staff       (20)     2328 2023-10-03 06:55:40.000000 textwiz-0.5.0/textwiz/data/memory_estimator/code-llama-13B-instruct/bfloat16.json
-drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-03-25 16:15:35.348913 textwiz-0.5.0/textwiz/data/memory_estimator/code-llama-13B-python/
--rw-r--r--   0 cyrilvallez   (501) staff       (20)     2335 2023-10-03 06:55:40.000000 textwiz-0.5.0/textwiz/data/memory_estimator/code-llama-13B-python/bfloat16.json
-drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-03-25 16:15:35.349692 textwiz-0.5.0/textwiz/data/memory_estimator/code-llama-34B/
--rw-r--r--   0 cyrilvallez   (501) staff       (20)     2365 2023-10-03 06:55:40.000000 textwiz-0.5.0/textwiz/data/memory_estimator/code-llama-34B/bfloat16.json
-drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-03-25 16:15:35.350543 textwiz-0.5.0/textwiz/data/memory_estimator/code-llama-34B-instruct/
--rw-r--r--   0 cyrilvallez   (501) staff       (20)     2364 2023-10-03 06:55:38.000000 textwiz-0.5.0/textwiz/data/memory_estimator/code-llama-34B-instruct/bfloat16.json
-drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-03-25 16:15:35.351292 textwiz-0.5.0/textwiz/data/memory_estimator/code-llama-34B-python/
--rw-r--r--   0 cyrilvallez   (501) staff       (20)     2365 2023-10-03 06:55:40.000000 textwiz-0.5.0/textwiz/data/memory_estimator/code-llama-34B-python/bfloat16.json
-drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-03-25 16:15:35.351977 textwiz-0.5.0/textwiz/data/memory_estimator/code-llama-7B/
--rw-r--r--   0 cyrilvallez   (501) staff       (20)     2346 2023-10-03 06:55:39.000000 textwiz-0.5.0/textwiz/data/memory_estimator/code-llama-7B/bfloat16.json
-drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-03-25 16:15:35.352399 textwiz-0.5.0/textwiz/data/memory_estimator/code-llama-7B-instruct/
--rw-r--r--   0 cyrilvallez   (501) staff       (20)     2328 2023-10-03 06:55:39.000000 textwiz-0.5.0/textwiz/data/memory_estimator/code-llama-7B-instruct/bfloat16.json
-drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-03-25 16:15:35.353012 textwiz-0.5.0/textwiz/data/memory_estimator/code-llama-7B-python/
--rw-r--r--   0 cyrilvallez   (501) staff       (20)     2346 2023-10-03 06:55:39.000000 textwiz-0.5.0/textwiz/data/memory_estimator/code-llama-7B-python/bfloat16.json
-drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-03-25 16:15:35.353666 textwiz-0.5.0/textwiz/data/memory_estimator/codegen-16B/
--rw-r--r--   0 cyrilvallez   (501) staff       (20)     2312 2023-10-03 06:55:39.000000 textwiz-0.5.0/textwiz/data/memory_estimator/codegen-16B/float16.json
-drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-03-25 16:15:35.354292 textwiz-0.5.0/textwiz/data/memory_estimator/codegen-2B/
--rw-r--r--   0 cyrilvallez   (501) staff       (20)     2342 2023-10-03 06:55:38.000000 textwiz-0.5.0/textwiz/data/memory_estimator/codegen-2B/float16.json
-drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-03-25 16:15:35.354833 textwiz-0.5.0/textwiz/data/memory_estimator/codegen-350M/
--rw-r--r--   0 cyrilvallez   (501) staff       (20)     2374 2023-10-03 06:55:37.000000 textwiz-0.5.0/textwiz/data/memory_estimator/codegen-350M/float16.json
-drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-03-25 16:15:35.355411 textwiz-0.5.0/textwiz/data/memory_estimator/codegen-6B/
--rw-r--r--   0 cyrilvallez   (501) staff       (20)     2337 2023-10-03 06:55:38.000000 textwiz-0.5.0/textwiz/data/memory_estimator/codegen-6B/float16.json
-drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-03-25 16:15:35.355946 textwiz-0.5.0/textwiz/data/memory_estimator/codegen2-16B/
--rw-r--r--   0 cyrilvallez   (501) staff       (20)     1153 2023-10-03 06:55:39.000000 textwiz-0.5.0/textwiz/data/memory_estimator/codegen2-16B/float16.json
-drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-03-25 16:15:35.356475 textwiz-0.5.0/textwiz/data/memory_estimator/codegen2-1B/
--rw-r--r--   0 cyrilvallez   (501) staff       (20)     1170 2023-10-03 06:55:37.000000 textwiz-0.5.0/textwiz/data/memory_estimator/codegen2-1B/float16.json
-drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-03-25 16:15:35.356965 textwiz-0.5.0/textwiz/data/memory_estimator/codegen2-3.7B/
--rw-r--r--   0 cyrilvallez   (501) staff       (20)     1164 2023-10-03 06:55:37.000000 textwiz-0.5.0/textwiz/data/memory_estimator/codegen2-3.7B/float16.json
-drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-03-25 16:15:35.357591 textwiz-0.5.0/textwiz/data/memory_estimator/codegen2-7B/
--rw-r--r--   0 cyrilvallez   (501) staff       (20)     1155 2023-10-03 06:55:39.000000 textwiz-0.5.0/textwiz/data/memory_estimator/codegen2-7B/float16.json
-drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-03-25 16:15:35.358309 textwiz-0.5.0/textwiz/data/memory_estimator/codegen25-7B/
--rw-r--r--   0 cyrilvallez   (501) staff       (20)     2332 2023-10-03 06:55:39.000000 textwiz-0.5.0/textwiz/data/memory_estimator/codegen25-7B/float16.json
-drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-03-25 16:15:35.358878 textwiz-0.5.0/textwiz/data/memory_estimator/codegen25-7B-instruct/
--rw-r--r--   0 cyrilvallez   (501) staff       (20)     2330 2023-10-03 06:55:38.000000 textwiz-0.5.0/textwiz/data/memory_estimator/codegen25-7B-instruct/float16.json
-drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-03-25 16:15:35.359398 textwiz-0.5.0/textwiz/data/memory_estimator/dialo-gpt-large/
--rw-r--r--   0 cyrilvallez   (501) staff       (20)     1163 2023-10-03 06:55:37.000000 textwiz-0.5.0/textwiz/data/memory_estimator/dialo-gpt-large/float32.json
-drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-03-25 16:15:35.359921 textwiz-0.5.0/textwiz/data/memory_estimator/dialo-gpt-medium/
--rw-r--r--   0 cyrilvallez   (501) staff       (20)     1178 2023-10-03 06:55:37.000000 textwiz-0.5.0/textwiz/data/memory_estimator/dialo-gpt-medium/float32.json
-drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-03-25 16:15:35.360704 textwiz-0.5.0/textwiz/data/memory_estimator/dialo-gpt-small/
--rw-r--r--   0 cyrilvallez   (501) staff       (20)     1189 2023-10-03 06:55:37.000000 textwiz-0.5.0/textwiz/data/memory_estimator/dialo-gpt-small/float32.json
-drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-03-25 16:15:35.361518 textwiz-0.5.0/textwiz/data/memory_estimator/gpt-j-6B/
--rw-r--r--   0 cyrilvallez   (501) staff       (20)     2333 2023-10-03 06:55:39.000000 textwiz-0.5.0/textwiz/data/memory_estimator/gpt-j-6B/float32.json
-drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-03-25 16:15:35.362137 textwiz-0.5.0/textwiz/data/memory_estimator/gpt-neo-1.3B/
--rw-r--r--   0 cyrilvallez   (501) staff       (20)     2342 2023-10-03 06:55:39.000000 textwiz-0.5.0/textwiz/data/memory_estimator/gpt-neo-1.3B/float32.json
-drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-03-25 16:15:35.362635 textwiz-0.5.0/textwiz/data/memory_estimator/gpt-neo-125M/
--rw-r--r--   0 cyrilvallez   (501) staff       (20)     2384 2023-10-03 06:55:37.000000 textwiz-0.5.0/textwiz/data/memory_estimator/gpt-neo-125M/float32.json
-drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-03-25 16:15:35.363175 textwiz-0.5.0/textwiz/data/memory_estimator/gpt-neo-2.7B/
--rw-r--r--   0 cyrilvallez   (501) staff       (20)     2333 2023-10-03 06:55:39.000000 textwiz-0.5.0/textwiz/data/memory_estimator/gpt-neo-2.7B/float32.json
-drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-03-25 16:15:35.363833 textwiz-0.5.0/textwiz/data/memory_estimator/gpt-neoX-20B/
--rw-r--r--   0 cyrilvallez   (501) staff       (20)     2299 2023-10-03 06:55:40.000000 textwiz-0.5.0/textwiz/data/memory_estimator/gpt-neoX-20B/float16.json
-drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-03-25 16:15:35.364402 textwiz-0.5.0/textwiz/data/memory_estimator/gpt2-large/
--rw-r--r--   0 cyrilvallez   (501) staff       (20)     1163 2023-10-03 06:55:38.000000 textwiz-0.5.0/textwiz/data/memory_estimator/gpt2-large/float32.json
-drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-03-25 16:15:35.365015 textwiz-0.5.0/textwiz/data/memory_estimator/gpt2-medium/
--rw-r--r--   0 cyrilvallez   (501) staff       (20)     1175 2023-10-03 06:55:37.000000 textwiz-0.5.0/textwiz/data/memory_estimator/gpt2-medium/float32.json
-drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-03-25 16:15:35.365561 textwiz-0.5.0/textwiz/data/memory_estimator/gpt2-xl/
--rw-r--r--   0 cyrilvallez   (501) staff       (20)     1158 2023-10-03 06:55:37.000000 textwiz-0.5.0/textwiz/data/memory_estimator/gpt2-xl/float32.json
-drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-03-25 16:15:35.366051 textwiz-0.5.0/textwiz/data/memory_estimator/llama2-13B/
--rw-r--r--   0 cyrilvallez   (501) staff       (20)     2331 2023-10-03 06:55:39.000000 textwiz-0.5.0/textwiz/data/memory_estimator/llama2-13B/float16.json
-drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-03-25 16:15:35.366490 textwiz-0.5.0/textwiz/data/memory_estimator/llama2-13B-chat/
--rw-r--r--   0 cyrilvallez   (501) staff       (20)     2328 2023-10-03 06:55:40.000000 textwiz-0.5.0/textwiz/data/memory_estimator/llama2-13B-chat/float16.json
-drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-03-25 16:15:35.367119 textwiz-0.5.0/textwiz/data/memory_estimator/llama2-70B/
--rw-r--r--   0 cyrilvallez   (501) staff       (20)     2354 2023-10-03 06:55:38.000000 textwiz-0.5.0/textwiz/data/memory_estimator/llama2-70B/float16.json
-drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-03-25 16:15:35.367737 textwiz-0.5.0/textwiz/data/memory_estimator/llama2-70B-chat/
--rw-r--r--   0 cyrilvallez   (501) staff       (20)     2350 2023-10-03 06:55:38.000000 textwiz-0.5.0/textwiz/data/memory_estimator/llama2-70B-chat/float16.json
-drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-03-25 16:15:35.369470 textwiz-0.5.0/textwiz/data/memory_estimator/llama2-7B/
--rw-r--r--   0 cyrilvallez   (501) staff       (20)     2349 2023-10-03 06:55:39.000000 textwiz-0.5.0/textwiz/data/memory_estimator/llama2-7B/float16.json
-drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-03-25 16:15:35.371901 textwiz-0.5.0/textwiz/data/memory_estimator/llama2-7B-chat/
--rw-r--r--   0 cyrilvallez   (501) staff       (20)     2344 2023-10-03 06:55:39.000000 textwiz-0.5.0/textwiz/data/memory_estimator/llama2-7B-chat/float16.json
-drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-03-25 16:15:35.372915 textwiz-0.5.0/textwiz/data/memory_estimator/opt-1.3B/
--rw-r--r--   0 cyrilvallez   (501) staff       (20)     2375 2023-10-03 06:55:37.000000 textwiz-0.5.0/textwiz/data/memory_estimator/opt-1.3B/float16.json
-drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-03-25 16:15:35.373594 textwiz-0.5.0/textwiz/data/memory_estimator/opt-125M/
--rw-r--r--   0 cyrilvallez   (501) staff       (20)     2400 2023-10-03 06:55:37.000000 textwiz-0.5.0/textwiz/data/memory_estimator/opt-125M/float16.json
-drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-03-25 16:15:35.374249 textwiz-0.5.0/textwiz/data/memory_estimator/opt-13B/
--rw-r--r--   0 cyrilvallez   (501) staff       (20)     2330 2023-10-03 06:55:39.000000 textwiz-0.5.0/textwiz/data/memory_estimator/opt-13B/float16.json
-drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-03-25 16:15:35.374812 textwiz-0.5.0/textwiz/data/memory_estimator/opt-2.7B/
--rw-r--r--   0 cyrilvallez   (501) staff       (20)     2339 2023-10-03 06:55:39.000000 textwiz-0.5.0/textwiz/data/memory_estimator/opt-2.7B/float16.json
-drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-03-25 16:15:35.375462 textwiz-0.5.0/textwiz/data/memory_estimator/opt-30B/
--rw-r--r--   0 cyrilvallez   (501) staff       (20)     2306 2023-10-03 06:55:40.000000 textwiz-0.5.0/textwiz/data/memory_estimator/opt-30B/float16.json
-drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-03-25 16:15:35.376007 textwiz-0.5.0/textwiz/data/memory_estimator/opt-350M/
--rw-r--r--   0 cyrilvallez   (501) staff       (20)     2389 2023-10-03 06:55:38.000000 textwiz-0.5.0/textwiz/data/memory_estimator/opt-350M/float16.json
-drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-03-25 16:15:35.376518 textwiz-0.5.0/textwiz/data/memory_estimator/opt-6.7B/
--rw-r--r--   0 cyrilvallez   (501) staff       (20)     2341 2023-10-03 06:55:39.000000 textwiz-0.5.0/textwiz/data/memory_estimator/opt-6.7B/float16.json
-drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-03-25 16:15:35.377163 textwiz-0.5.0/textwiz/data/memory_estimator/opt-66B/
--rw-r--r--   0 cyrilvallez   (501) staff       (20)     2286 2023-10-03 06:55:38.000000 textwiz-0.5.0/textwiz/data/memory_estimator/opt-66B/float16.json
-drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-03-25 16:15:35.377703 textwiz-0.5.0/textwiz/data/memory_estimator/stable-lm-3B/
--rw-r--r--   0 cyrilvallez   (501) staff       (20)     2342 2023-10-03 06:55:37.000000 textwiz-0.5.0/textwiz/data/memory_estimator/stable-lm-3B/float16.json
-drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-03-25 16:15:35.378254 textwiz-0.5.0/textwiz/data/memory_estimator/stable-lm-7B/
--rw-r--r--   0 cyrilvallez   (501) staff       (20)     2332 2023-10-03 06:55:37.000000 textwiz-0.5.0/textwiz/data/memory_estimator/stable-lm-7B/float16.json
-drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-03-25 16:15:35.378739 textwiz-0.5.0/textwiz/data/memory_estimator/star-chat-alpha/
--rw-r--r--   0 cyrilvallez   (501) staff       (20)     2345 2023-10-03 06:55:38.000000 textwiz-0.5.0/textwiz/data/memory_estimator/star-chat-alpha/float16.json
-drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-03-25 16:15:35.379189 textwiz-0.5.0/textwiz/data/memory_estimator/star-chat-beta/
--rw-r--r--   0 cyrilvallez   (501) staff       (20)     2345 2023-10-03 06:55:38.000000 textwiz-0.5.0/textwiz/data/memory_estimator/star-chat-beta/bfloat16.json
-drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-03-25 16:15:35.379653 textwiz-0.5.0/textwiz/data/memory_estimator/star-coder/
--rw-r--r--   0 cyrilvallez   (501) staff       (20)     2357 2023-10-03 06:55:38.000000 textwiz-0.5.0/textwiz/data/memory_estimator/star-coder/bfloat16.json
-drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-03-25 16:15:35.380076 textwiz-0.5.0/textwiz/data/memory_estimator/star-coder-base/
--rw-r--r--   0 cyrilvallez   (501) staff       (20)     2364 2023-10-03 06:55:38.000000 textwiz-0.5.0/textwiz/data/memory_estimator/star-coder-base/bfloat16.json
-drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-03-25 16:15:35.380620 textwiz-0.5.0/textwiz/data/memory_estimator/star-coder-plus/
--rw-r--r--   0 cyrilvallez   (501) staff       (20)     2364 2023-10-03 06:55:38.000000 textwiz-0.5.0/textwiz/data/memory_estimator/star-coder-plus/bfloat16.json
-drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-03-25 16:15:35.381110 textwiz-0.5.0/textwiz/data/memory_estimator/vicuna-13B/
--rw-r--r--   0 cyrilvallez   (501) staff       (20)     2329 2023-10-03 06:55:38.000000 textwiz-0.5.0/textwiz/data/memory_estimator/vicuna-13B/float16.json
-drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-03-25 16:15:35.381633 textwiz-0.5.0/textwiz/data/memory_estimator/vicuna-7B/
--rw-r--r--   0 cyrilvallez   (501) staff       (20)     2343 2023-10-03 06:55:38.000000 textwiz-0.5.0/textwiz/data/memory_estimator/vicuna-7B/float16.json
-drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-03-25 16:15:35.384194 textwiz-0.5.0/textwiz/helpers/
--rw-r--r--   0 cyrilvallez   (501) staff       (20)       33 2024-03-20 13:55:23.000000 textwiz-0.5.0/textwiz/helpers/__init__.py
--rw-r--r--   0 cyrilvallez   (501) staff       (20)      111 2023-12-04 10:40:32.000000 textwiz-0.5.0/textwiz/helpers/constants.py
--rw-r--r--   0 cyrilvallez   (501) staff       (20)     4495 2023-12-13 08:53:53.000000 textwiz-0.5.0/textwiz/helpers/utils.py
--rw-r--r--   0 cyrilvallez   (501) staff       (20)     4183 2023-12-01 15:07:13.000000 textwiz-0.5.0/textwiz/helpers/warnings_suppressor.py
--rw-r--r--   0 cyrilvallez   (501) staff       (20)    19863 2024-03-25 09:58:36.000000 textwiz-0.5.0/textwiz/loader.py
-drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-03-25 16:15:35.386322 textwiz-0.5.0/textwiz/models/
--rw-r--r--   0 cyrilvallez   (501) staff       (20)       73 2024-03-20 14:06:42.000000 textwiz-0.5.0/textwiz/models/__init__.py
--rw-r--r--   0 cyrilvallez   (501) staff       (20)     5870 2024-03-20 14:08:11.000000 textwiz-0.5.0/textwiz/models/base.py
--rw-r--r--   0 cyrilvallez   (501) staff       (20)    43608 2024-03-20 14:09:15.000000 textwiz-0.5.0/textwiz/models/causal.py
--rw-r--r--   0 cyrilvallez   (501) staff       (20)     4435 2024-03-20 17:28:41.000000 textwiz-0.5.0/textwiz/models/embedding.py
-drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-03-25 16:15:35.387012 textwiz-0.5.0/textwiz/parsers/
--rw-r--r--   0 cyrilvallez   (501) staff       (20)       49 2024-03-20 13:48:21.000000 textwiz-0.5.0/textwiz/parsers/__init__.py
--rw-r--r--   0 cyrilvallez   (501) staff       (20)     8049 2024-03-20 14:21:01.000000 textwiz-0.5.0/textwiz/parsers/code_parser.py
-drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-03-25 16:15:35.387632 textwiz-0.5.0/textwiz/stopping/
--rw-r--r--   0 cyrilvallez   (501) staff       (20)       84 2024-03-20 13:47:13.000000 textwiz-0.5.0/textwiz/stopping/__init__.py
--rw-r--r--   0 cyrilvallez   (501) staff       (20)    20387 2024-03-20 13:45:45.000000 textwiz-0.5.0/textwiz/stopping/stopping.py
-drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-03-25 16:15:35.389598 textwiz-0.5.0/textwiz/templates/
--rw-r--r--   0 cyrilvallez   (501) staff       (20)      196 2024-03-20 13:45:08.000000 textwiz-0.5.0/textwiz/templates/__init__.py
--rw-r--r--   0 cyrilvallez   (501) staff       (20)    21526 2024-03-20 13:40:31.000000 textwiz-0.5.0/textwiz/templates/conversation_template.py
--rw-r--r--   0 cyrilvallez   (501) staff       (20)    15884 2024-03-20 13:50:02.000000 textwiz-0.5.0/textwiz/templates/prompt_template.py
-drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-03-25 16:15:35.390671 textwiz-0.5.0/textwiz/webapp/
--rw-r--r--   0 cyrilvallez   (501) staff       (20)      213 2024-03-20 13:53:44.000000 textwiz-0.5.0/textwiz/webapp/__init__.py
--rw-r--r--   0 cyrilvallez   (501) staff       (20)     2456 2024-03-20 13:51:14.000000 textwiz-0.5.0/textwiz/webapp/streamer.py
--rw-r--r--   0 cyrilvallez   (501) staff       (20)    16274 2024-03-20 14:22:47.000000 textwiz-0.5.0/textwiz/webapp/web_interface.py
-drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-03-25 16:15:35.391167 textwiz-0.5.0/textwiz.egg-info/
--rw-r--r--   0 cyrilvallez   (501) staff       (20)    18685 2024-03-25 16:15:35.000000 textwiz-0.5.0/textwiz.egg-info/PKG-INFO
--rw-r--r--   0 cyrilvallez   (501) staff       (20)     4653 2024-03-25 16:15:35.000000 textwiz-0.5.0/textwiz.egg-info/SOURCES.txt
--rw-r--r--   0 cyrilvallez   (501) staff       (20)        1 2024-03-25 16:15:35.000000 textwiz-0.5.0/textwiz.egg-info/dependency_links.txt
--rw-r--r--   0 cyrilvallez   (501) staff       (20)      168 2024-03-25 16:15:35.000000 textwiz-0.5.0/textwiz.egg-info/requires.txt
--rw-r--r--   0 cyrilvallez   (501) staff       (20)        8 2024-03-25 16:15:35.000000 textwiz-0.5.0/textwiz.egg-info/top_level.txt
+drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-04-16 11:38:48.799729 textwiz-0.6.0/
+-rw-r--r--   0 cyrilvallez   (501) staff       (20)    11357 2023-12-04 15:22:38.000000 textwiz-0.6.0/LICENSE
+-rw-r--r--   0 cyrilvallez   (501) staff       (20)       55 2023-12-04 17:23:04.000000 textwiz-0.6.0/MANIFEST.in
+-rw-r--r--   0 cyrilvallez   (501) staff       (20)    18707 2024-04-16 11:38:48.798764 textwiz-0.6.0/PKG-INFO
+-rw-r--r--   0 cyrilvallez   (501) staff       (20)     4690 2024-03-20 17:39:43.000000 textwiz-0.6.0/README.md
+-rw-r--r--   0 cyrilvallez   (501) staff       (20)     1247 2024-03-26 14:43:30.000000 textwiz-0.6.0/pyproject.toml
+-rw-r--r--   0 cyrilvallez   (501) staff       (20)       38 2024-04-16 11:38:48.799897 textwiz-0.6.0/setup.cfg
+drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-04-16 11:38:48.709044 textwiz-0.6.0/textwiz/
+-rw-r--r--   0 cyrilvallez   (501) staff       (20)     5135 2024-04-16 11:37:18.000000 textwiz-0.6.0/textwiz/__init__.py
+drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-04-16 11:38:48.713094 textwiz-0.6.0/textwiz/configs/
+-rw-r--r--   0 cyrilvallez   (501) staff       (20)     3208 2024-03-20 16:54:16.000000 textwiz-0.6.0/textwiz/configs/__init__.py
+drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-04-16 11:38:48.730913 textwiz-0.6.0/textwiz/configs/causal/
+-rw-r--r--   0 cyrilvallez   (501) staff       (20)     1746 2024-03-20 16:54:53.000000 textwiz-0.6.0/textwiz/configs/causal/__init__.py
+-rw-r--r--   0 cyrilvallez   (501) staff       (20)      671 2024-03-20 10:17:49.000000 textwiz-0.6.0/textwiz/configs/causal/bloom.py
+-rw-r--r--   0 cyrilvallez   (501) staff       (20)     1637 2024-03-20 10:18:21.000000 textwiz-0.6.0/textwiz/configs/causal/code_llama.py
+-rw-r--r--   0 cyrilvallez   (501) staff       (20)      561 2024-03-20 10:18:42.000000 textwiz-0.6.0/textwiz/configs/causal/codegen.py
+-rw-r--r--   0 cyrilvallez   (501) staff       (20)     1464 2024-03-20 10:19:09.000000 textwiz-0.6.0/textwiz/configs/causal/codegen2.py
+-rw-r--r--   0 cyrilvallez   (501) staff       (20)      578 2024-04-11 14:21:19.000000 textwiz-0.6.0/textwiz/configs/causal/command.py
+-rw-r--r--   0 cyrilvallez   (501) staff       (20)      546 2024-03-20 10:19:29.000000 textwiz-0.6.0/textwiz/configs/causal/dialo_gpt.py
+-rw-r--r--   0 cyrilvallez   (501) staff       (20)      459 2024-03-20 10:20:21.000000 textwiz-0.6.0/textwiz/configs/causal/gpt2.py
+-rw-r--r--   0 cyrilvallez   (501) staff       (20)      816 2024-03-20 10:19:52.000000 textwiz-0.6.0/textwiz/configs/causal/gpt_j_neo.py
+-rw-r--r--   0 cyrilvallez   (501) staff       (20)      912 2024-03-20 10:20:47.000000 textwiz-0.6.0/textwiz/configs/causal/llama2.py
+-rw-r--r--   0 cyrilvallez   (501) staff       (20)      959 2024-04-15 08:48:40.000000 textwiz-0.6.0/textwiz/configs/causal/mistral.py
+-rw-r--r--   0 cyrilvallez   (501) staff       (20)      645 2024-03-20 10:21:49.000000 textwiz-0.6.0/textwiz/configs/causal/opt.py
+-rw-r--r--   0 cyrilvallez   (501) staff       (20)      482 2024-03-20 10:22:16.000000 textwiz-0.6.0/textwiz/configs/causal/stable_lm.py
+-rw-r--r--   0 cyrilvallez   (501) staff       (20)      476 2024-03-20 10:22:36.000000 textwiz-0.6.0/textwiz/configs/causal/star_chat.py
+-rw-r--r--   0 cyrilvallez   (501) staff       (20)      572 2024-03-20 10:22:58.000000 textwiz-0.6.0/textwiz/configs/causal/star_coder.py
+-rw-r--r--   0 cyrilvallez   (501) staff       (20)      760 2024-04-15 11:54:12.000000 textwiz-0.6.0/textwiz/configs/causal/starling.py
+-rw-r--r--   0 cyrilvallez   (501) staff       (20)      696 2024-03-20 10:23:24.000000 textwiz-0.6.0/textwiz/configs/causal/vicuna.py
+-rw-r--r--   0 cyrilvallez   (501) staff       (20)      742 2024-03-20 10:23:49.000000 textwiz-0.6.0/textwiz/configs/causal/zephyr.py
+drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-04-16 11:38:48.733264 textwiz-0.6.0/textwiz/configs/embedding/
+-rw-r--r--   0 cyrilvallez   (501) staff       (20)     1749 2024-03-20 16:54:36.000000 textwiz-0.6.0/textwiz/configs/embedding/__init__.py
+-rw-r--r--   0 cyrilvallez   (501) staff       (20)      716 2024-03-22 10:32:24.000000 textwiz-0.6.0/textwiz/configs/embedding/mistral.py
+drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-04-16 11:38:48.688030 textwiz-0.6.0/textwiz/data/
+drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-04-16 11:38:48.704295 textwiz-0.6.0/textwiz/data/memory_estimator/
+drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-04-16 11:38:48.734293 textwiz-0.6.0/textwiz/data/memory_estimator/bloom-1.7B/
+-rw-r--r--   0 cyrilvallez   (501) staff       (20)     2350 2023-10-03 06:55:37.000000 textwiz-0.6.0/textwiz/data/memory_estimator/bloom-1.7B/float16.json
+drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-04-16 11:38:48.735627 textwiz-0.6.0/textwiz/data/memory_estimator/bloom-3B/
+-rw-r--r--   0 cyrilvallez   (501) staff       (20)     2339 2023-10-03 06:55:37.000000 textwiz-0.6.0/textwiz/data/memory_estimator/bloom-3B/float16.json
+drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-04-16 11:38:48.737051 textwiz-0.6.0/textwiz/data/memory_estimator/bloom-560M/
+-rw-r--r--   0 cyrilvallez   (501) staff       (20)     2356 2023-10-03 06:55:37.000000 textwiz-0.6.0/textwiz/data/memory_estimator/bloom-560M/float16.json
+drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-04-16 11:38:48.738903 textwiz-0.6.0/textwiz/data/memory_estimator/bloom-7.1B/
+-rw-r--r--   0 cyrilvallez   (501) staff       (20)     2332 2023-10-03 06:55:38.000000 textwiz-0.6.0/textwiz/data/memory_estimator/bloom-7.1B/float16.json
+drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-04-16 11:38:48.740263 textwiz-0.6.0/textwiz/data/memory_estimator/code-llama-13B/
+-rw-r--r--   0 cyrilvallez   (501) staff       (20)     2338 2023-10-03 06:55:40.000000 textwiz-0.6.0/textwiz/data/memory_estimator/code-llama-13B/bfloat16.json
+drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-04-16 11:38:48.741361 textwiz-0.6.0/textwiz/data/memory_estimator/code-llama-13B-instruct/
+-rw-r--r--   0 cyrilvallez   (501) staff       (20)     2328 2023-10-03 06:55:40.000000 textwiz-0.6.0/textwiz/data/memory_estimator/code-llama-13B-instruct/bfloat16.json
+drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-04-16 11:38:48.742417 textwiz-0.6.0/textwiz/data/memory_estimator/code-llama-13B-python/
+-rw-r--r--   0 cyrilvallez   (501) staff       (20)     2335 2023-10-03 06:55:40.000000 textwiz-0.6.0/textwiz/data/memory_estimator/code-llama-13B-python/bfloat16.json
+drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-04-16 11:38:48.743334 textwiz-0.6.0/textwiz/data/memory_estimator/code-llama-34B/
+-rw-r--r--   0 cyrilvallez   (501) staff       (20)     2365 2023-10-03 06:55:40.000000 textwiz-0.6.0/textwiz/data/memory_estimator/code-llama-34B/bfloat16.json
+drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-04-16 11:38:48.744231 textwiz-0.6.0/textwiz/data/memory_estimator/code-llama-34B-instruct/
+-rw-r--r--   0 cyrilvallez   (501) staff       (20)     2364 2023-10-03 06:55:38.000000 textwiz-0.6.0/textwiz/data/memory_estimator/code-llama-34B-instruct/bfloat16.json
+drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-04-16 11:38:48.745050 textwiz-0.6.0/textwiz/data/memory_estimator/code-llama-34B-python/
+-rw-r--r--   0 cyrilvallez   (501) staff       (20)     2365 2023-10-03 06:55:40.000000 textwiz-0.6.0/textwiz/data/memory_estimator/code-llama-34B-python/bfloat16.json
+drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-04-16 11:38:48.746562 textwiz-0.6.0/textwiz/data/memory_estimator/code-llama-7B/
+-rw-r--r--   0 cyrilvallez   (501) staff       (20)     2346 2023-10-03 06:55:39.000000 textwiz-0.6.0/textwiz/data/memory_estimator/code-llama-7B/bfloat16.json
+drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-04-16 11:38:48.748094 textwiz-0.6.0/textwiz/data/memory_estimator/code-llama-7B-instruct/
+-rw-r--r--   0 cyrilvallez   (501) staff       (20)     2328 2023-10-03 06:55:39.000000 textwiz-0.6.0/textwiz/data/memory_estimator/code-llama-7B-instruct/bfloat16.json
+drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-04-16 11:38:48.749273 textwiz-0.6.0/textwiz/data/memory_estimator/code-llama-7B-python/
+-rw-r--r--   0 cyrilvallez   (501) staff       (20)     2346 2023-10-03 06:55:39.000000 textwiz-0.6.0/textwiz/data/memory_estimator/code-llama-7B-python/bfloat16.json
+drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-04-16 11:38:48.750085 textwiz-0.6.0/textwiz/data/memory_estimator/codegen-16B/
+-rw-r--r--   0 cyrilvallez   (501) staff       (20)     2312 2023-10-03 06:55:39.000000 textwiz-0.6.0/textwiz/data/memory_estimator/codegen-16B/float16.json
+drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-04-16 11:38:48.750817 textwiz-0.6.0/textwiz/data/memory_estimator/codegen-2B/
+-rw-r--r--   0 cyrilvallez   (501) staff       (20)     2342 2023-10-03 06:55:38.000000 textwiz-0.6.0/textwiz/data/memory_estimator/codegen-2B/float16.json
+drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-04-16 11:38:48.751686 textwiz-0.6.0/textwiz/data/memory_estimator/codegen-350M/
+-rw-r--r--   0 cyrilvallez   (501) staff       (20)     2374 2023-10-03 06:55:37.000000 textwiz-0.6.0/textwiz/data/memory_estimator/codegen-350M/float16.json
+drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-04-16 11:38:48.752415 textwiz-0.6.0/textwiz/data/memory_estimator/codegen-6B/
+-rw-r--r--   0 cyrilvallez   (501) staff       (20)     2337 2023-10-03 06:55:38.000000 textwiz-0.6.0/textwiz/data/memory_estimator/codegen-6B/float16.json
+drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-04-16 11:38:48.753306 textwiz-0.6.0/textwiz/data/memory_estimator/codegen2-16B/
+-rw-r--r--   0 cyrilvallez   (501) staff       (20)     1153 2023-10-03 06:55:39.000000 textwiz-0.6.0/textwiz/data/memory_estimator/codegen2-16B/float16.json
+drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-04-16 11:38:48.754016 textwiz-0.6.0/textwiz/data/memory_estimator/codegen2-1B/
+-rw-r--r--   0 cyrilvallez   (501) staff       (20)     1170 2023-10-03 06:55:37.000000 textwiz-0.6.0/textwiz/data/memory_estimator/codegen2-1B/float16.json
+drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-04-16 11:38:48.754751 textwiz-0.6.0/textwiz/data/memory_estimator/codegen2-3.7B/
+-rw-r--r--   0 cyrilvallez   (501) staff       (20)     1164 2023-10-03 06:55:37.000000 textwiz-0.6.0/textwiz/data/memory_estimator/codegen2-3.7B/float16.json
+drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-04-16 11:38:48.755610 textwiz-0.6.0/textwiz/data/memory_estimator/codegen2-7B/
+-rw-r--r--   0 cyrilvallez   (501) staff       (20)     1155 2023-10-03 06:55:39.000000 textwiz-0.6.0/textwiz/data/memory_estimator/codegen2-7B/float16.json
+drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-04-16 11:38:48.756334 textwiz-0.6.0/textwiz/data/memory_estimator/codegen25-7B/
+-rw-r--r--   0 cyrilvallez   (501) staff       (20)     2332 2023-10-03 06:55:39.000000 textwiz-0.6.0/textwiz/data/memory_estimator/codegen25-7B/float16.json
+drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-04-16 11:38:48.757014 textwiz-0.6.0/textwiz/data/memory_estimator/codegen25-7B-instruct/
+-rw-r--r--   0 cyrilvallez   (501) staff       (20)     2330 2023-10-03 06:55:38.000000 textwiz-0.6.0/textwiz/data/memory_estimator/codegen25-7B-instruct/float16.json
+drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-04-16 11:38:48.757808 textwiz-0.6.0/textwiz/data/memory_estimator/dialo-gpt-large/
+-rw-r--r--   0 cyrilvallez   (501) staff       (20)     1163 2023-10-03 06:55:37.000000 textwiz-0.6.0/textwiz/data/memory_estimator/dialo-gpt-large/float32.json
+drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-04-16 11:38:48.758560 textwiz-0.6.0/textwiz/data/memory_estimator/dialo-gpt-medium/
+-rw-r--r--   0 cyrilvallez   (501) staff       (20)     1178 2023-10-03 06:55:37.000000 textwiz-0.6.0/textwiz/data/memory_estimator/dialo-gpt-medium/float32.json
+drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-04-16 11:38:48.759412 textwiz-0.6.0/textwiz/data/memory_estimator/dialo-gpt-small/
+-rw-r--r--   0 cyrilvallez   (501) staff       (20)     1189 2023-10-03 06:55:37.000000 textwiz-0.6.0/textwiz/data/memory_estimator/dialo-gpt-small/float32.json
+drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-04-16 11:38:48.760187 textwiz-0.6.0/textwiz/data/memory_estimator/gpt-j-6B/
+-rw-r--r--   0 cyrilvallez   (501) staff       (20)     2333 2023-10-03 06:55:39.000000 textwiz-0.6.0/textwiz/data/memory_estimator/gpt-j-6B/float32.json
+drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-04-16 11:38:48.760828 textwiz-0.6.0/textwiz/data/memory_estimator/gpt-neo-1.3B/
+-rw-r--r--   0 cyrilvallez   (501) staff       (20)     2342 2023-10-03 06:55:39.000000 textwiz-0.6.0/textwiz/data/memory_estimator/gpt-neo-1.3B/float32.json
+drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-04-16 11:38:48.761541 textwiz-0.6.0/textwiz/data/memory_estimator/gpt-neo-125M/
+-rw-r--r--   0 cyrilvallez   (501) staff       (20)     2384 2023-10-03 06:55:37.000000 textwiz-0.6.0/textwiz/data/memory_estimator/gpt-neo-125M/float32.json
+drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-04-16 11:38:48.762227 textwiz-0.6.0/textwiz/data/memory_estimator/gpt-neo-2.7B/
+-rw-r--r--   0 cyrilvallez   (501) staff       (20)     2333 2023-10-03 06:55:39.000000 textwiz-0.6.0/textwiz/data/memory_estimator/gpt-neo-2.7B/float32.json
+drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-04-16 11:38:48.762927 textwiz-0.6.0/textwiz/data/memory_estimator/gpt-neoX-20B/
+-rw-r--r--   0 cyrilvallez   (501) staff       (20)     2299 2023-10-03 06:55:40.000000 textwiz-0.6.0/textwiz/data/memory_estimator/gpt-neoX-20B/float16.json
+drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-04-16 11:38:48.763630 textwiz-0.6.0/textwiz/data/memory_estimator/gpt2-large/
+-rw-r--r--   0 cyrilvallez   (501) staff       (20)     1163 2023-10-03 06:55:38.000000 textwiz-0.6.0/textwiz/data/memory_estimator/gpt2-large/float32.json
+drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-04-16 11:38:48.764638 textwiz-0.6.0/textwiz/data/memory_estimator/gpt2-medium/
+-rw-r--r--   0 cyrilvallez   (501) staff       (20)     1175 2023-10-03 06:55:37.000000 textwiz-0.6.0/textwiz/data/memory_estimator/gpt2-medium/float32.json
+drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-04-16 11:38:48.765695 textwiz-0.6.0/textwiz/data/memory_estimator/gpt2-xl/
+-rw-r--r--   0 cyrilvallez   (501) staff       (20)     1158 2023-10-03 06:55:37.000000 textwiz-0.6.0/textwiz/data/memory_estimator/gpt2-xl/float32.json
+drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-04-16 11:38:48.766449 textwiz-0.6.0/textwiz/data/memory_estimator/llama2-13B/
+-rw-r--r--   0 cyrilvallez   (501) staff       (20)     2331 2023-10-03 06:55:39.000000 textwiz-0.6.0/textwiz/data/memory_estimator/llama2-13B/float16.json
+drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-04-16 11:38:48.767241 textwiz-0.6.0/textwiz/data/memory_estimator/llama2-13B-chat/
+-rw-r--r--   0 cyrilvallez   (501) staff       (20)     2328 2023-10-03 06:55:40.000000 textwiz-0.6.0/textwiz/data/memory_estimator/llama2-13B-chat/float16.json
+drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-04-16 11:38:48.767957 textwiz-0.6.0/textwiz/data/memory_estimator/llama2-70B/
+-rw-r--r--   0 cyrilvallez   (501) staff       (20)     2354 2023-10-03 06:55:38.000000 textwiz-0.6.0/textwiz/data/memory_estimator/llama2-70B/float16.json
+drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-04-16 11:38:48.768740 textwiz-0.6.0/textwiz/data/memory_estimator/llama2-70B-chat/
+-rw-r--r--   0 cyrilvallez   (501) staff       (20)     2350 2023-10-03 06:55:38.000000 textwiz-0.6.0/textwiz/data/memory_estimator/llama2-70B-chat/float16.json
+drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-04-16 11:38:48.769597 textwiz-0.6.0/textwiz/data/memory_estimator/llama2-7B/
+-rw-r--r--   0 cyrilvallez   (501) staff       (20)     2349 2023-10-03 06:55:39.000000 textwiz-0.6.0/textwiz/data/memory_estimator/llama2-7B/float16.json
+drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-04-16 11:38:48.770224 textwiz-0.6.0/textwiz/data/memory_estimator/llama2-7B-chat/
+-rw-r--r--   0 cyrilvallez   (501) staff       (20)     2344 2023-10-03 06:55:39.000000 textwiz-0.6.0/textwiz/data/memory_estimator/llama2-7B-chat/float16.json
+drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-04-16 11:38:48.770960 textwiz-0.6.0/textwiz/data/memory_estimator/opt-1.3B/
+-rw-r--r--   0 cyrilvallez   (501) staff       (20)     2375 2023-10-03 06:55:37.000000 textwiz-0.6.0/textwiz/data/memory_estimator/opt-1.3B/float16.json
+drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-04-16 11:38:48.771774 textwiz-0.6.0/textwiz/data/memory_estimator/opt-125M/
+-rw-r--r--   0 cyrilvallez   (501) staff       (20)     2400 2023-10-03 06:55:37.000000 textwiz-0.6.0/textwiz/data/memory_estimator/opt-125M/float16.json
+drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-04-16 11:38:48.772544 textwiz-0.6.0/textwiz/data/memory_estimator/opt-13B/
+-rw-r--r--   0 cyrilvallez   (501) staff       (20)     2330 2023-10-03 06:55:39.000000 textwiz-0.6.0/textwiz/data/memory_estimator/opt-13B/float16.json
+drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-04-16 11:38:48.773245 textwiz-0.6.0/textwiz/data/memory_estimator/opt-2.7B/
+-rw-r--r--   0 cyrilvallez   (501) staff       (20)     2339 2023-10-03 06:55:39.000000 textwiz-0.6.0/textwiz/data/memory_estimator/opt-2.7B/float16.json
+drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-04-16 11:38:48.773968 textwiz-0.6.0/textwiz/data/memory_estimator/opt-30B/
+-rw-r--r--   0 cyrilvallez   (501) staff       (20)     2306 2023-10-03 06:55:40.000000 textwiz-0.6.0/textwiz/data/memory_estimator/opt-30B/float16.json
+drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-04-16 11:38:48.775514 textwiz-0.6.0/textwiz/data/memory_estimator/opt-350M/
+-rw-r--r--   0 cyrilvallez   (501) staff       (20)     2389 2023-10-03 06:55:38.000000 textwiz-0.6.0/textwiz/data/memory_estimator/opt-350M/float16.json
+drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-04-16 11:38:48.776731 textwiz-0.6.0/textwiz/data/memory_estimator/opt-6.7B/
+-rw-r--r--   0 cyrilvallez   (501) staff       (20)     2341 2023-10-03 06:55:39.000000 textwiz-0.6.0/textwiz/data/memory_estimator/opt-6.7B/float16.json
+drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-04-16 11:38:48.777593 textwiz-0.6.0/textwiz/data/memory_estimator/opt-66B/
+-rw-r--r--   0 cyrilvallez   (501) staff       (20)     2286 2023-10-03 06:55:38.000000 textwiz-0.6.0/textwiz/data/memory_estimator/opt-66B/float16.json
+drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-04-16 11:38:48.778536 textwiz-0.6.0/textwiz/data/memory_estimator/stable-lm-3B/
+-rw-r--r--   0 cyrilvallez   (501) staff       (20)     2342 2023-10-03 06:55:37.000000 textwiz-0.6.0/textwiz/data/memory_estimator/stable-lm-3B/float16.json
+drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-04-16 11:38:48.779773 textwiz-0.6.0/textwiz/data/memory_estimator/stable-lm-7B/
+-rw-r--r--   0 cyrilvallez   (501) staff       (20)     2332 2023-10-03 06:55:37.000000 textwiz-0.6.0/textwiz/data/memory_estimator/stable-lm-7B/float16.json
+drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-04-16 11:38:48.781096 textwiz-0.6.0/textwiz/data/memory_estimator/star-chat-alpha/
+-rw-r--r--   0 cyrilvallez   (501) staff       (20)     2345 2023-10-03 06:55:38.000000 textwiz-0.6.0/textwiz/data/memory_estimator/star-chat-alpha/float16.json
+drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-04-16 11:38:48.782240 textwiz-0.6.0/textwiz/data/memory_estimator/star-chat-beta/
+-rw-r--r--   0 cyrilvallez   (501) staff       (20)     2345 2023-10-03 06:55:38.000000 textwiz-0.6.0/textwiz/data/memory_estimator/star-chat-beta/bfloat16.json
+drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-04-16 11:38:48.782960 textwiz-0.6.0/textwiz/data/memory_estimator/star-coder/
+-rw-r--r--   0 cyrilvallez   (501) staff       (20)     2357 2023-10-03 06:55:38.000000 textwiz-0.6.0/textwiz/data/memory_estimator/star-coder/bfloat16.json
+drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-04-16 11:38:48.783749 textwiz-0.6.0/textwiz/data/memory_estimator/star-coder-base/
+-rw-r--r--   0 cyrilvallez   (501) staff       (20)     2364 2023-10-03 06:55:38.000000 textwiz-0.6.0/textwiz/data/memory_estimator/star-coder-base/bfloat16.json
+drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-04-16 11:38:48.784484 textwiz-0.6.0/textwiz/data/memory_estimator/star-coder-plus/
+-rw-r--r--   0 cyrilvallez   (501) staff       (20)     2364 2023-10-03 06:55:38.000000 textwiz-0.6.0/textwiz/data/memory_estimator/star-coder-plus/bfloat16.json
+drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-04-16 11:38:48.785197 textwiz-0.6.0/textwiz/data/memory_estimator/vicuna-13B/
+-rw-r--r--   0 cyrilvallez   (501) staff       (20)     2329 2023-10-03 06:55:38.000000 textwiz-0.6.0/textwiz/data/memory_estimator/vicuna-13B/float16.json
+drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-04-16 11:38:48.785953 textwiz-0.6.0/textwiz/data/memory_estimator/vicuna-7B/
+-rw-r--r--   0 cyrilvallez   (501) staff       (20)     2343 2023-10-03 06:55:38.000000 textwiz-0.6.0/textwiz/data/memory_estimator/vicuna-7B/float16.json
+drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-04-16 11:38:48.789262 textwiz-0.6.0/textwiz/helpers/
+-rw-r--r--   0 cyrilvallez   (501) staff       (20)       33 2024-03-20 13:55:23.000000 textwiz-0.6.0/textwiz/helpers/__init__.py
+-rw-r--r--   0 cyrilvallez   (501) staff       (20)      111 2023-12-04 10:40:32.000000 textwiz-0.6.0/textwiz/helpers/constants.py
+-rw-r--r--   0 cyrilvallez   (501) staff       (20)     4495 2023-12-13 08:53:53.000000 textwiz-0.6.0/textwiz/helpers/utils.py
+-rw-r--r--   0 cyrilvallez   (501) staff       (20)     4183 2023-12-01 15:07:13.000000 textwiz-0.6.0/textwiz/helpers/warnings_suppressor.py
+-rw-r--r--   0 cyrilvallez   (501) staff       (20)    20322 2024-04-16 11:34:51.000000 textwiz-0.6.0/textwiz/loader.py
+drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-04-16 11:38:48.791299 textwiz-0.6.0/textwiz/models/
+-rw-r--r--   0 cyrilvallez   (501) staff       (20)       73 2024-03-20 14:06:42.000000 textwiz-0.6.0/textwiz/models/__init__.py
+-rw-r--r--   0 cyrilvallez   (501) staff       (20)     5870 2024-03-20 14:08:11.000000 textwiz-0.6.0/textwiz/models/base.py
+-rw-r--r--   0 cyrilvallez   (501) staff       (20)    43574 2024-04-16 08:55:12.000000 textwiz-0.6.0/textwiz/models/causal.py
+-rw-r--r--   0 cyrilvallez   (501) staff       (20)     4401 2024-04-16 08:55:59.000000 textwiz-0.6.0/textwiz/models/embedding.py
+drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-04-16 11:38:48.792284 textwiz-0.6.0/textwiz/parsers/
+-rw-r--r--   0 cyrilvallez   (501) staff       (20)       49 2024-03-20 13:48:21.000000 textwiz-0.6.0/textwiz/parsers/__init__.py
+-rw-r--r--   0 cyrilvallez   (501) staff       (20)     8049 2024-03-20 14:21:01.000000 textwiz-0.6.0/textwiz/parsers/code_parser.py
+drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-04-16 11:38:48.793364 textwiz-0.6.0/textwiz/stopping/
+-rw-r--r--   0 cyrilvallez   (501) staff       (20)       84 2024-03-20 13:47:13.000000 textwiz-0.6.0/textwiz/stopping/__init__.py
+-rw-r--r--   0 cyrilvallez   (501) staff       (20)    20387 2024-03-20 13:45:45.000000 textwiz-0.6.0/textwiz/stopping/stopping.py
+drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-04-16 11:38:48.794885 textwiz-0.6.0/textwiz/templates/
+-rw-r--r--   0 cyrilvallez   (501) staff       (20)      196 2024-03-20 13:45:08.000000 textwiz-0.6.0/textwiz/templates/__init__.py
+-rw-r--r--   0 cyrilvallez   (501) staff       (20)    24639 2024-04-15 11:54:27.000000 textwiz-0.6.0/textwiz/templates/conversation_template.py
+-rw-r--r--   0 cyrilvallez   (501) staff       (20)    18014 2024-04-15 11:54:40.000000 textwiz-0.6.0/textwiz/templates/prompt_template.py
+drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-04-16 11:38:48.796400 textwiz-0.6.0/textwiz/webapp/
+-rw-r--r--   0 cyrilvallez   (501) staff       (20)      213 2024-03-20 13:53:44.000000 textwiz-0.6.0/textwiz/webapp/__init__.py
+-rw-r--r--   0 cyrilvallez   (501) staff       (20)     2456 2024-03-27 09:45:20.000000 textwiz-0.6.0/textwiz/webapp/streamer.py
+-rw-r--r--   0 cyrilvallez   (501) staff       (20)    14513 2024-03-27 09:45:16.000000 textwiz-0.6.0/textwiz/webapp/web_interface.py
+drwxr-xr-x   0 cyrilvallez   (501) staff       (20)        0 2024-04-16 11:38:48.797582 textwiz-0.6.0/textwiz.egg-info/
+-rw-r--r--   0 cyrilvallez   (501) staff       (20)    18707 2024-04-16 11:38:48.000000 textwiz-0.6.0/textwiz.egg-info/PKG-INFO
+-rw-r--r--   0 cyrilvallez   (501) staff       (20)     4722 2024-04-16 11:38:48.000000 textwiz-0.6.0/textwiz.egg-info/SOURCES.txt
+-rw-r--r--   0 cyrilvallez   (501) staff       (20)        1 2024-04-16 11:38:48.000000 textwiz-0.6.0/textwiz.egg-info/dependency_links.txt
+-rw-r--r--   0 cyrilvallez   (501) staff       (20)      175 2024-04-16 11:38:48.000000 textwiz-0.6.0/textwiz.egg-info/requires.txt
+-rw-r--r--   0 cyrilvallez   (501) staff       (20)        8 2024-04-16 11:38:48.000000 textwiz-0.6.0/textwiz.egg-info/top_level.txt
```

### Comparing `textwiz-0.5.0/LICENSE` & `textwiz-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `textwiz-0.5.0/PKG-INFO` & `textwiz-0.6.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textwiz
-Version: 0.5.0
+Version: 0.6.0
 Summary: An even simpler way to use open-source LLMs.
 Author-email: Cyril Vallez <cyril.vallez@gmail.com>
 Maintainer-email: Cyril Vallez <cyril.vallez@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -221,14 +221,15 @@
 Requires-Dist: packaging
 Requires-Dist: torch>=2.2.0
 Requires-Dist: transformers>=4.37
 Requires-Dist: tokenizers>=0.13.3
 Requires-Dist: sentencepiece
 Requires-Dist: protobuf
 Requires-Dist: tiktoken
+Requires-Dist: gradio
 Requires-Dist: accelerate>=0.22.0
 Requires-Dist: optimum>=1.12.0
 Requires-Dist: bitsandbytes>=0.41.1
 
 # TextWiz
 
 TextWiz is a wrapper around Huggingface's `transformers` library, allowing extremely easy text generation with state-of-the-art LLMs. It will always handle eveything for the user, so that people can focus on everything else beside inference with LLMs.
```

### Comparing `textwiz-0.5.0/README.md` & `textwiz-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `textwiz-0.5.0/pyproject.toml` & `textwiz-0.6.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -27,15 +27,16 @@
     "packaging",
     "torch>=2.2.0",
     "transformers>=4.37",
     "tokenizers>=0.13.3",
     "sentencepiece",
     "protobuf",
     "tiktoken",
-    # maybe optional (used for quantization)
+    # maybe optional
+    "gradio",
     "accelerate>=0.22.0",
     "optimum>=1.12.0",
     "bitsandbytes>=0.41.1"
 ]
 dynamic = ["version"]
```

### Comparing `textwiz-0.5.0/textwiz/__init__.py` & `textwiz-0.6.0/textwiz/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 # Define easy entry points for most useful features
 from .models import HFCausalModel, HFEmbeddingModel
 from .loader import load_model, load_tokenizer, load_model_and_tokenizer, estimate_model_gpu_footprint
-from .templates import get_prompt_template, get_empty_conversation_template, get_conversation_from_yaml_template
+from .templates import GenericConversation, GenericPromptTemplate, get_prompt_template, get_empty_conversation_template, get_conversation_from_yaml_template
 from .stopping import StoppingType, create_stopping_criteria, post_process_sequences
 from .parsers import PythonParser
 from .webapp import TextContinuationStreamer
 # import it here so that the warnings are suppressed when doing `import textwiz`
 from .helpers import warnings_suppressor
 # also directly import some of the submodules for convenience and auto-complete
 from . import loader, templates
 
 
-__version__ = '0.5.0'
+__version__ = '0.6.0'
 
 
 def is_chat_model(model_name: str) -> bool:
     """Check if given model is chat-optimized.
 
     Parameters
     ----------
```

### Comparing `textwiz-0.5.0/textwiz/configs/__init__.py` & `textwiz-0.6.0/textwiz/configs/__init__.py`

 * *Files identical despite different names*

### Comparing `textwiz-0.5.0/textwiz/configs/causal/__init__.py` & `textwiz-0.6.0/textwiz/configs/causal/__init__.py`

 * *Files identical despite different names*

### Comparing `textwiz-0.5.0/textwiz/configs/causal/bloom.py` & `textwiz-0.6.0/textwiz/configs/causal/bloom.py`

 * *Files identical despite different names*

### Comparing `textwiz-0.5.0/textwiz/configs/causal/code_llama.py` & `textwiz-0.6.0/textwiz/configs/causal/code_llama.py`

 * *Files identical despite different names*

### Comparing `textwiz-0.5.0/textwiz/configs/causal/codegen.py` & `textwiz-0.6.0/textwiz/configs/causal/codegen.py`

 * *Files identical despite different names*

### Comparing `textwiz-0.5.0/textwiz/configs/causal/codegen2.py` & `textwiz-0.6.0/textwiz/configs/causal/codegen2.py`

 * *Files identical despite different names*

### Comparing `textwiz-0.5.0/textwiz/configs/causal/dialo_gpt.py` & `textwiz-0.6.0/textwiz/configs/causal/dialo_gpt.py`

 * *Files identical despite different names*

### Comparing `textwiz-0.5.0/textwiz/configs/causal/gpt_j_neo.py` & `textwiz-0.6.0/textwiz/configs/causal/gpt_j_neo.py`

 * *Files identical despite different names*

### Comparing `textwiz-0.5.0/textwiz/configs/causal/llama2.py` & `textwiz-0.6.0/textwiz/configs/causal/llama2.py`

 * *Files identical despite different names*

### Comparing `textwiz-0.5.0/textwiz/configs/causal/mistral.py` & `textwiz-0.6.0/textwiz/configs/embedding/mistral.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 import torch
 
 from .. import _infer_model_sizes
 
-# Mistral models
+
 MODELS_MAPPING = {
-    'mistral-7B': 'mistralai/Mistral-7B-v0.1',
-    'mistral-7B-instruct': 'mistralai/Mistral-7B-Instruct-v0.1',
+    'SFR-Embedding-Mistral': 'Salesforce/SFR-Embedding-Mistral'
 }
 MODELS_DTYPES = {model: torch.bfloat16 for model in MODELS_MAPPING.keys()}
-MODELS_PARAMS = _infer_model_sizes(MODELS_MAPPING)
+MODELS_PARAMS = {model: 7 for model in MODELS_MAPPING.keys()}
 MODELS_FAMILY = {model: 'mistral' for model in MODELS_MAPPING.keys()}
-MODELS_CONTEXT_SIZE = {model: 8192 for model in MODELS_MAPPING.keys()}
+
+# We want to stay inside the context sliding window for maximum embedding accuracy
+MODELS_CONTEXT_SIZE = {model: 4096 for model in MODELS_MAPPING.keys()}
 
 
-MODELS_VERSIONS = {model: {'transformers': '>=4.34.0', 'tokenizers': '>=0.14.0'} for model in MODELS_MAPPING.keys()}
+MODELS_VERSIONS = {model: {'transformers': '>=4.37.0', 'tokenizers': '>=0.14.0'} for model in MODELS_MAPPING.keys()}
 MODELS_ADDITIONAL_TOKENIZER_KWARGS = {model: {'use_fast': False} for model in MODELS_MAPPING.keys()}
```

### Comparing `textwiz-0.5.0/textwiz/configs/causal/opt.py` & `textwiz-0.6.0/textwiz/configs/causal/opt.py`

 * *Files identical despite different names*

### Comparing `textwiz-0.5.0/textwiz/configs/causal/star_coder.py` & `textwiz-0.6.0/textwiz/configs/causal/star_coder.py`

 * *Files identical despite different names*

### Comparing `textwiz-0.5.0/textwiz/configs/causal/vicuna.py` & `textwiz-0.6.0/textwiz/configs/causal/vicuna.py`

 * *Files identical despite different names*

### Comparing `textwiz-0.5.0/textwiz/configs/causal/zephyr.py` & `textwiz-0.6.0/textwiz/configs/causal/zephyr.py`

 * *Files identical despite different names*

### Comparing `textwiz-0.5.0/textwiz/configs/embedding/__init__.py` & `textwiz-0.6.0/textwiz/configs/embedding/__init__.py`

 * *Files identical despite different names*

### Comparing `textwiz-0.5.0/textwiz/data/memory_estimator/bloom-1.7B/float16.json` & `textwiz-0.6.0/textwiz/data/memory_estimator/bloom-1.7B/float16.json`

 * *Files identical despite different names*

### Comparing `textwiz-0.5.0/textwiz/data/memory_estimator/bloom-3B/float16.json` & `textwiz-0.6.0/textwiz/data/memory_estimator/bloom-3B/float16.json`

 * *Files identical despite different names*

### Comparing `textwiz-0.5.0/textwiz/data/memory_estimator/bloom-560M/float16.json` & `textwiz-0.6.0/textwiz/data/memory_estimator/bloom-560M/float16.json`

 * *Files identical despite different names*

### Comparing `textwiz-0.5.0/textwiz/data/memory_estimator/bloom-7.1B/float16.json` & `textwiz-0.6.0/textwiz/data/memory_estimator/bloom-7.1B/float16.json`

 * *Files identical despite different names*

### Comparing `textwiz-0.5.0/textwiz/data/memory_estimator/code-llama-13B/bfloat16.json` & `textwiz-0.6.0/textwiz/data/memory_estimator/code-llama-13B/bfloat16.json`

 * *Files identical despite different names*

### Comparing `textwiz-0.5.0/textwiz/data/memory_estimator/code-llama-13B-instruct/bfloat16.json` & `textwiz-0.6.0/textwiz/data/memory_estimator/code-llama-13B-instruct/bfloat16.json`

 * *Files identical despite different names*

### Comparing `textwiz-0.5.0/textwiz/data/memory_estimator/code-llama-13B-python/bfloat16.json` & `textwiz-0.6.0/textwiz/data/memory_estimator/code-llama-13B-python/bfloat16.json`

 * *Files identical despite different names*

### Comparing `textwiz-0.5.0/textwiz/data/memory_estimator/code-llama-34B/bfloat16.json` & `textwiz-0.6.0/textwiz/data/memory_estimator/code-llama-34B/bfloat16.json`

 * *Files identical despite different names*

### Comparing `textwiz-0.5.0/textwiz/data/memory_estimator/code-llama-34B-instruct/bfloat16.json` & `textwiz-0.6.0/textwiz/data/memory_estimator/code-llama-34B-instruct/bfloat16.json`

 * *Files identical despite different names*

### Comparing `textwiz-0.5.0/textwiz/data/memory_estimator/code-llama-34B-python/bfloat16.json` & `textwiz-0.6.0/textwiz/data/memory_estimator/code-llama-34B-python/bfloat16.json`

 * *Files identical despite different names*

### Comparing `textwiz-0.5.0/textwiz/data/memory_estimator/code-llama-7B/bfloat16.json` & `textwiz-0.6.0/textwiz/data/memory_estimator/code-llama-7B/bfloat16.json`

 * *Files identical despite different names*

### Comparing `textwiz-0.5.0/textwiz/data/memory_estimator/code-llama-7B-instruct/bfloat16.json` & `textwiz-0.6.0/textwiz/data/memory_estimator/code-llama-7B-instruct/bfloat16.json`

 * *Files identical despite different names*

### Comparing `textwiz-0.5.0/textwiz/data/memory_estimator/code-llama-7B-python/bfloat16.json` & `textwiz-0.6.0/textwiz/data/memory_estimator/code-llama-7B-python/bfloat16.json`

 * *Files identical despite different names*

### Comparing `textwiz-0.5.0/textwiz/data/memory_estimator/codegen-16B/float16.json` & `textwiz-0.6.0/textwiz/data/memory_estimator/codegen-16B/float16.json`

 * *Files identical despite different names*

### Comparing `textwiz-0.5.0/textwiz/data/memory_estimator/codegen-2B/float16.json` & `textwiz-0.6.0/textwiz/data/memory_estimator/codegen-2B/float16.json`

 * *Files identical despite different names*

### Comparing `textwiz-0.5.0/textwiz/data/memory_estimator/codegen-350M/float16.json` & `textwiz-0.6.0/textwiz/data/memory_estimator/codegen-350M/float16.json`

 * *Files identical despite different names*

### Comparing `textwiz-0.5.0/textwiz/data/memory_estimator/codegen-6B/float16.json` & `textwiz-0.6.0/textwiz/data/memory_estimator/codegen-6B/float16.json`

 * *Files identical despite different names*

### Comparing `textwiz-0.5.0/textwiz/data/memory_estimator/codegen2-16B/float16.json` & `textwiz-0.6.0/textwiz/data/memory_estimator/codegen2-16B/float16.json`

 * *Files identical despite different names*

### Comparing `textwiz-0.5.0/textwiz/data/memory_estimator/codegen2-1B/float16.json` & `textwiz-0.6.0/textwiz/data/memory_estimator/codegen2-1B/float16.json`

 * *Files identical despite different names*

### Comparing `textwiz-0.5.0/textwiz/data/memory_estimator/codegen2-3.7B/float16.json` & `textwiz-0.6.0/textwiz/data/memory_estimator/codegen2-3.7B/float16.json`

 * *Files identical despite different names*

### Comparing `textwiz-0.5.0/textwiz/data/memory_estimator/codegen2-7B/float16.json` & `textwiz-0.6.0/textwiz/data/memory_estimator/codegen2-7B/float16.json`

 * *Files identical despite different names*

### Comparing `textwiz-0.5.0/textwiz/data/memory_estimator/codegen25-7B/float16.json` & `textwiz-0.6.0/textwiz/data/memory_estimator/codegen25-7B/float16.json`

 * *Files identical despite different names*

### Comparing `textwiz-0.5.0/textwiz/data/memory_estimator/codegen25-7B-instruct/float16.json` & `textwiz-0.6.0/textwiz/data/memory_estimator/codegen25-7B-instruct/float16.json`

 * *Files identical despite different names*

### Comparing `textwiz-0.5.0/textwiz/data/memory_estimator/dialo-gpt-large/float32.json` & `textwiz-0.6.0/textwiz/data/memory_estimator/dialo-gpt-large/float32.json`

 * *Files identical despite different names*

### Comparing `textwiz-0.5.0/textwiz/data/memory_estimator/dialo-gpt-medium/float32.json` & `textwiz-0.6.0/textwiz/data/memory_estimator/dialo-gpt-medium/float32.json`

 * *Files identical despite different names*

### Comparing `textwiz-0.5.0/textwiz/data/memory_estimator/dialo-gpt-small/float32.json` & `textwiz-0.6.0/textwiz/data/memory_estimator/dialo-gpt-small/float32.json`

 * *Files identical despite different names*

### Comparing `textwiz-0.5.0/textwiz/data/memory_estimator/gpt-j-6B/float32.json` & `textwiz-0.6.0/textwiz/data/memory_estimator/gpt-j-6B/float32.json`

 * *Files identical despite different names*

### Comparing `textwiz-0.5.0/textwiz/data/memory_estimator/gpt-neo-1.3B/float32.json` & `textwiz-0.6.0/textwiz/data/memory_estimator/gpt-neo-1.3B/float32.json`

 * *Files identical despite different names*

### Comparing `textwiz-0.5.0/textwiz/data/memory_estimator/gpt-neo-125M/float32.json` & `textwiz-0.6.0/textwiz/data/memory_estimator/gpt-neo-125M/float32.json`

 * *Files identical despite different names*

### Comparing `textwiz-0.5.0/textwiz/data/memory_estimator/gpt-neo-2.7B/float32.json` & `textwiz-0.6.0/textwiz/data/memory_estimator/gpt-neo-2.7B/float32.json`

 * *Files identical despite different names*

### Comparing `textwiz-0.5.0/textwiz/data/memory_estimator/gpt-neoX-20B/float16.json` & `textwiz-0.6.0/textwiz/data/memory_estimator/gpt-neoX-20B/float16.json`

 * *Files identical despite different names*

### Comparing `textwiz-0.5.0/textwiz/data/memory_estimator/gpt2-large/float32.json` & `textwiz-0.6.0/textwiz/data/memory_estimator/gpt2-large/float32.json`

 * *Files identical despite different names*

### Comparing `textwiz-0.5.0/textwiz/data/memory_estimator/gpt2-medium/float32.json` & `textwiz-0.6.0/textwiz/data/memory_estimator/gpt2-medium/float32.json`

 * *Files identical despite different names*

### Comparing `textwiz-0.5.0/textwiz/data/memory_estimator/gpt2-xl/float32.json` & `textwiz-0.6.0/textwiz/data/memory_estimator/gpt2-xl/float32.json`

 * *Files identical despite different names*

### Comparing `textwiz-0.5.0/textwiz/data/memory_estimator/llama2-13B/float16.json` & `textwiz-0.6.0/textwiz/data/memory_estimator/llama2-13B/float16.json`

 * *Files identical despite different names*

### Comparing `textwiz-0.5.0/textwiz/data/memory_estimator/llama2-13B-chat/float16.json` & `textwiz-0.6.0/textwiz/data/memory_estimator/llama2-13B-chat/float16.json`

 * *Files identical despite different names*

### Comparing `textwiz-0.5.0/textwiz/data/memory_estimator/llama2-70B/float16.json` & `textwiz-0.6.0/textwiz/data/memory_estimator/llama2-70B/float16.json`

 * *Files identical despite different names*

### Comparing `textwiz-0.5.0/textwiz/data/memory_estimator/llama2-70B-chat/float16.json` & `textwiz-0.6.0/textwiz/data/memory_estimator/llama2-70B-chat/float16.json`

 * *Files identical despite different names*

### Comparing `textwiz-0.5.0/textwiz/data/memory_estimator/llama2-7B/float16.json` & `textwiz-0.6.0/textwiz/data/memory_estimator/llama2-7B/float16.json`

 * *Files identical despite different names*

### Comparing `textwiz-0.5.0/textwiz/data/memory_estimator/llama2-7B-chat/float16.json` & `textwiz-0.6.0/textwiz/data/memory_estimator/llama2-7B-chat/float16.json`

 * *Files identical despite different names*

### Comparing `textwiz-0.5.0/textwiz/data/memory_estimator/opt-1.3B/float16.json` & `textwiz-0.6.0/textwiz/data/memory_estimator/opt-1.3B/float16.json`

 * *Files identical despite different names*

### Comparing `textwiz-0.5.0/textwiz/data/memory_estimator/opt-125M/float16.json` & `textwiz-0.6.0/textwiz/data/memory_estimator/opt-125M/float16.json`

 * *Files identical despite different names*

### Comparing `textwiz-0.5.0/textwiz/data/memory_estimator/opt-13B/float16.json` & `textwiz-0.6.0/textwiz/data/memory_estimator/opt-13B/float16.json`

 * *Files identical despite different names*

### Comparing `textwiz-0.5.0/textwiz/data/memory_estimator/opt-2.7B/float16.json` & `textwiz-0.6.0/textwiz/data/memory_estimator/opt-2.7B/float16.json`

 * *Files identical despite different names*

### Comparing `textwiz-0.5.0/textwiz/data/memory_estimator/opt-30B/float16.json` & `textwiz-0.6.0/textwiz/data/memory_estimator/opt-30B/float16.json`

 * *Files identical despite different names*

### Comparing `textwiz-0.5.0/textwiz/data/memory_estimator/opt-350M/float16.json` & `textwiz-0.6.0/textwiz/data/memory_estimator/opt-350M/float16.json`

 * *Files identical despite different names*

### Comparing `textwiz-0.5.0/textwiz/data/memory_estimator/opt-6.7B/float16.json` & `textwiz-0.6.0/textwiz/data/memory_estimator/opt-6.7B/float16.json`

 * *Files identical despite different names*

### Comparing `textwiz-0.5.0/textwiz/data/memory_estimator/opt-66B/float16.json` & `textwiz-0.6.0/textwiz/data/memory_estimator/opt-66B/float16.json`

 * *Files identical despite different names*

### Comparing `textwiz-0.5.0/textwiz/data/memory_estimator/stable-lm-3B/float16.json` & `textwiz-0.6.0/textwiz/data/memory_estimator/stable-lm-3B/float16.json`

 * *Files identical despite different names*

### Comparing `textwiz-0.5.0/textwiz/data/memory_estimator/stable-lm-7B/float16.json` & `textwiz-0.6.0/textwiz/data/memory_estimator/stable-lm-7B/float16.json`

 * *Files identical despite different names*

### Comparing `textwiz-0.5.0/textwiz/data/memory_estimator/star-chat-alpha/float16.json` & `textwiz-0.6.0/textwiz/data/memory_estimator/star-chat-alpha/float16.json`

 * *Files identical despite different names*

### Comparing `textwiz-0.5.0/textwiz/data/memory_estimator/star-chat-beta/bfloat16.json` & `textwiz-0.6.0/textwiz/data/memory_estimator/star-chat-beta/bfloat16.json`

 * *Files identical despite different names*

### Comparing `textwiz-0.5.0/textwiz/data/memory_estimator/star-coder/bfloat16.json` & `textwiz-0.6.0/textwiz/data/memory_estimator/star-coder/bfloat16.json`

 * *Files identical despite different names*

### Comparing `textwiz-0.5.0/textwiz/data/memory_estimator/star-coder-base/bfloat16.json` & `textwiz-0.6.0/textwiz/data/memory_estimator/star-coder-base/bfloat16.json`

 * *Files identical despite different names*

### Comparing `textwiz-0.5.0/textwiz/data/memory_estimator/star-coder-plus/bfloat16.json` & `textwiz-0.6.0/textwiz/data/memory_estimator/star-coder-plus/bfloat16.json`

 * *Files identical despite different names*

### Comparing `textwiz-0.5.0/textwiz/data/memory_estimator/vicuna-13B/float16.json` & `textwiz-0.6.0/textwiz/data/memory_estimator/vicuna-13B/float16.json`

 * *Files identical despite different names*

### Comparing `textwiz-0.5.0/textwiz/data/memory_estimator/vicuna-7B/float16.json` & `textwiz-0.6.0/textwiz/data/memory_estimator/vicuna-7B/float16.json`

 * *Files identical despite different names*

### Comparing `textwiz-0.5.0/textwiz/helpers/utils.py` & `textwiz-0.6.0/textwiz/helpers/utils.py`

 * *Files identical despite different names*

### Comparing `textwiz-0.5.0/textwiz/helpers/warnings_suppressor.py` & `textwiz-0.6.0/textwiz/helpers/warnings_suppressor.py`

 * *Files identical despite different names*

### Comparing `textwiz-0.5.0/textwiz/loader.py` & `textwiz-0.6.0/textwiz/loader.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import warnings
 import re
 import math
 import importlib.metadata
+import difflib
 from packaging import version
 
 import torch
 from transformers import AutoModelForCausalLM, AutoModel, AutoTokenizer
 
 from .configs import (
     ALL_MODELS_MAPPING,
@@ -30,31 +31,50 @@
 # Mapping between purpose and transformer class
 BASE_MODEL_CLASS_MAPPING = {
     'causal': AutoModelForCausalLM,
     'embedding': AutoModel,
 }
 
 
+
+def check_model_name(model_name: str, available_models: list[str] | tuple[str] = ALLOWED_MODELS):
+    """Ensure that the `model_name` is valid, and raise an error trying to find closest model otherwise.
+
+    Parameters
+    ----------
+    model_name : str
+        The model name.
+    available_models : list[str] | tuple[str], optional
+        List of available models to check for closest match. By default check all models.
+    """
+
+    if model_name not in available_models:
+        closest_match = difflib.get_close_matches(model_name, available_models, n=1)
+        if len(closest_match) > 0:
+            raise ValueError(f'The model name you provided is invalid. Perhaps you meant "{closest_match[0]}"?')
+        else:
+            raise ValueError(f'The model name you provided is invalid and we could not find any close match.') 
+    else:
+        return
+
+
 def get_model_params(model_name: str) -> float:
     """Return the approximate number of params of the model, in billions.
 
     Parameters
     ----------
     model_name : str
         The name of the model.
 
     Returns
     -------
     float
         The number of parameters.
     """
-
-    if model_name not in ALLOWED_MODELS:
-        raise ValueError(f'The model name must be one of {*ALLOWED_MODELS,}.')
-    
+    check_model_name(model_name)
     return ALL_MODELS_PARAMS[model_name]
 
 
 def get_model_dtype(model_name: str) -> torch.dtype:
     """Return the default dtype used by the model.
 
     Parameters
@@ -63,18 +83,15 @@
         The name of the model.
 
     Returns
     -------
     torch.dtype
         The default dtype.
     """
-
-    if model_name not in ALLOWED_MODELS:
-        raise ValueError(f'The model name must be one of {*ALLOWED_MODELS,}.')
-    
+    check_model_name(model_name)
     return ALL_MODELS_DTYPES[model_name]
 
 
 def get_model_context_size(model_name: str) -> int:
     """Return the maximum context size used by the model.
 
     Parameters
@@ -83,18 +100,15 @@
         The name of the model.
 
     Returns
     -------
     int
         The context size.
     """
-
-    if model_name not in ALLOWED_MODELS:
-        raise ValueError(f'The model name must be one of {*ALLOWED_MODELS,}.')
-    
+    check_model_name(model_name)
     return ALL_MODELS_CONTEXT_SIZE[model_name]
 
 
 
 def check_versions(model_name: str):
     """Ensure that the versions are compatible with the current `model_name`, and raises an error if it is 
     not the case.
@@ -266,16 +280,16 @@
         is provided. By default 0.
 
     Returns
     -------
         The model.
     """
 
-    if model_name not in ALLOWED_MODELS:
-        raise ValueError(f'The model name must be one of {*ALLOWED_MODELS,}.')
+    # Check name
+    check_model_name(model_name)
     
     # Check package versions
     check_versions(model_name)
     
     # Set the dtype if not provided
     if dtype is None:
         dtype = ALL_MODELS_DTYPES[model_name]
@@ -404,16 +418,16 @@
         The model name.
 
     Returns
     -------
         The tokenizer.
     """
 
-    if model_name not in ALLOWED_MODELS:
-        raise ValueError(f'The model name must be one of {*ALLOWED_MODELS,}.') 
+    # Check name
+    check_model_name(model_name)
     
     # Check package versions
     check_versions(model_name)
     
     if model_name in ALL_MODELS_ADDITIONAL_TOKENIZER_KWARGS.keys():
         additional_kwargs = ALL_MODELS_ADDITIONAL_TOKENIZER_KWARGS[model_name]
     else:
```

### Comparing `textwiz-0.5.0/textwiz/models/base.py` & `textwiz-0.6.0/textwiz/models/base.py`

 * *Files identical despite different names*

### Comparing `textwiz-0.5.0/textwiz/models/causal.py` & `textwiz-0.6.0/textwiz/models/causal.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,16 +30,16 @@
     """Class encapsulating a HuggingFace model and its tokenizer to generate text. 
     """
 
     def __init__(self, model_name: str, quantization_8bits: bool = False, quantization_4bits: bool = False,
                  dtype: torch.dtype | None = None, max_fraction_gpu_0: float = 0.8, max_fraction_gpus: float = 0.8,
                  device_map: dict | str | None = None, gpu_rank: int = 0):
         
-        if model_name not in loader.ALLOWED_CAUSAL_MODELS:
-            raise ValueError(f'The model name must be one of {*loader.ALLOWED_CAUSAL_MODELS,}.')
+        # Check name against only causal models
+        loader.check_model_name(model_name, loader.ALLOWED_CAUSAL_MODELS)
         
         super().__init__(model_name, quantization_8bits, quantization_4bits, dtype, max_fraction_gpu_0,
                          max_fraction_gpus, device_map, gpu_rank)
 
         # Initialize the prompt template to use 
         self.prompt_template = get_prompt_template(self.model_name)
```

### Comparing `textwiz-0.5.0/textwiz/models/embedding.py` & `textwiz-0.6.0/textwiz/models/embedding.py`

 * *Files 5% similar despite different names*

```diff
@@ -10,16 +10,16 @@
     """Class encapsulating a HuggingFace model and its tokenizer to create text embedding. 
     """
 
     def __init__(self, model_name: str, quantization_8bits: bool = False, quantization_4bits: bool = False,
                  dtype: torch.dtype | None = None, max_fraction_gpu_0: float = 0.8, max_fraction_gpus: float = 0.8,
                  device_map: dict | str | None = None, gpu_rank: int = 0):
         
-        if model_name not in loader.ALLOWED_EMBEDDING_MODELS:
-            raise ValueError(f'The model name must be one of {*loader.ALLOWED_EMBEDDING_MODELS,}.')
+        # Check name against only embedding models
+        loader.check_model_name(model_name, loader.ALLOWED_EMBEDDING_MODELS)
         
         super().__init__(model_name, quantization_8bits, quantization_4bits, dtype, max_fraction_gpu_0,
                          max_fraction_gpus, device_map, gpu_rank)
 
     
     def last_token_pool(self, last_hidden_states: torch.Tensor, attention_mask: torch.Tensor) -> torch.Tensor:
         """Extract hidden state for the last token, given potential padding.
```

### Comparing `textwiz-0.5.0/textwiz/parsers/code_parser.py` & `textwiz-0.6.0/textwiz/parsers/code_parser.py`

 * *Files identical despite different names*

### Comparing `textwiz-0.5.0/textwiz/stopping/stopping.py` & `textwiz-0.6.0/textwiz/stopping/stopping.py`

 * *Files identical despite different names*

### Comparing `textwiz-0.5.0/textwiz/templates/conversation_template.py` & `textwiz-0.6.0/textwiz/templates/conversation_template.py`

 * *Files 3% similar despite different names*

```diff
@@ -60,23 +60,22 @@
         data = utils.load_yaml(path)
 
         if 'system_prompt' in data.keys():
             conv.set_system_prompt(data['system_prompt'])
         
         if 'few_shot_examples' in data.keys():
             few_shot_examples = data['few_shot_examples']
-            user_few_shot = ['']*len(few_shot_examples)
-            model_few_shot = ['']*len(few_shot_examples)
+            user_few_shot = []
+            model_few_shot = []
 
             for turn in few_shot_examples:
-                if sorted(list(turn.keys())) != ['index', 'model', 'user']:
+                if sorted(list(turn.keys())) != ['model', 'user']:
                     raise RuntimeError('The format of the yaml file is incorrect.')
-                k = turn['index']
-                user_few_shot[k] = turn['user']
-                model_few_shot[k] = turn['model']
+                user_few_shot.append(turn['user'])
+                model_few_shot.append(turn['model'])
 
             conv.set_few_shot_examples(user_few_shot, model_few_shot)
 
         return conv
 
 
     def __len__(self) -> int:
@@ -512,14 +511,100 @@
             else:
                 prompt += self.assistant_token + '\n'
 
         return prompt
     
 
 
+# reference: https://huggingface.co/Nexusflow/Starling-LM-7B-beta/tree/main
+class StarlingConversation(GenericConversation):
+
+    def __init__(self, eos_token: str):
+
+        super().__init__(eos_token)
+
+        # Override value
+        self.add_space_to_continuation_prompt = True
+
+        self.system_prompt = (
+            "Always assist with care, respect, and truth. Respond with utmost utility yet securely. Avoid harmful, "
+            "unethical, prejudiced, or negative content. Ensure replies promote fairness and positivity."
+        )
+
+        self.user_token = 'GPT4 Correct User:'
+        self.assistant_token = 'GPT4 Correct Assistant:'
+        self.end_turn = '<|end_of_turn|>'
+
+
+    def get_prompt(self) -> str:
+        """Format the prompt representing the conversation that we will feed to the tokenizer.
+        """
+
+        prompt = ''
+
+        for i, (user_message, model_response) in enumerate(self):
+
+            # System prompt embedded in first user interaction
+            if i == 0:
+                prompt += self.user_token + ' ' + self.system_prompt.strip() + ' ' + user_message.strip() + self.end_turn
+            else:
+                prompt += self.user_token + ' ' + user_message.strip() + self.end_turn
+
+            if model_response is not None:
+                prompt += self.assistant_token + ' ' + model_response.strip() + self.end_turn
+            else:
+                prompt += self.assistant_token
+
+        return prompt
+    
+
+
+# reference: https://huggingface.co/CohereForAI/c4ai-command-r-plus
+class CommandConversation(GenericConversation):
+
+    def __init__(self, eos_token: str):
+
+        super().__init__(eos_token)
+
+        # Override value
+        self.add_space_to_continuation_prompt = False
+
+        self.system_prompt = (
+            "You are Command-R, a brilliant, sophisticated, AI-assistant trained to assist human users by providing "
+            "thorough responses. You are trained by Cohere."
+        )
+
+        self.system_token = '<|SYSTEM_TOKEN|>'
+        self.user_token = '<|USER_TOKEN|>'
+        self.assistant_token = '<|CHATBOT_TOKEN|>'
+        self.start_turn = '<|START_OF_TURN_TOKEN|>'
+        self.end_turn = '<|END_OF_TURN_TOKEN|>'
+
+
+    def get_prompt(self) -> str:
+        """Format the prompt representing the conversation that we will feed to the tokenizer.
+        """
+
+        if self.system_prompt.strip() != '':
+            prompt = self.start_turn + self.system_token + self.system_prompt.strip() + self.end_turn
+        else:
+            prompt = ''
+
+        for user_message, model_response in self:
+
+            prompt += self.start_turn + self.user_token + user_message.strip() + self.end_turn
+
+            if model_response is not None:
+                prompt += self.start_turn + self.assistant_token + model_response.strip() + self.end_turn
+            else:
+                prompt += self.start_turn + self.assistant_token
+
+        return prompt
+
+
 # Mapping from model name to conversation class name
 CONVERSATION_MAPPING = {
     # StarChat
     'star-chat-alpha': StarChatConversation,
     'star-chat-beta': StarChatConversation,
 
     # Vicuna (1.3)
@@ -535,19 +620,28 @@
     'code-llama-7B-instruct': Llama2Conversation,
     'code-llama-13B-instruct': Llama2Conversation,
     'code-llama-34B-instruct': Llama2Conversation,
     # Special syntax for the 70B version
     'code-llama-70B-instruct': CodeLlama70BConversation,
 
     # Mistral
-    'mistral-7B-instruct': MistralConversation,
+    'mistral-7B-instruct-v1': MistralConversation,
+    'mistral-7B-instruct-v2': MistralConversation,
 
     # Zephyr
     'zephyr-7B-alpha': ZephyrConversation,
     'zephyr-7B-beta': ZephyrConversation,
+
+    # Starling
+    'starling-7B-alpha': StarlingConversation,
+    'starling-7B-beta': StarlingConversation,
+
+    # Command
+    'command-r': CommandConversation,
+    'command-r-plus': CommandConversation,
 }
 
 
 
 def get_empty_conversation_template(model_name: str) -> GenericConversation:
     """Return the conversation object corresponding to `model_name`.
```

### Comparing `textwiz-0.5.0/textwiz/templates/prompt_template.py` & `textwiz-0.6.0/textwiz/templates/prompt_template.py`

 * *Files 16% similar despite different names*

```diff
@@ -369,14 +369,69 @@
         formatted_prompt += self.user_token + '\n' + prompt.strip() + self.eos_token + '\n' + self.assistant_token + '\n'
 
         if model_context != '':
             formatted_prompt += model_context
 
         return formatted_prompt
 
+
+# reference: https://huggingface.co/HuggingFaceH4/zephyr-7b-beta
+class StarlingPromptTemplate(GenericPromptTemplate):
+
+    def __init__(self, mode: str = 'default'):
+
+        super().__init__(mode)
+        self.default_mode = 'chat'
+
+        self.user_token = 'GPT4 Correct User:'
+        self.assistant_token = 'GPT4 Correct Assistant:'
+        self.end_turn = '<|end_of_turn|>'
+
+
+    def format_chat(self, prompt: str, model_context: str = '', system_prompt: str = '') -> str:
+
+        # If we are not using system prompt, do not add the template formatting with empty prompt
+
+        formatted_prompt = self.user_token + ' ' + system_prompt.strip() + ' ' + prompt.strip() + self.end_turn + self.assistant_token
+
+        if model_context != '':
+            formatted_prompt += ' ' + model_context
+
+        return formatted_prompt
+    
+
+# reference: https://huggingface.co/CohereForAI/c4ai-command-r-plus
+class CommandPromptTemplate(GenericPromptTemplate):
+
+    def __init__(self, mode: str = 'default'):
+
+        super().__init__(mode)
+        self.default_mode = 'chat'
+
+        self.system_token = '<|SYSTEM_TOKEN|>'
+        self.user_token = '<|USER_TOKEN|>'
+        self.assistant_token = '<|CHATBOT_TOKEN|>'
+        self.start_turn = '<|START_OF_TURN_TOKEN|>'
+        self.end_turn = '<|END_OF_TURN_TOKEN|>'
+
+
+    def format_chat(self, prompt: str, model_context: str = '', system_prompt: str = '') -> str:
+
+        if system_prompt.strip() != '':
+            formatted_prompt = self.start_turn + self.system_token + system_prompt.strip() + self.end_turn
+        else:
+            formatted_prompt = ''
+
+        formatted_prompt += self.start_turn + self.user_token + prompt.strip() + self.end_turn + self.start_turn + self.assistant_token
+
+        if model_context != '':
+            formatted_prompt += model_context
+
+        return formatted_prompt
+
     
 
 # Mapping from model name to prompt class name
 PROMPT_MAPPING = {
     # DialoGPT
     'dialo-gpt-small': DialoGPTPromptTemplate,
     'dialo-gpt-medium': DialoGPTPromptTemplate,
@@ -412,19 +467,28 @@
     'code-llama-7B-instruct': Llama2ChatPromptTemplate,
     'code-llama-13B-instruct': Llama2ChatPromptTemplate,
     'code-llama-34B-instruct': Llama2ChatPromptTemplate,
     # Special template for the 70B version
     'code-llama-70B-instruct': CodeLlama70BInstructPromptTemplate,
 
     # Mistral
-    'mistral-7B-instruct': MistralPromptTemplate,
+    'mistral-7B-instruct-v1': MistralPromptTemplate,
+    'mistral-7B-instruct-v2': MistralPromptTemplate,
 
     # Zephyr
     'zephyr-7B-alpha': ZephyrPromptTemplate,
     'zephyr-7B-beta': ZephyrPromptTemplate,
+
+    # Starling
+    'starling-7B-alpha': StarlingPromptTemplate,
+    'starling-7B-beta': StarlingPromptTemplate,
+
+    # Command
+    'command-r': CommandPromptTemplate,
+    'command-r-plus': CommandPromptTemplate,
 }
 
 
 def get_prompt_template(model_name: str, mode: str = 'default') -> GenericPromptTemplate:
     """Return the prompt template class formating corresponding to `model_name`.
 
     Parameters
```

### Comparing `textwiz-0.5.0/textwiz/webapp/streamer.py` & `textwiz-0.6.0/textwiz/webapp/streamer.py`

 * *Files identical despite different names*

### Comparing `textwiz-0.5.0/textwiz/webapp/web_interface.py` & `textwiz-0.6.0/textwiz/webapp/web_interface.py`

 * *Files 9% similar despite different names*

```diff
@@ -288,61 +288,25 @@
         gr.Warning(f'You cannot retry generation on an empty conversation.')
         yield conversation, conversation.to_gradio_format()
         return
     if conversation.model_history_text[-1] is None:
         gr.Warning('You cannot retry generation on an empty last turn')
         yield conversation, conversation.to_gradio_format()
         return
-    
-    if not use_seed:
-        seed = None
 
     # Remove last turn
     prompt = conversation.user_history_text[-1]
     _ = conversation.user_history_text.pop(-1)
     _ = conversation.model_history_text.pop(-1)
 
-    # To show text as it is being generated
-    streamer = TextIteratorStreamer(model.tokenizer, skip_prompt=True, timeout=TIMEOUT, skip_special_tokens=True)
-
-    conv_copy = copy.deepcopy(conversation)
-    conv_copy.append_user_message(prompt)
-    
-    # We need to launch a new thread to get text from the streamer in real-time as it is being generated. We
-    # use an executor because it makes it easier to catch possible exceptions
-    with ThreadPoolExecutor(max_workers=1) as executor:
-        # This will update `conversation` in-place
-        future = executor.submit(model.generate_conversation, prompt, system_prompt=None, conv_history=conversation,
-                                 max_new_tokens=max_new_tokens, do_sample=do_sample, top_k=top_k, top_p=top_p,
-                                 temperature=temperature, seed=seed, truncate_if_conv_too_long=True, streamer=streamer,
-                                 **kwargs)
-        
-        # Get results from the streamer and yield it
-        try:
-            generated_text = ''
-            for new_text in streamer:
-                generated_text += new_text
-                # Update model answer (on a copy of the conversation) as it is being generated
-                conv_copy.model_history_text[-1] = generated_text
-                # The first output is an empty string to clear the input box, the second is the format output
-                # to use in a gradio chatbot component
-                yield conv_copy, conv_copy.to_gradio_format()
-
-        # If for some reason the queue (from the streamer) is still empty after timeout, we probably
-        # encountered an exception
-        except queue.Empty:
-            e = future.exception()
-            if e is not None:
-                raise gr.Error(f'The following error happened during generation: {repr(e)}')
-            else:
-                raise gr.Error(f'Generation timed out (no new tokens were generated after {TIMEOUT} s)')
-    
-    
-    # Update the chatbot with the real conversation (which may be slightly different due to postprocessing)
-    yield conversation, conversation.to_gradio_format()
+    # Yield from chat_generation, but remove first value
+    for _, conv, chatbot in chat_generation(model=model, conversation=conversation, prompt=prompt, max_new_tokens=max_new_tokens,
+                                            do_sample=do_sample, top_k=top_k, top_p=top_p, temperature=temperature,
+                                            use_seed=use_seed, seed=seed, **kwargs):
+        yield conv, chatbot
 
 
 
 def simple_authentication(credentials_file: str, username: str, password: str) -> bool:
     """Simple authentication method.
 
     Parameters
```

### Comparing `textwiz-0.5.0/textwiz.egg-info/PKG-INFO` & `textwiz-0.6.0/textwiz.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: textwiz
-Version: 0.5.0
+Version: 0.6.0
 Summary: An even simpler way to use open-source LLMs.
 Author-email: Cyril Vallez <cyril.vallez@gmail.com>
 Maintainer-email: Cyril Vallez <cyril.vallez@gmail.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
@@ -221,14 +221,15 @@
 Requires-Dist: packaging
 Requires-Dist: torch>=2.2.0
 Requires-Dist: transformers>=4.37
 Requires-Dist: tokenizers>=0.13.3
 Requires-Dist: sentencepiece
 Requires-Dist: protobuf
 Requires-Dist: tiktoken
+Requires-Dist: gradio
 Requires-Dist: accelerate>=0.22.0
 Requires-Dist: optimum>=1.12.0
 Requires-Dist: bitsandbytes>=0.41.1
 
 # TextWiz
 
 TextWiz is a wrapper around Huggingface's `transformers` library, allowing extremely easy text generation with state-of-the-art LLMs. It will always handle eveything for the user, so that people can focus on everything else beside inference with LLMs.
```

### Comparing `textwiz-0.5.0/textwiz.egg-info/SOURCES.txt` & `textwiz-0.6.0/textwiz.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -11,23 +11,25 @@
 textwiz.egg-info/top_level.txt
 textwiz/configs/__init__.py
 textwiz/configs/causal/__init__.py
 textwiz/configs/causal/bloom.py
 textwiz/configs/causal/code_llama.py
 textwiz/configs/causal/codegen.py
 textwiz/configs/causal/codegen2.py
+textwiz/configs/causal/command.py
 textwiz/configs/causal/dialo_gpt.py
 textwiz/configs/causal/gpt2.py
 textwiz/configs/causal/gpt_j_neo.py
 textwiz/configs/causal/llama2.py
 textwiz/configs/causal/mistral.py
 textwiz/configs/causal/opt.py
 textwiz/configs/causal/stable_lm.py
 textwiz/configs/causal/star_chat.py
 textwiz/configs/causal/star_coder.py
+textwiz/configs/causal/starling.py
 textwiz/configs/causal/vicuna.py
 textwiz/configs/causal/zephyr.py
 textwiz/configs/embedding/__init__.py
 textwiz/configs/embedding/mistral.py
 textwiz/data/memory_estimator/bloom-1.7B/float16.json
 textwiz/data/memory_estimator/bloom-3B/float16.json
 textwiz/data/memory_estimator/bloom-560M/float16.json
```

