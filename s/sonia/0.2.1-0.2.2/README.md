# Comparing `tmp/sonia-0.2.1.tar.gz` & `tmp/sonia-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sonia-0.2.1.tar", last modified: Mon Apr 15 09:10:25 2024, max compression
+gzip compressed data, was "sonia-0.2.2.tar", last modified: Tue Apr 16 09:50:34 2024, max compression
```

## Comparing `sonia-0.2.1.tar` & `sonia-0.2.2.tar`

### file list

```diff
@@ -1,77 +1,84 @@
-drwxr-xr-x   0 giulioisac   (502) staff       (20)        0 2024-04-15 09:10:25.821685 sonia-0.2.1/
--rw-r--r--   0 giulioisac   (502) staff       (20)    35126 2023-03-20 16:42:22.000000 sonia-0.2.1/LICENSE
--rw-r--r--   0 giulioisac   (502) staff       (20)       41 2023-03-20 16:42:22.000000 sonia-0.2.1/MANIFEST.in
--rw-r--r--   0 giulioisac   (502) staff       (20)    44695 2024-04-15 09:10:25.821383 sonia-0.2.1/PKG-INFO
--rw-r--r--   0 giulioisac   (502) staff       (20)     2864 2023-03-20 16:42:22.000000 sonia-0.2.1/README.md
--rw-r--r--   0 giulioisac   (502) staff       (20)     1738 2024-04-15 09:01:00.000000 sonia-0.2.1/pyproject.toml
--rw-r--r--   0 giulioisac   (502) staff       (20)       38 2024-04-15 09:10:25.821763 sonia-0.2.1/setup.cfg
-drwxr-xr-x   0 giulioisac   (502) staff       (20)        0 2024-04-15 09:10:25.795002 sonia-0.2.1/sonia/
--rw-r--r--   0 giulioisac   (502) staff       (20)        0 2023-03-20 16:42:22.000000 sonia-0.2.1/sonia/__init__.py
-drwxr-xr-x   0 giulioisac   (502) staff       (20)        0 2024-04-15 09:10:25.789802 sonia-0.2.1/sonia/default_models/
-drwxr-xr-x   0 giulioisac   (502) staff       (20)        0 2024-04-15 09:10:25.808134 sonia-0.2.1/sonia/default_models/human_B_heavy/
--rw-r--r--   0 giulioisac   (502) staff       (20)      255 2023-03-20 16:42:22.000000 sonia-0.2.1/sonia/default_models/human_B_heavy/J_gene_CDR3_anchors.csv
--rw-r--r--   0 giulioisac   (502) staff       (20)     5839 2023-03-20 16:42:22.000000 sonia-0.2.1/sonia/default_models/human_B_heavy/V_gene_CDR3_anchors.csv
--rw-r--r--   0 giulioisac   (502) staff       (20)    89230 2023-03-20 16:42:22.000000 sonia-0.2.1/sonia/default_models/human_B_heavy/features.tsv
--rw-r--r--   0 giulioisac   (502) staff       (20)      111 2023-03-20 16:42:22.000000 sonia-0.2.1/sonia/default_models/human_B_heavy/log.txt
--rw-r--r--   0 giulioisac   (502) staff       (20)   483313 2023-03-20 16:42:22.000000 sonia-0.2.1/sonia/default_models/human_B_heavy/model_marginals.txt
--rw-r--r--   0 giulioisac   (502) staff       (20)    35291 2023-03-20 16:42:22.000000 sonia-0.2.1/sonia/default_models/human_B_heavy/model_params.txt
-drwxr-xr-x   0 giulioisac   (502) staff       (20)        0 2024-04-15 09:10:25.809845 sonia-0.2.1/sonia/default_models/human_B_kappa/
--rw-r--r--   0 giulioisac   (502) staff       (20)      144 2023-03-20 16:42:22.000000 sonia-0.2.1/sonia/default_models/human_B_kappa/J_gene_CDR3_anchors.csv
--rw-r--r--   0 giulioisac   (502) staff       (20)     1179 2023-03-20 16:42:22.000000 sonia-0.2.1/sonia/default_models/human_B_kappa/V_gene_CDR3_anchors.csv
--rw-r--r--   0 giulioisac   (502) staff       (20)    81160 2023-03-20 16:42:22.000000 sonia-0.2.1/sonia/default_models/human_B_kappa/features.tsv
--rw-r--r--   0 giulioisac   (502) staff       (20)      111 2023-03-20 16:42:22.000000 sonia-0.2.1/sonia/default_models/human_B_kappa/log.txt
--rw-r--r--   0 giulioisac   (502) staff       (20)    18959 2023-03-20 16:42:22.000000 sonia-0.2.1/sonia/default_models/human_B_kappa/model_marginals.txt
--rw-r--r--   0 giulioisac   (502) staff       (20)    20986 2023-03-20 16:42:22.000000 sonia-0.2.1/sonia/default_models/human_B_kappa/model_params.txt
-drwxr-xr-x   0 giulioisac   (502) staff       (20)        0 2024-04-15 09:10:25.811498 sonia-0.2.1/sonia/default_models/human_B_lambda/
--rw-r--r--   0 giulioisac   (502) staff       (20)      118 2023-03-20 16:42:22.000000 sonia-0.2.1/sonia/default_models/human_B_lambda/J_gene_CDR3_anchors.csv
--rw-r--r--   0 giulioisac   (502) staff       (20)     1264 2023-03-20 16:42:22.000000 sonia-0.2.1/sonia/default_models/human_B_lambda/V_gene_CDR3_anchors.csv
--rw-r--r--   0 giulioisac   (502) staff       (20)    84252 2023-03-20 16:42:22.000000 sonia-0.2.1/sonia/default_models/human_B_lambda/features.tsv
--rw-r--r--   0 giulioisac   (502) staff       (20)      111 2023-03-20 16:42:22.000000 sonia-0.2.1/sonia/default_models/human_B_lambda/log.txt
--rw-r--r--   0 giulioisac   (502) staff       (20)    17632 2023-03-20 16:42:22.000000 sonia-0.2.1/sonia/default_models/human_B_lambda/model_marginals.txt
--rw-r--r--   0 giulioisac   (502) staff       (20)    23091 2023-03-20 16:42:22.000000 sonia-0.2.1/sonia/default_models/human_B_lambda/model_params.txt
-drwxr-xr-x   0 giulioisac   (502) staff       (20)        0 2024-04-15 09:10:25.813441 sonia-0.2.1/sonia/default_models/human_T_alpha/
--rw-r--r--   0 giulioisac   (502) staff       (20)     1127 2023-03-20 16:42:22.000000 sonia-0.2.1/sonia/default_models/human_T_alpha/J_gene_CDR3_anchors.csv
--rw-r--r--   0 giulioisac   (502) staff       (20)     1901 2023-03-20 16:42:22.000000 sonia-0.2.1/sonia/default_models/human_T_alpha/V_gene_CDR3_anchors.csv
--rw-r--r--   0 giulioisac   (502) staff       (20)   273848 2023-03-20 16:42:22.000000 sonia-0.2.1/sonia/default_models/human_T_alpha/features.tsv
--rw-r--r--   0 giulioisac   (502) staff       (20)      111 2023-03-20 16:42:22.000000 sonia-0.2.1/sonia/default_models/human_T_alpha/log.txt
--rw-r--r--   0 giulioisac   (502) staff       (20)    75679 2023-03-20 16:42:22.000000 sonia-0.2.1/sonia/default_models/human_T_alpha/model_marginals.txt
--rw-r--r--   0 giulioisac   (502) staff       (20)    35883 2023-03-20 16:42:22.000000 sonia-0.2.1/sonia/default_models/human_T_alpha/model_params.txt
-drwxr-xr-x   0 giulioisac   (502) staff       (20)        0 2024-04-15 09:10:25.816462 sonia-0.2.1/sonia/default_models/human_T_beta/
--rw-r--r--   0 giulioisac   (502) staff       (20)      283 2023-03-20 16:42:22.000000 sonia-0.2.1/sonia/default_models/human_T_beta/J_gene_CDR3_anchors.csv
--rw-r--r--   0 giulioisac   (502) staff       (20)     2570 2023-03-20 16:42:22.000000 sonia-0.2.1/sonia/default_models/human_T_beta/V_gene_CDR3_anchors.csv
--rw-r--r--   0 giulioisac   (502) staff       (20)   110228 2023-03-20 16:42:22.000000 sonia-0.2.1/sonia/default_models/human_T_beta/features.tsv
--rw-r--r--   0 giulioisac   (502) staff       (20)      111 2023-03-20 16:42:22.000000 sonia-0.2.1/sonia/default_models/human_T_beta/log.txt
--rw-r--r--   0 giulioisac   (502) staff       (20)    27384 2023-03-20 16:42:22.000000 sonia-0.2.1/sonia/default_models/human_T_beta/model_marginals.txt
--rw-r--r--   0 giulioisac   (502) staff       (20)    30009 2023-03-20 16:42:22.000000 sonia-0.2.1/sonia/default_models/human_T_beta/model_params.txt
-drwxr-xr-x   0 giulioisac   (502) staff       (20)        0 2024-04-15 09:10:25.818631 sonia-0.2.1/sonia/default_models/mouse_T_alpha/
--rw-r--r--   0 giulioisac   (502) staff       (20)      785 2023-03-20 16:42:22.000000 sonia-0.2.1/sonia/default_models/mouse_T_alpha/J_gene_CDR3_anchors.csv
--rw-r--r--   0 giulioisac   (502) staff       (20)     1981 2023-03-20 16:42:22.000000 sonia-0.2.1/sonia/default_models/mouse_T_alpha/V_gene_CDR3_anchors.csv
--rw-r--r--   0 giulioisac   (502) staff       (20)   476729 2023-03-20 16:42:22.000000 sonia-0.2.1/sonia/default_models/mouse_T_alpha/features.tsv
--rw-r--r--   0 giulioisac   (502) staff       (20)      131 2023-03-20 16:42:22.000000 sonia-0.2.1/sonia/default_models/mouse_T_alpha/log.txt
--rw-r--r--   0 giulioisac   (502) staff       (20)    81928 2023-03-20 16:42:22.000000 sonia-0.2.1/sonia/default_models/mouse_T_alpha/model_marginals.txt
--rw-r--r--   0 giulioisac   (502) staff       (20)    36713 2023-03-20 16:42:22.000000 sonia-0.2.1/sonia/default_models/mouse_T_alpha/model_params.txt
-drwxr-xr-x   0 giulioisac   (502) staff       (20)        0 2024-04-15 09:10:25.820225 sonia-0.2.1/sonia/default_models/mouse_T_beta/
--rw-r--r--   0 giulioisac   (502) staff       (20)      257 2023-03-20 16:42:22.000000 sonia-0.2.1/sonia/default_models/mouse_T_beta/J_gene_CDR3_anchors.csv
--rw-r--r--   0 giulioisac   (502) staff       (20)      448 2023-03-20 16:42:22.000000 sonia-0.2.1/sonia/default_models/mouse_T_beta/V_gene_CDR3_anchors.csv
--rw-r--r--   0 giulioisac   (502) staff       (20)    85621 2023-03-20 16:42:22.000000 sonia-0.2.1/sonia/default_models/mouse_T_beta/features.tsv
--rw-r--r--   0 giulioisac   (502) staff       (20)      105 2023-03-20 16:42:22.000000 sonia-0.2.1/sonia/default_models/mouse_T_beta/log.txt
--rw-r--r--   0 giulioisac   (502) staff       (20)    12795 2023-03-20 16:42:22.000000 sonia-0.2.1/sonia/default_models/mouse_T_beta/model_marginals.txt
--rw-r--r--   0 giulioisac   (502) staff       (20)    13475 2023-03-20 16:42:22.000000 sonia-0.2.1/sonia/default_models/mouse_T_beta/model_params.txt
--rwxr-xr-x   0 giulioisac   (502) staff       (20)    23323 2023-03-20 16:42:22.000000 sonia-0.2.1/sonia/evaluate.py
--rw-r--r--   0 giulioisac   (502) staff       (20)    12477 2023-03-20 16:42:22.000000 sonia-0.2.1/sonia/evaluate_model.py
--rwxr-xr-x   0 giulioisac   (502) staff       (20)    10672 2023-03-20 16:42:22.000000 sonia-0.2.1/sonia/generate.py
--rwxr-xr-x   0 giulioisac   (502) staff       (20)    27193 2023-03-20 16:42:22.000000 sonia-0.2.1/sonia/infer.py
--rw-r--r--   0 giulioisac   (502) staff       (20)    19593 2024-04-15 08:10:44.000000 sonia-0.2.1/sonia/plotting.py
--rw-r--r--   0 giulioisac   (502) staff       (20)     7108 2023-03-20 16:42:22.000000 sonia-0.2.1/sonia/sequence_generation.py
--rw-r--r--   0 giulioisac   (502) staff       (20)    37910 2024-04-15 09:10:01.000000 sonia-0.2.1/sonia/sonia.py
--rw-r--r--   0 giulioisac   (502) staff       (20)    15113 2023-03-20 16:42:22.000000 sonia-0.2.1/sonia/sonia_leftpos_rightpos.py
--rw-r--r--   0 giulioisac   (502) staff       (20)    12373 2023-03-20 16:42:22.000000 sonia-0.2.1/sonia/sonia_length_pos.py
--rw-r--r--   0 giulioisac   (502) staff       (20)    14525 2023-03-20 16:42:22.000000 sonia-0.2.1/sonia/sonia_vjl.py
--rw-r--r--   0 giulioisac   (502) staff       (20)     3591 2023-03-20 16:42:22.000000 sonia-0.2.1/sonia/utils.py
-drwxr-xr-x   0 giulioisac   (502) staff       (20)        0 2024-04-15 09:10:25.820623 sonia-0.2.1/sonia.egg-info/
--rw-r--r--   0 giulioisac   (502) staff       (20)    44695 2024-04-15 09:10:25.000000 sonia-0.2.1/sonia.egg-info/PKG-INFO
--rw-r--r--   0 giulioisac   (502) staff       (20)     2673 2024-04-15 09:10:25.000000 sonia-0.2.1/sonia.egg-info/SOURCES.txt
--rw-r--r--   0 giulioisac   (502) staff       (20)        1 2024-04-15 09:10:25.000000 sonia-0.2.1/sonia.egg-info/dependency_links.txt
--rw-r--r--   0 giulioisac   (502) staff       (20)      123 2024-04-15 09:10:25.000000 sonia-0.2.1/sonia.egg-info/entry_points.txt
--rw-r--r--   0 giulioisac   (502) staff       (20)       52 2024-04-15 09:10:25.000000 sonia-0.2.1/sonia.egg-info/requires.txt
--rw-r--r--   0 giulioisac   (502) staff       (20)        6 2024-04-15 09:10:25.000000 sonia-0.2.1/sonia.egg-info/top_level.txt
+drwxr-xr-x   0 giulioisac   (502) staff       (20)        0 2024-04-16 09:50:34.848639 sonia-0.2.2/
+-rw-r--r--   0 giulioisac   (502) staff       (20)    35126 2024-04-16 09:24:10.000000 sonia-0.2.2/LICENSE
+-rw-r--r--   0 giulioisac   (502) staff       (20)       41 2024-04-16 09:26:05.000000 sonia-0.2.2/MANIFEST.in
+-rw-r--r--   0 giulioisac   (502) staff       (20)    44921 2024-04-16 09:50:34.848369 sonia-0.2.2/PKG-INFO
+-rw-r--r--   0 giulioisac   (502) staff       (20)     3090 2024-04-16 09:49:45.000000 sonia-0.2.2/README.md
+-rw-r--r--   0 giulioisac   (502) staff       (20)     1738 2024-04-16 09:49:57.000000 sonia-0.2.2/pyproject.toml
+-rw-r--r--   0 giulioisac   (502) staff       (20)       38 2024-04-16 09:50:34.848683 sonia-0.2.2/setup.cfg
+drwxr-xr-x   0 giulioisac   (502) staff       (20)        0 2024-04-16 09:50:34.820138 sonia-0.2.2/sonia/
+-rw-r--r--   0 giulioisac   (502) staff       (20)        0 2024-04-16 09:24:10.000000 sonia-0.2.2/sonia/__init__.py
+drwxr-xr-x   0 giulioisac   (502) staff       (20)        0 2024-04-16 09:50:34.815934 sonia-0.2.2/sonia/default_models/
+drwxr-xr-x   0 giulioisac   (502) staff       (20)        0 2024-04-16 09:50:34.833778 sonia-0.2.2/sonia/default_models/human_B_heavy/
+-rw-r--r--   0 giulioisac   (502) staff       (20)      255 2024-04-16 09:24:10.000000 sonia-0.2.2/sonia/default_models/human_B_heavy/J_gene_CDR3_anchors.csv
+-rw-r--r--   0 giulioisac   (502) staff       (20)     5839 2024-04-16 09:24:10.000000 sonia-0.2.2/sonia/default_models/human_B_heavy/V_gene_CDR3_anchors.csv
+-rw-r--r--   0 giulioisac   (502) staff       (20)    89230 2024-04-16 09:24:10.000000 sonia-0.2.2/sonia/default_models/human_B_heavy/features.tsv
+-rw-r--r--   0 giulioisac   (502) staff       (20)      111 2024-04-16 09:24:10.000000 sonia-0.2.2/sonia/default_models/human_B_heavy/log.txt
+-rw-r--r--   0 giulioisac   (502) staff       (20)    16992 2024-04-16 09:24:10.000000 sonia-0.2.2/sonia/default_models/human_B_heavy/model.h5
+-rw-r--r--   0 giulioisac   (502) staff       (20)   483313 2024-04-16 09:24:10.000000 sonia-0.2.2/sonia/default_models/human_B_heavy/model_marginals.txt
+-rw-r--r--   0 giulioisac   (502) staff       (20)    35291 2024-04-16 09:24:10.000000 sonia-0.2.2/sonia/default_models/human_B_heavy/model_params.txt
+drwxr-xr-x   0 giulioisac   (502) staff       (20)        0 2024-04-16 09:50:34.836238 sonia-0.2.2/sonia/default_models/human_B_kappa/
+-rw-r--r--   0 giulioisac   (502) staff       (20)      144 2024-04-16 09:24:10.000000 sonia-0.2.2/sonia/default_models/human_B_kappa/J_gene_CDR3_anchors.csv
+-rw-r--r--   0 giulioisac   (502) staff       (20)     1179 2024-04-16 09:24:10.000000 sonia-0.2.2/sonia/default_models/human_B_kappa/V_gene_CDR3_anchors.csv
+-rw-r--r--   0 giulioisac   (502) staff       (20)    81160 2024-04-16 09:24:10.000000 sonia-0.2.2/sonia/default_models/human_B_kappa/features.tsv
+-rw-r--r--   0 giulioisac   (502) staff       (20)      111 2024-04-16 09:24:10.000000 sonia-0.2.2/sonia/default_models/human_B_kappa/log.txt
+-rw-r--r--   0 giulioisac   (502) staff       (20)    16012 2024-04-16 09:24:10.000000 sonia-0.2.2/sonia/default_models/human_B_kappa/model.h5
+-rw-r--r--   0 giulioisac   (502) staff       (20)    18959 2024-04-16 09:24:10.000000 sonia-0.2.2/sonia/default_models/human_B_kappa/model_marginals.txt
+-rw-r--r--   0 giulioisac   (502) staff       (20)    20986 2024-04-16 09:24:10.000000 sonia-0.2.2/sonia/default_models/human_B_kappa/model_params.txt
+drwxr-xr-x   0 giulioisac   (502) staff       (20)        0 2024-04-16 09:50:34.838183 sonia-0.2.2/sonia/default_models/human_B_lambda/
+-rw-r--r--   0 giulioisac   (502) staff       (20)      118 2024-04-16 09:24:10.000000 sonia-0.2.2/sonia/default_models/human_B_lambda/J_gene_CDR3_anchors.csv
+-rw-r--r--   0 giulioisac   (502) staff       (20)     1264 2024-04-16 09:24:10.000000 sonia-0.2.2/sonia/default_models/human_B_lambda/V_gene_CDR3_anchors.csv
+-rw-r--r--   0 giulioisac   (502) staff       (20)    84252 2024-04-16 09:24:10.000000 sonia-0.2.2/sonia/default_models/human_B_lambda/features.tsv
+-rw-r--r--   0 giulioisac   (502) staff       (20)      111 2024-04-16 09:24:10.000000 sonia-0.2.2/sonia/default_models/human_B_lambda/log.txt
+-rw-r--r--   0 giulioisac   (502) staff       (20)    15852 2024-04-16 09:24:10.000000 sonia-0.2.2/sonia/default_models/human_B_lambda/model.h5
+-rw-r--r--   0 giulioisac   (502) staff       (20)    17632 2024-04-16 09:24:10.000000 sonia-0.2.2/sonia/default_models/human_B_lambda/model_marginals.txt
+-rw-r--r--   0 giulioisac   (502) staff       (20)    23091 2024-04-16 09:24:10.000000 sonia-0.2.2/sonia/default_models/human_B_lambda/model_params.txt
+drwxr-xr-x   0 giulioisac   (502) staff       (20)        0 2024-04-16 09:50:34.840832 sonia-0.2.2/sonia/default_models/human_T_alpha/
+-rw-r--r--   0 giulioisac   (502) staff       (20)     1127 2024-04-16 09:24:10.000000 sonia-0.2.2/sonia/default_models/human_T_alpha/J_gene_CDR3_anchors.csv
+-rw-r--r--   0 giulioisac   (502) staff       (20)     1901 2024-04-16 09:24:10.000000 sonia-0.2.2/sonia/default_models/human_T_alpha/V_gene_CDR3_anchors.csv
+-rw-r--r--   0 giulioisac   (502) staff       (20)   273848 2024-04-16 09:24:10.000000 sonia-0.2.2/sonia/default_models/human_T_alpha/features.tsv
+-rw-r--r--   0 giulioisac   (502) staff       (20)      111 2024-04-16 09:24:10.000000 sonia-0.2.2/sonia/default_models/human_T_alpha/log.txt
+-rw-r--r--   0 giulioisac   (502) staff       (20)    26660 2024-04-16 09:24:10.000000 sonia-0.2.2/sonia/default_models/human_T_alpha/model.h5
+-rw-r--r--   0 giulioisac   (502) staff       (20)    75679 2024-04-16 09:24:10.000000 sonia-0.2.2/sonia/default_models/human_T_alpha/model_marginals.txt
+-rw-r--r--   0 giulioisac   (502) staff       (20)    35883 2024-04-16 09:24:10.000000 sonia-0.2.2/sonia/default_models/human_T_alpha/model_params.txt
+drwxr-xr-x   0 giulioisac   (502) staff       (20)        0 2024-04-16 09:50:34.842737 sonia-0.2.2/sonia/default_models/human_T_beta/
+-rw-r--r--   0 giulioisac   (502) staff       (20)      283 2024-04-16 09:24:10.000000 sonia-0.2.2/sonia/default_models/human_T_beta/J_gene_CDR3_anchors.csv
+-rw-r--r--   0 giulioisac   (502) staff       (20)     2570 2024-04-16 09:24:10.000000 sonia-0.2.2/sonia/default_models/human_T_beta/V_gene_CDR3_anchors.csv
+-rw-r--r--   0 giulioisac   (502) staff       (20)   110228 2024-04-16 09:24:10.000000 sonia-0.2.2/sonia/default_models/human_T_beta/features.tsv
+-rw-r--r--   0 giulioisac   (502) staff       (20)      111 2024-04-16 09:24:10.000000 sonia-0.2.2/sonia/default_models/human_T_beta/log.txt
+-rw-r--r--   0 giulioisac   (502) staff       (20)    18260 2024-04-16 09:24:10.000000 sonia-0.2.2/sonia/default_models/human_T_beta/model.h5
+-rw-r--r--   0 giulioisac   (502) staff       (20)    27384 2024-04-16 09:24:10.000000 sonia-0.2.2/sonia/default_models/human_T_beta/model_marginals.txt
+-rw-r--r--   0 giulioisac   (502) staff       (20)    30009 2024-04-16 09:24:10.000000 sonia-0.2.2/sonia/default_models/human_T_beta/model_params.txt
+drwxr-xr-x   0 giulioisac   (502) staff       (20)        0 2024-04-16 09:50:34.845329 sonia-0.2.2/sonia/default_models/mouse_T_alpha/
+-rw-r--r--   0 giulioisac   (502) staff       (20)      785 2024-04-16 09:24:10.000000 sonia-0.2.2/sonia/default_models/mouse_T_alpha/J_gene_CDR3_anchors.csv
+-rw-r--r--   0 giulioisac   (502) staff       (20)     1981 2024-04-16 09:24:10.000000 sonia-0.2.2/sonia/default_models/mouse_T_alpha/V_gene_CDR3_anchors.csv
+-rw-r--r--   0 giulioisac   (502) staff       (20)   476729 2024-04-16 09:24:10.000000 sonia-0.2.2/sonia/default_models/mouse_T_alpha/features.tsv
+-rw-r--r--   0 giulioisac   (502) staff       (20)      130 2024-04-16 09:24:10.000000 sonia-0.2.2/sonia/default_models/mouse_T_alpha/log.txt
+-rw-r--r--   0 giulioisac   (502) staff       (20)    37020 2024-04-16 09:24:10.000000 sonia-0.2.2/sonia/default_models/mouse_T_alpha/model.h5
+-rw-r--r--   0 giulioisac   (502) staff       (20)    81928 2024-04-16 09:24:10.000000 sonia-0.2.2/sonia/default_models/mouse_T_alpha/model_marginals.txt
+-rw-r--r--   0 giulioisac   (502) staff       (20)    36713 2024-04-16 09:24:10.000000 sonia-0.2.2/sonia/default_models/mouse_T_alpha/model_params.txt
+drwxr-xr-x   0 giulioisac   (502) staff       (20)        0 2024-04-16 09:50:34.847610 sonia-0.2.2/sonia/default_models/mouse_T_beta/
+-rw-r--r--   0 giulioisac   (502) staff       (20)      257 2024-04-16 09:24:10.000000 sonia-0.2.2/sonia/default_models/mouse_T_beta/J_gene_CDR3_anchors.csv
+-rw-r--r--   0 giulioisac   (502) staff       (20)      448 2024-04-16 09:24:10.000000 sonia-0.2.2/sonia/default_models/mouse_T_beta/V_gene_CDR3_anchors.csv
+-rw-r--r--   0 giulioisac   (502) staff       (20)    85621 2024-04-16 09:24:10.000000 sonia-0.2.2/sonia/default_models/mouse_T_beta/features.tsv
+-rw-r--r--   0 giulioisac   (502) staff       (20)      105 2024-04-16 09:24:10.000000 sonia-0.2.2/sonia/default_models/mouse_T_beta/log.txt
+-rw-r--r--   0 giulioisac   (502) staff       (20)    17152 2024-04-16 09:24:10.000000 sonia-0.2.2/sonia/default_models/mouse_T_beta/model.h5
+-rw-r--r--   0 giulioisac   (502) staff       (20)    12795 2024-04-16 09:24:10.000000 sonia-0.2.2/sonia/default_models/mouse_T_beta/model_marginals.txt
+-rw-r--r--   0 giulioisac   (502) staff       (20)    13475 2024-04-16 09:24:10.000000 sonia-0.2.2/sonia/default_models/mouse_T_beta/model_params.txt
+-rwxr-xr-x   0 giulioisac   (502) staff       (20)    23386 2024-04-16 09:24:10.000000 sonia-0.2.2/sonia/evaluate.py
+-rw-r--r--   0 giulioisac   (502) staff       (20)    12480 2024-04-16 09:24:10.000000 sonia-0.2.2/sonia/evaluate_model.py
+-rwxr-xr-x   0 giulioisac   (502) staff       (20)    10672 2024-04-16 09:24:10.000000 sonia-0.2.2/sonia/generate.py
+-rwxr-xr-x   0 giulioisac   (502) staff       (20)    27193 2024-04-16 09:24:10.000000 sonia-0.2.2/sonia/infer.py
+-rw-r--r--   0 giulioisac   (502) staff       (20)    19593 2024-04-16 09:24:10.000000 sonia-0.2.2/sonia/plotting.py
+-rw-r--r--   0 giulioisac   (502) staff       (20)     8022 2024-04-16 09:24:10.000000 sonia-0.2.2/sonia/sequence_generation.py
+-rw-r--r--   0 giulioisac   (502) staff       (20)    38149 2024-04-16 09:24:10.000000 sonia-0.2.2/sonia/sonia.py
+-rw-r--r--   0 giulioisac   (502) staff       (20)    15104 2024-04-16 09:24:10.000000 sonia-0.2.2/sonia/sonia_leftpos_rightpos.py
+-rw-r--r--   0 giulioisac   (502) staff       (20)    12372 2024-04-16 09:24:10.000000 sonia-0.2.2/sonia/sonia_length_pos.py
+-rw-r--r--   0 giulioisac   (502) staff       (20)    14525 2024-04-16 09:24:10.000000 sonia-0.2.2/sonia/sonia_vjl.py
+-rw-r--r--   0 giulioisac   (502) staff       (20)     3943 2024-04-16 09:24:10.000000 sonia-0.2.2/sonia/utils.py
+drwxr-xr-x   0 giulioisac   (502) staff       (20)        0 2024-04-16 09:50:34.847895 sonia-0.2.2/sonia.egg-info/
+-rw-r--r--   0 giulioisac   (502) staff       (20)    44921 2024-04-16 09:50:34.000000 sonia-0.2.2/sonia.egg-info/PKG-INFO
+-rw-r--r--   0 giulioisac   (502) staff       (20)     2980 2024-04-16 09:50:34.000000 sonia-0.2.2/sonia.egg-info/SOURCES.txt
+-rw-r--r--   0 giulioisac   (502) staff       (20)        1 2024-04-16 09:50:34.000000 sonia-0.2.2/sonia.egg-info/dependency_links.txt
+-rw-r--r--   0 giulioisac   (502) staff       (20)      123 2024-04-16 09:50:34.000000 sonia-0.2.2/sonia.egg-info/entry_points.txt
+-rw-r--r--   0 giulioisac   (502) staff       (20)       52 2024-04-16 09:50:34.000000 sonia-0.2.2/sonia.egg-info/requires.txt
+-rw-r--r--   0 giulioisac   (502) staff       (20)        6 2024-04-16 09:50:34.000000 sonia-0.2.2/sonia.egg-info/top_level.txt
```

### Comparing `sonia-0.2.1/LICENSE` & `sonia-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `sonia-0.2.1/PKG-INFO` & `sonia-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sonia
-Version: 0.2.1
+Version: 0.2.2
 Summary: SONIA is a python 3.6 software developed to infer selection pressures on features of amino acid CDR3 sequences. The model can be used to calculate the probability of observing any sequence after selection and sample from the selected repertoire.
 Author: Zachary Sethna
 Author-email: Giulio Isacchini <giulioisac@gmail.com>
 Maintainer-email: Giulio Isacchini <giulioisac@gmail.com>
 License: GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
@@ -697,40 +697,41 @@
 Requires-Dist: tensorflow>=2.1.0
 Requires-Dist: matplotlib
 Requires-Dist: olga>=1.1.3
 Requires-Dist: tqdm
 
 # SONIA
 
+This Package is not actively mantained, please refer to the most updated SoNNia package which includes sonia models as well: https://github.com/statbiophys/soNNia
+
 SONIA is a python 3.6/2.7 software developed to infer selection pressures on features of amino acid CDR3 sequences. The inference is based on maximizing the likelihood of observing a selected data sample given a representative pre-selected sample. This method was first used in Elhanati et al (2014) to study thymic selection. For this purpose, the pre-selected sample can be generated internally using the OLGA software package, but SONIA allows it also to be supplied externally, in the same way the data sample is provided.
 
 ![](docs/source/model.png)
 
 SONIA takes as input TCR CDR3 amino acid sequences, with or without per sequence lists of possible V and J genes suspected to be used in the recombination process for this sequence. Its output is selection factors for each amino acid ,(relative) position , CDR3 length combinations, and also for each V and J gene choice. These selection factors can be used to calculate sequence level selection factors which indicate how more or less represented this sequence would be in the selected pool as compared to the the pre-selected pool. These in turn could be used to calculate the probability to observe any sequence after selection and sample from the selected repertoire. 
 
 ![](docs/source/workflow.png)
 ## Version
-Latest released version: 0.0.45
+Latest released version: 0.2.2
 
 ## Installation
 SONIA is a python 2.7/3.6 software. It is available on PyPI and can be downloaded and installed through pip:
 
  ```pip install sonia```.
 
-SONIA is also available on [GitHub](https://github.com/statbiophys/SONIA). The command line entry points can be installed by using the setup.py script:
-
- ```python setup.py install```.
+SONIA is also available on [GitHub](https://github.com/statbiophys/SONIA).
  
 Sometimes pip fails to install the dependencies correctly. Thus, if you get any error try first to install the dependencies separately:
  ```
 pip install tensorflow
 pip install matplotlib
 pip install olga
 pip install sonia 
  ```
+For mac user on new metal devices, make sure to install additional dependencies. Currently, the configuration tensorflow-macos==2.9 and tensorflow-metal==0.5.0 should work.
 
 ## References
 
 1. Sethna Z, Isacchini G, Dupic T, Mora T, Walczak AM, Elhanati Y, Population variability in the generation and thymic selection of T-cell repertoires, (2020) bioRxiv, https://doi.org/10.1101/2020.01.08.899682
 2. Isacchini G, Sethna Z, Elhanati Y ,Nourmohammad A, Mora T, Walczak AM, Generative models of T-cell receptor sequences, (2020) Phys. Rev. E 101, 062414, https://journals.aps.org/pre/abstract/10.1103/PhysRevE.101.062414
 3. Elhanati Y, Murugan A , Callan CGJ ,  Mora T , Walczak AM, Quantifying selection in immune receptor repertoires, PNAS July 8, 2014 111 (27) 9875-9880, https://doi.org/10.1073/pnas.1409572111
```

### Comparing `sonia-0.2.1/README.md` & `sonia-0.2.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 # SONIA
 
+This Package is not actively mantained, please refer to the most updated SoNNia package which includes sonia models as well: https://github.com/statbiophys/soNNia
+
 SONIA is a python 3.6/2.7 software developed to infer selection pressures on features of amino acid CDR3 sequences. The inference is based on maximizing the likelihood of observing a selected data sample given a representative pre-selected sample. This method was first used in Elhanati et al (2014) to study thymic selection. For this purpose, the pre-selected sample can be generated internally using the OLGA software package, but SONIA allows it also to be supplied externally, in the same way the data sample is provided.
 
 ![](docs/source/model.png)
 
 SONIA takes as input TCR CDR3 amino acid sequences, with or without per sequence lists of possible V and J genes suspected to be used in the recombination process for this sequence. Its output is selection factors for each amino acid ,(relative) position , CDR3 length combinations, and also for each V and J gene choice. These selection factors can be used to calculate sequence level selection factors which indicate how more or less represented this sequence would be in the selected pool as compared to the the pre-selected pool. These in turn could be used to calculate the probability to observe any sequence after selection and sample from the selected repertoire. 
 
 ![](docs/source/workflow.png)
 ## Version
-Latest released version: 0.0.45
+Latest released version: 0.2.2
 
 ## Installation
 SONIA is a python 2.7/3.6 software. It is available on PyPI and can be downloaded and installed through pip:
 
  ```pip install sonia```.
 
-SONIA is also available on [GitHub](https://github.com/statbiophys/SONIA). The command line entry points can be installed by using the setup.py script:
-
- ```python setup.py install```.
+SONIA is also available on [GitHub](https://github.com/statbiophys/SONIA).
  
 Sometimes pip fails to install the dependencies correctly. Thus, if you get any error try first to install the dependencies separately:
  ```
 pip install tensorflow
 pip install matplotlib
 pip install olga
 pip install sonia 
  ```
+For mac user on new metal devices, make sure to install additional dependencies. Currently, the configuration tensorflow-macos==2.9 and tensorflow-metal==0.5.0 should work.
 
 ## References
 
 1. Sethna Z, Isacchini G, Dupic T, Mora T, Walczak AM, Elhanati Y, Population variability in the generation and thymic selection of T-cell repertoires, (2020) bioRxiv, https://doi.org/10.1101/2020.01.08.899682
 2. Isacchini G, Sethna Z, Elhanati Y ,Nourmohammad A, Mora T, Walczak AM, Generative models of T-cell receptor sequences, (2020) Phys. Rev. E 101, 062414, https://journals.aps.org/pre/abstract/10.1103/PhysRevE.101.062414
 3. Elhanati Y, Murugan A , Callan CGJ ,  Mora T , Walczak AM, Quantifying selection in immune receptor repertoires, PNAS July 8, 2014 111 (27) 9875-9880, https://doi.org/10.1073/pnas.1409572111
```

### Comparing `sonia-0.2.1/pyproject.toml` & `sonia-0.2.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 [build-system]
 requires = ["setuptools >= 61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "sonia"
-version = "0.2.1"
+version = "0.2.2"
 #dynamic = ["version"]
 dependencies = ['numpy','tensorflow>=2.1.0','matplotlib','olga>=1.1.3','tqdm']
 authors = [ {name = "Zachary Sethna"}, {name = "Giulio Isacchini", email = "giulioisac@gmail.com"}]
 maintainers = [{name = "Giulio Isacchini", email = "giulioisac@gmail.com"}]
 description = 'SONIA is a python 3.6 software developed to infer selection pressures on features of amino acid CDR3 sequences. The model can be used to calculate the probability of observing any sequence after selection and sample from the selected repertoire.'
 readme = "README.md"
 license = {file = "LICENSE"}
```

### Comparing `sonia-0.2.1/sonia/default_models/human_B_heavy/V_gene_CDR3_anchors.csv` & `sonia-0.2.2/sonia/default_models/human_B_heavy/V_gene_CDR3_anchors.csv`

 * *Files identical despite different names*

### Comparing `sonia-0.2.1/sonia/default_models/human_B_heavy/features.tsv` & `sonia-0.2.2/sonia/default_models/human_B_heavy/features.tsv`

 * *Files identical despite different names*

### Comparing `sonia-0.2.1/sonia/default_models/human_B_heavy/model_marginals.txt` & `sonia-0.2.2/sonia/default_models/human_B_heavy/model_marginals.txt`

 * *Files identical despite different names*

### Comparing `sonia-0.2.1/sonia/default_models/human_B_heavy/model_params.txt` & `sonia-0.2.2/sonia/default_models/human_B_heavy/model_params.txt`

 * *Files identical despite different names*

### Comparing `sonia-0.2.1/sonia/default_models/human_B_kappa/V_gene_CDR3_anchors.csv` & `sonia-0.2.2/sonia/default_models/human_B_kappa/V_gene_CDR3_anchors.csv`

 * *Files identical despite different names*

### Comparing `sonia-0.2.1/sonia/default_models/human_B_kappa/features.tsv` & `sonia-0.2.2/sonia/default_models/human_B_kappa/features.tsv`

 * *Files identical despite different names*

### Comparing `sonia-0.2.1/sonia/default_models/human_B_kappa/model_marginals.txt` & `sonia-0.2.2/sonia/default_models/human_B_kappa/model_marginals.txt`

 * *Files identical despite different names*

### Comparing `sonia-0.2.1/sonia/default_models/human_B_kappa/model_params.txt` & `sonia-0.2.2/sonia/default_models/human_B_kappa/model_params.txt`

 * *Files identical despite different names*

### Comparing `sonia-0.2.1/sonia/default_models/human_B_lambda/V_gene_CDR3_anchors.csv` & `sonia-0.2.2/sonia/default_models/human_B_lambda/V_gene_CDR3_anchors.csv`

 * *Files identical despite different names*

### Comparing `sonia-0.2.1/sonia/default_models/human_B_lambda/features.tsv` & `sonia-0.2.2/sonia/default_models/human_B_lambda/features.tsv`

 * *Files identical despite different names*

### Comparing `sonia-0.2.1/sonia/default_models/human_B_lambda/model_marginals.txt` & `sonia-0.2.2/sonia/default_models/human_B_lambda/model_marginals.txt`

 * *Files identical despite different names*

### Comparing `sonia-0.2.1/sonia/default_models/human_B_lambda/model_params.txt` & `sonia-0.2.2/sonia/default_models/human_B_lambda/model_params.txt`

 * *Files identical despite different names*

### Comparing `sonia-0.2.1/sonia/default_models/human_T_alpha/J_gene_CDR3_anchors.csv` & `sonia-0.2.2/sonia/default_models/human_T_alpha/J_gene_CDR3_anchors.csv`

 * *Files identical despite different names*

### Comparing `sonia-0.2.1/sonia/default_models/human_T_alpha/V_gene_CDR3_anchors.csv` & `sonia-0.2.2/sonia/default_models/human_T_alpha/V_gene_CDR3_anchors.csv`

 * *Files identical despite different names*

### Comparing `sonia-0.2.1/sonia/default_models/human_T_alpha/features.tsv` & `sonia-0.2.2/sonia/default_models/human_T_alpha/features.tsv`

 * *Files identical despite different names*

### Comparing `sonia-0.2.1/sonia/default_models/human_T_alpha/model_marginals.txt` & `sonia-0.2.2/sonia/default_models/human_T_alpha/model_marginals.txt`

 * *Files identical despite different names*

### Comparing `sonia-0.2.1/sonia/default_models/human_T_alpha/model_params.txt` & `sonia-0.2.2/sonia/default_models/human_T_alpha/model_params.txt`

 * *Files identical despite different names*

### Comparing `sonia-0.2.1/sonia/default_models/human_T_beta/V_gene_CDR3_anchors.csv` & `sonia-0.2.2/sonia/default_models/human_T_beta/V_gene_CDR3_anchors.csv`

 * *Files identical despite different names*

### Comparing `sonia-0.2.1/sonia/default_models/human_T_beta/features.tsv` & `sonia-0.2.2/sonia/default_models/human_T_beta/features.tsv`

 * *Files identical despite different names*

### Comparing `sonia-0.2.1/sonia/default_models/human_T_beta/model_marginals.txt` & `sonia-0.2.2/sonia/default_models/human_T_beta/model_marginals.txt`

 * *Files identical despite different names*

### Comparing `sonia-0.2.1/sonia/default_models/human_T_beta/model_params.txt` & `sonia-0.2.2/sonia/default_models/human_T_beta/model_params.txt`

 * *Files identical despite different names*

### Comparing `sonia-0.2.1/sonia/default_models/mouse_T_alpha/J_gene_CDR3_anchors.csv` & `sonia-0.2.2/sonia/default_models/mouse_T_alpha/J_gene_CDR3_anchors.csv`

 * *Files identical despite different names*

### Comparing `sonia-0.2.1/sonia/default_models/mouse_T_alpha/V_gene_CDR3_anchors.csv` & `sonia-0.2.2/sonia/default_models/mouse_T_alpha/V_gene_CDR3_anchors.csv`

 * *Files identical despite different names*

### Comparing `sonia-0.2.1/sonia/default_models/mouse_T_alpha/features.tsv` & `sonia-0.2.2/sonia/default_models/mouse_T_alpha/features.tsv`

 * *Files identical despite different names*

### Comparing `sonia-0.2.1/sonia/default_models/mouse_T_alpha/model_marginals.txt` & `sonia-0.2.2/sonia/default_models/mouse_T_alpha/model_marginals.txt`

 * *Files identical despite different names*

### Comparing `sonia-0.2.1/sonia/default_models/mouse_T_alpha/model_params.txt` & `sonia-0.2.2/sonia/default_models/mouse_T_alpha/model_params.txt`

 * *Files identical despite different names*

### Comparing `sonia-0.2.1/sonia/default_models/mouse_T_beta/features.tsv` & `sonia-0.2.2/sonia/default_models/mouse_T_beta/features.tsv`

 * *Files identical despite different names*

### Comparing `sonia-0.2.1/sonia/default_models/mouse_T_beta/model_marginals.txt` & `sonia-0.2.2/sonia/default_models/mouse_T_beta/model_marginals.txt`

 * *Files identical despite different names*

### Comparing `sonia-0.2.1/sonia/default_models/mouse_T_beta/model_params.txt` & `sonia-0.2.2/sonia/default_models/mouse_T_beta/model_params.txt`

 * *Files identical despite different names*

### Comparing `sonia-0.2.1/sonia/evaluate.py` & `sonia-0.2.2/sonia/evaluate.py`

 * *Files 1% similar despite different names*

```diff
@@ -405,29 +405,29 @@
                     if options.ppost:
                         Q,pgen,ppost=ev.evaluate_seqs(t)
                         for i in range(len(Q)):file.write(str(Q[i])+delimiter_out+str(pgen[i])+delimiter_out+str(ppost[i])+'\n')
                     elif options.Q:
                         Q=ev.evaluate_selection_factors(t)
                         for i in range(len(Q)):file.write(str(Q[i])+'\n')
                     elif options.pgen:
-                        pgens=ev.compute_all_pgens(t)
+                        pgens=ev.compute_all_pgens(t)/ev.sonia_model.norm_productive
                         for i in range(len(pgens)):file.write(str(pgens[i])+'\n')
 
         else: #print to stdout
             for t in chunks(zipped,options.chunck_size):
                 if options.ppost:
                     Q,pgen,ppost=ev.evaluate_seqs(t)
                     print ('Q, Pgen, Ppost')
                     for i in range(len(Q)):print(Q[i],pgen[i],ppost[i])
                 elif options.Q:
                     Q=ev.evaluate_selection_factors(t)
                     print ('Q')
                     print(Q)
                 elif options.pgen:
-                    pgens=ev.compute_all_pgens(t)
+                    pgens=ev.compute_all_pgens(t)/ev.sonia_model.norm_productive
                     print ('Pgen')
                     print(pgens)
                 else:
                     print('Specify one option: --ppost, --pgen or --Q')
 
 
-if __name__ == '__main__': main()
+if __name__ == '__main__': main()
```

### Comparing `sonia-0.2.1/sonia/evaluate_model.py` & `sonia-0.2.2/sonia/evaluate_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 import numpy as np
 import os
 import multiprocessing as mp
 import olga.load_model as olga_load_model
 import olga.generation_probability as pgen
 from sonia.utils import compute_pgen_expand,compute_pgen_expand_novj,partial_joint_marginals
 import itertools
+
 class EvaluateModel(object):
     """Class used to evaluate sequences with the sonia model: Ppost=Q*Pgen
 
 
     Attributes
     ----------
     sonia_model: object
@@ -289,15 +290,15 @@
         energies =self.sonia_model.compute_energy(seq_features) # compute energies
         Q= np.exp(-energies)/self.sonia_model.Z # compute Q
         pgens=self.compute_all_pgens(seqs)/self.sonia_model.norm_productive # compute pgen
         pposts=pgens*Q # compute ppost
         self.entropy=-np.mean(Q*np.log2(pposts))
         return self.entropy
     
-    def DklPostGen(self,seqs=None,n=int(1e5)):
+    def dkl_post_gen(self,seqs=None,n=int(1e5)):
         '''Compute D_KL(P_post|P_gen)
 
         Returns
         -------
         dkl: float
             D_KL(P_post|P_gen)
```

### Comparing `sonia-0.2.1/sonia/generate.py` & `sonia-0.2.2/sonia/generate.py`

 * *Files identical despite different names*

### Comparing `sonia-0.2.1/sonia/infer.py` & `sonia-0.2.2/sonia/infer.py`

 * *Files identical despite different names*

### Comparing `sonia-0.2.1/sonia/plotting.py` & `sonia-0.2.2/sonia/plotting.py`

 * *Files 1% similar despite different names*

```diff
@@ -383,21 +383,21 @@
             File name to save output figure. If None (default) does not save.
 
         """
         try:
             self.sonia_model.energies_gen
             self.sonia_model.energies_data
         except:
-            self.sonia_model.energies_gen=self.sonia_model.compute_energy(self.sonia_model.gen_seq_features)+np.log(self.sonia_model.Z)
-            self.sonia_model.energies_data=self.sonia_model.compute_energy(self.sonia_model.data_seq_features)+np.log(self.sonia_model.Z)
+            self.sonia_model.energies_gen=self.sonia_model.compute_energy(self.sonia_model.gen_seq_features)
+            self.sonia_model.energies_data=self.sonia_model.compute_energy(self.sonia_model.data_seq_features)
         
         fig=plt.figure(figsize=(8,4))
         binning=np.linspace(-self.sonia_model.max_energy_clip-1,-self.sonia_model.min_energy_clip+1,100)
-        hist_gen,bins=np.histogram(-self.sonia_model.energies_gen,binning,density=True)
-        hist_data,bins=np.histogram(-self.sonia_model.energies_data,binning,density=True)
+        hist_gen,bins=np.histogram(-self.sonia_model.energies_gen-np.log(self.sonia_model.Z),binning,density=True)
+        hist_data,bins=np.histogram(-self.sonia_model.energies_data-np.log(self.sonia_model.Z),binning,density=True)
         plt.plot(bins[:-1],hist_gen,label='generated')
         plt.plot(bins[:-1],hist_data,label='data')
         plt.ylabel('density',fontsize=20)
         plt.xlabel('log Q',fontsize=20)
         plt.legend(fontsize=20)
         plt.tight_layout()
         if save_name is not None:
```

### Comparing `sonia-0.2.1/sonia/sequence_generation.py` & `sonia-0.2.2/sonia/sequence_generation.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,16 @@
 # -*- coding: utf-8 -*-
 # @author: Giulio Isacchini
 
 import numpy as np
 import os
 import olga.load_model as olga_load_model
 import olga.sequence_generation as seq_gen
+from sonia.utils import generate_sequence
+import multiprocessing as mp
 
 class SequenceGeneration(object):
 
     """Class used to evaluate sequences with the sonia model
 
     Attributes
     ----------
@@ -33,21 +35,23 @@
     
     rejection_sampling(upper_bound=10,energies=None)
         Returns acceptance from rejection sampling of a list of energies.
         By default uses the generated sequences within the sonia model.
 
     """
 
-    def __init__(self,sonia_model=None, custom_olga_model=None, custom_genomic_data=None):
+    def __init__(self,sonia_model=None, custom_olga_model=None, custom_genomic_data=None,processes=None):
 
         if type(sonia_model)==str or sonia_model is None: 
             print('ERROR: you need to pass a Sonia object')
             return
 
         self.sonia_model=sonia_model # sonia model passed as an argument
+        if processes is None: self.processes = mp.cpu_count()
+        else: self.processes = processes
 
         # define olga sequence_generation model
         if custom_olga_model is not None:
             if type(custom_olga_model)==str: 
                 print('ERROR: you need to pass a olga object for the seq_gen model')
                 return
 
@@ -80,16 +84,16 @@
             else:
                 self.genomic_data = olga_load_model.GenomicDataVJ()
                 self.genomic_data.load_igor_genomic_data(params_file_name, V_anchor_pos_file, J_anchor_pos_file)
                 self.generative_model = olga_load_model.GenerativeModelVJ()
                 self.generative_model.load_and_process_igor_model(marginals_file_name)   
                 self.seq_gen_model = seq_gen.SequenceGenerationVJ(self.generative_model, self.genomic_data)
 
-    def generate_sequences_pre(self, num_seqs = 1, nucleotide=True):
-        """Generates MonteCarlo sequences for gen_seqs using OLGA.
+    def generate_sequences_pre(self, num_seqs = 1, nucleotide=True,custom_seq_gen_model=None,custom_genomic_data=None):
+        """Generates MonteCarlo sequences for gen_seqs using OLGA in parallel.
 
         Only generates seqs from a V(D)J model. Requires the OLGA package
         (pip install olga).
 
         Parameters
         ----------
         num_seqs : int or float
@@ -99,19 +103,30 @@
         Returns
         --------------
         seqs : list
             MonteCarlo sequences drawn from a VDJ recomb model
 
         """
         
-        #Generate sequences
-        seqs_generated=[self.seq_gen_model.gen_rnd_prod_CDR3(conserved_J_residues='ABCEDFGHIJKLMNOPQRSTUVWXYZ') for i in range(int(num_seqs))]
-        if nucleotide: seqs= [[seq[1], self.genomic_data.genV[seq[2]][0].split('*')[0], self.genomic_data.genJ[seq[3]][0].split('*')[0],seq[0]] for seq in seqs_generated]
-        else: seqs = [[seq[1], self.genomic_data.genV[seq[2]][0].split('*')[0], self.genomic_data.genJ[seq[3]][0].split('*')[0]] for seq in seqs_generated]
-        return seqs
+        if custom_seq_gen_model is None: final_models = [self.seq_gen_model for i in range(int(num_seqs))] 
+        else: final_models=[custom_seq_gen_model for i in range(int(num_seqs))] 
+        if custom_genomic_data is None: final_genomic_data = [self.genomic_data for i in range(int(num_seqs))] 
+        else: final_genomic_data = [self.genomic_data for i in range(int(num_seqs))] 
+        seeds=np.random.randint(2**32-1,size=num_seqs)
+        
+        pool = mp.Pool(processes=self.processes)
+        seqs=np.array(pool.map(generate_sequence, zip(final_models,final_genomic_data,seeds)))
+        pool.close()
+        if nucleotide: return seqs
+        else: return seqs[:,:-1] 
+
+        #seqs_generated=[self.seq_gen_model.gen_rnd_prod_CDR3(conserved_J_residues='ABCEDFGHIJKLMNOPQRSTUVWXYZ') for i in range(int(num_seqs))]
+        #if nucleotide: seqs= [[seq[1], self.genomic_data.genV[seq[2]][0].split('*')[0], self.genomic_data.genJ[seq[3]][0].split('*')[0],seq[0]] for seq in seqs_generated]
+        #else: seqs = [[seq[1], self.genomic_data.genV[seq[2]][0].split('*')[0], self.genomic_data.genJ[seq[3]][0].split('*')[0]] for seq in seqs_generated]
+        #return seqs
     
     def generate_sequences_post(self,num_seqs = 1,upper_bound=10,nucleotide=True):
         """Generates MonteCarlo sequences from Sonia through rejection sampling.
 
         Parameters
         ----------
         num_seqs : int or float
```

### Comparing `sonia-0.2.1/sonia/sonia.py` & `sonia-0.2.2/sonia/sonia.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,24 +139,25 @@
         self.gamma=1.
         self.Z=1.
         default_chain_types = { 'humanTRA': 'human_T_alpha', 'human_T_alpha': 'human_T_alpha', 
                                 'humanTRB': 'human_T_beta', 'human_T_beta': 'human_T_beta', 
                                 'humanIGH': 'human_B_heavy', 'human_B_heavy': 'human_B_heavy', 
                                 'humanIGK': 'human_B_kappa', 'human_B_kappa': 'human_B_kappa', 
                                 'humanIGL': 'human_B_lambda', 'human_B_lambda': 'human_B_lambda', 
-                                'mouseTRB': 'mouse_T_beta', 'mouse_T_beta': 'mouse_T_beta'}
+                                'mouseTRB': 'mouse_T_beta', 'mouse_T_beta': 'mouse_T_beta',
+                                'mouseTRA': 'mouse_T_alpha','mouse_T_alpha':'mouse_T_alpha'}
         if chain_type not in default_chain_types.keys():
-            print('Unrecognized chain_type (not a default OLGA model). Please specify one of the following options: humanTRA, humanTRB, humanIGH, humanIGK, humanIGL or mouseTRB.')
+            print('Unrecognized chain_type (not a default OLGA model). Please specify one of the following options: humanTRA, humanTRB, humanIGH, humanIGK, humanIGL, mouseTRB or mouseTRA.')
             return None
         self.chain_type = default_chain_types[chain_type]
         self.vj=vj
         if self.chain_type in ['human_T_alpha','human_B_kappa','human_B_lambda','mouse_T_alpha']: self.vj=True
 
         norms={'human_T_beta':0.2442847269027897,'human_T_alpha':0.2847166577727317,'human_B_heavy': 0.1499265655936305, 
-                'human_B_lambda':0.29489499727399304, 'human_B_kappa':0.29247125650320943, 'mouse_T_beta':0.2727148540013573}
+                'human_B_lambda':0.29489499727399304, 'human_B_kappa':0.29247125650320943, 'mouse_T_beta':0.2727148540013573,'mouse_T_alpha':0.321870924914448}
         self.norm_productive=norms[self.chain_type]
 
         if any([x is not None for x in [load_dir, feature_file, model_file]]):
             self.load_model(load_dir = load_dir, feature_file = feature_file, model_file = model_file, data_seq_file = data_seq_file, gen_seq_file = gen_seq_file, log_file = log_file, load_seqs = load_seqs)
             if len(self.data_seqs) == 0: self.update_model(add_data_seqs = data_seqs)
             if len(self.gen_seqs) == 0: self.update_model(add_data_seqs = gen_seqs)
         else:
@@ -539,15 +540,15 @@
             self.gen_seq_features = [self.find_seq_features(seq) for seq in tqdm(self.gen_seqs)]
 
 
         if (len(add_gen_seqs + add_features + remove_features) > 0 or auto_update_marginals) and len(self.features)>0:
             self.gen_marginals = self.compute_marginals(seq_model_features = self.gen_seq_features, use_flat_distribution = True)
             self.model_marginals = self.compute_marginals(seq_model_features = self.gen_seq_features)
 
-    def add_generated_seqs(self, num_gen_seqs = 0, reset_gen_seqs = True, custom_model_folder = None, add_error=False,custom_error=None):
+    def add_generated_seqs(self, num_gen_seqs = 0, reset_gen_seqs = True, custom_model_folder = None, add_error=False,custom_error=None,processes=None):
         """Generates MonteCarlo sequences for gen_seqs using OLGA.
 
         Only generates seqs from a V(D)J model. Requires the OLGA package
         (pip install olga).
 
         Parameters
         ----------
@@ -568,16 +569,17 @@
         --------------
         gen_seqs : list
             MonteCarlo sequences drawn from a VDJ recomb model
         gen_seq_features : list
             Features gen_seqs have been projected onto.
 
         """
-        from sonia.utils import add_random_error
+        from sonia.utils import add_random_error,generate_sequence
         from olga.utils import nt2aa
+        import multiprocessing as mp
 
         #Load generative model
         if custom_model_folder is None:
             try:
                 if self.custom_pgen_model is None: main_folder = os.path.join(os.path.dirname(__file__), 'default_models', self.chain_type)
                 else: main_folder=self.custom_pgen_model
             except:
@@ -621,16 +623,27 @@
             genomic_data.load_igor_genomic_data(params_file_name, V_anchor_pos_file, J_anchor_pos_file)
             generative_model = olga_load_model.GenerativeModelVDJ()
             generative_model.load_and_process_igor_model(marginals_file_name)
             sg_model = seq_gen.SequenceGenerationVDJ(generative_model, genomic_data)
 
         #Generate sequences
         print('Generate sequences.')
-        if add_error: seqs = [[nt2aa(add_random_error(seq[0],self.error_rate)), genomic_data.genV[seq[2]][0].split('*')[0], genomic_data.genJ[seq[3]][0].split('*')[0]] for seq in [sg_model.gen_rnd_prod_CDR3(conserved_J_residues='ABCEDFGHIJKLMNOPQRSTUVWXYZ') for _ in tqdm(range(int(num_gen_seqs)))]]
-        else: seqs = [[seq[1], genomic_data.genV[seq[2]][0].split('*')[0], genomic_data.genJ[seq[3]][0].split('*')[0]] for seq in [sg_model.gen_rnd_prod_CDR3(conserved_J_residues='ABCEDFGHIJKLMNOPQRSTUVWXYZ') for _ in tqdm(range(int(num_gen_seqs)))]]
+        if processes is None: processes = mp.cpu_count()
+
+        final_models = [sg_model for i in range(int(num_gen_seqs))] 
+        final_genomic_data = [genomic_data for i in range(int(num_gen_seqs))] 
+        seeds=np.random.randint(2**32-1,size=num_gen_seqs)
+
+        pool = mp.Pool(processes=processes)
+        seqs_=np.array(pool.map(generate_sequence, zip(final_models,final_genomic_data,seeds)))
+        pool.close()
+
+
+        if add_error: seqs = [[nt2aa(add_random_error(seq[-1],self.error_rate)), seq[1], seq[2]] for seq in seqs]
+        else: seqs = list(seqs_[:,:-1])
         if reset_gen_seqs: #reset gen_seqs if needed
             self.gen_seqs = []
         #Add to specified pool(s)
         self.update_model(add_gen_seqs = seqs)
 
     def save_model(self, save_dir, attributes_to_save = None,force=True):
         """Saves model parameters and sequences
```

### Comparing `sonia-0.2.1/sonia/sonia_leftpos_rightpos.py` & `sonia-0.2.2/sonia/sonia_leftpos_rightpos.py`

 * *Files 0% similar despite different names*

```diff
@@ -260,16 +260,16 @@
 
         if 'model' in attributes_to_save:
             model_energy_dict = self.get_energy_parameters(return_as_dict = True)
             with open(os.path.join(save_dir, 'features.tsv'), 'w') as feature_file:
                 feature_file.write('Feature,Energy,Marginal_data,Marginal_model,Marginal_gen\n')
                 for i in range(len(self.features)):
                     feature_file.write(';'.join(self.features[i])+','+ str(model_energy_dict[tuple(self.features[i])])+','+str(self.data_marginals[i])+','+str(self.model_marginals[i])+','+str(self.gen_marginals[i])+'\n')
-            #self.model.save(os.path.join(save_dir, 'model.h5'))
-                #save pgen model too.
+            self.model.save(os.path.join(save_dir, 'model.h5'))
+        #save pgen model too.
         try:
             if self.custom_pgen_model is None: main_folder = os.path.join(os.path.dirname(__file__), 'default_models', self.chain_type)
             else: main_folder=self.custom_pgen_model
         except:
             main_folder = os.path.join(os.path.dirname(__file__), 'default_models', self.chain_type)
         shutil.copy2(os.path.join(main_folder,'model_params.txt'),save_dir)
         shutil.copy2(os.path.join(main_folder,'model_marginals.txt'),save_dir)
```

### Comparing `sonia-0.2.1/sonia/sonia_length_pos.py` & `sonia-0.2.2/sonia/sonia_length_pos.py`

 * *Files 0% similar despite different names*

```diff
@@ -240,15 +240,15 @@
                     L1_file.write(str(self.likelihood_train[i])+','+str(self.likelihood_test[i])+'\n')
 
         if 'model' in attributes_to_save:
             model_energy_dict = self.get_energy_parameters(return_as_dict = True)
             with open(os.path.join(save_dir, 'features.tsv'), 'w') as feature_file:
                 feature_file.write('Feature\tEnergy\n')
                 feature_file.write('\n'.join([';'.join(f) + '\t' + str(model_energy_dict[tuple(f)]) for f in self.features]))
-            #self.model.save(os.path.join(save_dir, 'model.h5'))
+            self.model.save(os.path.join(save_dir, 'model.h5'))
 
         return None
 
     def _load_features_and_model(self, feature_file, model_file = None, verbose = True):
         """Loads left+right features and sets up model.
 
         Ignores model_file.
```

### Comparing `sonia-0.2.1/sonia/sonia_vjl.py` & `sonia-0.2.2/sonia/sonia_vjl.py`

 * *Files identical despite different names*

### Comparing `sonia-0.2.1/sonia/utils.py` & `sonia-0.2.2/sonia/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -47,28 +47,38 @@
     # compute pgen conditioned on gene usage
     return x[1].compute_aa_CDR3_pgen(x[0][0],x[0][1],x[0][2])
 
 def compute_pgen_expand_novj(x):
     # compute pgen unconditioned on gene usage
     return x[1].compute_aa_CDR3_pgen(x[0][0])
 
+def generate_sequence(x):
+    seq_gen_model=x[0]
+    genomic_data=x[1]
+    np.random.seed(x[2])
+    seq=seq_gen_model.gen_rnd_prod_CDR3(conserved_J_residues='ABCEDFGHIJKLMNOPQRSTUVWXYZ')
+    return [seq[1], genomic_data.genV[seq[2]][0].split('*')[0], genomic_data.genJ[seq[3]][0].split('*')[0],seq[0]]
+
 def partial_joint_marginals(args):
     # compute joint marginals on subset of seqs.
     features = args[0]
     Qs = args[1]
     marginals=args[2]
     l=int(np.sqrt(len(marginals)))
     Z=0
     for seq_features,Q in zip(features,Qs):
         for i,j in itertools.combinations(np.array(seq_features),2):
             if i>j:marginals[i,j] += Q
             else: marginals[j,i] += Q
         Z += Q
     return [marginals,Z]
 
+def parallel_function(x):
+    return x[0](x[1])
+
 class computeL1(Callback):
     # compute L1 distance at the end of each epoch of the inference.
 
     def __init__(self, sonia):
         self.data_marginals = sonia.data_marginals
         self.sonia=sonia
         self.len_features=len(sonia.features)
```

### Comparing `sonia-0.2.1/sonia.egg-info/PKG-INFO` & `sonia-0.2.2/sonia.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sonia
-Version: 0.2.1
+Version: 0.2.2
 Summary: SONIA is a python 3.6 software developed to infer selection pressures on features of amino acid CDR3 sequences. The model can be used to calculate the probability of observing any sequence after selection and sample from the selected repertoire.
 Author: Zachary Sethna
 Author-email: Giulio Isacchini <giulioisac@gmail.com>
 Maintainer-email: Giulio Isacchini <giulioisac@gmail.com>
 License: GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
@@ -697,40 +697,41 @@
 Requires-Dist: tensorflow>=2.1.0
 Requires-Dist: matplotlib
 Requires-Dist: olga>=1.1.3
 Requires-Dist: tqdm
 
 # SONIA
 
+This Package is not actively mantained, please refer to the most updated SoNNia package which includes sonia models as well: https://github.com/statbiophys/soNNia
+
 SONIA is a python 3.6/2.7 software developed to infer selection pressures on features of amino acid CDR3 sequences. The inference is based on maximizing the likelihood of observing a selected data sample given a representative pre-selected sample. This method was first used in Elhanati et al (2014) to study thymic selection. For this purpose, the pre-selected sample can be generated internally using the OLGA software package, but SONIA allows it also to be supplied externally, in the same way the data sample is provided.
 
 ![](docs/source/model.png)
 
 SONIA takes as input TCR CDR3 amino acid sequences, with or without per sequence lists of possible V and J genes suspected to be used in the recombination process for this sequence. Its output is selection factors for each amino acid ,(relative) position , CDR3 length combinations, and also for each V and J gene choice. These selection factors can be used to calculate sequence level selection factors which indicate how more or less represented this sequence would be in the selected pool as compared to the the pre-selected pool. These in turn could be used to calculate the probability to observe any sequence after selection and sample from the selected repertoire. 
 
 ![](docs/source/workflow.png)
 ## Version
-Latest released version: 0.0.45
+Latest released version: 0.2.2
 
 ## Installation
 SONIA is a python 2.7/3.6 software. It is available on PyPI and can be downloaded and installed through pip:
 
  ```pip install sonia```.
 
-SONIA is also available on [GitHub](https://github.com/statbiophys/SONIA). The command line entry points can be installed by using the setup.py script:
-
- ```python setup.py install```.
+SONIA is also available on [GitHub](https://github.com/statbiophys/SONIA).
  
 Sometimes pip fails to install the dependencies correctly. Thus, if you get any error try first to install the dependencies separately:
  ```
 pip install tensorflow
 pip install matplotlib
 pip install olga
 pip install sonia 
  ```
+For mac user on new metal devices, make sure to install additional dependencies. Currently, the configuration tensorflow-macos==2.9 and tensorflow-metal==0.5.0 should work.
 
 ## References
 
 1. Sethna Z, Isacchini G, Dupic T, Mora T, Walczak AM, Elhanati Y, Population variability in the generation and thymic selection of T-cell repertoires, (2020) bioRxiv, https://doi.org/10.1101/2020.01.08.899682
 2. Isacchini G, Sethna Z, Elhanati Y ,Nourmohammad A, Mora T, Walczak AM, Generative models of T-cell receptor sequences, (2020) Phys. Rev. E 101, 062414, https://journals.aps.org/pre/abstract/10.1103/PhysRevE.101.062414
 3. Elhanati Y, Murugan A , Callan CGJ ,  Mora T , Walczak AM, Quantifying selection in immune receptor repertoires, PNAS July 8, 2014 111 (27) 9875-9880, https://doi.org/10.1073/pnas.1409572111
```

### Comparing `sonia-0.2.1/sonia.egg-info/SOURCES.txt` & `sonia-0.2.2/sonia.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -20,45 +20,52 @@
 sonia.egg-info/entry_points.txt
 sonia.egg-info/requires.txt
 sonia.egg-info/top_level.txt
 sonia/default_models/human_B_heavy/J_gene_CDR3_anchors.csv
 sonia/default_models/human_B_heavy/V_gene_CDR3_anchors.csv
 sonia/default_models/human_B_heavy/features.tsv
 sonia/default_models/human_B_heavy/log.txt
+sonia/default_models/human_B_heavy/model.h5
 sonia/default_models/human_B_heavy/model_marginals.txt
 sonia/default_models/human_B_heavy/model_params.txt
 sonia/default_models/human_B_kappa/J_gene_CDR3_anchors.csv
 sonia/default_models/human_B_kappa/V_gene_CDR3_anchors.csv
 sonia/default_models/human_B_kappa/features.tsv
 sonia/default_models/human_B_kappa/log.txt
+sonia/default_models/human_B_kappa/model.h5
 sonia/default_models/human_B_kappa/model_marginals.txt
 sonia/default_models/human_B_kappa/model_params.txt
 sonia/default_models/human_B_lambda/J_gene_CDR3_anchors.csv
 sonia/default_models/human_B_lambda/V_gene_CDR3_anchors.csv
 sonia/default_models/human_B_lambda/features.tsv
 sonia/default_models/human_B_lambda/log.txt
+sonia/default_models/human_B_lambda/model.h5
 sonia/default_models/human_B_lambda/model_marginals.txt
 sonia/default_models/human_B_lambda/model_params.txt
 sonia/default_models/human_T_alpha/J_gene_CDR3_anchors.csv
 sonia/default_models/human_T_alpha/V_gene_CDR3_anchors.csv
 sonia/default_models/human_T_alpha/features.tsv
 sonia/default_models/human_T_alpha/log.txt
+sonia/default_models/human_T_alpha/model.h5
 sonia/default_models/human_T_alpha/model_marginals.txt
 sonia/default_models/human_T_alpha/model_params.txt
 sonia/default_models/human_T_beta/J_gene_CDR3_anchors.csv
 sonia/default_models/human_T_beta/V_gene_CDR3_anchors.csv
 sonia/default_models/human_T_beta/features.tsv
 sonia/default_models/human_T_beta/log.txt
+sonia/default_models/human_T_beta/model.h5
 sonia/default_models/human_T_beta/model_marginals.txt
 sonia/default_models/human_T_beta/model_params.txt
 sonia/default_models/mouse_T_alpha/J_gene_CDR3_anchors.csv
 sonia/default_models/mouse_T_alpha/V_gene_CDR3_anchors.csv
 sonia/default_models/mouse_T_alpha/features.tsv
 sonia/default_models/mouse_T_alpha/log.txt
+sonia/default_models/mouse_T_alpha/model.h5
 sonia/default_models/mouse_T_alpha/model_marginals.txt
 sonia/default_models/mouse_T_alpha/model_params.txt
 sonia/default_models/mouse_T_beta/J_gene_CDR3_anchors.csv
 sonia/default_models/mouse_T_beta/V_gene_CDR3_anchors.csv
 sonia/default_models/mouse_T_beta/features.tsv
 sonia/default_models/mouse_T_beta/log.txt
+sonia/default_models/mouse_T_beta/model.h5
 sonia/default_models/mouse_T_beta/model_marginals.txt
 sonia/default_models/mouse_T_beta/model_params.txt
```

