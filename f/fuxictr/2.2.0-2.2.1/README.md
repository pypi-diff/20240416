# Comparing `tmp/fuxictr-2.2.0.tar.gz` & `tmp/fuxictr-2.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/fuxictr-2.2.0.tar", last modified: Fri Apr  5 14:22:28 2024, max compression
+gzip compressed data, was "dist/fuxictr-2.2.1.tar", last modified: Tue Apr 16 03:53:28 2024, max compression
```

## Comparing `fuxictr-2.2.0.tar` & `fuxictr-2.2.1.tar`

### file list

```diff
@@ -1,95 +1,95 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:22:28.000000 fuxictr-2.2.0/
--rw-r--r--   0 runner    (1001) docker     (127)    29940 2024-04-05 14:22:28.000000 fuxictr-2.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    27518 2024-04-05 14:22:22.000000 fuxictr-2.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:22:28.000000 fuxictr-2.2.0/fuxictr/
--rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-05 14:22:22.000000 fuxictr-2.2.0/fuxictr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6558 2024-04-05 14:22:22.000000 fuxictr-2.2.0/fuxictr/autotuner.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:22:28.000000 fuxictr-2.2.0/fuxictr/datasets/
--rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-05 14:22:22.000000 fuxictr-2.2.0/fuxictr/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-04-05 14:22:22.000000 fuxictr-2.2.0/fuxictr/datasets/avazu.py
--rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-04-05 14:22:22.000000 fuxictr-2.2.0/fuxictr/datasets/criteo.py
--rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-04-05 14:22:22.000000 fuxictr-2.2.0/fuxictr/datasets/kkbox.py
--rw-r--r--   0 runner    (1001) docker     (127)     5503 2024-04-05 14:22:22.000000 fuxictr-2.2.0/fuxictr/features.py
--rw-r--r--   0 runner    (1001) docker     (127)     4369 2024-04-05 14:22:22.000000 fuxictr-2.2.0/fuxictr/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:22:28.000000 fuxictr-2.2.0/fuxictr/preprocess/
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-05 14:22:22.000000 fuxictr-2.2.0/fuxictr/preprocess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5651 2024-04-05 14:22:22.000000 fuxictr-2.2.0/fuxictr/preprocess/build_dataset.py
--rw-r--r--   0 runner    (1001) docker     (127)    18478 2024-04-05 14:22:22.000000 fuxictr-2.2.0/fuxictr/preprocess/feature_processor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-04-05 14:22:22.000000 fuxictr-2.2.0/fuxictr/preprocess/normalizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     6703 2024-04-05 14:22:22.000000 fuxictr-2.2.0/fuxictr/preprocess/tokenizer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:22:28.000000 fuxictr-2.2.0/fuxictr/pytorch/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 14:22:22.000000 fuxictr-2.2.0/fuxictr/pytorch/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:22:28.000000 fuxictr-2.2.0/fuxictr/pytorch/dataloaders/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-05 14:22:22.000000 fuxictr-2.2.0/fuxictr/pytorch/dataloaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3710 2024-04-05 14:22:22.000000 fuxictr-2.2.0/fuxictr/pytorch/dataloaders/npz_block_dataloader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-04-05 14:22:22.000000 fuxictr-2.2.0/fuxictr/pytorch/dataloaders/npz_dataloader.py
--rw-r--r--   0 runner    (1001) docker     (127)     2698 2024-04-05 14:22:22.000000 fuxictr-2.2.0/fuxictr/pytorch/dataloaders/rank_dataloader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:22:28.000000 fuxictr-2.2.0/fuxictr/pytorch/layers/
--rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-05 14:22:22.000000 fuxictr-2.2.0/fuxictr/pytorch/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-04-05 14:22:22.000000 fuxictr-2.2.0/fuxictr/pytorch/layers/activations.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:22:28.000000 fuxictr-2.2.0/fuxictr/pytorch/layers/attentions/
--rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-05 14:22:22.000000 fuxictr-2.2.0/fuxictr/pytorch/layers/attentions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-04-05 14:22:22.000000 fuxictr-2.2.0/fuxictr/pytorch/layers/attentions/dot_product_attention.py
--rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-04-05 14:22:22.000000 fuxictr-2.2.0/fuxictr/pytorch/layers/attentions/squeeze_excitation.py
--rw-r--r--   0 runner    (1001) docker     (127)     5616 2024-04-05 14:22:22.000000 fuxictr-2.2.0/fuxictr/pytorch/layers/attentions/target_attention.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:22:28.000000 fuxictr-2.2.0/fuxictr/pytorch/layers/blocks/
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-05 14:22:22.000000 fuxictr-2.2.0/fuxictr/pytorch/layers/blocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-04-05 14:22:22.000000 fuxictr-2.2.0/fuxictr/pytorch/layers/blocks/factorization_machine.py
--rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-04-05 14:22:22.000000 fuxictr-2.2.0/fuxictr/pytorch/layers/blocks/logistic_regression.py
--rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-04-05 14:22:22.000000 fuxictr-2.2.0/fuxictr/pytorch/layers/blocks/mlp_block.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:22:28.000000 fuxictr-2.2.0/fuxictr/pytorch/layers/embeddings/
--rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-05 14:22:22.000000 fuxictr-2.2.0/fuxictr/pytorch/layers/embeddings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10164 2024-04-05 14:22:22.000000 fuxictr-2.2.0/fuxictr/pytorch/layers/embeddings/feature_embedding.py
--rw-r--r--   0 runner    (1001) docker     (127)     6213 2024-04-05 14:22:22.000000 fuxictr-2.2.0/fuxictr/pytorch/layers/embeddings/pretrained_embedding.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:22:28.000000 fuxictr-2.2.0/fuxictr/pytorch/layers/interactions/
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-05 14:22:22.000000 fuxictr-2.2.0/fuxictr/pytorch/layers/interactions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4734 2024-04-05 14:22:22.000000 fuxictr-2.2.0/fuxictr/pytorch/layers/interactions/bilinear_interaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-04-05 14:22:22.000000 fuxictr-2.2.0/fuxictr/pytorch/layers/interactions/compressed_interaction_net.py
--rw-r--r--   0 runner    (1001) docker     (127)     5228 2024-04-05 14:22:22.000000 fuxictr-2.2.0/fuxictr/pytorch/layers/interactions/cross_net.py
--rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-04-05 14:22:22.000000 fuxictr-2.2.0/fuxictr/pytorch/layers/interactions/holographic_interaction.py
--rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-04-05 14:22:22.000000 fuxictr-2.2.0/fuxictr/pytorch/layers/interactions/inner_product.py
--rw-r--r--   0 runner    (1001) docker     (127)     2780 2024-04-05 14:22:22.000000 fuxictr-2.2.0/fuxictr/pytorch/layers/interactions/interaction_machine.py
--rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-04-05 14:22:22.000000 fuxictr-2.2.0/fuxictr/pytorch/layers/pooling.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:22:28.000000 fuxictr-2.2.0/fuxictr/pytorch/models/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-05 14:22:22.000000 fuxictr-2.2.0/fuxictr/pytorch/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     6804 2024-04-05 14:22:22.000000 fuxictr-2.2.0/fuxictr/pytorch/models/multitask_model.py
--rw-r--r--   0 runner    (1001) docker     (127)    12848 2024-04-05 14:22:22.000000 fuxictr-2.2.0/fuxictr/pytorch/models/rank_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     4344 2024-04-05 14:22:22.000000 fuxictr-2.2.0/fuxictr/pytorch/torch_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:22:28.000000 fuxictr-2.2.0/fuxictr/tensorflow/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 14:22:22.000000 fuxictr-2.2.0/fuxictr/tensorflow/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:22:28.000000 fuxictr-2.2.0/fuxictr/tensorflow/dataloaders/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-05 14:22:22.000000 fuxictr-2.2.0/fuxictr/tensorflow/dataloaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-04-05 14:22:22.000000 fuxictr-2.2.0/fuxictr/tensorflow/dataloaders/tf_dataloader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:22:28.000000 fuxictr-2.2.0/fuxictr/tensorflow/layers/
--rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-05 14:22:22.000000 fuxictr-2.2.0/fuxictr/tensorflow/layers/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:22:28.000000 fuxictr-2.2.0/fuxictr/tensorflow/layers/blocks/
--rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-05 14:22:22.000000 fuxictr-2.2.0/fuxictr/tensorflow/layers/blocks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-04-05 14:22:22.000000 fuxictr-2.2.0/fuxictr/tensorflow/layers/blocks/factorization_machine.py
--rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-04-05 14:22:22.000000 fuxictr-2.2.0/fuxictr/tensorflow/layers/blocks/linear.py
--rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-04-05 14:22:22.000000 fuxictr-2.2.0/fuxictr/tensorflow/layers/blocks/logistic_regression.py
--rw-r--r--   0 runner    (1001) docker     (127)     3619 2024-04-05 14:22:22.000000 fuxictr-2.2.0/fuxictr/tensorflow/layers/blocks/mlp_block.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:22:28.000000 fuxictr-2.2.0/fuxictr/tensorflow/layers/embeddings/
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-05 14:22:22.000000 fuxictr-2.2.0/fuxictr/tensorflow/layers/embeddings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    11938 2024-04-05 14:22:22.000000 fuxictr-2.2.0/fuxictr/tensorflow/layers/embeddings/feature_embedding.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:22:28.000000 fuxictr-2.2.0/fuxictr/tensorflow/layers/interactions/
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-05 14:22:22.000000 fuxictr-2.2.0/fuxictr/tensorflow/layers/interactions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-04-05 14:22:22.000000 fuxictr-2.2.0/fuxictr/tensorflow/layers/interactions/cross_net.py
--rw-r--r--   0 runner    (1001) docker     (127)     2969 2024-04-05 14:22:22.000000 fuxictr-2.2.0/fuxictr/tensorflow/layers/interactions/inner_product.py
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-05 14:22:22.000000 fuxictr-2.2.0/fuxictr/tensorflow/layers/pooling.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:22:28.000000 fuxictr-2.2.0/fuxictr/tensorflow/models/
--rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-05 14:22:22.000000 fuxictr-2.2.0/fuxictr/tensorflow/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9279 2024-04-05 14:22:22.000000 fuxictr-2.2.0/fuxictr/tensorflow/models/rank_model.py
--rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-04-05 14:22:22.000000 fuxictr-2.2.0/fuxictr/tensorflow/tf_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)     4357 2024-04-05 14:22:22.000000 fuxictr-2.2.0/fuxictr/utils.py
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-05 14:22:22.000000 fuxictr-2.2.0/fuxictr/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:22:28.000000 fuxictr-2.2.0/fuxictr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    29940 2024-04-05 14:22:28.000000 fuxictr-2.2.0/fuxictr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2850 2024-04-05 14:22:28.000000 fuxictr-2.2.0/fuxictr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 14:22:28.000000 fuxictr-2.2.0/fuxictr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-05 14:22:28.000000 fuxictr-2.2.0/fuxictr.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-05 14:22:28.000000 fuxictr-2.2.0/fuxictr.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:22:28.000000 fuxictr-2.2.0/model_zoo/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 14:22:28.000000 fuxictr-2.2.0/model_zoo/multitask/
--rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-05 14:22:22.000000 fuxictr-2.2.0/model_zoo/multitask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 14:22:28.000000 fuxictr-2.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-04-05 14:22:22.000000 fuxictr-2.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:53:28.000000 fuxictr-2.2.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    29940 2024-04-16 03:53:28.000000 fuxictr-2.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    27518 2024-04-16 03:53:25.000000 fuxictr-2.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:53:28.000000 fuxictr-2.2.1/fuxictr/
+-rw-r--r--   0 runner    (1001) docker     (127)       32 2024-04-16 03:53:25.000000 fuxictr-2.2.1/fuxictr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6558 2024-04-16 03:53:25.000000 fuxictr-2.2.1/fuxictr/autotuner.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:53:28.000000 fuxictr-2.2.1/fuxictr/datasets/
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-16 03:53:25.000000 fuxictr-2.2.1/fuxictr/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1590 2024-04-16 03:53:25.000000 fuxictr-2.2.1/fuxictr/datasets/avazu.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1225 2024-04-16 03:53:25.000000 fuxictr-2.2.1/fuxictr/datasets/criteo.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1822 2024-04-16 03:53:25.000000 fuxictr-2.2.1/fuxictr/datasets/kkbox.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5503 2024-04-16 03:53:25.000000 fuxictr-2.2.1/fuxictr/features.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4369 2024-04-16 03:53:25.000000 fuxictr-2.2.1/fuxictr/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:53:28.000000 fuxictr-2.2.1/fuxictr/preprocess/
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-16 03:53:25.000000 fuxictr-2.2.1/fuxictr/preprocess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5651 2024-04-16 03:53:25.000000 fuxictr-2.2.1/fuxictr/preprocess/build_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18478 2024-04-16 03:53:25.000000 fuxictr-2.2.1/fuxictr/preprocess/feature_processor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1716 2024-04-16 03:53:25.000000 fuxictr-2.2.1/fuxictr/preprocess/normalizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6871 2024-04-16 03:53:25.000000 fuxictr-2.2.1/fuxictr/preprocess/tokenizer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:53:28.000000 fuxictr-2.2.1/fuxictr/pytorch/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 03:53:25.000000 fuxictr-2.2.1/fuxictr/pytorch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:53:28.000000 fuxictr-2.2.1/fuxictr/pytorch/dataloaders/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-16 03:53:25.000000 fuxictr-2.2.1/fuxictr/pytorch/dataloaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3675 2024-04-16 03:53:25.000000 fuxictr-2.2.1/fuxictr/pytorch/dataloaders/npz_block_dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2366 2024-04-16 03:53:25.000000 fuxictr-2.2.1/fuxictr/pytorch/dataloaders/npz_dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2698 2024-04-16 03:53:25.000000 fuxictr-2.2.1/fuxictr/pytorch/dataloaders/rank_dataloader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:53:28.000000 fuxictr-2.2.1/fuxictr/pytorch/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)      164 2024-04-16 03:53:25.000000 fuxictr-2.2.1/fuxictr/pytorch/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1463 2024-04-16 03:53:25.000000 fuxictr-2.2.1/fuxictr/pytorch/layers/activations.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:53:28.000000 fuxictr-2.2.1/fuxictr/pytorch/layers/attentions/
+-rw-r--r--   0 runner    (1001) docker     (127)      108 2024-04-16 03:53:25.000000 fuxictr-2.2.1/fuxictr/pytorch/layers/attentions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1810 2024-04-16 03:53:25.000000 fuxictr-2.2.1/fuxictr/pytorch/layers/attentions/dot_product_attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1750 2024-04-16 03:53:25.000000 fuxictr-2.2.1/fuxictr/pytorch/layers/attentions/squeeze_excitation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5616 2024-04-16 03:53:25.000000 fuxictr-2.2.1/fuxictr/pytorch/layers/attentions/target_attention.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:53:28.000000 fuxictr-2.2.1/fuxictr/pytorch/layers/blocks/
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-16 03:53:25.000000 fuxictr-2.2.1/fuxictr/pytorch/layers/blocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1416 2024-04-16 03:53:25.000000 fuxictr-2.2.1/fuxictr/pytorch/layers/blocks/factorization_machine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1489 2024-04-16 03:53:25.000000 fuxictr-2.2.1/fuxictr/pytorch/layers/blocks/logistic_regression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2740 2024-04-16 03:53:25.000000 fuxictr-2.2.1/fuxictr/pytorch/layers/blocks/mlp_block.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:53:28.000000 fuxictr-2.2.1/fuxictr/pytorch/layers/embeddings/
+-rw-r--r--   0 runner    (1001) docker     (127)       71 2024-04-16 03:53:25.000000 fuxictr-2.2.1/fuxictr/pytorch/layers/embeddings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10164 2024-04-16 03:53:25.000000 fuxictr-2.2.1/fuxictr/pytorch/layers/embeddings/feature_embedding.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6213 2024-04-16 03:53:25.000000 fuxictr-2.2.1/fuxictr/pytorch/layers/embeddings/pretrained_embedding.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:53:28.000000 fuxictr-2.2.1/fuxictr/pytorch/layers/interactions/
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-16 03:53:25.000000 fuxictr-2.2.1/fuxictr/pytorch/layers/interactions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4734 2024-04-16 03:53:25.000000 fuxictr-2.2.1/fuxictr/pytorch/layers/interactions/bilinear_interaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2303 2024-04-16 03:53:25.000000 fuxictr-2.2.1/fuxictr/pytorch/layers/interactions/compressed_interaction_net.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5228 2024-04-16 03:53:25.000000 fuxictr-2.2.1/fuxictr/pytorch/layers/interactions/cross_net.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-04-16 03:53:25.000000 fuxictr-2.2.1/fuxictr/pytorch/layers/interactions/holographic_interaction.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2924 2024-04-16 03:53:25.000000 fuxictr-2.2.1/fuxictr/pytorch/layers/interactions/inner_product.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2780 2024-04-16 03:53:25.000000 fuxictr-2.2.1/fuxictr/pytorch/layers/interactions/interaction_machine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1820 2024-04-16 03:53:25.000000 fuxictr-2.2.1/fuxictr/pytorch/layers/pooling.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:53:28.000000 fuxictr-2.2.1/fuxictr/pytorch/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-16 03:53:25.000000 fuxictr-2.2.1/fuxictr/pytorch/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6804 2024-04-16 03:53:25.000000 fuxictr-2.2.1/fuxictr/pytorch/models/multitask_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12848 2024-04-16 03:53:25.000000 fuxictr-2.2.1/fuxictr/pytorch/models/rank_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4344 2024-04-16 03:53:25.000000 fuxictr-2.2.1/fuxictr/pytorch/torch_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:53:28.000000 fuxictr-2.2.1/fuxictr/tensorflow/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 03:53:25.000000 fuxictr-2.2.1/fuxictr/tensorflow/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:53:28.000000 fuxictr-2.2.1/fuxictr/tensorflow/dataloaders/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-16 03:53:25.000000 fuxictr-2.2.1/fuxictr/tensorflow/dataloaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3344 2024-04-16 03:53:25.000000 fuxictr-2.2.1/fuxictr/tensorflow/dataloaders/tf_dataloader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:53:28.000000 fuxictr-2.2.1/fuxictr/tensorflow/layers/
+-rw-r--r--   0 runner    (1001) docker     (127)      107 2024-04-16 03:53:25.000000 fuxictr-2.2.1/fuxictr/tensorflow/layers/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:53:28.000000 fuxictr-2.2.1/fuxictr/tensorflow/layers/blocks/
+-rw-r--r--   0 runner    (1001) docker     (127)      123 2024-04-16 03:53:25.000000 fuxictr-2.2.1/fuxictr/tensorflow/layers/blocks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1482 2024-04-16 03:53:25.000000 fuxictr-2.2.1/fuxictr/tensorflow/layers/blocks/factorization_machine.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1517 2024-04-16 03:53:25.000000 fuxictr-2.2.1/fuxictr/tensorflow/layers/blocks/linear.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1673 2024-04-16 03:53:25.000000 fuxictr-2.2.1/fuxictr/tensorflow/layers/blocks/logistic_regression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3619 2024-04-16 03:53:25.000000 fuxictr-2.2.1/fuxictr/tensorflow/layers/blocks/mlp_block.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:53:28.000000 fuxictr-2.2.1/fuxictr/tensorflow/layers/embeddings/
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-16 03:53:25.000000 fuxictr-2.2.1/fuxictr/tensorflow/layers/embeddings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11938 2024-04-16 03:53:25.000000 fuxictr-2.2.1/fuxictr/tensorflow/layers/embeddings/feature_embedding.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:53:28.000000 fuxictr-2.2.1/fuxictr/tensorflow/layers/interactions/
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-16 03:53:25.000000 fuxictr-2.2.1/fuxictr/tensorflow/layers/interactions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2088 2024-04-16 03:53:25.000000 fuxictr-2.2.1/fuxictr/tensorflow/layers/interactions/cross_net.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2969 2024-04-16 03:53:25.000000 fuxictr-2.2.1/fuxictr/tensorflow/layers/interactions/inner_product.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-16 03:53:25.000000 fuxictr-2.2.1/fuxictr/tensorflow/layers/pooling.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:53:28.000000 fuxictr-2.2.1/fuxictr/tensorflow/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-16 03:53:25.000000 fuxictr-2.2.1/fuxictr/tensorflow/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9279 2024-04-16 03:53:25.000000 fuxictr-2.2.1/fuxictr/tensorflow/models/rank_model.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2730 2024-04-16 03:53:25.000000 fuxictr-2.2.1/fuxictr/tensorflow/tf_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4357 2024-04-16 03:53:25.000000 fuxictr-2.2.1/fuxictr/utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-16 03:53:25.000000 fuxictr-2.2.1/fuxictr/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:53:28.000000 fuxictr-2.2.1/fuxictr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    29940 2024-04-16 03:53:28.000000 fuxictr-2.2.1/fuxictr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2850 2024-04-16 03:53:28.000000 fuxictr-2.2.1/fuxictr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 03:53:28.000000 fuxictr-2.2.1/fuxictr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-16 03:53:28.000000 fuxictr-2.2.1/fuxictr.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-16 03:53:28.000000 fuxictr-2.2.1/fuxictr.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:53:28.000000 fuxictr-2.2.1/model_zoo/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 03:53:28.000000 fuxictr-2.2.1/model_zoo/multitask/
+-rw-r--r--   0 runner    (1001) docker     (127)       69 2024-04-16 03:53:25.000000 fuxictr-2.2.1/model_zoo/multitask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 03:53:28.000000 fuxictr-2.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1547 2024-04-16 03:53:25.000000 fuxictr-2.2.1/setup.py
```

### Comparing `fuxictr-2.2.0/PKG-INFO` & `fuxictr-2.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fuxictr
-Version: 2.2.0
+Version: 2.2.1
 Summary: A configurable, tunable, and reproducible library for CTR prediction
 Home-page: https://github.com/reczoo/FuxiCTR
 Author: RECZOO
 Author-email: reczoo@users.noreply.github.com
 License: Apache-2.0 License
 Download-URL: https://github.com/reczoo/FuxiCTR/tags
 Description: <div align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fuxictr Version: 2.2.0 Summary: A configurable,
+Metadata-Version: 2.1 Name: fuxictr Version: 2.2.1 Summary: A configurable,
 tunable, and reproducible library for CTR prediction Home-page: https://
 github.com/reczoo/FuxiCTR Author: RECZOO Author-email:
 reczoo@users.noreply.github.com License: Apache-2.0 License Download-URL:
 https://github.com/reczoo/FuxiCTR/tags Description:
                                     [Logo]
   _[_P_y_t_h_o_n_ _v_e_r_s_i_o_n_]_[_P_y_t_o_r_c_h_ _v_e_r_s_i_o_n_]_[_P_y_t_o_r_c_h_ _v_e_r_s_i_o_n_]_[_P_y_p_i_ _v_e_r_s_i_o_n_]_[_D_o_w_n_l_o_a_d_s_]
                                    _[_L_i_c_e_n_s_e_]
```

### Comparing `fuxictr-2.2.0/README.md` & `fuxictr-2.2.1/README.md`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.0/fuxictr/autotuner.py` & `fuxictr-2.2.1/fuxictr/autotuner.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.0/fuxictr/datasets/avazu.py` & `fuxictr-2.2.1/fuxictr/datasets/avazu.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.0/fuxictr/datasets/criteo.py` & `fuxictr-2.2.1/fuxictr/datasets/criteo.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.0/fuxictr/datasets/kkbox.py` & `fuxictr-2.2.1/fuxictr/datasets/kkbox.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.0/fuxictr/features.py` & `fuxictr-2.2.1/fuxictr/features.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.0/fuxictr/metrics.py` & `fuxictr-2.2.1/fuxictr/metrics.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.0/fuxictr/preprocess/build_dataset.py` & `fuxictr-2.2.1/fuxictr/preprocess/build_dataset.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.0/fuxictr/preprocess/feature_processor.py` & `fuxictr-2.2.1/fuxictr/preprocess/feature_processor.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.0/fuxictr/preprocess/normalizer.py` & `fuxictr-2.2.1/fuxictr/preprocess/normalizer.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.0/fuxictr/preprocess/tokenizer.py` & `fuxictr-2.2.1/fuxictr/preprocess/tokenizer.py`

 * *Files 8% similar despite different names*

```diff
@@ -123,17 +123,21 @@
                 sequence_list.append([self.vocab.get(x, self.vocab["__OOV__"]) if x != self._na_value \
                                       else self.vocab["__PAD__"] for x in text.split(self._splitter)])
         sequence_list = pad_sequences(sequence_list, maxlen=self.max_len, value=self.vocab["__PAD__"],
                                       padding=self.padding, truncating=self.padding)
         return np.array(sequence_list)
     
     def load_pretrained_vocab(self, feature_dtype, pretrain_path, expand_vocab=True):
-        with h5py.File(pretrain_path, 'r') as hf:
-            keys = hf["key"][:]
-            keys = keys.astype(feature_dtype) # in case mismatch of dtype between int and str
+        if pretrain_path.endswith(".h5"):
+            with h5py.File(pretrain_path, 'r') as hf:
+                keys = hf["key"][:]
+                # in case mismatch of dtype between int and str
+                keys = keys.astype(feature_dtype)
+        elif pretrain_path.endswith(".npz"):
+            keys = np.load(pretrain_path)["key"]
         # Update vocab with pretrained keys in case new tokens appear in validation or test set
         # Do NOT update OOV index here since it is used in PretrainedEmbedding
         if expand_vocab:
             vocab_size = self.vocab_size()
             for word in keys:
                 if word not in self.vocab:
                     self.vocab[word] = vocab_size
```

### Comparing `fuxictr-2.2.0/fuxictr/pytorch/dataloaders/npz_block_dataloader.py` & `fuxictr-2.2.1/fuxictr/pytorch/dataloaders/npz_block_dataloader.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,13 +78,12 @@
                                                  num_workers=num_workers)
 
     def __len__(self):
         return self.num_batches
 
     def count_batches_and_samples(self):
         num_samples = 0
-        num_batches = 0
         for block_path in self.data_blocks:
             block_size = np.load(block_path)[self.feature_map.labels[0]].shape[0]
             num_samples += block_size
-            num_batches += int(np.ceil(block_size * 1.0 / self.batch_size))
+        num_batches = int(np.ceil(num_samples / self.batch_size))
         return num_batches, num_samples
```

### Comparing `fuxictr-2.2.0/fuxictr/pytorch/dataloaders/npz_dataloader.py` & `fuxictr-2.2.1/fuxictr/pytorch/dataloaders/npz_dataloader.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.0/fuxictr/pytorch/dataloaders/rank_dataloader.py` & `fuxictr-2.2.1/fuxictr/pytorch/dataloaders/rank_dataloader.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.0/fuxictr/pytorch/layers/activations.py` & `fuxictr-2.2.1/fuxictr/pytorch/layers/activations.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.0/fuxictr/pytorch/layers/attentions/dot_product_attention.py` & `fuxictr-2.2.1/fuxictr/pytorch/layers/attentions/dot_product_attention.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.0/fuxictr/pytorch/layers/attentions/squeeze_excitation.py` & `fuxictr-2.2.1/fuxictr/pytorch/layers/attentions/squeeze_excitation.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.0/fuxictr/pytorch/layers/attentions/target_attention.py` & `fuxictr-2.2.1/fuxictr/pytorch/layers/attentions/target_attention.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.0/fuxictr/pytorch/layers/blocks/factorization_machine.py` & `fuxictr-2.2.1/fuxictr/pytorch/layers/blocks/factorization_machine.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.0/fuxictr/pytorch/layers/blocks/logistic_regression.py` & `fuxictr-2.2.1/fuxictr/pytorch/layers/blocks/logistic_regression.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.0/fuxictr/pytorch/layers/blocks/mlp_block.py` & `fuxictr-2.2.1/fuxictr/pytorch/layers/blocks/mlp_block.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.0/fuxictr/pytorch/layers/embeddings/feature_embedding.py` & `fuxictr-2.2.1/fuxictr/pytorch/layers/embeddings/feature_embedding.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.0/fuxictr/pytorch/layers/embeddings/pretrained_embedding.py` & `fuxictr-2.2.1/fuxictr/pytorch/layers/embeddings/pretrained_embedding.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.0/fuxictr/pytorch/layers/interactions/bilinear_interaction.py` & `fuxictr-2.2.1/fuxictr/pytorch/layers/interactions/bilinear_interaction.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.0/fuxictr/pytorch/layers/interactions/compressed_interaction_net.py` & `fuxictr-2.2.1/fuxictr/pytorch/layers/interactions/compressed_interaction_net.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.0/fuxictr/pytorch/layers/interactions/cross_net.py` & `fuxictr-2.2.1/fuxictr/pytorch/layers/interactions/cross_net.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.0/fuxictr/pytorch/layers/interactions/holographic_interaction.py` & `fuxictr-2.2.1/fuxictr/pytorch/layers/interactions/holographic_interaction.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.0/fuxictr/pytorch/layers/interactions/inner_product.py` & `fuxictr-2.2.1/fuxictr/pytorch/layers/interactions/inner_product.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.0/fuxictr/pytorch/layers/interactions/interaction_machine.py` & `fuxictr-2.2.1/fuxictr/pytorch/layers/interactions/interaction_machine.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.0/fuxictr/pytorch/layers/pooling.py` & `fuxictr-2.2.1/fuxictr/pytorch/layers/pooling.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.0/fuxictr/pytorch/models/multitask_model.py` & `fuxictr-2.2.1/fuxictr/pytorch/models/multitask_model.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.0/fuxictr/pytorch/models/rank_model.py` & `fuxictr-2.2.1/fuxictr/pytorch/models/rank_model.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.0/fuxictr/pytorch/torch_utils.py` & `fuxictr-2.2.1/fuxictr/pytorch/torch_utils.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.0/fuxictr/tensorflow/dataloaders/tf_dataloader.py` & `fuxictr-2.2.1/fuxictr/tensorflow/dataloaders/tf_dataloader.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.0/fuxictr/tensorflow/layers/blocks/factorization_machine.py` & `fuxictr-2.2.1/fuxictr/tensorflow/layers/blocks/factorization_machine.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.0/fuxictr/tensorflow/layers/blocks/linear.py` & `fuxictr-2.2.1/fuxictr/tensorflow/layers/blocks/linear.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.0/fuxictr/tensorflow/layers/blocks/logistic_regression.py` & `fuxictr-2.2.1/fuxictr/tensorflow/layers/blocks/logistic_regression.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.0/fuxictr/tensorflow/layers/blocks/mlp_block.py` & `fuxictr-2.2.1/fuxictr/tensorflow/layers/blocks/mlp_block.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.0/fuxictr/tensorflow/layers/embeddings/feature_embedding.py` & `fuxictr-2.2.1/fuxictr/tensorflow/layers/embeddings/feature_embedding.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.0/fuxictr/tensorflow/layers/interactions/cross_net.py` & `fuxictr-2.2.1/fuxictr/tensorflow/layers/interactions/cross_net.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.0/fuxictr/tensorflow/layers/interactions/inner_product.py` & `fuxictr-2.2.1/fuxictr/tensorflow/layers/interactions/inner_product.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.0/fuxictr/tensorflow/layers/pooling.py` & `fuxictr-2.2.1/fuxictr/tensorflow/layers/pooling.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.0/fuxictr/tensorflow/models/rank_model.py` & `fuxictr-2.2.1/fuxictr/tensorflow/models/rank_model.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.0/fuxictr/tensorflow/tf_utils.py` & `fuxictr-2.2.1/fuxictr/tensorflow/tf_utils.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.0/fuxictr/utils.py` & `fuxictr-2.2.1/fuxictr/utils.py`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.0/fuxictr.egg-info/PKG-INFO` & `fuxictr-2.2.1/fuxictr.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fuxictr
-Version: 2.2.0
+Version: 2.2.1
 Summary: A configurable, tunable, and reproducible library for CTR prediction
 Home-page: https://github.com/reczoo/FuxiCTR
 Author: RECZOO
 Author-email: reczoo@users.noreply.github.com
 License: Apache-2.0 License
 Download-URL: https://github.com/reczoo/FuxiCTR/tags
 Description: <div align="center">
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: fuxictr Version: 2.2.0 Summary: A configurable,
+Metadata-Version: 2.1 Name: fuxictr Version: 2.2.1 Summary: A configurable,
 tunable, and reproducible library for CTR prediction Home-page: https://
 github.com/reczoo/FuxiCTR Author: RECZOO Author-email:
 reczoo@users.noreply.github.com License: Apache-2.0 License Download-URL:
 https://github.com/reczoo/FuxiCTR/tags Description:
                                     [Logo]
   _[_P_y_t_h_o_n_ _v_e_r_s_i_o_n_]_[_P_y_t_o_r_c_h_ _v_e_r_s_i_o_n_]_[_P_y_t_o_r_c_h_ _v_e_r_s_i_o_n_]_[_P_y_p_i_ _v_e_r_s_i_o_n_]_[_D_o_w_n_l_o_a_d_s_]
                                    _[_L_i_c_e_n_s_e_]
```

### Comparing `fuxictr-2.2.0/fuxictr.egg-info/SOURCES.txt` & `fuxictr-2.2.1/fuxictr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fuxictr-2.2.0/setup.py` & `fuxictr-2.2.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fd:
     long_description = fd.read()
 
 setuptools.setup(
     name="fuxictr",
-    version="2.2.0",
+    version="2.2.1",
     author="RECZOO",
     author_email="reczoo@users.noreply.github.com",
     description="A configurable, tunable, and reproducible library for CTR prediction",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/reczoo/FuxiCTR",
     download_url='https://github.com/reczoo/FuxiCTR/tags',
```

