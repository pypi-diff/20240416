# Comparing `tmp/curated-transformers-2.0.0.dev2.tar.gz` & `tmp/curated-transformers-2.0.0.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "curated-transformers-2.0.0.dev2.tar", last modified: Wed Apr 10 07:03:40 2024, max compression
+gzip compressed data, was "curated-transformers-2.0.0.dev3.tar", last modified: Fri Apr 12 13:37:36 2024, max compression
```

## Comparing `curated-transformers-2.0.0.dev2.tar` & `curated-transformers-2.0.0.dev3.tar`

### file list

```diff
@@ -1,241 +1,241 @@
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:40.817957 curated-transformers-2.0.0.dev2/
--rw-r--r--   0 vsts      (1001) docker     (127)     1088 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (127)      116 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (127)     5279 2024-04-10 07:03:40.817957 curated-transformers-2.0.0.dev2/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     4606 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:40.793956 curated-transformers-2.0.0.dev2/curated_transformers/
--rw-r--r--   0 vsts      (1001) docker     (127)      728 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      757 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/_compat.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:40.797956 curated-transformers-2.0.0.dev2/curated_transformers/generation/
--rw-r--r--   0 vsts      (1001) docker     (127)     1346 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/generation/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2685 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/generation/auto_generator.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4000 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/generation/config.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3787 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/generation/default_generator.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1962 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/generation/dolly_v2.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1200 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/generation/falcon.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4303 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/generation/generator.py
--rw-r--r--   0 vsts      (1001) docker     (127)      791 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/generation/generator_wrapper.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1756 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/generation/hf_hub.py
--rw-r--r--   0 vsts      (1001) docker     (127)      753 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/generation/llama.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6591 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/generation/logits.py
--rw-r--r--   0 vsts      (1001) docker     (127)      631 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/generation/mpt.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4827 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/generation/state.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2794 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/generation/stop_conditions.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2105 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/generation/string_generator.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:40.797956 curated-transformers-2.0.0.dev2/curated_transformers/layers/
--rw-r--r--   0 vsts      (1001) docker     (127)     1335 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/layers/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4055 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/layers/activations.py
--rw-r--r--   0 vsts      (1001) docker     (127)    35234 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/layers/attention.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1437 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/layers/cache.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10495 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/layers/embeddings.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3174 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/layers/feedforward.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1522 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/layers/normalization.py
--rw-r--r--   0 vsts      (1001) docker     (127)    16063 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/layers/transformer.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:40.797956 curated-transformers-2.0.0.dev2/curated_transformers/models/
--rw-r--r--   0 vsts      (1001) docker     (127)     1921 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/models/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:40.801956 curated-transformers-2.0.0.dev2/curated_transformers/models/albert/
--rw-r--r--   0 vsts      (1001) docker     (127)      105 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/models/albert/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4136 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/models/albert/_hf.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4593 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/models/albert/config.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4481 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/models/albert/encoder.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3650 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/models/albert/layer_group.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7766 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/models/auto_model.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:40.801956 curated-transformers-2.0.0.dev2/curated_transformers/models/bert/
--rw-r--r--   0 vsts      (1001) docker     (127)       64 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/models/bert/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3599 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/models/bert/_hf.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3582 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/models/bert/config.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5325 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/models/bert/encoder.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:40.801956 curated-transformers-2.0.0.dev2/curated_transformers/models/camembert/
--rw-r--r--   0 vsts      (1001) docker     (127)       38 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/models/camembert/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      643 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/models/camembert/_hf.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1159 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/models/camembert/encoder.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3729 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/models/config.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:40.801956 curated-transformers-2.0.0.dev2/curated_transformers/models/electra/
--rw-r--r--   0 vsts      (1001) docker     (127)       36 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/models/electra/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3881 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/models/electra/_hf.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1369 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/models/electra/encoder.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:40.801956 curated-transformers-2.0.0.dev2/curated_transformers/models/falcon/
--rw-r--r--   0 vsts      (1001) docker     (127)      147 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/models/falcon/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9443 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/models/falcon/_hf.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2770 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/models/falcon/causal_lm.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4097 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/models/falcon/config.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6930 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/models/falcon/decoder.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5677 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/models/falcon/layer.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:40.801956 curated-transformers-2.0.0.dev2/curated_transformers/models/gpt_neox/
--rw-r--r--   0 vsts      (1001) docker     (127)      109 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/models/gpt_neox/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3834 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/models/gpt_neox/_hf.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2737 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/models/gpt_neox/causal_lm.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3905 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/models/gpt_neox/config.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5763 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/models/gpt_neox/decoder.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:40.801956 curated-transformers-2.0.0.dev2/curated_transformers/models/hf_hub/
--rw-r--r--   0 vsts      (1001) docker     (127)       29 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/models/hf_hub/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12330 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/models/hf_hub/conversion.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10952 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/models/hf_hub/mixin.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:40.805956 curated-transformers-2.0.0.dev2/curated_transformers/models/llama/
--rw-r--r--   0 vsts      (1001) docker     (127)      103 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/models/llama/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4307 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/models/llama/_hf.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2819 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/models/llama/causal_lm.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3746 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/models/llama/config.py
--rw-r--r--   0 vsts      (1001) docker     (127)     6035 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/models/llama/decoder.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5468 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/models/module.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:40.805956 curated-transformers-2.0.0.dev2/curated_transformers/models/mpt/
--rw-r--r--   0 vsts      (1001) docker     (127)       97 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/models/mpt/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4331 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/models/mpt/_hf.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4081 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/models/mpt/causal_lm.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3553 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/models/mpt/config.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5505 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/models/mpt/decoder.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2629 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/models/output.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:40.805956 curated-transformers-2.0.0.dev2/curated_transformers/models/roberta/
--rw-r--r--   0 vsts      (1001) docker     (127)       70 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/models/roberta/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3789 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/models/roberta/_hf.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2104 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/models/roberta/config.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3406 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/models/roberta/embeddings.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5330 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/models/roberta/encoder.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4187 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/models/transformer.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:40.805956 curated-transformers-2.0.0.dev2/curated_transformers/models/xlm_roberta/
--rw-r--r--   0 vsts      (1001) docker     (127)       33 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/models/xlm_roberta/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      646 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/models/xlm_roberta/_hf.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1162 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/models/xlm_roberta/encoder.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:40.805956 curated-transformers-2.0.0.dev2/curated_transformers/quantization/
--rw-r--r--   0 vsts      (1001) docker     (127)      163 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/quantization/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:40.805956 curated-transformers-2.0.0.dev2/curated_transformers/quantization/bnb/
--rw-r--r--   0 vsts      (1001) docker     (127)      183 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/quantization/bnb/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2558 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/quantization/bnb/config.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5987 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/quantization/bnb/impl.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1118 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/quantization/helpers.py
--rw-r--r--   0 vsts      (1001) docker     (127)      676 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/quantization/quantizable.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:40.805956 curated-transformers-2.0.0.dev2/curated_transformers/repository/
--rw-r--r--   0 vsts      (1001) docker     (127)      517 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/repository/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1050 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/repository/_hf.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2105 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/repository/file.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4362 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/repository/fsspec.py
--rw-r--r--   0 vsts      (1001) docker     (127)    11957 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/repository/hf_hub.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9625 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/repository/repository.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1490 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/repository/transaction.py
--rw-r--r--   0 vsts      (1001) docker     (127)      605 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/semver.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:40.809956 curated-transformers-2.0.0.dev2/curated_transformers/tests/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      588 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/compat.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3349 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/conftest.py
--rw-r--r--   0 vsts      (1001) docker     (127)      133 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/enable_gpu.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:40.809956 curated-transformers-2.0.0.dev2/curated_transformers/tests/generation/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/generation/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      933 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/generation/test_auto_generator.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5058 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/generation/test_dolly_v2.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4514 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/generation/test_falcon.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5152 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/generation/test_generic.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5066 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/generation/test_logits.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2954 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/generation/test_stop.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:40.809956 curated-transformers-2.0.0.dev2/curated_transformers/tests/layers/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/layers/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     9040 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/layers/test_attention.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7236 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/layers/test_embeddings.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:40.809956 curated-transformers-2.0.0.dev2/curated_transformers/tests/models/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/models/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:40.809956 curated-transformers-2.0.0.dev2/curated_transformers/tests/models/albert/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/models/albert/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1821 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/models/albert/test_encoder.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:40.809956 curated-transformers-2.0.0.dev2/curated_transformers/tests/models/bert/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/models/bert/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1611 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/models/bert/test_encoder.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:40.809956 curated-transformers-2.0.0.dev2/curated_transformers/tests/models/camembert/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/models/camembert/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1651 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/models/camembert/test_encoder.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:40.809956 curated-transformers-2.0.0.dev2/curated_transformers/tests/models/electra/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/models/electra/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      722 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/models/electra/test_encoder.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:40.809956 curated-transformers-2.0.0.dev2/curated_transformers/tests/models/falcon/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/models/falcon/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     5424 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/models/falcon/test_decoder.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:40.809956 curated-transformers-2.0.0.dev2/curated_transformers/tests/models/gpt_neox/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/models/gpt_neox/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1961 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/models/gpt_neox/test_causal_lm.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2300 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/models/gpt_neox/test_decoder.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:40.809956 curated-transformers-2.0.0.dev2/curated_transformers/tests/models/llama/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/models/llama/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2267 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/models/llama/test_causal_lm.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2229 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/models/llama/test_decoder.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:40.813957 curated-transformers-2.0.0.dev2/curated_transformers/tests/models/mpt/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/models/mpt/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1976 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/models/mpt/test_causal_lm.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2395 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/models/mpt/test_decoder.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:40.813957 curated-transformers-2.0.0.dev2/curated_transformers/tests/models/roberta/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/models/roberta/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1635 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/models/roberta/test_encoder.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3081 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/models/test_auto_models.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4029 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/models/test_hf_hub.py
--rw-r--r--   0 vsts      (1001) docker     (127)    14286 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/models/util.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:40.813957 curated-transformers-2.0.0.dev2/curated_transformers/tests/models/xlm_roberta/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/models/xlm_roberta/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1639 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/models/xlm_roberta/test_encoder.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:40.813957 curated-transformers-2.0.0.dev2/curated_transformers/tests/quantization/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/quantization/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3736 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/quantization/test_generation.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:40.813957 curated-transformers-2.0.0.dev2/curated_transformers/tests/repository/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/repository/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2648 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/repository/test_hf_hub.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:40.813957 curated-transformers-2.0.0.dev2/curated_transformers/tests/tokenizers/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/tokenizers/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:40.813957 curated-transformers-2.0.0.dev2/curated_transformers/tests/tokenizers/legacy/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/tokenizers/legacy/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10775 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/tokenizers/legacy/test_bert_tokenizer.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10748 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/tokenizers/legacy/test_camembert_tokenizer.py
--rw-r--r--   0 vsts      (1001) docker     (127)      653 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/tokenizers/legacy/test_electra_tokenizer.py
--rw-r--r--   0 vsts      (1001) docker     (127)      734 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/tokenizers/legacy/test_llama_tokenizer.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10809 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/tokenizers/legacy/test_roberta_tokenizer.py
--rw-r--r--   0 vsts      (1001) docker     (127)    10557 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/tokenizers/legacy/test_xlmr_tokenizer.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4690 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/tokenizers/legacy/toy-merges.txt
--rw-r--r--   0 vsts      (1001) docker     (127)    14493 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/tokenizers/legacy/toy-vocab.json
--rw-r--r--   0 vsts      (1001) docker     (127)   253270 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/tokenizers/legacy/toy.model
--rw-r--r--   0 vsts      (1001) docker     (127)     4968 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/tokenizers/legacy/toy.wordpieces
--rw-r--r--   0 vsts      (1001) docker     (127)     1419 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/tokenizers/test_auto_tokenizer.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1748 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/tokenizers/test_chunks.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1930 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/tokenizers/test_hf_hub.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3856 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/tokenizers/test_tokenizer.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:40.813957 curated-transformers-2.0.0.dev2/curated_transformers/tests/tokenizers/toy-roberta/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/tokenizers/toy-roberta/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)    30593 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/tokenizers/toy-roberta/tokenizer.json
--rw-r--r--   0 vsts      (1001) docker     (127)     1939 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/tokenizers/util.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:40.813957 curated-transformers-2.0.0.dev2/curated_transformers/tests/util/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/util/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)      483 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tests/utils.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:40.817957 curated-transformers-2.0.0.dev2/curated_transformers/tokenizers/
--rw-r--r--   0 vsts      (1001) docker     (127)      370 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tokenizers/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2924 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tokenizers/_hf_compat.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4904 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tokenizers/auto_tokenizer.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2661 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tokenizers/chunks.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4980 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tokenizers/hf_hub.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:40.817957 curated-transformers-2.0.0.dev2/curated_transformers/tokenizers/legacy/
--rw-r--r--   0 vsts      (1001) docker     (127)      812 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tokenizers/legacy/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2325 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tokenizers/legacy/_fairseq.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2903 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tokenizers/legacy/bbpe_tokenizer.py
--rw-r--r--   0 vsts      (1001) docker     (127)    12006 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tokenizers/legacy/bert_tokenizer.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4508 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tokenizers/legacy/camembert_tokenizer.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7320 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tokenizers/legacy/legacy_tokenizer.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3011 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tokenizers/legacy/llama_tokenizer.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4255 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tokenizers/legacy/roberta_tokenizer.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2287 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tokenizers/legacy/sentencepiece_tokenizer.py
--rw-r--r--   0 vsts      (1001) docker     (127)     3230 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tokenizers/legacy/wordpiece_tokenizer.py
--rw-r--r--   0 vsts      (1001) docker     (127)     4017 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tokenizers/legacy/xlmr_tokenizer.py
--rw-r--r--   0 vsts      (1001) docker     (127)    13473 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tokenizers/tokenizer.py
--rw-r--r--   0 vsts      (1001) docker     (127)      221 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/tokenizers/util.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:40.817957 curated-transformers-2.0.0.dev2/curated_transformers/util/
--rw-r--r--   0 vsts      (1001) docker     (127)       54 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/util/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1445 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/util/profile.py
--rw-r--r--   0 vsts      (1001) docker     (127)     1208 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/util/pytorch.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:40.817957 curated-transformers-2.0.0.dev2/curated_transformers/util/serde/
--rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/util/serde/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (127)     2730 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/util/serde/checkpoint.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7302 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/util/serde/load.py
--rw-r--r--   0 vsts      (1001) docker     (127)     7231 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/curated_transformers/util/string.py
-drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-10 07:03:40.817957 curated-transformers-2.0.0.dev2/curated_transformers.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (127)     5279 2024-04-10 07:03:40.000000 curated-transformers-2.0.0.dev2/curated_transformers.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (127)     9297 2024-04-10 07:03:40.000000 curated-transformers-2.0.0.dev2/curated_transformers.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-10 07:03:40.000000 curated-transformers-2.0.0.dev2/curated_transformers.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (127)     1123 2024-04-10 07:03:40.000000 curated-transformers-2.0.0.dev2/curated_transformers.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (127)      159 2024-04-10 07:03:40.000000 curated-transformers-2.0.0.dev2/curated_transformers.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (127)       21 2024-04-10 07:03:40.000000 curated-transformers-2.0.0.dev2/curated_transformers.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-10 07:03:40.000000 curated-transformers-2.0.0.dev2/curated_transformers.egg-info/zip-safe
--rw-r--r--   0 vsts      (1001) docker     (127)      134 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (127)     1986 2024-04-10 07:03:40.821957 curated-transformers-2.0.0.dev2/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (127)      204 2024-04-10 07:03:28.000000 curated-transformers-2.0.0.dev2/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 13:37:36.607583 curated-transformers-2.0.0.dev3/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1088 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (127)      116 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (127)     5284 2024-04-12 13:37:36.607583 curated-transformers-2.0.0.dev3/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     4606 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 13:37:36.583582 curated-transformers-2.0.0.dev3/curated_transformers/
+-rw-r--r--   0 vsts      (1001) docker     (127)      728 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      757 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/_compat.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 13:37:36.587582 curated-transformers-2.0.0.dev3/curated_transformers/generation/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1346 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/generation/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2685 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/generation/auto_generator.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4000 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/generation/config.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3787 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/generation/default_generator.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1962 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/generation/dolly_v2.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1200 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/generation/falcon.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4303 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/generation/generator.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      791 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/generation/generator_wrapper.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1756 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/generation/hf_hub.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      753 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/generation/llama.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6591 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/generation/logits.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      631 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/generation/mpt.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4827 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/generation/state.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2794 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/generation/stop_conditions.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2105 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/generation/string_generator.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 13:37:36.587582 curated-transformers-2.0.0.dev3/curated_transformers/layers/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1335 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/layers/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4055 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/layers/activations.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    35234 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/layers/attention.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1437 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/layers/cache.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10495 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/layers/embeddings.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3174 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/layers/feedforward.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1522 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/layers/normalization.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    16063 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/layers/transformer.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 13:37:36.587582 curated-transformers-2.0.0.dev3/curated_transformers/models/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1921 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/models/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 13:37:36.587582 curated-transformers-2.0.0.dev3/curated_transformers/models/albert/
+-rw-r--r--   0 vsts      (1001) docker     (127)      105 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/models/albert/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4136 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/models/albert/_hf.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4593 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/models/albert/config.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4481 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/models/albert/encoder.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3650 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/models/albert/layer_group.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7766 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/models/auto_model.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 13:37:36.591583 curated-transformers-2.0.0.dev3/curated_transformers/models/bert/
+-rw-r--r--   0 vsts      (1001) docker     (127)       64 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/models/bert/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3599 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/models/bert/_hf.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3582 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/models/bert/config.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5325 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/models/bert/encoder.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 13:37:36.591583 curated-transformers-2.0.0.dev3/curated_transformers/models/camembert/
+-rw-r--r--   0 vsts      (1001) docker     (127)       38 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/models/camembert/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      643 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/models/camembert/_hf.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1159 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/models/camembert/encoder.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3729 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/models/config.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 13:37:36.591583 curated-transformers-2.0.0.dev3/curated_transformers/models/electra/
+-rw-r--r--   0 vsts      (1001) docker     (127)       36 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/models/electra/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3881 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/models/electra/_hf.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1369 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/models/electra/encoder.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 13:37:36.591583 curated-transformers-2.0.0.dev3/curated_transformers/models/falcon/
+-rw-r--r--   0 vsts      (1001) docker     (127)      147 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/models/falcon/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9443 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/models/falcon/_hf.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2770 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/models/falcon/causal_lm.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4097 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/models/falcon/config.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6930 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/models/falcon/decoder.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5677 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/models/falcon/layer.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 13:37:36.591583 curated-transformers-2.0.0.dev3/curated_transformers/models/gpt_neox/
+-rw-r--r--   0 vsts      (1001) docker     (127)      109 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/models/gpt_neox/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3834 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/models/gpt_neox/_hf.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2737 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/models/gpt_neox/causal_lm.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3905 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/models/gpt_neox/config.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5763 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/models/gpt_neox/decoder.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 13:37:36.591583 curated-transformers-2.0.0.dev3/curated_transformers/models/hf_hub/
+-rw-r--r--   0 vsts      (1001) docker     (127)       29 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/models/hf_hub/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12330 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/models/hf_hub/conversion.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10952 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/models/hf_hub/mixin.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 13:37:36.591583 curated-transformers-2.0.0.dev3/curated_transformers/models/llama/
+-rw-r--r--   0 vsts      (1001) docker     (127)      103 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/models/llama/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4307 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/models/llama/_hf.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2819 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/models/llama/causal_lm.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3746 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/models/llama/config.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     6035 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/models/llama/decoder.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5468 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/models/module.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 13:37:36.595583 curated-transformers-2.0.0.dev3/curated_transformers/models/mpt/
+-rw-r--r--   0 vsts      (1001) docker     (127)       97 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/models/mpt/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4331 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/models/mpt/_hf.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4081 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/models/mpt/causal_lm.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3553 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/models/mpt/config.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5505 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/models/mpt/decoder.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2629 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/models/output.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 13:37:36.595583 curated-transformers-2.0.0.dev3/curated_transformers/models/roberta/
+-rw-r--r--   0 vsts      (1001) docker     (127)       70 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/models/roberta/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3789 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/models/roberta/_hf.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2104 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/models/roberta/config.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3406 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/models/roberta/embeddings.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5330 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/models/roberta/encoder.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4187 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/models/transformer.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 13:37:36.595583 curated-transformers-2.0.0.dev3/curated_transformers/models/xlm_roberta/
+-rw-r--r--   0 vsts      (1001) docker     (127)       33 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/models/xlm_roberta/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      646 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/models/xlm_roberta/_hf.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1162 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/models/xlm_roberta/encoder.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 13:37:36.595583 curated-transformers-2.0.0.dev3/curated_transformers/quantization/
+-rw-r--r--   0 vsts      (1001) docker     (127)      163 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/quantization/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 13:37:36.595583 curated-transformers-2.0.0.dev3/curated_transformers/quantization/bnb/
+-rw-r--r--   0 vsts      (1001) docker     (127)      183 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/quantization/bnb/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2558 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/quantization/bnb/config.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5987 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/quantization/bnb/impl.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1118 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/quantization/helpers.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      676 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/quantization/quantizable.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 13:37:36.595583 curated-transformers-2.0.0.dev3/curated_transformers/repository/
+-rw-r--r--   0 vsts      (1001) docker     (127)      517 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/repository/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1050 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/repository/_hf.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2105 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/repository/file.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4362 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/repository/fsspec.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    11957 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/repository/hf_hub.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9625 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/repository/repository.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1490 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/repository/transaction.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      605 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/semver.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 13:37:36.595583 curated-transformers-2.0.0.dev3/curated_transformers/tests/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/tests/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      588 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/tests/compat.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3349 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/tests/conftest.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      133 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/tests/enable_gpu.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 13:37:36.599583 curated-transformers-2.0.0.dev3/curated_transformers/tests/generation/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/tests/generation/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      933 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/tests/generation/test_auto_generator.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5058 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/tests/generation/test_dolly_v2.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4514 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/tests/generation/test_falcon.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5152 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/tests/generation/test_generic.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5066 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/tests/generation/test_logits.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2954 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/tests/generation/test_stop.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 13:37:36.599583 curated-transformers-2.0.0.dev3/curated_transformers/tests/layers/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/tests/layers/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     9040 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/tests/layers/test_attention.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7236 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/tests/layers/test_embeddings.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 13:37:36.599583 curated-transformers-2.0.0.dev3/curated_transformers/tests/models/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/tests/models/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 13:37:36.599583 curated-transformers-2.0.0.dev3/curated_transformers/tests/models/albert/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/tests/models/albert/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1821 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/tests/models/albert/test_encoder.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 13:37:36.599583 curated-transformers-2.0.0.dev3/curated_transformers/tests/models/bert/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/tests/models/bert/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1611 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/tests/models/bert/test_encoder.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 13:37:36.599583 curated-transformers-2.0.0.dev3/curated_transformers/tests/models/camembert/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/tests/models/camembert/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1651 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/tests/models/camembert/test_encoder.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 13:37:36.599583 curated-transformers-2.0.0.dev3/curated_transformers/tests/models/electra/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/tests/models/electra/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      722 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/tests/models/electra/test_encoder.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 13:37:36.599583 curated-transformers-2.0.0.dev3/curated_transformers/tests/models/falcon/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/tests/models/falcon/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     5424 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/tests/models/falcon/test_decoder.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 13:37:36.599583 curated-transformers-2.0.0.dev3/curated_transformers/tests/models/gpt_neox/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/tests/models/gpt_neox/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1961 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/tests/models/gpt_neox/test_causal_lm.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2300 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/tests/models/gpt_neox/test_decoder.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 13:37:36.599583 curated-transformers-2.0.0.dev3/curated_transformers/tests/models/llama/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/tests/models/llama/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2267 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/tests/models/llama/test_causal_lm.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2229 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/tests/models/llama/test_decoder.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 13:37:36.599583 curated-transformers-2.0.0.dev3/curated_transformers/tests/models/mpt/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/tests/models/mpt/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1976 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/tests/models/mpt/test_causal_lm.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2395 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/tests/models/mpt/test_decoder.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 13:37:36.599583 curated-transformers-2.0.0.dev3/curated_transformers/tests/models/roberta/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/tests/models/roberta/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1635 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/tests/models/roberta/test_encoder.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3081 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/tests/models/test_auto_models.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4029 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/tests/models/test_hf_hub.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    14286 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/tests/models/util.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 13:37:36.603583 curated-transformers-2.0.0.dev3/curated_transformers/tests/models/xlm_roberta/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/tests/models/xlm_roberta/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1639 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/tests/models/xlm_roberta/test_encoder.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 13:37:36.603583 curated-transformers-2.0.0.dev3/curated_transformers/tests/quantization/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/tests/quantization/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3736 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/tests/quantization/test_generation.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 13:37:36.603583 curated-transformers-2.0.0.dev3/curated_transformers/tests/repository/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/tests/repository/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2648 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/tests/repository/test_hf_hub.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 13:37:36.603583 curated-transformers-2.0.0.dev3/curated_transformers/tests/tokenizers/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/tests/tokenizers/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 13:37:36.603583 curated-transformers-2.0.0.dev3/curated_transformers/tests/tokenizers/legacy/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/tests/tokenizers/legacy/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10775 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/tests/tokenizers/legacy/test_bert_tokenizer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10748 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/tests/tokenizers/legacy/test_camembert_tokenizer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      653 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/tests/tokenizers/legacy/test_electra_tokenizer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      734 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/tests/tokenizers/legacy/test_llama_tokenizer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10809 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/tests/tokenizers/legacy/test_roberta_tokenizer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    10557 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/tests/tokenizers/legacy/test_xlmr_tokenizer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4690 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/tests/tokenizers/legacy/toy-merges.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)    14493 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/tests/tokenizers/legacy/toy-vocab.json
+-rw-r--r--   0 vsts      (1001) docker     (127)   253270 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/tests/tokenizers/legacy/toy.model
+-rw-r--r--   0 vsts      (1001) docker     (127)     4968 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/tests/tokenizers/legacy/toy.wordpieces
+-rw-r--r--   0 vsts      (1001) docker     (127)     1419 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/tests/tokenizers/test_auto_tokenizer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1748 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/tests/tokenizers/test_chunks.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1930 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/tests/tokenizers/test_hf_hub.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3856 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/tests/tokenizers/test_tokenizer.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 13:37:36.603583 curated-transformers-2.0.0.dev3/curated_transformers/tests/tokenizers/toy-roberta/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/tests/tokenizers/toy-roberta/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    30593 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/tests/tokenizers/toy-roberta/tokenizer.json
+-rw-r--r--   0 vsts      (1001) docker     (127)     1939 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/tests/tokenizers/util.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 13:37:36.603583 curated-transformers-2.0.0.dev3/curated_transformers/tests/util/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/tests/util/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      483 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/tests/utils.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 13:37:36.607583 curated-transformers-2.0.0.dev3/curated_transformers/tokenizers/
+-rw-r--r--   0 vsts      (1001) docker     (127)      370 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/tokenizers/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2924 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/tokenizers/_hf_compat.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4904 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/tokenizers/auto_tokenizer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2661 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/tokenizers/chunks.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4980 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/tokenizers/hf_hub.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 13:37:36.607583 curated-transformers-2.0.0.dev3/curated_transformers/tokenizers/legacy/
+-rw-r--r--   0 vsts      (1001) docker     (127)      812 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/tokenizers/legacy/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2325 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/tokenizers/legacy/_fairseq.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2903 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/tokenizers/legacy/bbpe_tokenizer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    12006 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/tokenizers/legacy/bert_tokenizer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4508 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/tokenizers/legacy/camembert_tokenizer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7320 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/tokenizers/legacy/legacy_tokenizer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3011 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/tokenizers/legacy/llama_tokenizer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4255 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/tokenizers/legacy/roberta_tokenizer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2287 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/tokenizers/legacy/sentencepiece_tokenizer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     3230 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/tokenizers/legacy/wordpiece_tokenizer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     4017 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/tokenizers/legacy/xlmr_tokenizer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)    13473 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/tokenizers/tokenizer.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      221 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/tokenizers/util.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 13:37:36.607583 curated-transformers-2.0.0.dev3/curated_transformers/util/
+-rw-r--r--   0 vsts      (1001) docker     (127)       54 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/util/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1445 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/util/profile.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     1208 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/util/pytorch.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 13:37:36.607583 curated-transformers-2.0.0.dev3/curated_transformers/util/serde/
+-rw-r--r--   0 vsts      (1001) docker     (127)        0 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/util/serde/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     2730 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/util/serde/checkpoint.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7302 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/util/serde/load.py
+-rw-r--r--   0 vsts      (1001) docker     (127)     7231 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/curated_transformers/util/string.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-12 13:37:36.607583 curated-transformers-2.0.0.dev3/curated_transformers.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)     5284 2024-04-12 13:37:36.000000 curated-transformers-2.0.0.dev3/curated_transformers.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     9297 2024-04-12 13:37:36.000000 curated-transformers-2.0.0.dev3/curated_transformers.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-12 13:37:36.000000 curated-transformers-2.0.0.dev3/curated_transformers.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)     1123 2024-04-12 13:37:36.000000 curated-transformers-2.0.0.dev3/curated_transformers.egg-info/entry_points.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)      164 2024-04-12 13:37:36.000000 curated-transformers-2.0.0.dev3/curated_transformers.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       21 2024-04-12 13:37:36.000000 curated-transformers-2.0.0.dev3/curated_transformers.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-12 13:37:36.000000 curated-transformers-2.0.0.dev3/curated_transformers.egg-info/zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (127)      134 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/pyproject.toml
+-rw-r--r--   0 vsts      (1001) docker     (127)     1991 2024-04-12 13:37:36.611583 curated-transformers-2.0.0.dev3/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (127)      204 2024-04-12 13:37:27.000000 curated-transformers-2.0.0.dev3/setup.py
```

### Comparing `curated-transformers-2.0.0.dev2/LICENSE` & `curated-transformers-2.0.0.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/PKG-INFO` & `curated-transformers-2.0.0.dev3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: curated-transformers
-Version: 2.0.0.dev2
+Version: 2.0.0.dev3
 Summary: A PyTorch library of transformer models and components
 Home-page: https://github.com/explosion/curated-transformers
 Author: Explosion
 Author-email: contact@explosion.ai
 License: MIT
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: catalogue<2.1.0,>=2.0.4
-Requires-Dist: curated-tokenizers<1.0.0,>=0.9.1
+Requires-Dist: curated-tokenizers<3.0.0,>=2.0.0.dev0
 Requires-Dist: huggingface-hub>=0.14
 Requires-Dist: tokenizers>=0.13.3
 Requires-Dist: torch>=1.12.0
 Provides-Extra: quantization
 Requires-Dist: bitsandbytes>=0.40; extra == "quantization"
 Requires-Dist: scipy>=1.11; extra == "quantization"
```

### Comparing `curated-transformers-2.0.0.dev2/README.md` & `curated-transformers-2.0.0.dev3/README.md`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/__init__.py` & `curated-transformers-2.0.0.dev3/curated_transformers/__init__.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/_compat.py` & `curated-transformers-2.0.0.dev3/curated_transformers/_compat.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/generation/__init__.py` & `curated-transformers-2.0.0.dev3/curated_transformers/generation/__init__.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/generation/auto_generator.py` & `curated-transformers-2.0.0.dev3/curated_transformers/generation/auto_generator.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/generation/config.py` & `curated-transformers-2.0.0.dev3/curated_transformers/generation/config.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/generation/default_generator.py` & `curated-transformers-2.0.0.dev3/curated_transformers/generation/default_generator.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/generation/dolly_v2.py` & `curated-transformers-2.0.0.dev3/curated_transformers/generation/dolly_v2.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/generation/falcon.py` & `curated-transformers-2.0.0.dev3/curated_transformers/generation/falcon.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/generation/generator.py` & `curated-transformers-2.0.0.dev3/curated_transformers/generation/generator.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/generation/generator_wrapper.py` & `curated-transformers-2.0.0.dev3/curated_transformers/generation/generator_wrapper.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/generation/hf_hub.py` & `curated-transformers-2.0.0.dev3/curated_transformers/generation/hf_hub.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/generation/llama.py` & `curated-transformers-2.0.0.dev3/curated_transformers/generation/llama.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/generation/logits.py` & `curated-transformers-2.0.0.dev3/curated_transformers/generation/logits.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/generation/mpt.py` & `curated-transformers-2.0.0.dev3/curated_transformers/generation/mpt.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/generation/state.py` & `curated-transformers-2.0.0.dev3/curated_transformers/generation/state.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/generation/stop_conditions.py` & `curated-transformers-2.0.0.dev3/curated_transformers/generation/stop_conditions.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/generation/string_generator.py` & `curated-transformers-2.0.0.dev3/curated_transformers/generation/string_generator.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/layers/__init__.py` & `curated-transformers-2.0.0.dev3/curated_transformers/layers/__init__.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/layers/activations.py` & `curated-transformers-2.0.0.dev3/curated_transformers/layers/activations.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/layers/attention.py` & `curated-transformers-2.0.0.dev3/curated_transformers/layers/attention.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/layers/cache.py` & `curated-transformers-2.0.0.dev3/curated_transformers/layers/cache.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/layers/embeddings.py` & `curated-transformers-2.0.0.dev3/curated_transformers/layers/embeddings.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/layers/feedforward.py` & `curated-transformers-2.0.0.dev3/curated_transformers/layers/feedforward.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/layers/normalization.py` & `curated-transformers-2.0.0.dev3/curated_transformers/layers/normalization.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/layers/transformer.py` & `curated-transformers-2.0.0.dev3/curated_transformers/layers/transformer.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/models/__init__.py` & `curated-transformers-2.0.0.dev3/curated_transformers/models/__init__.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/models/albert/_hf.py` & `curated-transformers-2.0.0.dev3/curated_transformers/models/albert/_hf.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/models/albert/config.py` & `curated-transformers-2.0.0.dev3/curated_transformers/models/albert/config.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/models/albert/encoder.py` & `curated-transformers-2.0.0.dev3/curated_transformers/models/albert/encoder.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/models/albert/layer_group.py` & `curated-transformers-2.0.0.dev3/curated_transformers/models/albert/layer_group.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/models/auto_model.py` & `curated-transformers-2.0.0.dev3/curated_transformers/models/auto_model.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/models/bert/_hf.py` & `curated-transformers-2.0.0.dev3/curated_transformers/models/bert/_hf.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/models/bert/config.py` & `curated-transformers-2.0.0.dev3/curated_transformers/models/bert/config.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/models/bert/encoder.py` & `curated-transformers-2.0.0.dev3/curated_transformers/models/bert/encoder.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/models/camembert/_hf.py` & `curated-transformers-2.0.0.dev3/curated_transformers/models/camembert/_hf.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/models/camembert/encoder.py` & `curated-transformers-2.0.0.dev3/curated_transformers/models/camembert/encoder.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/models/config.py` & `curated-transformers-2.0.0.dev3/curated_transformers/models/config.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/models/electra/_hf.py` & `curated-transformers-2.0.0.dev3/curated_transformers/models/electra/_hf.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/models/electra/encoder.py` & `curated-transformers-2.0.0.dev3/curated_transformers/models/electra/encoder.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/models/falcon/_hf.py` & `curated-transformers-2.0.0.dev3/curated_transformers/models/falcon/_hf.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/models/falcon/causal_lm.py` & `curated-transformers-2.0.0.dev3/curated_transformers/models/falcon/causal_lm.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/models/falcon/config.py` & `curated-transformers-2.0.0.dev3/curated_transformers/models/falcon/config.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/models/falcon/decoder.py` & `curated-transformers-2.0.0.dev3/curated_transformers/models/falcon/decoder.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/models/falcon/layer.py` & `curated-transformers-2.0.0.dev3/curated_transformers/models/falcon/layer.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/models/gpt_neox/_hf.py` & `curated-transformers-2.0.0.dev3/curated_transformers/models/gpt_neox/_hf.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/models/gpt_neox/causal_lm.py` & `curated-transformers-2.0.0.dev3/curated_transformers/models/gpt_neox/causal_lm.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/models/gpt_neox/config.py` & `curated-transformers-2.0.0.dev3/curated_transformers/models/gpt_neox/config.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/models/gpt_neox/decoder.py` & `curated-transformers-2.0.0.dev3/curated_transformers/models/gpt_neox/decoder.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/models/hf_hub/conversion.py` & `curated-transformers-2.0.0.dev3/curated_transformers/models/hf_hub/conversion.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/models/hf_hub/mixin.py` & `curated-transformers-2.0.0.dev3/curated_transformers/models/hf_hub/mixin.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/models/llama/_hf.py` & `curated-transformers-2.0.0.dev3/curated_transformers/models/llama/_hf.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/models/llama/causal_lm.py` & `curated-transformers-2.0.0.dev3/curated_transformers/models/llama/causal_lm.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/models/llama/config.py` & `curated-transformers-2.0.0.dev3/curated_transformers/models/llama/config.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/models/llama/decoder.py` & `curated-transformers-2.0.0.dev3/curated_transformers/models/llama/decoder.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/models/module.py` & `curated-transformers-2.0.0.dev3/curated_transformers/models/module.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/models/mpt/_hf.py` & `curated-transformers-2.0.0.dev3/curated_transformers/models/mpt/_hf.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/models/mpt/causal_lm.py` & `curated-transformers-2.0.0.dev3/curated_transformers/models/mpt/causal_lm.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/models/mpt/config.py` & `curated-transformers-2.0.0.dev3/curated_transformers/models/mpt/config.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/models/mpt/decoder.py` & `curated-transformers-2.0.0.dev3/curated_transformers/models/mpt/decoder.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/models/output.py` & `curated-transformers-2.0.0.dev3/curated_transformers/models/output.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/models/roberta/_hf.py` & `curated-transformers-2.0.0.dev3/curated_transformers/models/roberta/_hf.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/models/roberta/config.py` & `curated-transformers-2.0.0.dev3/curated_transformers/models/roberta/config.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/models/roberta/embeddings.py` & `curated-transformers-2.0.0.dev3/curated_transformers/models/roberta/embeddings.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/models/roberta/encoder.py` & `curated-transformers-2.0.0.dev3/curated_transformers/models/roberta/encoder.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/models/transformer.py` & `curated-transformers-2.0.0.dev3/curated_transformers/models/transformer.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/models/xlm_roberta/_hf.py` & `curated-transformers-2.0.0.dev3/curated_transformers/models/xlm_roberta/_hf.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/models/xlm_roberta/encoder.py` & `curated-transformers-2.0.0.dev3/curated_transformers/models/xlm_roberta/encoder.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/quantization/bnb/config.py` & `curated-transformers-2.0.0.dev3/curated_transformers/quantization/bnb/config.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/quantization/bnb/impl.py` & `curated-transformers-2.0.0.dev3/curated_transformers/quantization/bnb/impl.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/quantization/helpers.py` & `curated-transformers-2.0.0.dev3/curated_transformers/quantization/helpers.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/quantization/quantizable.py` & `curated-transformers-2.0.0.dev3/curated_transformers/quantization/quantizable.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/repository/__init__.py` & `curated-transformers-2.0.0.dev3/curated_transformers/repository/__init__.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/repository/_hf.py` & `curated-transformers-2.0.0.dev3/curated_transformers/repository/_hf.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/repository/file.py` & `curated-transformers-2.0.0.dev3/curated_transformers/repository/file.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/repository/fsspec.py` & `curated-transformers-2.0.0.dev3/curated_transformers/repository/fsspec.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/repository/hf_hub.py` & `curated-transformers-2.0.0.dev3/curated_transformers/repository/hf_hub.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/repository/repository.py` & `curated-transformers-2.0.0.dev3/curated_transformers/repository/repository.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/repository/transaction.py` & `curated-transformers-2.0.0.dev3/curated_transformers/repository/transaction.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/semver.py` & `curated-transformers-2.0.0.dev3/curated_transformers/semver.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/tests/compat.py` & `curated-transformers-2.0.0.dev3/curated_transformers/tests/compat.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/tests/conftest.py` & `curated-transformers-2.0.0.dev3/curated_transformers/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/tests/generation/test_auto_generator.py` & `curated-transformers-2.0.0.dev3/curated_transformers/tests/generation/test_auto_generator.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/tests/generation/test_dolly_v2.py` & `curated-transformers-2.0.0.dev3/curated_transformers/tests/generation/test_dolly_v2.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/tests/generation/test_falcon.py` & `curated-transformers-2.0.0.dev3/curated_transformers/tests/generation/test_falcon.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/tests/generation/test_generic.py` & `curated-transformers-2.0.0.dev3/curated_transformers/tests/generation/test_generic.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/tests/generation/test_logits.py` & `curated-transformers-2.0.0.dev3/curated_transformers/tests/generation/test_logits.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/tests/generation/test_stop.py` & `curated-transformers-2.0.0.dev3/curated_transformers/tests/generation/test_stop.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/tests/layers/test_attention.py` & `curated-transformers-2.0.0.dev3/curated_transformers/tests/layers/test_attention.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/tests/layers/test_embeddings.py` & `curated-transformers-2.0.0.dev3/curated_transformers/tests/layers/test_embeddings.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/tests/models/albert/test_encoder.py` & `curated-transformers-2.0.0.dev3/curated_transformers/tests/models/albert/test_encoder.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/tests/models/bert/test_encoder.py` & `curated-transformers-2.0.0.dev3/curated_transformers/tests/models/bert/test_encoder.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/tests/models/camembert/test_encoder.py` & `curated-transformers-2.0.0.dev3/curated_transformers/tests/models/camembert/test_encoder.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/tests/models/electra/test_encoder.py` & `curated-transformers-2.0.0.dev3/curated_transformers/tests/models/electra/test_encoder.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/tests/models/falcon/test_decoder.py` & `curated-transformers-2.0.0.dev3/curated_transformers/tests/models/falcon/test_decoder.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/tests/models/gpt_neox/test_causal_lm.py` & `curated-transformers-2.0.0.dev3/curated_transformers/tests/models/gpt_neox/test_causal_lm.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/tests/models/gpt_neox/test_decoder.py` & `curated-transformers-2.0.0.dev3/curated_transformers/tests/models/gpt_neox/test_decoder.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/tests/models/llama/test_causal_lm.py` & `curated-transformers-2.0.0.dev3/curated_transformers/tests/models/llama/test_causal_lm.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/tests/models/llama/test_decoder.py` & `curated-transformers-2.0.0.dev3/curated_transformers/tests/models/llama/test_decoder.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/tests/models/mpt/test_causal_lm.py` & `curated-transformers-2.0.0.dev3/curated_transformers/tests/models/mpt/test_causal_lm.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/tests/models/mpt/test_decoder.py` & `curated-transformers-2.0.0.dev3/curated_transformers/tests/models/mpt/test_decoder.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/tests/models/roberta/test_encoder.py` & `curated-transformers-2.0.0.dev3/curated_transformers/tests/models/roberta/test_encoder.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/tests/models/test_auto_models.py` & `curated-transformers-2.0.0.dev3/curated_transformers/tests/models/test_auto_models.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/tests/models/test_hf_hub.py` & `curated-transformers-2.0.0.dev3/curated_transformers/tests/models/test_hf_hub.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/tests/models/util.py` & `curated-transformers-2.0.0.dev3/curated_transformers/tests/models/util.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/tests/models/xlm_roberta/test_encoder.py` & `curated-transformers-2.0.0.dev3/curated_transformers/tests/models/xlm_roberta/test_encoder.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/tests/quantization/test_generation.py` & `curated-transformers-2.0.0.dev3/curated_transformers/tests/quantization/test_generation.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/tests/repository/test_hf_hub.py` & `curated-transformers-2.0.0.dev3/curated_transformers/tests/repository/test_hf_hub.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/tests/tokenizers/legacy/test_bert_tokenizer.py` & `curated-transformers-2.0.0.dev3/curated_transformers/tests/tokenizers/legacy/test_bert_tokenizer.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/tests/tokenizers/legacy/test_camembert_tokenizer.py` & `curated-transformers-2.0.0.dev3/curated_transformers/tests/tokenizers/legacy/test_camembert_tokenizer.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/tests/tokenizers/legacy/test_electra_tokenizer.py` & `curated-transformers-2.0.0.dev3/curated_transformers/tests/tokenizers/legacy/test_electra_tokenizer.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/tests/tokenizers/legacy/test_llama_tokenizer.py` & `curated-transformers-2.0.0.dev3/curated_transformers/tests/tokenizers/legacy/test_llama_tokenizer.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/tests/tokenizers/legacy/test_roberta_tokenizer.py` & `curated-transformers-2.0.0.dev3/curated_transformers/tests/tokenizers/legacy/test_roberta_tokenizer.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/tests/tokenizers/legacy/test_xlmr_tokenizer.py` & `curated-transformers-2.0.0.dev3/curated_transformers/tests/tokenizers/legacy/test_xlmr_tokenizer.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/tests/tokenizers/legacy/toy-merges.txt` & `curated-transformers-2.0.0.dev3/curated_transformers/tests/tokenizers/legacy/toy-merges.txt`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/tests/tokenizers/legacy/toy-vocab.json` & `curated-transformers-2.0.0.dev3/curated_transformers/tests/tokenizers/legacy/toy-vocab.json`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/tests/tokenizers/legacy/toy.model` & `curated-transformers-2.0.0.dev3/curated_transformers/tests/tokenizers/legacy/toy.model`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/tests/tokenizers/legacy/toy.wordpieces` & `curated-transformers-2.0.0.dev3/curated_transformers/tests/tokenizers/legacy/toy.wordpieces`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/tests/tokenizers/test_auto_tokenizer.py` & `curated-transformers-2.0.0.dev3/curated_transformers/tests/tokenizers/test_auto_tokenizer.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/tests/tokenizers/test_chunks.py` & `curated-transformers-2.0.0.dev3/curated_transformers/tests/tokenizers/test_chunks.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/tests/tokenizers/test_hf_hub.py` & `curated-transformers-2.0.0.dev3/curated_transformers/tests/tokenizers/test_hf_hub.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/tests/tokenizers/test_tokenizer.py` & `curated-transformers-2.0.0.dev3/curated_transformers/tests/tokenizers/test_tokenizer.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/tests/tokenizers/toy-roberta/tokenizer.json` & `curated-transformers-2.0.0.dev3/curated_transformers/tests/tokenizers/toy-roberta/tokenizer.json`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/tests/tokenizers/util.py` & `curated-transformers-2.0.0.dev3/curated_transformers/tests/tokenizers/util.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/tokenizers/_hf_compat.py` & `curated-transformers-2.0.0.dev3/curated_transformers/tokenizers/_hf_compat.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/tokenizers/auto_tokenizer.py` & `curated-transformers-2.0.0.dev3/curated_transformers/tokenizers/auto_tokenizer.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/tokenizers/chunks.py` & `curated-transformers-2.0.0.dev3/curated_transformers/tokenizers/chunks.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/tokenizers/hf_hub.py` & `curated-transformers-2.0.0.dev3/curated_transformers/tokenizers/hf_hub.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/tokenizers/legacy/__init__.py` & `curated-transformers-2.0.0.dev3/curated_transformers/tokenizers/legacy/__init__.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/tokenizers/legacy/_fairseq.py` & `curated-transformers-2.0.0.dev3/curated_transformers/tokenizers/legacy/_fairseq.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/tokenizers/legacy/bbpe_tokenizer.py` & `curated-transformers-2.0.0.dev3/curated_transformers/tokenizers/legacy/bbpe_tokenizer.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/tokenizers/legacy/bert_tokenizer.py` & `curated-transformers-2.0.0.dev3/curated_transformers/tokenizers/legacy/bert_tokenizer.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/tokenizers/legacy/camembert_tokenizer.py` & `curated-transformers-2.0.0.dev3/curated_transformers/tokenizers/legacy/camembert_tokenizer.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/tokenizers/legacy/legacy_tokenizer.py` & `curated-transformers-2.0.0.dev3/curated_transformers/tokenizers/legacy/legacy_tokenizer.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/tokenizers/legacy/llama_tokenizer.py` & `curated-transformers-2.0.0.dev3/curated_transformers/tokenizers/legacy/llama_tokenizer.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/tokenizers/legacy/roberta_tokenizer.py` & `curated-transformers-2.0.0.dev3/curated_transformers/tokenizers/legacy/roberta_tokenizer.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/tokenizers/legacy/sentencepiece_tokenizer.py` & `curated-transformers-2.0.0.dev3/curated_transformers/tokenizers/legacy/sentencepiece_tokenizer.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/tokenizers/legacy/wordpiece_tokenizer.py` & `curated-transformers-2.0.0.dev3/curated_transformers/tokenizers/legacy/wordpiece_tokenizer.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/tokenizers/legacy/xlmr_tokenizer.py` & `curated-transformers-2.0.0.dev3/curated_transformers/tokenizers/legacy/xlmr_tokenizer.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/tokenizers/tokenizer.py` & `curated-transformers-2.0.0.dev3/curated_transformers/tokenizers/tokenizer.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/util/profile.py` & `curated-transformers-2.0.0.dev3/curated_transformers/util/profile.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/util/pytorch.py` & `curated-transformers-2.0.0.dev3/curated_transformers/util/pytorch.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/util/serde/checkpoint.py` & `curated-transformers-2.0.0.dev3/curated_transformers/util/serde/checkpoint.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/util/serde/load.py` & `curated-transformers-2.0.0.dev3/curated_transformers/util/serde/load.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers/util/string.py` & `curated-transformers-2.0.0.dev3/curated_transformers/util/string.py`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers.egg-info/PKG-INFO` & `curated-transformers-2.0.0.dev3/curated_transformers.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: curated-transformers
-Version: 2.0.0.dev2
+Version: 2.0.0.dev3
 Summary: A PyTorch library of transformer models and components
 Home-page: https://github.com/explosion/curated-transformers
 Author: Explosion
 Author-email: contact@explosion.ai
 License: MIT
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: catalogue<2.1.0,>=2.0.4
-Requires-Dist: curated-tokenizers<1.0.0,>=0.9.1
+Requires-Dist: curated-tokenizers<3.0.0,>=2.0.0.dev0
 Requires-Dist: huggingface-hub>=0.14
 Requires-Dist: tokenizers>=0.13.3
 Requires-Dist: torch>=1.12.0
 Provides-Extra: quantization
 Requires-Dist: bitsandbytes>=0.40; extra == "quantization"
 Requires-Dist: scipy>=1.11; extra == "quantization"
```

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers.egg-info/SOURCES.txt` & `curated-transformers-2.0.0.dev3/curated_transformers.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/curated_transformers.egg-info/entry_points.txt` & `curated-transformers-2.0.0.dev3/curated_transformers.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `curated-transformers-2.0.0.dev2/setup.cfg` & `curated-transformers-2.0.0.dev3/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [metadata]
-version = 2.0.0.dev2
+version = 2.0.0.dev3
 description = A PyTorch library of transformer models and components
 url = https://github.com/explosion/curated-transformers
 author = Explosion
 author_email = contact@explosion.ai
 license = MIT
 license_file = LICENSE
 long_description = file: README.md
 long_description_content_type = text/markdown
 
 [options]
 zip_safe = true
 include_package_data = true
-python_requires = >=3.8
+python_requires = >=3.9
 install_requires = 
 	catalogue>=2.0.4,<2.1.0
-	curated-tokenizers>=0.9.1,<1.0.0
+	curated-tokenizers>=2.0.0.dev0,<3.0.0
 	huggingface-hub>=0.14
 	tokenizers>=0.13.3
 	torch>=1.12.0
 
 [options.extras_require]
 quantization = 
 	bitsandbytes>=0.40
```

