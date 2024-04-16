# Comparing `tmp/bicleaner-ai-2.3.2.tar.gz` & `tmp/bicleaner_ai-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bicleaner-ai-2.3.2.tar", last modified: Mon Aug 21 15:08:33 2023, max compression
+gzip compressed data, was "bicleaner_ai-3.0.0.tar", last modified: Tue Apr 16 14:12:40 2024, max compression
```

## Comparing `bicleaner-ai-2.3.2.tar` & `bicleaner_ai-3.0.0.tar`

### file list

```diff
@@ -1,35 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-21 15:08:33.213195 bicleaner-ai-2.3.2/
--rw-r--r--   0 runner    (1001) docker     (122)    35147 2023-08-21 15:08:23.000000 bicleaner-ai-2.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)    65922 2023-08-21 15:08:33.213195 bicleaner-ai-2.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    24441 2023-08-21 15:08:23.000000 bicleaner-ai-2.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (122)     2037 2023-08-21 15:08:23.000000 bicleaner-ai-2.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-08-21 15:08:33.213195 bicleaner-ai-2.3.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-21 15:08:33.209195 bicleaner-ai-2.3.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-21 15:08:33.213195 bicleaner-ai-2.3.2/src/bicleaner_ai/
--rwxr-xr-x   0 runner    (1001) docker     (122)      112 2023-08-21 15:08:23.000000 bicleaner-ai-2.3.2/src/bicleaner_ai/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     4547 2023-08-21 15:08:23.000000 bicleaner-ai-2.3.2/src/bicleaner_ai/bicleaner_ai_classifier.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     4467 2023-08-21 15:08:23.000000 bicleaner-ai-2.3.2/src/bicleaner_ai/bicleaner_ai_download.py
--rwxr-xr-x   0 runner    (1001) docker     (122)      642 2023-08-21 15:08:23.000000 bicleaner-ai-2.3.2/src/bicleaner_ai/bicleaner_ai_download_hf.py
--rwxr-xr-x   0 runner    (1001) docker     (122)    16502 2023-08-21 15:08:23.000000 bicleaner-ai-2.3.2/src/bicleaner_ai/bicleaner_ai_train.py
--rw-r--r--   0 runner    (1001) docker     (122)     2964 2023-08-21 15:08:23.000000 bicleaner-ai-2.3.2/src/bicleaner_ai/calibrate.py
--rw-r--r--   0 runner    (1001) docker     (122)    14118 2023-08-21 15:08:23.000000 bicleaner-ai-2.3.2/src/bicleaner_ai/classify.py
--rw-r--r--   0 runner    (1001) docker     (122)     6479 2023-08-21 15:08:23.000000 bicleaner-ai-2.3.2/src/bicleaner_ai/datagen.py
--rw-r--r--   0 runner    (1001) docker     (122)     7456 2023-08-21 15:08:23.000000 bicleaner-ai-2.3.2/src/bicleaner_ai/decomposable_attention.py
--rw-r--r--   0 runner    (1001) docker     (122)     3927 2023-08-21 15:08:23.000000 bicleaner-ai-2.3.2/src/bicleaner_ai/layers.py
--rw-r--r--   0 runner    (1001) docker     (122)     2283 2023-08-21 15:08:23.000000 bicleaner-ai-2.3.2/src/bicleaner_ai/losses.py
--rw-r--r--   0 runner    (1001) docker     (122)     6372 2023-08-21 15:08:23.000000 bicleaner-ai-2.3.2/src/bicleaner_ai/metrics.py
--rw-r--r--   0 runner    (1001) docker     (122)    25236 2023-08-21 15:08:23.000000 bicleaner-ai-2.3.2/src/bicleaner_ai/models.py
--rw-r--r--   0 runner    (1001) docker     (122)     4101 2023-08-21 15:08:23.000000 bicleaner-ai-2.3.2/src/bicleaner_ai/models_util.py
--rw-r--r--   0 runner    (1001) docker     (122)     1197 2023-08-21 15:08:23.000000 bicleaner-ai-2.3.2/src/bicleaner_ai/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (122)    13140 2023-08-21 15:08:23.000000 bicleaner-ai-2.3.2/src/bicleaner_ai/training.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     4004 2023-08-21 15:08:23.000000 bicleaner-ai-2.3.2/src/bicleaner_ai/util.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     1351 2023-08-21 15:08:23.000000 bicleaner-ai-2.3.2/src/bicleaner_ai/word_freqs_list.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     3123 2023-08-21 15:08:23.000000 bicleaner-ai-2.3.2/src/bicleaner_ai/word_freqs_zipf.py
--rwxr-xr-x   0 runner    (1001) docker     (122)     1082 2023-08-21 15:08:23.000000 bicleaner-ai-2.3.2/src/bicleaner_ai/word_freqs_zipf_double_linked.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-08-21 15:08:33.213195 bicleaner-ai-2.3.2/src/bicleaner_ai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    65922 2023-08-21 15:08:33.000000 bicleaner-ai-2.3.2/src/bicleaner_ai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      950 2023-08-21 15:08:33.000000 bicleaner-ai-2.3.2/src/bicleaner_ai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-08-21 15:08:33.000000 bicleaner-ai-2.3.2/src/bicleaner_ai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      276 2023-08-21 15:08:33.000000 bicleaner-ai-2.3.2/src/bicleaner_ai.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      291 2023-08-21 15:08:33.000000 bicleaner-ai-2.3.2/src/bicleaner_ai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       13 2023-08-21 15:08:33.000000 bicleaner-ai-2.3.2/src/bicleaner_ai.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:12:40.500031 bicleaner_ai-3.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-04-16 14:12:34.000000 bicleaner_ai-3.0.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    57475 2024-04-16 14:12:40.500031 bicleaner_ai-3.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15362 2024-04-16 14:12:34.000000 bicleaner_ai-3.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-04-16 14:12:34.000000 bicleaner_ai-3.0.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 14:12:40.500031 bicleaner_ai-3.0.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:12:40.492031 bicleaner_ai-3.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:12:40.500031 bicleaner_ai-3.0.0/src/bicleaner_ai/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      112 2024-04-16 14:12:34.000000 bicleaner_ai-3.0.0/src/bicleaner_ai/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4586 2024-04-16 14:12:34.000000 bicleaner_ai-3.0.0/src/bicleaner_ai/bicleaner_ai_classifier.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4458 2024-04-16 14:12:34.000000 bicleaner_ai-3.0.0/src/bicleaner_ai/bicleaner_ai_download.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      642 2024-04-16 14:12:34.000000 bicleaner_ai-3.0.0/src/bicleaner_ai/bicleaner_ai_download_hf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-04-16 14:12:34.000000 bicleaner_ai-3.0.0/src/bicleaner_ai/bicleaner_ai_generate_train.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13857 2024-04-16 14:12:34.000000 bicleaner_ai-3.0.0/src/bicleaner_ai/bicleaner_ai_train.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2964 2024-04-16 14:12:34.000000 bicleaner_ai-3.0.0/src/bicleaner_ai/calibrate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15330 2024-04-16 14:12:34.000000 bicleaner_ai-3.0.0/src/bicleaner_ai/classify.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6479 2024-04-16 14:12:34.000000 bicleaner_ai-3.0.0/src/bicleaner_ai/datagen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7456 2024-04-16 14:12:34.000000 bicleaner_ai-3.0.0/src/bicleaner_ai/decomposable_attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3927 2024-04-16 14:12:34.000000 bicleaner_ai-3.0.0/src/bicleaner_ai/layers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-04-16 14:12:34.000000 bicleaner_ai-3.0.0/src/bicleaner_ai/losses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6372 2024-04-16 14:12:34.000000 bicleaner_ai-3.0.0/src/bicleaner_ai/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25856 2024-04-16 14:12:34.000000 bicleaner_ai-3.0.0/src/bicleaner_ai/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4101 2024-04-16 14:12:34.000000 bicleaner_ai-3.0.0/src/bicleaner_ai/models_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12203 2024-04-16 14:12:34.000000 bicleaner_ai-3.0.0/src/bicleaner_ai/noise_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-16 14:12:34.000000 bicleaner_ai-3.0.0/src/bicleaner_ai/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4744 2024-04-16 14:12:34.000000 bicleaner_ai-3.0.0/src/bicleaner_ai/training.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4249 2024-04-16 14:12:34.000000 bicleaner_ai-3.0.0/src/bicleaner_ai/util.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1351 2024-04-16 14:12:34.000000 bicleaner_ai-3.0.0/src/bicleaner_ai/word_freqs_list.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3123 2024-04-16 14:12:34.000000 bicleaner_ai-3.0.0/src/bicleaner_ai/word_freqs_zipf.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1082 2024-04-16 14:12:34.000000 bicleaner_ai-3.0.0/src/bicleaner_ai/word_freqs_zipf_double_linked.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:12:40.500031 bicleaner_ai-3.0.0/src/bicleaner_ai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    57475 2024-04-16 14:12:40.000000 bicleaner_ai-3.0.0/src/bicleaner_ai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-04-16 14:12:40.000000 bicleaner_ai-3.0.0/src/bicleaner_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 14:12:40.000000 bicleaner_ai-3.0.0/src/bicleaner_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-16 14:12:40.000000 bicleaner_ai-3.0.0/src/bicleaner_ai.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-16 14:12:40.000000 bicleaner_ai-3.0.0/src/bicleaner_ai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-16 14:12:40.000000 bicleaner_ai-3.0.0/src/bicleaner_ai.egg-info/top_level.txt
```

### Comparing `bicleaner-ai-2.3.2/LICENSE` & `bicleaner_ai-3.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `bicleaner-ai-2.3.2/PKG-INFO` & `bicleaner_ai-3.0.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bicleaner-ai
-Version: 2.3.2
+Version: 3.0.0
 Summary: Parallel corpus classifier, indicating the likelihood of a pair of sentences being mutual translations or not (neural version)
 Author-email: Prompsit Language Engineering <info@prompsit.com>
 Maintainer-email: Jaume Zaragoza <jzaragoza@prompsit.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
@@ -686,93 +686,93 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Text Processing :: Linguistic
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Text Processing :: Filters
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: transliterate
 License-File: LICENSE
+Requires-Dist: scikit-learn>=0.22.1
+Requires-Dist: PyYAML>=5.1.2
+Requires-Dist: numpy
+Requires-Dist: pytest
+Requires-Dist: toolwrapper
+Requires-Dist: joblib
+Requires-Dist: sacremoses
+Requires-Dist: bicleaner-hardrules==2.10.3
+Requires-Dist: sentencepiece
+Requires-Dist: protobuf==3.20.3
+Requires-Dist: tensorflow<2.16,>=2.6.5
+Requires-Dist: bicleaner-ai-glove==0.2.1
+Requires-Dist: fuzzywuzzy
+Requires-Dist: python-Levenshtein
+Requires-Dist: transformers==4.36.1
+Requires-Dist: huggingface-hub<0.23,>=0.22
+Requires-Dist: zstandard
+Requires-Dist: psutil
+Requires-Dist: regex
+Provides-Extra: transliterate
+Requires-Dist: cyrtranslit==1.1; extra == "transliterate"
 
 
 # Bicleaner AI
 
 ![License](https://img.shields.io/badge/License-GPLv3-blue.svg)
 
 Bicleaner AI (`bicleaner-ai-classify`) is a tool in Python that aims at detecting noisy sentence pairs in a parallel corpus. It
 indicates the likelihood of a pair of sentences being mutual translations (with a value near to 1) or not (with a value near to 0).
 Sentence pairs considered very noisy are scored with 0.
 
 Although a training tool (`bicleaner-ai-train`) is provided, you may want to use the available ready-to-use language packages.
 Please, use `bicleaner-ai-download` to download the latest language packages or visit the [Github releases](https://github.com/bitextor/bicleaner-ai-data/releases/latest) for lite models and [Hugging Face Hub](https://huggingface.co/bitextor) for full models since v2.0.
-Visit our [Wiki](https://github.com/bitextor/bicleaner-ai/wiki/How-to-train-your-Bicleaner-AI) for a detailed example on Bicleaner training.
+Visit our [docs](docs/TRAINING.md) for a detailed example on Bicleaner training.
 
-## Citation
-If you find Bicleaner AI useful, please consider citing the following paper:
+If you find Bicleaner AI useful, please consider [citing us](#citation).
 
-> J. Zaragoza-Bernabeu, M. Bañón, G. Ramírez-Sánchez, S. Ortiz-Rojas, \
-> "[Bicleaner AI: Bicleaner Goes Neural](https://aclanthology.org/2022.lrec-1.87/)", \
-> in *Proceedings of the 13th Language Resources and Evaluation Conference*. \
-> Marseille, France: Language Resources and Evaluation Conference, June 2022
+## What is New?
+### v3.0.0 Improving Multilinguality!
+New improved multilingual models for zero-shot classification.
 
-```latex
-@inproceedings{zaragoza-bernabeu-etal-2022-bicleaner,
-    title = {"Bicleaner {AI}: Bicleaner Goes Neural"},
-    author = {"Zaragoza-Bernabeu, Jaume  and
-      Ram{\'\i}rez-S{\'a}nchez, Gema  and
-      Ba{\~n}{\'o}n, Marta  and
-      Ortiz Rojas, Sergio"},
-    booktitle = {"Proceedings of the Thirteenth Language Resources and Evaluation Conference"},
-    month = jun,
-    year = {"2022"},
-    address = {"Marseille, France"},
-    publisher = {"European Language Resources Association"},
-    url = {"https://aclanthology.org/2022.lrec-1.87"},
-    pages = {"824--831"},
-    abstract = {"This paper describes the experiments carried out during the development of the latest version of Bicleaner, named Bicleaner AI, a tool that aims at detecting noisy sentences in parallel corpora. The tool, which now implements a new neural classifier, uses state-of-the-art techniques based on pre-trained transformer-based language models fine-tuned on a binary classification task. After that, parallel corpus filtering is performed, discarding the sentences that have lower probability of being mutual translations. Our experiments, based on the training of neural machine translation (NMT) with corpora filtered using Bicleaner AI for two different scenarios, show significant improvements in translation quality compared to the previous version of the tool which implemented a classifier based on Extremely Randomized Trees."},
-}
-```
+<details>
+<summary>Previous news</summary>
 
-## What is New?
+### v2.0.0, March 10, 2023
+Model accuracy improvements and HF integration! See [CHANGELOG](https://github.com/bitextor/bicleaner-ai/blob/v2.0/CHANGELOG.md).
+
+### v1.0.0, June 6 2021
 Bicleaner AI is a [Bicleaner](https://github.com/bitextor/bicleaner) fork that uses neural networks.
 It comes with two types of models, lite models for fast scoring and full models for high performance.
 Lite models use [A Decomposable Attention Model for Natural Language Inference (Parikh et al.)](https://arxiv.org/abs/1606.01933).
 Full models use fine-tuned XLMRoberta ([Unsupervised Cross-lingual Representation Learning at Scale](https://arxiv.org/abs/1911.02116)).
 
 The use of XLMRoberta and 1:10 positive to negative ratio were inspired in the winner of WMT20 Parallel Corpus Filtering Task paper ([Filtering noisy parallel corpus using transformers with proxy task learning](https://www.statmt.org/wmt20/pdf/2020.wmt-1.105.pdf)).
 
+</details>
+
 ## Installation & Requirements
-- Python >= 3.7
-- TensorFlow >= 2.6.5
-- CUDA 11.2 (for training and inference with full models)
+- Python >= 3.8
+- PIP >= 23.0
+- CUDA >=11.2 (for training and inference with full models)
 
 Bicleaner AI is written in Python and can be installed using `pip`.
 It also requires the [KenLM](https://github.com/kpu/kenlm) Python bindings with support for 7-gram language models.
-You can easily install it by running the following commands:
+Hardrules uses [FastSpell](https://github.com/mbanon/fastspell) that requires `cyhunspell` to be installed manually.
+You can easily install all the requirements by running the following commands:
 
 ```bash
-pip install bicleaner-ai
+pip install bicleaner-ai git+https://github.com/MSeal/cython_hunspell@2.0.3
 pip install --config-settings="--build-option=--max_order=7" https://github.com/kpu/kenlm/archive/master.zip
 ```
 
-Hardrules uses [FastSpell](https://github.com/mbanon/fastspell) that requires `python-dev` and `libhunspell-dev`:
-```bash
-sudo apt install python-dev libhunspell-dev
-```
-
-Hunspell dictionaries used by default are automatically installed.
-If you need to change default configuration for language identification, see https://github.com/mbanon/fastspell#configuration.
-
 After installation, three binary files (`bicleaner-ai-train`, `bicleaner-ai-classify`, `bicleaner-ai-download`) will be located in your `python/installation/prefix/bin` directory. This is usually `$HOME/.local/bin` or `/usr/local/bin/`.
 
 ### TensorFlow
-TensorFlow 2 will be installed as a dependency and [GPU support](https://www.tensorflow.org/install/gpu) is required for training.
-`pip` will install latest TensorFlow but older versions `>=2.6.5` are supported and can be installed if your machine does not meet TensorFlow CUDA requirements.
+TensorFlow 2 will be installed as a dependency and GPU support is required for training.
+`pip` will install latest TensorFlow supported version, but older versions `>=2.6.5` are supported and can be installed if your machine does not meet TensorFlow CUDA requirements.
 See [this](https://www.tensorflow.org/install/source#gpu) table for the CUDA and TensorFlow versions compatibility.
-But current allowed versions only supoport **CUDA 11.2**.
 In case you want a different TensorFlow version, you can downgrade using:
 ```bash
 pip install tensorflow==2.6.5
 ```
 
 TensorFlow logging messages are suppressed by default, in case you want to see them you have to explicitly set `TF_CPP_MIN_LOG_LEVEL` environment variable.
 For example:
@@ -787,15 +787,15 @@
 ```
 pip install bicleaner-ai[transliterate]
 ```
 Note that this won't transliterate the output text, it will be used only for scoring.
 
 
 ## Cleaning
-### Getting Started
+### Getting started
 `bicleaner-ai-classify` aims at detecting noisy sentence pairs in a parallel corpus. It
 indicates the likelihood of a pair of sentences being mutual translations (with a value near to 1) or not (with a value near to 0). Sentence pairs considered very noisy are scored with 0.
 
 By default, the input file (the parallel corpus to be classified) expects at least four columns, being:
 
 * col1: URL 1
 * col2: URL 2
@@ -838,221 +838,103 @@
         corpus.en-fr.tsv  \
         corpus.en-fr.classifed.tsv  \
         bitextor/bicleaner-ai-full-en-fr
 ```
 where `--scol` and `--tcol` indicate the location of source and target sentence,
 `corpus.en-fr.tsv` the input file,
 `corpus.en-fr.classified.tsv` output file and `bitextor/bicleaner-ai-en-fr` is the HuggingFace model name.
-Each line of the new file will contain the same content as the input file, adding a column with the score given by the Bicleaner classifier.
+Each line of the new file will contain the same content as the input file, adding a column with the score given by the Bicleaner AI classifier.
 
 Note that, to use a lite model, you need to provide model path in your local file system, instead of HuggingFace model name.
 
 
-### Parameters
-The complete list of parameters is:
-
-* positional arguments:
-  * `input`: Tab-separated files to be classified (default line format: `URL1 URL2 SOURCE_SENTENCE TARGET_SENTENCE [EXTRA_COLUMNS]`, tab-separated). When input is -, reads standard input.
-  * `output`: Output of the classification (default: standard output). When output is -, writes standard output.
-  * `metadata`: Training metadata (YAML file), generated by `bicleaner-ai-train` or downloaded as a part of a language pack.
-  There's a script that can download and unpack it for you, use:
-  ```bash
-  $ bicleaner-ai-download en cs lite ./models
-  ```
-  to download English-Czech lite language pack to the ./models directory and unpack it.
-* optional arguments:
-  * `-h, --help`: show this help message and exit
-* Optional:
-  * `-S SOURCE_TOKENIZER_COMMAND`: Source language tokenizer full command (including flags if needed). If not given, Sacremoses tokenizer is used (with `escape=False` option).
-  * `-T TARGET_TOKENIZER_COMMAND`: Target language tokenizer full command (including flags if needed). If not given, Sacremoses tokenizer is used (with `escape=False` option).
-  * `--scol SCOL`: Source sentence column (starting in 1). If `--header` is set, the expected value will be the name of the field (default: 3 if `--header` is not set else src_text)
-  * `--tcol TCOL`: Target sentence column (starting in 1). If `--header` is set, the expected value will be the name of the field (default: 4 if `--header` is not set else trg_text)
-  * `--tmp_dir TMP_DIR`: Temporary directory where creating the temporary files of this program (default: default system temp dir, defined by the environment variable TMPDIR in Unix)
-  * `-b BLOCK_SIZE, --block_size BLOCK_SIZE`: Sentence pairs per block (default: 10000)
-  * `--lm_threshold LM_THRESHOLD`: Threshold for language model fluency scoring. All sentence pairs whose LM fluency score falls below the threshold are removed (classifier score set to 0), unless the option --keep_lm_result is set. (default: 0.5)
-  * `--score_only`: Only output one column which is the bicleaner score (default: False)
-  * `--calibrated`: Output calibrated scores (default: False)
-  * `--raw_output`: Return raw output without computing positive class probability. (default: False)
-  * `--disable_hardrules`: Disables the bicleaner_hardrules filtering (only bicleaner_classify is applied) (default: False)
-  * `--disable_lm_filter`: Disables LM filtering.
-  * `--disable_porn_removal`: Disables porn removal.
-  * `--disable_minimal_length` : Don't apply minimal length rule (default: False).
-
-* Logging:
-  * `-q, --quiet`: Silent logging mode (default: False)
-  * `--debug`: Debug logging mode (default: False)
-  * `--logfile LOGFILE`: Store log to a file (default: \<\_io.TextIOWrapper name='<stderr>' mode='w' encoding='UTF-8'\>)
-  * `-v, --version`: show version of this script and exit
-
-## Training classifiers
-
-In case you need to train a new classifier (i.e. because it is not available in the language packs provided at [bicleaner-ai-data](https://github.com/bitextor/bicleaner-ai-data/releases/latest)), you can use `bicleaner-ai-train`.
-`bicleaner-ai-train` is a Python tool that allows you to train a classifier which predicts
-whether a pair of sentences are mutual translations or not and discards too noisy sentence pairs. Visit our [Wiki](https://github.com/bitextor/bicleaner-ai/wiki/How-to-train-your-Bicleaner-AI) for a detailed example on Bicleaner AI training.
-
-### Requirements
-
-In order to train a new classifier, you must provide:
-* A clean parallel corpus (500k pairs of sentences is the recommended size).
-* Monolingual corpus for the source and the target language (not necessary for `xlmr` classifier).
-* Gzipped lists of monolingual word frequencies. You can check their format by downloading any of the available language packs.
-   * The SL list of word frequencies with one entry per line. Each entry must contain the following 2 fields, split by space, in this order: word frequency (number of times a word appears in text), SL word.
-   * The TL list of word frequencies with one entry per line. Each entry must contain the following 2 fields, split by space, in this order: word frequency (number of times a word appears in text), TL word.
-   * These lists can easily be obtained from a monolingual corpus and a command line in bash:
-```bash
-$ cat monolingual.SL \
-    | sacremoses -l SL tokenize -x \
-    | awk '{print tolower($0)}' \
-    | tr ' ' '\n' \
-    | LC_ALL=C sort | uniq -c \
-    | LC_ALL=C sort -nr \ \
-    | grep -v '[[:space:]]*1' \
-    | gzip > wordfreq-SL.gz
-$ cat monolingual.TL \
-    | sacremoses -l TL tokenize -x \
-    | awk '{print tolower($0)}' \
-    | tr ' ' '\n' \
-    | LC_ALL=C sort | uniq -c \
-    | LC_ALL=C sort -nr \ \
-    | grep -v '[[:space:]]*1' \
-    | gzip > wordfreq-TL.gz
-
-```
-Optionally, if you want the classifier to include a porn filter, you must also provide:
-* File with training dataset for porn removal classifier. Each sentence must contain at the beginning the `__label__negative` or `__label__positive` according to FastText convention. It should be lowercased and tokenized.
-
-### Parameters
-It can be used as follows.
-
-```bash
-bicleaner-ai-train [-h]
-    -m MODEL_DIR
-    -s SOURCE_LANG
-    -t TARGET_LANG
-    [--mono_train MONO_TRAIN]
-    --parallel_train PARALLEL_TRAIN
-    --parallel_dev PARALLEL_DEV
-    [-S SOURCE_TOKENIZER_COMMAND]
-    [-T TARGET_TOKENIZER_COMMAND]
-    [-F TARGET_WORD_FREQS]
-    [--block_size BLOCK_SIZE]
-    [-p PROCESSES]
-    [-g GPU]
-    [--mixed_precision]
-    [--save_train_data SAVE_TRAIN_DATA]
-    [--distilled]
-    [--seed SEED]
-    [--classifier_type {dec_attention,transformer,xlmr}]
-    [--batch_size BATCH_SIZE]
-    [--steps_per_epoch STEPS_PER_EPOCH]
-    [--epochs EPOCHS]
-    [--patience PATIENCE]
-    [--pos_ratio POS_RATIO]
-    [--rand_ratio RAND_RATIO]
-    [--womit_ratio WOMIT_RATIO]
-    [--freq_ratio FREQ_RATIO]
-    [--fuzzy_ratio FUZZY_RATIO]
-    [--neighbour_mix NEIGHBOUR_MIX]
-    [--porn_removal_train PORN_REMOVAL_TRAIN]
-    [--porn_removal_test PORN_REMOVAL_TEST]
-    [--porn_removal_file PORN_REMOVAL_FILE]
-    [--porn_removal_side {sl,tl}]
-    [--noisy_examples_file_sl NOISY_EXAMPLES_FILE_SL]
-    [--noisy_examples_file_tl NOISY_EXAMPLES_FILE_TL]
-    [--lm_dev_size LM_DEV_SIZE]
-    [--lm_file_sl LM_FILE_SL]
-    [--lm_file_tl LM_FILE_TL]
-    [--lm_training_file_sl LM_TRAINING_FILE_SL]
-    [--lm_training_file_tl LM_TRAINING_FILE_TL]
-    [--lm_clean_examples_file_sl LM_CLEAN_EXAMPLES_FILE_SL]
-    [--lm_clean_examples_file_tl LM_CLEAN_EXAMPLES_FILE_TL]
-    [-q]
-    [--debug]
-    [--logfile LOGFILE]
-```
-
-* positional arguments:
-  * `input`: Tab-separated bilingual input file (default: Standard input)(line format: SOURCE_SENTENCE TARGET_SENTENCE, tab-separated)
-* optional arguments:
-  * `-h, --help`: show this help message and exit
-* Mandatory:
-  * `-m MODEL_DIR, --model_dir MODEL_DIR`: Model directory, metadata, classifier and SentencePiece models will be saved in the same directory (default: None)
-  * `-s SOURCE_LANG, --source_lang SOURCE_LANG`: Source language (default: None)
-  * `-t TARGET_LANG, --target_lang TARGET_LANG`: Target language (default: None)
-  * `--mono_train MONO_TRAIN`: File containing monolingual sentences of both languages shuffled together, used to train SentencePiece embeddings. Not required for XLMR. (default: None)
-  * `--parallel_train PARALLEL_TRAIN`: TSV file containing parallel sentences to train the classifier (default: None)
-  * `--parallel_dev PARALLEL_DEV`: TSV file containing parallel sentences for development (default: None)
-
-* Options:
-  * `-S SOURCE_TOKENIZER_COMMAND, --source_tokenizer_command SOURCE_TOKENIZER_COMMAND`: Source language tokenizer full command (default: None)
-  * `-T TARGET_TOKENIZER_COMMAND, --target_tokenizer_command TARGET_TOKENIZER_COMMAND`: Target language tokenizer full command (default: None)
-  * `-F TARGET_WORD_FREQS, --target_word_freqs TARGET_WORD_FREQS`: R language gzipped list of word frequencies (needed for frequence based noise) (default: None)
-  * `--block_size BLOCK_SIZE`: Sentence pairs per block when apliying multiprocessing in the noise function (default: 10000)
-  * `-p PROCESSES, --processes PROCESSES`: Number of process to use (default: 71)
-  * `-g GPU, --gpu GPU`: Which GPU use, starting from 0. Will set the CUDA_VISIBLE_DEVICES. (default: None)
-  * `--mixed_precision`: Use mixed precision float16 for training (default: False)
-  * `--save_train_data SAVE_TRAIN_DATA`: Save the generated dataset into a file. If the file already exists the training dataset will be loaded from there. (default: None)
-  * `--distilled`: Enable Knowledge Distillation training. It needs pre-built training set with raw scores from a teacher model. (default: False)
-  * `--seed`: SEED           Seed for random number generation. By default, no seeed is used. (default: None)
-  * `--classifier_type {dec_attention,transformer,xlmr}`: Neural network architecture of the classifier (default: dec_attention)
-  * `--batch_size BATCH_SIZE`: Batch size during classifier training. If None, default architecture value will be used. (default: None)
-  * `--steps_per_epoch STEPS_PER_EPOCH`: Number of batch updates per epoch during training. If None, default architecture value will be used or the full dataset size. (default: None)
-  * `--epochs EPOCHS`: Number of epochs for training. If None, default architecture value will be used. (default: None)
-  * `--patience PATIENCE`: Stop training when validation has stopped improving after PATIENCE number of epochs (default: None)
-  * `--pos_ratio POS_RATIO`: Ratio of positive samples used to oversample on validation and test sets (default: 1)
-  * `--rand_ratio RAND_RATIO`: Ratio of negative samples misaligned randomly (default: 3)
-  * `--womit_ratio WOMIT_RATIO`: Ratio of negative samples misaligned by randomly omitting words (default: 3)
-  * `--freq_ratio FREQ_RATIO`: Ratio of negative samples misaligned by replacing words by frequence (needs --target_word_freq) (default: 3)
-  * `--fuzzy_ratio FUZZY_RATIO`: Ratio of negative samples misaligned by fuzzy matching (default: 0)
-  * `--neighbour_mix NEIGHBOUR_MIX`: If use negative samples misaligned by neighbourhood (default: False)
-  * `--porn_removal_train PORN_REMOVAL_TRAIN`: File with training dataset for FastText classifier. Each sentence must contain at the beginning the '__label__negative' or '__label__positive' according to FastText convention. It should be lowercased and tokenized. (default: None)
-  * `--porn_removal_test PORN_REMOVAL_TEST`: Test set to compute precision and accuracy of the porn removal classifier (default: None)
-  * `--porn_removal_file PORN_REMOVAL_FILE`: Porn removal classifier output file (default: porn_removal.bin)
-  * `--porn_removal_side {sl,tl}`: Whether the porn removal should be applied at the source or at the target language. (default: sl)
-  * `--noisy_examples_file_sl NOISY_EXAMPLES_FILE_SL`: File with noisy text in the SL. These are used to estimate the perplexity of noisy text. (default: None)
-  * `--noisy_examples_file_tl NOISY_EXAMPLES_FILE_TL`: File with noisy text in the TL. These are used to estimate the perplexity of noisy text. (default: None)
-  * `--lm_dev_size LM_DEV_SIZE`: Number of sentences to be removed from clean text before training LMs. These are used to estimate the perplexity of clean text. (default: 2000)
-  * `--lm_file_sl LM_FILE_SL`: SL language model output file. (default: None)
-  * `--lm_file_tl LM_FILE_TL`: TL language model output file. (default: None)
-  * `--lm_training_file_sl LM_TRAINING_FILE_SL`: SL text from which the SL LM is trained. If this parameter is not specified, SL LM is trained from the SL side of the input file, after removing --lm_dev_size sentences. (default: None)
-  * `--lm_training_file_tl LM_TRAINING_FILE_TL`: TL text from which the TL LM is trained. If this parameter is not specified, TL LM is trained from the TL side of the input file, after removing --lm_dev_size sentences. (default: None)
-  * `--lm_clean_examples_file_sl LM_CLEAN_EXAMPLES_FILE_SL`: File with clean text in the SL. Used to estimate the perplexity of clean text. This option must be used together with --lm_training_file_sl and both files must not have common sentences. This option replaces --lm_dev_size. (default: None)
-  * `--lm_clean_examples_file_tl LM_CLEAN_EXAMPLES_FILE_TL`: File with clean text in the TL. Used to estimate the perplexity of clean text. This option must be used together with --lm_training_file_tl and both files must not have common sentences. This option replaces --lm_dev_size. (default: None)
-* Logging:
-  * `-q, --quiet`: Silent logging mode (default: False)
-  * `--debug`: Debug logging mode (default: False)
-  * `--logfile LOGFILE`: Store log to a file (default: \<\_io.TextIOWrapper name='<stderr>' mode='w' encoding='UTF-8'>)
-
-### Example
-
-```bash
-bicleaner-ai-train \
-          --parallel_train corpus.en-cs.train \
-          --parallel_dev corpus.en-cs.dev \
-          --mono_train mono.en-cs \
-          -m models/en-cs \
-          -s en \
-          -t cs \
-          -F wordfreqs-cs.gz \
-          --lm_file_sl models/en-cs/lm.en  --lm_file_tl models/en-cs/lm.cs \
-          --porn_removal_train porn-removal.txt.en  --porn_removal_file models/en-cs/porn-model.en \
-```
-
-This will train a lite classifier for English-Czech using the corpus `corpus.en-cs.train`, the `corpus.en-cs.dev` as development set and the monolingual corpus `mono.en-cs` to train the vocabulary embeddings.
-All the model files created during training, the language model files, the porn removal file, and the `metadata.yaml` will be stored in the model directory `models/en-cs`.
-
-To train full models you would need to use `--classifier_type xlmr` and `--mono_train` is not needed.
-
-### Synthetic noise
-By default the training will use `rand_ratio`, `womit_ratio` and `freq_ratio` options with a value of 3.
-Both `womit_ratio` and `freq_ratio` will use Sacremoses tokenizer by default.
-So, for languages that are not supported by this tokenizer or are poorly supported, `source_tokenizer_command` and/or `target_tokenizer_command` should be provided.
-Also note that, if a tokenizer command is used, the word frequencies need to be tokenized in the same way to allow noise based on frequency work correctly.
-
-If no tokenization is available for your languages, you can disable these noise option that use tokenization and use fuzzy mathing noise: `--womit_ratio 0 --freq_ratio 0 --fuzzy_ratio 6`.
+#### Multilingual models
+There are multilingual full models available.
+They can work with, potentially, any language (currently only paired with English) that XLMR [supports](https://github.com/facebookresearch/fairseq/tree/main/examples/xlmr#introduction).
+To see a further explaination on how to train a multilingual model or how our models perform, take a look [here](docs/training/multilingual.md) and [here](docs/training/multilingual.md#performance).
+
+**WARNING**: multilingual models will disable hardrules that expect language parameter.
+You can, however, overwrite the language code in the model configuration with `-s`/`--source_lang` or `-t`/`--target_lang` options during classify. For example when scoring English-Icelandic data, use:
+```
+bicleaner-ai-classify \
+    --scol 1 --tcol 2 \
+    -t is \
+    corpus.en-is.tsv \
+    corpus.en-is.classified.tsv \
+    bitextor/bicleaner-ai-full-en-xx
+```
+
+### Usage
+
+<details>
+<summary>Full description of the command-line parameters:</summary>
+
+```
+usage: bicleaner-ai-classify [-h] [-s SOURCE_LANG] [-t TARGET_LANG] [-S SOURCE_TOKENIZER_COMMAND] [-T TARGET_TOKENIZER_COMMAND] [--header] [--scol SCOL] [--tcol TCOL] [-b BLOCK_SIZE] [-p PROCESSES] [--batch_size BATCH_SIZE]
+                             [--tmp_dir TMP_DIR] [--score_only] [--calibrated] [--raw_output] [--lm_threshold LM_THRESHOLD] [--disable_hardrules] [--disable_lm_filter] [--disable_porn_removal] [--disable_minimal_length]
+                             [--run_all_rules] [--rules_config RULES_CONFIG] [--offline] [--auth_token AUTH_TOKEN] [-q] [--debug] [--logfile LOGFILE] [-v]
+                             input [output] model
+
+positional arguments:
+  input                 Tab-separated files to be classified
+  output                Output of the classification (default: <_io.TextIOWrapper name='<stdout>' mode='w' encoding='utf-8'>)
+  model                 Path to model directory or HuggingFace Hub model identifier (such as 'bitextor/bicleaner-ai-full-en-fr')
+
+options:
+  -h, --help            show this help message and exit
+
+Optional:
+  -s SOURCE_LANG, --source_lang SOURCE_LANG
+                        Overwrite model config source language (default: None)
+  -t TARGET_LANG, --target_lang TARGET_LANG
+                        Overwrite model config target language (default: None)
+  -S SOURCE_TOKENIZER_COMMAND, --source_tokenizer_command SOURCE_TOKENIZER_COMMAND
+                        Source language (SL) tokenizer full command (default: None)
+  -T TARGET_TOKENIZER_COMMAND, --target_tokenizer_command TARGET_TOKENIZER_COMMAND
+                        Target language (TL) tokenizer full command (default: None)
+  --header              Input file will be expected to have a header, and the output will have a header as well (default: False)
+  --scol SCOL           Source sentence column (starting in 1). The name of the field is expected instead of the position if --header is set (default: 3)
+  --tcol TCOL           Target sentence column (starting in 1). The name of the field is expected instead of the position if --header is set (default: 4)
+  -b BLOCK_SIZE, --block_size BLOCK_SIZE
+                        Sentence pairs per block (default: 10000)
+  -p PROCESSES, --processes PROCESSES
+                        Option no longer available, please set BICLEANER_AI_THREADS environment variable (default: None)
+  --batch_size BATCH_SIZE
+                        Sentence pairs per block (default: 32)
+  --tmp_dir TMP_DIR     Temporary directory where creating the temporary files of this program (default: /tmp)
+  --score_only          Only output one column which is the bicleaner score (default: False)
+  --calibrated          Output calibrated scores (default: False)
+  --raw_output          Return raw output without computing positive class probability. (default: False)
+  --lm_threshold LM_THRESHOLD
+                        Threshold for language model fluency scoring. All TUs whose LM fluency score falls below the threshold will are removed (classifier score set to 0), unless the option --keep_lm_result set. (default: 0.5)
+  --disable_hardrules   Disables the bicleaner_hardrules filtering (only bicleaner_classify is applied) (default: False)
+  --disable_lm_filter   Disables LM filtering (default: False)
+  --disable_porn_removal
+                        Don't apply porn removal (default: False)
+  --disable_minimal_length
+                        Don't apply minimal length rule (default: False)
+  --run_all_rules       Run all rules of Hardrules instead of stopping at first discard (default: False)
+  --rules_config RULES_CONFIG
+                        Hardrules configuration file (default: None)
+  --offline             Don't try to download the model, instead try directly to load from local storage (default: False)
+  --auth_token AUTH_TOKEN
+                        Auth token for the Hugging Face Hub (default: None)
+
+Logging:
+  -q, --quiet           Silent logging mode (default: False)
+  --debug               Debug logging mode (default: False)
+  --logfile LOGFILE     Store log to a file (default: <_io.TextIOWrapper name='<stderr>' mode='w' encoding='utf-8'>)
+  -v, --version         Show version of the package and exit
+```
+
+</details>
+
+## Training models
+Bicleaner AI provides a command-line tool to train your own model, in case available models do not fit your needs.
+Please go to our [training documentation](docs/training) for a quick start and further details.
 
 ## Setting the number of threads
 To set the maximum number of threads/processes to be used during training or classifying, `--processes` option is no longer available.
 You will need to set `BICLEANER_AI_THREADS` environment variable to the desired value.
 For example:
 ```
 BICLEANER_AI_THREADS=12 bicleaner-ai-classify ...
@@ -1065,12 +947,38 @@
 | model | speed CPUx1 | speed GPUx1 |
 | ----- | ----------- | ----------- |
 | full | 1.78 rows/sec | 200 rows/sec |
 | lite | 600 rows/sec | 10,000 rows/sec |
 
 * CPU: Intel Core i9-9960X single core (lite model batch 16, full model batch 1)
 * GPU: Nvidia V100 (lite model batch 2048, full model batch 16)
+
+## Citation
+
+> J. Zaragoza-Bernabeu, M. Bañón, G. Ramírez-Sánchez, S. Ortiz-Rojas, \
+> "[Bicleaner AI: Bicleaner Goes Neural](https://aclanthology.org/2022.lrec-1.87/)", \
+> in *Proceedings of the 13th Language Resources and Evaluation Conference*. \
+> Marseille, France: Language Resources and Evaluation Conference, June 2022
+
+```latex
+@inproceedings{zaragoza-bernabeu-etal-2022-bicleaner,
+    title = {"Bicleaner {AI}: Bicleaner Goes Neural"},
+    author = {"Zaragoza-Bernabeu, Jaume  and
+      Ram{\'\i}rez-S{\'a}nchez, Gema  and
+      Ba{\~n}{\'o}n, Marta  and
+      Ortiz Rojas, Sergio"},
+    booktitle = {"Proceedings of the Thirteenth Language Resources and Evaluation Conference"},
+    month = jun,
+    year = {"2022"},
+    address = {"Marseille, France"},
+    publisher = {"European Language Resources Association"},
+    url = {"https://aclanthology.org/2022.lrec-1.87"},
+    pages = {"824--831"},
+    abstract = {"This paper describes the experiments carried out during the development of the latest version of Bicleaner, named Bicleaner AI, a tool that aims at detecting noisy sentences in parallel corpora. The tool, which now implements a new neural classifier, uses state-of-the-art techniques based on pre-trained transformer-based language models fine-tuned on a binary classification task. After that, parallel corpus filtering is performed, discarding the sentences that have lower probability of being mutual translations. Our experiments, based on the training of neural machine translation (NMT) with corpora filtered using Bicleaner AI for two different scenarios, show significant improvements in translation quality compared to the previous version of the tool which implemented a classifier based on Extremely Randomized Trees."},
+}
+```
+
 ___
 
 ![Connecting Europe Facility](https://www.paracrawl.eu/images/logo_en_cef273x39.png)
 
 All documents and software contained in this repository reflect only the authors' view. The Innovation and Networks Executive Agency of the European Union is not responsible for any use that may be made of the information it contains.
```

### Comparing `bicleaner-ai-2.3.2/pyproject.toml` & `bicleaner_ai-3.0.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "bicleaner-ai"
-version = "2.3.2"
+version = "3.0.0"
 license = {file = "LICENSE"}
 authors = [
     { "name" = "Prompsit Language Engineering", "email" = "info@prompsit.com" }
 ]
 maintainers = [
     { "name" = "Jaume Zaragoza", "email" = "jzaragoza@prompsit.com" }
 ]
@@ -15,22 +15,24 @@
     "scikit-learn>=0.22.1",
     "PyYAML>=5.1.2",
     "numpy",
     "pytest",
     "toolwrapper",
     "joblib",
     "sacremoses",
-    "bicleaner-hardrules==2.9.0",
+    "bicleaner-hardrules==2.10.3",
     "sentencepiece",
-    "tensorflow>=2.6.5,<2.12",
+    "protobuf==3.20.3",
+    "tensorflow>=2.6.5,<2.16",
     "bicleaner-ai-glove==0.2.1",
     "fuzzywuzzy",
     "python-Levenshtein",
-    "transformers==4.30.2",
-    "huggingface-hub==0.15.1",
+    "transformers==4.36.1",
+    "huggingface-hub>=0.22,<0.23",
+    "zstandard",
     "psutil",
     "regex",
 ]
 classifiers = [
     "Environment :: Console",
     "Intended Audience :: Science/Research",
     "Programming Language :: Python :: 3.7",
@@ -53,14 +55,15 @@
 build-backend = "setuptools.build_meta"
 
 [project.scripts]
 bicleaner-ai-train = "bicleaner_ai.bicleaner_ai_train:main"
 bicleaner-ai-classify = "bicleaner_ai.bicleaner_ai_classifier:main"
 bicleaner-ai-download = "bicleaner_ai.bicleaner_ai_download:main"
 bicleaner-ai-download-hf = "bicleaner_ai.bicleaner_ai_download_hf:main"
+bicleaner-ai-generate-train = "bicleaner_ai.bicleaner_ai_generate_train:main"
 
 [project_urls]
 "Bicleaner on GitHub" = "https://github.com/bitextor/bicleaner"
 "Prompsit Language Engineering" = "http://www.prompsit.com"
 "Paracrawl" = "https://paracrawl.eu/"
 "MaCoCu" = "https://macocu.eu/"
 "HPLT Project" = "https://hplt-project.org"
```

### Comparing `bicleaner-ai-2.3.2/src/bicleaner_ai/bicleaner_ai_classifier.py` & `bicleaner_ai-3.0.0/src/bicleaner_ai/bicleaner_ai_classifier.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,18 +17,18 @@
 from timeit import default_timer
 from multiprocessing import cpu_count
 import regex
 
 #Allows to load modules while inside or outside the package
 try:
     from .classify import classify, argument_parser, load_metadata
-    from .util import logging_setup
+    from .util import logging_setup, check_gpu
 except (ImportError, SystemError):
     from classify import classify, argument_parser, load_metadata
-    from util import logging_setup
+    from util import logging_setup, check_gpu
 
 logging_level = 0
 
 # Argument parsing
 def initialization(argv = None):
     global logging_level
 
@@ -86,14 +86,16 @@
 
     if not os.path.isfile(args.metadata):
         if hub_not_found:
             logging.error(
                     f"Model {args.model} not found at HF Hub. If the model is private use --auth_token option.")
         raise FileNotFoundError(f"model {args.metadata} no such file")
 
+    check_gpu()
+
     # Load metadata YAML
     args = load_metadata(args, parser)
 
     logging.debug(args)
 
     return args
```

### Comparing `bicleaner-ai-2.3.2/src/bicleaner_ai/bicleaner_ai_download.py` & `bicleaner_ai-3.0.0/src/bicleaner_ai/bicleaner_ai_download.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,39 +34,39 @@
 def main():
     parser = ArgumentParser(
             description='Download Bicleaner AI models from the HuggingFace Hub or GitHub')
     parser.add_argument('src_lang', type=str,
                         help='Source language')
     parser.add_argument('trg_lang', type=str,
                         help='Target language')
-    parser.add_argument('model_type', type=str, choices=['full', 'lite'],
+    parser.add_argument('model_type', type=str, choices=['full', 'full-large', 'lite'],
                         help='Download lite or full model')
     parser.add_argument('download_path', type=str, nargs='?',
-                        help='Path to download the model (only for old Github models)')
+                        help='Path where model files will be stored')
     parser.add_argument('-t', '--auth_token', default=None, type=str,
                         help='Authentication token for private models downloading')
     parser.add_argument('-q', '--quiet', action='store_true', help='Suppress logging messages')
     parser.add_argument('--debug', action='store_true')
 
     args = parser.parse_args()
     logging_setup(args)
 
     if not args.download_path and args.model_type == 'lite':
         raise Exception("Lite models need a download path")
 
-    if args.model_type == 'full':
-        #TODO fallback to github if does not exist?
-        name = f'bitextor/bicleaner-ai-full-{args.src_lang}-{args.trg_lang}'
+    if args.model_type.startswith('full'):
+        large = "-large" if args.model_type == 'full-large' else ""
+        name = f'bitextor/bicleaner-ai-full{large}-{args.src_lang}-{args.trg_lang}'
         logging.info(f'Downloading {name}')
         try:
             if not args.download_path:
                 snapshot_download(name, use_auth_token=args.auth_token,
                                   etag_timeout=100, max_workers=1)
             else:
-                local_dir = f"{args.download_path}/{args.src_lang}-{args.trg_lang}"
+                local_dir = args.download_path
                 logging.debug(f"Saving model to local dir: {local_dir}")
                 snapshot_download(name, use_auth_token=args.auth_token,
                                   local_dir=local_dir,
                                   local_dir_use_symlinks=False,
                                   etag_timeout=100, max_workers=1)
             return
         except RepositoryNotFoundError:
```

### Comparing `bicleaner-ai-2.3.2/src/bicleaner_ai/bicleaner_ai_download_hf.py` & `bicleaner_ai-3.0.0/src/bicleaner_ai/bicleaner_ai_download_hf.py`

 * *Files identical despite different names*

### Comparing `bicleaner-ai-2.3.2/src/bicleaner_ai/bicleaner_ai_train.py` & `bicleaner_ai-3.0.0/src/bicleaner_ai/bicleaner_ai_train.py`

 * *Files 22% similar despite different names*

```diff
@@ -21,77 +21,62 @@
 import random
 import sys
 import shutil
 
 #Allows to load modules while inside or outside the package  
 try:
     from . import __version__
-    from .word_freqs_zipf import WordZipfFreqDist
-    from .word_freqs_zipf_double_linked import WordZipfFreqDistDoubleLinked
     from .util import *
-    from .training import build_noise, write_metadata
+    from .training import write_metadata
+    from .noise_generation import add_noise_options, setup_noise, build_noise
 except (SystemError, ImportError):
     from bicleaner_ai import __version__
-    from word_freqs_zipf import WordZipfFreqDist
-    from word_freqs_zipf_double_linked import WordZipfFreqDistDoubleLinked
     from util import *
     from training import build_noise, write_metadata
+    from noise_generation import add_noise_options, setup_noise, build_noise
 
 logging_level = 0
 
 # Argument parsing
 def get_arguments(argv = None):
     global logging_level
 
     parser = argparse.ArgumentParser(prog=os.path.basename(sys.argv[0]), formatter_class=argparse.ArgumentDefaultsHelpFormatter, description=__doc__)
 
     groupM = parser.add_argument_group("Mandatory")
-    groupM.add_argument('-m', '--model_dir', type=check_dir, required=True, help="Model directory, metadata, classifier and SentencePiece models will be saved in the same directory")
+    groupM.add_argument('-m', '--model_dir', type=check_dir, required=True, help="Model directory, metadata, classifier and SentencePiece vocabulary will be saved in the same directory")
     groupM.add_argument('-s', '--source_lang', required=True, help="Source language")
     groupM.add_argument('-t', '--target_lang', required=True, help="Target language")
     groupM.add_argument('--mono_train', type=argparse.FileType('r'), default=None, required=False, help="File containing monolingual sentences of both languages shuffled together, used to train SentencePiece embeddings. Not required for XLMR.")
-    groupM.add_argument('--parallel_train', type=argparse.FileType('r'), default=None, required=True, help="TSV file containing parallel sentences to train the classifier")
-    groupM.add_argument('--parallel_valid', type=argparse.FileType('r'), default=None, required=True, help="TSV file containing parallel sentences for validation")
+    groupM.add_argument('--parallel_train', type=argparse.FileType('r'), default=None, required='--generated_train' not in sys.argv, help="TSV file containing parallel sentences to train the classifier")
+    groupM.add_argument('--parallel_valid', type=argparse.FileType('r'), default=None, required='--generated_valid' not in sys.argv, help="TSV file containing parallel sentences for validation")
 
     groupO = parser.add_argument_group('Options')
     groupO.add_argument('--model_name', type=str, default=None, help='The name of the model. For the XLMR models it will be used as the name in Hugging Face Hub.')
-    groupO.add_argument('--base_model', type=str, default=None, help='The name of the base model to start of. Only used in XLMR models, must be an XLMR instance.')
-    #groupO.add_argument('-f', '--source_word_freqs', type=argparse.FileType('r'), default=None, required=False, help="L language gzipped list of word frequencies")
-    groupO.add_argument('-F', '--target_word_freqs', type=argparse.FileType('r'), default=None, required=False, help="R language gzipped list of word frequencies (needed for frequence based noise)")
-    groupO.add_argument('--target_tokenizer_type', choices=['word', 'char'], default='word', help='Type of tokenization for noise generation.')
-    groupO.add_argument('--block_size', type=check_positive, default=2000, help="Sentence pairs per block when apliying multiprocessing in the noise function")
-    groupO.add_argument('-p', '--processes', default=None, help="Option no longer available, please set BICLEANER_AI_THREADS environment variable")
+    groupO.add_argument('--base_model', type=str, default=None, help='The name of the base model to start from. Only used in XLMR classifiers, must be an XLMR instance.')
     groupO.add_argument('-g', '--gpu', type=check_positive_or_zero, help="Which GPU use, starting from 0. Will set the CUDA_VISIBLE_DEVICES.")
     groupO.add_argument('--mixed_precision', action='store_true', default=False, help="Use mixed precision float16 for training")
-    groupO.add_argument('--save_train', type=str, default=None, help="Save the generated training dataset into a file. If the file already exists the training dataset will be loaded from there.")
-    groupO.add_argument('--save_valid', type=str, default=None, help="Save the generated validation dataset into a file. If the file already exists the validation dataset will be loaded from there.")
     groupO.add_argument('--distilled', action='store_true', help='Enable Knowledge Distillation training. It needs pre-built training set with raw scores from a teacher model.')
     groupO.add_argument('--seed', default=None, type=int, help="Seed for random number generation. By default, no seeed is used.")
+    groupO.add_argument('--generated_train', type=str, default=None, help="Generated training dataset. If the file already exists the training dataset will be loaded from here.")
+    groupO.add_argument('--generated_valid', type=str, default=None, help="Generated validation dataset. If the file already exists the validation dataset will be loaded from here.")
 
-    # Classifier training options
-    groupO.add_argument('--classifier_type', choices=model_classes.keys(), default="dec_attention", help="Neural network architecture of the classifier")
+    # Model training options
+    groupO.add_argument('--classifier_type', choices=model_classes.keys(), default="dec_attention", help="Neural network architecture for the classifier")
     groupO.add_argument('--batch_size', type=check_positive, default=None, help="Batch size during classifier training. If None, default architecture value will be used.")
     groupO.add_argument('--steps_per_epoch', type=check_positive, default=None, help="Number of batch updates per epoch during training. If None, default architecture value will be used or the full dataset size.")
     groupO.add_argument('--epochs', type=check_positive, default=None, help="Number of epochs for training. If None, default architecture value will be used.")
     groupO.add_argument('--patience', type=check_positive, default=None, help="Stop training when validation has stopped improving after PATIENCE number of epochs")
 
-    # Negative sampling options
-    groupO.add_argument('--pos_ratio', default=1, type=int, help="Ratio of positive samples used to oversample on validation and test sets")
-    groupO.add_argument('--rand_ratio', default=3, type=int, help="Ratio of negative samples misaligned randomly")
-    groupO.add_argument('--womit_ratio', default=3, type=int, help="Ratio of negative samples misaligned by randomly omitting words")
-    groupO.add_argument('--freq_ratio', default=3, type=int, help="Ratio of negative samples misaligned by replacing words by frequence (needs --target_word_freq)")
-    groupO.add_argument('--fuzzy_ratio', default=0, type=int, help="Ratio of negative samples misaligned by fuzzy matching")
-    groupO.add_argument('--neighbour_mix', default=False, type=bool, help="If use negative samples misaligned by neighbourhood")
-    groupO.add_argument('--min_omit_words', default=1, type=int, help="Minimum words to omit per sentence in omit noise")
-    groupO.add_argument('--min_freq_words', default=1, type=int, help="Minimum words to replace per sentence in freq noise")
+    add_noise_options(groupO)
 
     # Porn removal training options
-    groupO.add_argument('--porn_removal_train', type=argparse.FileType('r'), help="File with training dataset for FastText classifier. Each sentence must contain at the beginning the '__label__negative' or '__label__positive' according to FastText convention. It should be lowercased and tokenized.")
-    groupO.add_argument('--porn_removal_test', type=argparse.FileType('r'), help="Test set to compute precision and accuracy of the porn removal classifier")
-    groupO.add_argument('--porn_removal_file', type=str, default="porn_removal.bin", help="Porn removal classifier output file")
+    groupO.add_argument('--porn_removal_train', type=argparse.FileType('r'), help="File with training dataset for porn filter. Each sentence must contain at the beginning the '__label__negative' or '__label__positive' according to FastText convention. It should be lowercased and tokenized.")
+    groupO.add_argument('--porn_removal_test', type=argparse.FileType('r'), help="Test set to compute precision and accuracy of the porn removal filter")
+    groupO.add_argument('--porn_removal_file', type=str, default="porn_removal.bin", help="Porn removal output file")
     groupO.add_argument('--porn_removal_side', choices=['sl','tl'], default="sl", help="Whether the porn removal should be applied at the source or at the target language.")
 
     # LM fluency filter training options
     groupO.add_argument('--noisy_examples_file_sl', type=str, help="File with noisy text in the SL. These are used to estimate the perplexity of noisy text.")
     groupO.add_argument('--noisy_examples_file_tl', type=str, help="File with noisy text in the TL. These are used to estimate the perplexity of noisy text.")
     groupO.add_argument('--lm_dev_size', type=check_positive_or_zero, default=2000, help="Number of sentences to be removed from clean text before training LMs. These are used to estimate the perplexity of clean text.")
     groupO.add_argument('--lm_file_sl', type=str, help="SL language model output file.")
@@ -106,40 +91,31 @@
     groupL.add_argument('--debug', action='store_true', help='Debug logging mode')
     groupL.add_argument('--logfile', type=argparse.FileType('a'), default=sys.stderr, help="Store log to a file")
     groupL.add_argument('-v', '--version', action='version', version="%(prog)s " + __version__, help="Show version of the package and exit")
 
     return parser.parse_args(argv)
 
 def initialization(args):
-    if args.freq_ratio > 0 and args.target_word_freqs is None:
-        raise Exception("Frequence based noise needs target language word frequencies")
+    # initialization of noise generation related arguments
+    setup_noise(args)
+
     if args.mono_train is None and args.classifier_type != 'xlmr':
-        raise Exception("Argument --mono_train not found, required when not training XLMR classifier")
+        logging.error("Argument --mono_train not found, required when not training XLMR classifier")
+        sys.exit(1)
 
     if args.seed is not None:
         np.random.seed(args.seed)
         random.seed(args.seed)
         os.environ["PYTHONHASHSEED"] = str(args.seed)
         tf.random.seed = args.seed
         spm.set_random_generator_seed(args.seed)
 
     if args.gpu is not None:
         os.environ["CUDA_VISIBLE_DEVICES"] = str(args.gpu)
 
-    # Warn about args.processes deprecation
-    if args.processes is not None:
-        logging.warning("--processes option is not available anymore, please use BICLEANER_AI_THREADS environment variable instead.")
-
-    # Set the number of processes from the environment variable
-    # or instead use all cores
-    if "BICLEANER_AI_THREADS" in os.environ and os.environ["BICLEANER_AI_THREADS"]:
-        args.processes = int(os.environ["BICLEANER_AI_THREADS"])
-    else:
-        args.processes = max(1, cpu_count()-1)
-
     if args.mixed_precision:
         from tensorflow.keras import mixed_precision
         mixed_precision.set_global_policy('mixed_float16')
 
     # Remove trailing / in model dir
     args.model_dir.rstrip('/')
 
@@ -162,50 +138,42 @@
     logging.debug(args)
 
 # Main loop of the program
 def perform_training(args):
     time_start = default_timer()
     logging.debug("Starting process")
 
-    # Load word frequencies
-    #if args.source_word_freqs:
-    #    args.sl_word_freqs = WordZipfFreqDist(args.source_word_freqs)
-    if args.target_word_freqs:
-        args.tl_word_freqs = WordZipfFreqDistDoubleLinked(args.target_word_freqs)
-    else:
-        args.tl_word_freqs = None
-
     # Train porn removal classifier
     if args.porn_removal_file is not None and args.porn_removal_train is not None:
         from hardrules.training import train_porn_removal
         train_porn_removal(args)
 
-    # If save_train is not provided or empty build new train set
+    # If generated_train is not provided or empty build new train set
     # otherwise use the prebuilt training set
-    if (args.save_train is None
-            or not os.path.isfile(args.save_train)
-            or os.stat(args.save_train).st_size == 0):
+    if (args.generated_train is None
+            or not os.path.isfile(args.generated_train)
+            or os.stat(args.generated_train).st_size == 0):
         logging.info("Building training set")
         train_sentences = build_noise(args.parallel_train, args)
-        if args.save_train is not None:
-            shutil.copyfile(train_sentences, args.save_train)
+        if args.generated_train:
+            shutil.copyfile(train_sentences, args.generated_train)
     else:
-        train_sentences = args.save_train
+        train_sentences = args.generated_train
         logging.info("Using pre-built training set: " + train_sentences)
 
     # Same for valid set
-    if (args.save_valid is None
-            or not os.path.isfile(args.save_valid)
-            or os.stat(args.save_valid).st_size == 0):
+    if (args.generated_valid is None
+            or not os.path.isfile(args.generated_valid)
+            or os.stat(args.generated_valid).st_size == 0):
         logging.info("Building validation set")
         valid_sentences = build_noise(args.parallel_valid, args)
-        if args.save_valid is not None:
-            shutil.copyfile(valid_sentences, args.save_valid)
+        if args.generated_valid:
+            shutil.copyfile(valid_sentences, args.generated_valid)
     else:
-        valid_sentences = args.save_valid
+        valid_sentences = args.generated_valid
         logging.info("Using pre-built validation set: " + valid_sentences)
     test_sentences = valid_sentences
 
     logging.debug(f"Training sentences file: {train_sentences}")
     logging.debug(f"Validation sentences file: {valid_sentences}")
 
     # Train LM fluency filter
@@ -214,16 +182,19 @@
         args.parallel_train.seek(0)
         args.input = args.parallel_train
         args.source_tokenizer_command = None
         args.target_tokenizer_command = None
         lm_stats = train_fluency_filter(args)
     else:
         lm_stats = None
-    args.parallel_train.close()
-    args.parallel_valid.close()
+
+    if args.parallel_train:
+        args.parallel_train.close()
+    if args.parallel_valid:
+        args.parallel_valid.close()
 
     # Define the model name
     if args.model_name is None:
         model_name = 'bitextor/bicleaner-ai'
         if args.classifier_type in ['dec_attention', 'transformer']:
             model_name += f'-lite-{args.source_lang}-{args.target_lang}'
         else:
@@ -251,17 +222,18 @@
             classifier.load_spm()
             classifier.load_embed()
         except:
             classifier.train_vocab(args.mono_train, args.processes)
 
     y_true, y_pred = classifier.train(train_sentences, valid_sentences)
 
-    if args.save_train is not None and train_sentences != args.save_train:
+    if args.generated_train and train_sentences != args.generated_train:
         os.unlink(train_sentences)
-    os.unlink(valid_sentences)
+    if args.generated_valid and valid_sentences != args.generated_valid:
+        os.unlink(valid_sentences)
     logging.info("End training")
 
     args.metadata = open(args.model_dir + '/metadata.yaml', 'w+')
     write_metadata(args, classifier, y_true, y_pred, lm_stats)
     args.metadata.close()
 
     # Stats
```

### Comparing `bicleaner-ai-2.3.2/src/bicleaner_ai/calibrate.py` & `bicleaner_ai-3.0.0/src/bicleaner_ai/calibrate.py`

 * *Files identical despite different names*

### Comparing `bicleaner-ai-2.3.2/src/bicleaner_ai/classify.py` & `bicleaner_ai-3.0.0/src/bicleaner_ai/classify.py`

 * *Files 14% similar despite different names*

```diff
@@ -17,28 +17,32 @@
     from . import __version__
     from .util import check_positive, check_positive_or_zero, check_positive_between_zero_and_one, logging_setup, get_model
 except (ImportError, SystemError):
     from bicleaner_ai import __version__
     from util import check_positive, check_positive_or_zero, check_positive_between_zero_and_one, logging_setup, get_model
 
 HBS_CYR = ('hbs', 'sr', 'me', 'cnr')
+# Hardrules to be disabled when using multilingual model
+MULTI_DISABLE = ("not_too_short", "length_ratio", "no_only_numbers", "no_repeated_words", "no_wrong_language")
 
 
 # Create an argument parser and add all the arguments
 def argument_parser():
     header = "--header" in sys.argv
     parser = argparse.ArgumentParser(prog=os.path.basename(sys.argv[0]), formatter_class=argparse.ArgumentDefaultsHelpFormatter, description=__doc__)
     # Mandatory parameters
     ## Input file. Try to open it to check if it exists
     parser.add_argument('input', type=argparse.FileType('rt'), default=None, help="Tab-separated files to be classified")
     parser.add_argument('output', nargs='?', type=argparse.FileType('w'), default=sys.stdout, help="Output of the classification")
     parser.add_argument('model', type=str, default=None, help="Path to model directory or HuggingFace Hub model identifier (such as 'bitextor/bicleaner-ai-full-en-fr')")
 
     # Options group
     groupO = parser.add_argument_group('Optional')
+    groupO.add_argument("-s", "--source_lang", type=str, help="Overwrite model config source language")
+    groupO.add_argument("-t", "--target_lang", type=str, help="Overwrite model config target language")
     groupO.add_argument("-S", "--source_tokenizer_command", type=str, help="Source language (SL) tokenizer full command")
     groupO.add_argument("-T", "--target_tokenizer_command", type=str, help="Target language (TL) tokenizer full command")
 
     groupO.add_argument("--header", action='store_true', help ="Input file will be expected to have a header, and the output will have a header as well")
     groupO.add_argument("--scol", default=3 if not header else "src_text", type=check_positive if not header else str, help ="Source sentence column (starting in 1). The name of the field is expected instead of the position if --header is set")
     groupO.add_argument("--tcol", default=4 if not header else "trg_text", type=check_positive if not header else str, help ="Target sentence column (starting in 1). The name of the field is expected instead of the position if --header is set")
     groupO.add_argument('-b', '--block_size', type=int, default=10000, help="Sentence pairs per block")
@@ -78,16 +82,18 @@
     try:
         # Load YAML
         metadata_yaml = yaml.safe_load(metadata_file)
         yamldir = os.path.dirname(os.path.abspath(args.metadata))
         metadata_yaml["yamldir"] = yamldir
 
         # Read language pair and tokenizers
-        args.source_lang=metadata_yaml["source_lang"]
-        args.target_lang=metadata_yaml["target_lang"]
+        if not args.source_lang:
+            args.source_lang = metadata_yaml["source_lang"]
+        if not args.target_lang:
+            args.target_lang = metadata_yaml["target_lang"]
         if "source_tokenizer_command" in metadata_yaml:
             args.source_tokenizer_command=metadata_yaml["source_tokenizer_command"]
         if "target_tokenizer_command" in metadata_yaml:
             args.target_tokenizer_command=metadata_yaml["target_tokenizer_command"]
 
         # Load classifier
         if "calibration_params" in metadata_yaml["classifier_settings"]:
@@ -96,14 +102,20 @@
                 logging.info(f"Enabling calibrated output with parameters: {cal_params}")
         else:
             cal_params = None
         args.clf = get_model(metadata_yaml["classifier_type"])(yamldir,
                                                 metadata_yaml["classifier_settings"])
         args.clf.load()
 
+        # Check if it is a multilingual model
+        args.multilingual = False
+        if args.source_lang in ("xx", "xxx") or args.target_lang in ("xx", "xxx") \
+                or ("multilingual" in metadata_yaml and metadata["multilingual"]):
+            args.multilingual = True
+
         if "disable_lang_ident" in metadata_yaml:
             args.disable_lang_ident = metadata_yaml["disable_lang_ident"]
         else:
             args.disable_lang_ident = False
 
         # Try loading metadata for LM filtering
         if not args.disable_lm_filter:
@@ -140,18 +152,28 @@
                                 "This improves accuracy and"
                                 " does not change output text.")
         # Load rules config
         if args.rules_config:
             yaml_file = args.rules_config
             args.rules_config = yaml.safe_load(args.rules_config)
             yaml_file.close()
+        else:
+            args.rules_config = {}
+
+        # Disable the language-dependant hardules when using multilingual model
+        if args.multilingual:
+            logging.warning("Using multilingual model, disabling language-dependant rules: " + ', '.join(MULTI_DISABLE))
+            for rule in MULTI_DISABLE:
+                args.rules_config[rule] = False
 
 
-        logging.debug("YAML")
+        logging.debug("Model configuration")
         logging.debug(metadata_yaml)
+        logging.debug("Hardrules configuration")
+        logging.debug(args.rules_config)
         args.metadata_yaml = metadata_yaml
         parser.set_defaults(**metadata_yaml)
     except:
         logging.error("Error loading metadata")
         traceback.print_exc()
         sys.exit(1)
     finally:
```

### Comparing `bicleaner-ai-2.3.2/src/bicleaner_ai/datagen.py` & `bicleaner_ai-3.0.0/src/bicleaner_ai/datagen.py`

 * *Files identical despite different names*

### Comparing `bicleaner-ai-2.3.2/src/bicleaner_ai/decomposable_attention.py` & `bicleaner_ai-3.0.0/src/bicleaner_ai/decomposable_attention.py`

 * *Files identical despite different names*

### Comparing `bicleaner-ai-2.3.2/src/bicleaner_ai/layers.py` & `bicleaner_ai-3.0.0/src/bicleaner_ai/layers.py`

 * *Files identical despite different names*

### Comparing `bicleaner-ai-2.3.2/src/bicleaner_ai/losses.py` & `bicleaner_ai-3.0.0/src/bicleaner_ai/losses.py`

 * *Files identical despite different names*

### Comparing `bicleaner-ai-2.3.2/src/bicleaner_ai/metrics.py` & `bicleaner_ai-3.0.0/src/bicleaner_ai/metrics.py`

 * *Files identical despite different names*

### Comparing `bicleaner-ai-2.3.2/src/bicleaner_ai/models.py` & `bicleaner_ai-3.0.0/src/bicleaner_ai/models.py`

 * *Files 3% similar despite different names*

```diff
@@ -470,23 +470,34 @@
 
     def get_generator(self, batch_size, shuffle):
         return ConcatSentenceGenerator(
                 self.tokenizer, shuffle=shuffle,
                 batch_size=batch_size,
                 maxlen=self.settings["maxlen"])
 
-    def load_model(self, model_file):
+    def load_model(self, model_file, train=False):
         settings = self.settings
 
-        tf_model = TFXLMRBicleanerAI.from_pretrained(
-                        model_file,
-                        num_labels=settings["n_classes"],
-                        head_hidden_size=settings["n_hidden"],
-                        head_dropout=settings["dropout"],
-                        head_activation=settings["activation"])
+        tf_model, loading_info = TFXLMRBicleanerAI.from_pretrained(
+                model_file,
+                num_labels=settings["n_classes"],
+                head_hidden_size=settings["n_hidden"],
+                head_dropout=settings["dropout"],
+                head_activation=settings["activation"],
+                output_loading_info=True)
+
+        logging.debug(loading_info)
+
+        # Warn if layers do not load correctly (might be a bug)
+        # only check missng keys when inference, for training is expected
+        if loading_info["unexpected_keys"] or loading_info["mismatched_keys"] \
+                or (loading_info["missing_keys"] and not train):
+            logging.warning("Some layers were not initialized when loading model file. "
+                            "Please check that the model has been downloaded correctly "
+                            "or report this error if persists after checking.")
 
         return tf_model
 
     def load(self):
         ''' Load fine-tuned model '''
         # If vocab and model files are in a subdirectory, load from there
         if "vocab_file" in self.settings:
@@ -554,15 +565,15 @@
                                   restore_best_weights=True)
 
         logging.info("Training classifier")
 
         strategy = tf.distribute.MirroredStrategy()
         num_devices = strategy.num_replicas_in_sync
         with strategy.scope():
-            self.model = self.load_model(self.settings["base_model"])
+            self.model = self.load_model(self.settings["base_model"], train=True)
             self.model.compile(optimizer=self.settings["optimizer"],
                                loss=SparseCategoricalCrossentropy(
                                         from_logits=True),
                                metrics=[FScore(argmax=True),
                                         MatthewsCorrCoef(argmax=True)])
         self.model.config._name_or_path = self.settings["model_name"]
```

### Comparing `bicleaner-ai-2.3.2/src/bicleaner_ai/models_util.py` & `bicleaner_ai-3.0.0/src/bicleaner_ai/models_util.py`

 * *Files identical despite different names*

### Comparing `bicleaner-ai-2.3.2/src/bicleaner_ai/tokenizer.py` & `bicleaner_ai-3.0.0/src/bicleaner_ai/tokenizer.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 try:
     from .util import no_escaping
 except (SystemError, ImportError):
     from util import  no_escaping
 
 class Tokenizer:
+    @classmethod
     def get_tokenizer(cls, tok_type, l='eng'):
         if tok_type == 'char':
             return CharTokenizer()
         else:
             return WordTokenizer(l)
 
     def tokenize(self, text):
```

### Comparing `bicleaner-ai-2.3.2/src/bicleaner_ai/util.py` & `bicleaner_ai-3.0.0/src/bicleaner_ai/util.py`

 * *Files 4% similar despite different names*

```diff
@@ -110,14 +110,21 @@
     if logging.getLogger().level != logging.DEBUG:
         from transformers import logging as hf_logging
         hf_logging.set_verbosity_error()
 
         import tensorflow as tf
         tf.get_logger().setLevel('ERROR')
 
+
+def check_gpu():
+    import tensorflow as tf
+    devices = tf.config.list_physical_devices('GPU') + tf.config.list_physical_devices('TPU')
+    if not devices:
+        logging.warning("No GPU or TPU was detected. Running on CPU will be slow.")
+
 def shuffle_file(input: typing.TextIO, output: typing.TextIO):
     offsets=[]
     with TemporaryFile("w+") as temp:
         count = 0
         for line in input:
             offsets.append(count)
             count += len(bytearray(line, "UTF-8"))
```

### Comparing `bicleaner-ai-2.3.2/src/bicleaner_ai/word_freqs_list.py` & `bicleaner_ai-3.0.0/src/bicleaner_ai/word_freqs_list.py`

 * *Files identical despite different names*

### Comparing `bicleaner-ai-2.3.2/src/bicleaner_ai/word_freqs_zipf.py` & `bicleaner_ai-3.0.0/src/bicleaner_ai/word_freqs_zipf.py`

 * *Files identical despite different names*

### Comparing `bicleaner-ai-2.3.2/src/bicleaner_ai/word_freqs_zipf_double_linked.py` & `bicleaner_ai-3.0.0/src/bicleaner_ai/word_freqs_zipf_double_linked.py`

 * *Files identical despite different names*

### Comparing `bicleaner-ai-2.3.2/src/bicleaner_ai.egg-info/PKG-INFO` & `bicleaner_ai-3.0.0/src/bicleaner_ai.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bicleaner-ai
-Version: 2.3.2
+Version: 3.0.0
 Summary: Parallel corpus classifier, indicating the likelihood of a pair of sentences being mutual translations or not (neural version)
 Author-email: Prompsit Language Engineering <info@prompsit.com>
 Maintainer-email: Jaume Zaragoza <jzaragoza@prompsit.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
@@ -686,93 +686,93 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Text Processing :: Linguistic
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Text Processing :: Filters
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
-Provides-Extra: transliterate
 License-File: LICENSE
+Requires-Dist: scikit-learn>=0.22.1
+Requires-Dist: PyYAML>=5.1.2
+Requires-Dist: numpy
+Requires-Dist: pytest
+Requires-Dist: toolwrapper
+Requires-Dist: joblib
+Requires-Dist: sacremoses
+Requires-Dist: bicleaner-hardrules==2.10.3
+Requires-Dist: sentencepiece
+Requires-Dist: protobuf==3.20.3
+Requires-Dist: tensorflow<2.16,>=2.6.5
+Requires-Dist: bicleaner-ai-glove==0.2.1
+Requires-Dist: fuzzywuzzy
+Requires-Dist: python-Levenshtein
+Requires-Dist: transformers==4.36.1
+Requires-Dist: huggingface-hub<0.23,>=0.22
+Requires-Dist: zstandard
+Requires-Dist: psutil
+Requires-Dist: regex
+Provides-Extra: transliterate
+Requires-Dist: cyrtranslit==1.1; extra == "transliterate"
 
 
 # Bicleaner AI
 
 ![License](https://img.shields.io/badge/License-GPLv3-blue.svg)
 
 Bicleaner AI (`bicleaner-ai-classify`) is a tool in Python that aims at detecting noisy sentence pairs in a parallel corpus. It
 indicates the likelihood of a pair of sentences being mutual translations (with a value near to 1) or not (with a value near to 0).
 Sentence pairs considered very noisy are scored with 0.
 
 Although a training tool (`bicleaner-ai-train`) is provided, you may want to use the available ready-to-use language packages.
 Please, use `bicleaner-ai-download` to download the latest language packages or visit the [Github releases](https://github.com/bitextor/bicleaner-ai-data/releases/latest) for lite models and [Hugging Face Hub](https://huggingface.co/bitextor) for full models since v2.0.
-Visit our [Wiki](https://github.com/bitextor/bicleaner-ai/wiki/How-to-train-your-Bicleaner-AI) for a detailed example on Bicleaner training.
+Visit our [docs](docs/TRAINING.md) for a detailed example on Bicleaner training.
 
-## Citation
-If you find Bicleaner AI useful, please consider citing the following paper:
+If you find Bicleaner AI useful, please consider [citing us](#citation).
 
-> J. Zaragoza-Bernabeu, M. Bañón, G. Ramírez-Sánchez, S. Ortiz-Rojas, \
-> "[Bicleaner AI: Bicleaner Goes Neural](https://aclanthology.org/2022.lrec-1.87/)", \
-> in *Proceedings of the 13th Language Resources and Evaluation Conference*. \
-> Marseille, France: Language Resources and Evaluation Conference, June 2022
+## What is New?
+### v3.0.0 Improving Multilinguality!
+New improved multilingual models for zero-shot classification.
 
-```latex
-@inproceedings{zaragoza-bernabeu-etal-2022-bicleaner,
-    title = {"Bicleaner {AI}: Bicleaner Goes Neural"},
-    author = {"Zaragoza-Bernabeu, Jaume  and
-      Ram{\'\i}rez-S{\'a}nchez, Gema  and
-      Ba{\~n}{\'o}n, Marta  and
-      Ortiz Rojas, Sergio"},
-    booktitle = {"Proceedings of the Thirteenth Language Resources and Evaluation Conference"},
-    month = jun,
-    year = {"2022"},
-    address = {"Marseille, France"},
-    publisher = {"European Language Resources Association"},
-    url = {"https://aclanthology.org/2022.lrec-1.87"},
-    pages = {"824--831"},
-    abstract = {"This paper describes the experiments carried out during the development of the latest version of Bicleaner, named Bicleaner AI, a tool that aims at detecting noisy sentences in parallel corpora. The tool, which now implements a new neural classifier, uses state-of-the-art techniques based on pre-trained transformer-based language models fine-tuned on a binary classification task. After that, parallel corpus filtering is performed, discarding the sentences that have lower probability of being mutual translations. Our experiments, based on the training of neural machine translation (NMT) with corpora filtered using Bicleaner AI for two different scenarios, show significant improvements in translation quality compared to the previous version of the tool which implemented a classifier based on Extremely Randomized Trees."},
-}
-```
+<details>
+<summary>Previous news</summary>
 
-## What is New?
+### v2.0.0, March 10, 2023
+Model accuracy improvements and HF integration! See [CHANGELOG](https://github.com/bitextor/bicleaner-ai/blob/v2.0/CHANGELOG.md).
+
+### v1.0.0, June 6 2021
 Bicleaner AI is a [Bicleaner](https://github.com/bitextor/bicleaner) fork that uses neural networks.
 It comes with two types of models, lite models for fast scoring and full models for high performance.
 Lite models use [A Decomposable Attention Model for Natural Language Inference (Parikh et al.)](https://arxiv.org/abs/1606.01933).
 Full models use fine-tuned XLMRoberta ([Unsupervised Cross-lingual Representation Learning at Scale](https://arxiv.org/abs/1911.02116)).
 
 The use of XLMRoberta and 1:10 positive to negative ratio were inspired in the winner of WMT20 Parallel Corpus Filtering Task paper ([Filtering noisy parallel corpus using transformers with proxy task learning](https://www.statmt.org/wmt20/pdf/2020.wmt-1.105.pdf)).
 
+</details>
+
 ## Installation & Requirements
-- Python >= 3.7
-- TensorFlow >= 2.6.5
-- CUDA 11.2 (for training and inference with full models)
+- Python >= 3.8
+- PIP >= 23.0
+- CUDA >=11.2 (for training and inference with full models)
 
 Bicleaner AI is written in Python and can be installed using `pip`.
 It also requires the [KenLM](https://github.com/kpu/kenlm) Python bindings with support for 7-gram language models.
-You can easily install it by running the following commands:
+Hardrules uses [FastSpell](https://github.com/mbanon/fastspell) that requires `cyhunspell` to be installed manually.
+You can easily install all the requirements by running the following commands:
 
 ```bash
-pip install bicleaner-ai
+pip install bicleaner-ai git+https://github.com/MSeal/cython_hunspell@2.0.3
 pip install --config-settings="--build-option=--max_order=7" https://github.com/kpu/kenlm/archive/master.zip
 ```
 
-Hardrules uses [FastSpell](https://github.com/mbanon/fastspell) that requires `python-dev` and `libhunspell-dev`:
-```bash
-sudo apt install python-dev libhunspell-dev
-```
-
-Hunspell dictionaries used by default are automatically installed.
-If you need to change default configuration for language identification, see https://github.com/mbanon/fastspell#configuration.
-
 After installation, three binary files (`bicleaner-ai-train`, `bicleaner-ai-classify`, `bicleaner-ai-download`) will be located in your `python/installation/prefix/bin` directory. This is usually `$HOME/.local/bin` or `/usr/local/bin/`.
 
 ### TensorFlow
-TensorFlow 2 will be installed as a dependency and [GPU support](https://www.tensorflow.org/install/gpu) is required for training.
-`pip` will install latest TensorFlow but older versions `>=2.6.5` are supported and can be installed if your machine does not meet TensorFlow CUDA requirements.
+TensorFlow 2 will be installed as a dependency and GPU support is required for training.
+`pip` will install latest TensorFlow supported version, but older versions `>=2.6.5` are supported and can be installed if your machine does not meet TensorFlow CUDA requirements.
 See [this](https://www.tensorflow.org/install/source#gpu) table for the CUDA and TensorFlow versions compatibility.
-But current allowed versions only supoport **CUDA 11.2**.
 In case you want a different TensorFlow version, you can downgrade using:
 ```bash
 pip install tensorflow==2.6.5
 ```
 
 TensorFlow logging messages are suppressed by default, in case you want to see them you have to explicitly set `TF_CPP_MIN_LOG_LEVEL` environment variable.
 For example:
@@ -787,15 +787,15 @@
 ```
 pip install bicleaner-ai[transliterate]
 ```
 Note that this won't transliterate the output text, it will be used only for scoring.
 
 
 ## Cleaning
-### Getting Started
+### Getting started
 `bicleaner-ai-classify` aims at detecting noisy sentence pairs in a parallel corpus. It
 indicates the likelihood of a pair of sentences being mutual translations (with a value near to 1) or not (with a value near to 0). Sentence pairs considered very noisy are scored with 0.
 
 By default, the input file (the parallel corpus to be classified) expects at least four columns, being:
 
 * col1: URL 1
 * col2: URL 2
@@ -838,221 +838,103 @@
         corpus.en-fr.tsv  \
         corpus.en-fr.classifed.tsv  \
         bitextor/bicleaner-ai-full-en-fr
 ```
 where `--scol` and `--tcol` indicate the location of source and target sentence,
 `corpus.en-fr.tsv` the input file,
 `corpus.en-fr.classified.tsv` output file and `bitextor/bicleaner-ai-en-fr` is the HuggingFace model name.
-Each line of the new file will contain the same content as the input file, adding a column with the score given by the Bicleaner classifier.
+Each line of the new file will contain the same content as the input file, adding a column with the score given by the Bicleaner AI classifier.
 
 Note that, to use a lite model, you need to provide model path in your local file system, instead of HuggingFace model name.
 
 
-### Parameters
-The complete list of parameters is:
-
-* positional arguments:
-  * `input`: Tab-separated files to be classified (default line format: `URL1 URL2 SOURCE_SENTENCE TARGET_SENTENCE [EXTRA_COLUMNS]`, tab-separated). When input is -, reads standard input.
-  * `output`: Output of the classification (default: standard output). When output is -, writes standard output.
-  * `metadata`: Training metadata (YAML file), generated by `bicleaner-ai-train` or downloaded as a part of a language pack.
-  There's a script that can download and unpack it for you, use:
-  ```bash
-  $ bicleaner-ai-download en cs lite ./models
-  ```
-  to download English-Czech lite language pack to the ./models directory and unpack it.
-* optional arguments:
-  * `-h, --help`: show this help message and exit
-* Optional:
-  * `-S SOURCE_TOKENIZER_COMMAND`: Source language tokenizer full command (including flags if needed). If not given, Sacremoses tokenizer is used (with `escape=False` option).
-  * `-T TARGET_TOKENIZER_COMMAND`: Target language tokenizer full command (including flags if needed). If not given, Sacremoses tokenizer is used (with `escape=False` option).
-  * `--scol SCOL`: Source sentence column (starting in 1). If `--header` is set, the expected value will be the name of the field (default: 3 if `--header` is not set else src_text)
-  * `--tcol TCOL`: Target sentence column (starting in 1). If `--header` is set, the expected value will be the name of the field (default: 4 if `--header` is not set else trg_text)
-  * `--tmp_dir TMP_DIR`: Temporary directory where creating the temporary files of this program (default: default system temp dir, defined by the environment variable TMPDIR in Unix)
-  * `-b BLOCK_SIZE, --block_size BLOCK_SIZE`: Sentence pairs per block (default: 10000)
-  * `--lm_threshold LM_THRESHOLD`: Threshold for language model fluency scoring. All sentence pairs whose LM fluency score falls below the threshold are removed (classifier score set to 0), unless the option --keep_lm_result is set. (default: 0.5)
-  * `--score_only`: Only output one column which is the bicleaner score (default: False)
-  * `--calibrated`: Output calibrated scores (default: False)
-  * `--raw_output`: Return raw output without computing positive class probability. (default: False)
-  * `--disable_hardrules`: Disables the bicleaner_hardrules filtering (only bicleaner_classify is applied) (default: False)
-  * `--disable_lm_filter`: Disables LM filtering.
-  * `--disable_porn_removal`: Disables porn removal.
-  * `--disable_minimal_length` : Don't apply minimal length rule (default: False).
-
-* Logging:
-  * `-q, --quiet`: Silent logging mode (default: False)
-  * `--debug`: Debug logging mode (default: False)
-  * `--logfile LOGFILE`: Store log to a file (default: \<\_io.TextIOWrapper name='<stderr>' mode='w' encoding='UTF-8'\>)
-  * `-v, --version`: show version of this script and exit
-
-## Training classifiers
-
-In case you need to train a new classifier (i.e. because it is not available in the language packs provided at [bicleaner-ai-data](https://github.com/bitextor/bicleaner-ai-data/releases/latest)), you can use `bicleaner-ai-train`.
-`bicleaner-ai-train` is a Python tool that allows you to train a classifier which predicts
-whether a pair of sentences are mutual translations or not and discards too noisy sentence pairs. Visit our [Wiki](https://github.com/bitextor/bicleaner-ai/wiki/How-to-train-your-Bicleaner-AI) for a detailed example on Bicleaner AI training.
-
-### Requirements
-
-In order to train a new classifier, you must provide:
-* A clean parallel corpus (500k pairs of sentences is the recommended size).
-* Monolingual corpus for the source and the target language (not necessary for `xlmr` classifier).
-* Gzipped lists of monolingual word frequencies. You can check their format by downloading any of the available language packs.
-   * The SL list of word frequencies with one entry per line. Each entry must contain the following 2 fields, split by space, in this order: word frequency (number of times a word appears in text), SL word.
-   * The TL list of word frequencies with one entry per line. Each entry must contain the following 2 fields, split by space, in this order: word frequency (number of times a word appears in text), TL word.
-   * These lists can easily be obtained from a monolingual corpus and a command line in bash:
-```bash
-$ cat monolingual.SL \
-    | sacremoses -l SL tokenize -x \
-    | awk '{print tolower($0)}' \
-    | tr ' ' '\n' \
-    | LC_ALL=C sort | uniq -c \
-    | LC_ALL=C sort -nr \ \
-    | grep -v '[[:space:]]*1' \
-    | gzip > wordfreq-SL.gz
-$ cat monolingual.TL \
-    | sacremoses -l TL tokenize -x \
-    | awk '{print tolower($0)}' \
-    | tr ' ' '\n' \
-    | LC_ALL=C sort | uniq -c \
-    | LC_ALL=C sort -nr \ \
-    | grep -v '[[:space:]]*1' \
-    | gzip > wordfreq-TL.gz
-
-```
-Optionally, if you want the classifier to include a porn filter, you must also provide:
-* File with training dataset for porn removal classifier. Each sentence must contain at the beginning the `__label__negative` or `__label__positive` according to FastText convention. It should be lowercased and tokenized.
-
-### Parameters
-It can be used as follows.
-
-```bash
-bicleaner-ai-train [-h]
-    -m MODEL_DIR
-    -s SOURCE_LANG
-    -t TARGET_LANG
-    [--mono_train MONO_TRAIN]
-    --parallel_train PARALLEL_TRAIN
-    --parallel_dev PARALLEL_DEV
-    [-S SOURCE_TOKENIZER_COMMAND]
-    [-T TARGET_TOKENIZER_COMMAND]
-    [-F TARGET_WORD_FREQS]
-    [--block_size BLOCK_SIZE]
-    [-p PROCESSES]
-    [-g GPU]
-    [--mixed_precision]
-    [--save_train_data SAVE_TRAIN_DATA]
-    [--distilled]
-    [--seed SEED]
-    [--classifier_type {dec_attention,transformer,xlmr}]
-    [--batch_size BATCH_SIZE]
-    [--steps_per_epoch STEPS_PER_EPOCH]
-    [--epochs EPOCHS]
-    [--patience PATIENCE]
-    [--pos_ratio POS_RATIO]
-    [--rand_ratio RAND_RATIO]
-    [--womit_ratio WOMIT_RATIO]
-    [--freq_ratio FREQ_RATIO]
-    [--fuzzy_ratio FUZZY_RATIO]
-    [--neighbour_mix NEIGHBOUR_MIX]
-    [--porn_removal_train PORN_REMOVAL_TRAIN]
-    [--porn_removal_test PORN_REMOVAL_TEST]
-    [--porn_removal_file PORN_REMOVAL_FILE]
-    [--porn_removal_side {sl,tl}]
-    [--noisy_examples_file_sl NOISY_EXAMPLES_FILE_SL]
-    [--noisy_examples_file_tl NOISY_EXAMPLES_FILE_TL]
-    [--lm_dev_size LM_DEV_SIZE]
-    [--lm_file_sl LM_FILE_SL]
-    [--lm_file_tl LM_FILE_TL]
-    [--lm_training_file_sl LM_TRAINING_FILE_SL]
-    [--lm_training_file_tl LM_TRAINING_FILE_TL]
-    [--lm_clean_examples_file_sl LM_CLEAN_EXAMPLES_FILE_SL]
-    [--lm_clean_examples_file_tl LM_CLEAN_EXAMPLES_FILE_TL]
-    [-q]
-    [--debug]
-    [--logfile LOGFILE]
-```
-
-* positional arguments:
-  * `input`: Tab-separated bilingual input file (default: Standard input)(line format: SOURCE_SENTENCE TARGET_SENTENCE, tab-separated)
-* optional arguments:
-  * `-h, --help`: show this help message and exit
-* Mandatory:
-  * `-m MODEL_DIR, --model_dir MODEL_DIR`: Model directory, metadata, classifier and SentencePiece models will be saved in the same directory (default: None)
-  * `-s SOURCE_LANG, --source_lang SOURCE_LANG`: Source language (default: None)
-  * `-t TARGET_LANG, --target_lang TARGET_LANG`: Target language (default: None)
-  * `--mono_train MONO_TRAIN`: File containing monolingual sentences of both languages shuffled together, used to train SentencePiece embeddings. Not required for XLMR. (default: None)
-  * `--parallel_train PARALLEL_TRAIN`: TSV file containing parallel sentences to train the classifier (default: None)
-  * `--parallel_dev PARALLEL_DEV`: TSV file containing parallel sentences for development (default: None)
-
-* Options:
-  * `-S SOURCE_TOKENIZER_COMMAND, --source_tokenizer_command SOURCE_TOKENIZER_COMMAND`: Source language tokenizer full command (default: None)
-  * `-T TARGET_TOKENIZER_COMMAND, --target_tokenizer_command TARGET_TOKENIZER_COMMAND`: Target language tokenizer full command (default: None)
-  * `-F TARGET_WORD_FREQS, --target_word_freqs TARGET_WORD_FREQS`: R language gzipped list of word frequencies (needed for frequence based noise) (default: None)
-  * `--block_size BLOCK_SIZE`: Sentence pairs per block when apliying multiprocessing in the noise function (default: 10000)
-  * `-p PROCESSES, --processes PROCESSES`: Number of process to use (default: 71)
-  * `-g GPU, --gpu GPU`: Which GPU use, starting from 0. Will set the CUDA_VISIBLE_DEVICES. (default: None)
-  * `--mixed_precision`: Use mixed precision float16 for training (default: False)
-  * `--save_train_data SAVE_TRAIN_DATA`: Save the generated dataset into a file. If the file already exists the training dataset will be loaded from there. (default: None)
-  * `--distilled`: Enable Knowledge Distillation training. It needs pre-built training set with raw scores from a teacher model. (default: False)
-  * `--seed`: SEED           Seed for random number generation. By default, no seeed is used. (default: None)
-  * `--classifier_type {dec_attention,transformer,xlmr}`: Neural network architecture of the classifier (default: dec_attention)
-  * `--batch_size BATCH_SIZE`: Batch size during classifier training. If None, default architecture value will be used. (default: None)
-  * `--steps_per_epoch STEPS_PER_EPOCH`: Number of batch updates per epoch during training. If None, default architecture value will be used or the full dataset size. (default: None)
-  * `--epochs EPOCHS`: Number of epochs for training. If None, default architecture value will be used. (default: None)
-  * `--patience PATIENCE`: Stop training when validation has stopped improving after PATIENCE number of epochs (default: None)
-  * `--pos_ratio POS_RATIO`: Ratio of positive samples used to oversample on validation and test sets (default: 1)
-  * `--rand_ratio RAND_RATIO`: Ratio of negative samples misaligned randomly (default: 3)
-  * `--womit_ratio WOMIT_RATIO`: Ratio of negative samples misaligned by randomly omitting words (default: 3)
-  * `--freq_ratio FREQ_RATIO`: Ratio of negative samples misaligned by replacing words by frequence (needs --target_word_freq) (default: 3)
-  * `--fuzzy_ratio FUZZY_RATIO`: Ratio of negative samples misaligned by fuzzy matching (default: 0)
-  * `--neighbour_mix NEIGHBOUR_MIX`: If use negative samples misaligned by neighbourhood (default: False)
-  * `--porn_removal_train PORN_REMOVAL_TRAIN`: File with training dataset for FastText classifier. Each sentence must contain at the beginning the '__label__negative' or '__label__positive' according to FastText convention. It should be lowercased and tokenized. (default: None)
-  * `--porn_removal_test PORN_REMOVAL_TEST`: Test set to compute precision and accuracy of the porn removal classifier (default: None)
-  * `--porn_removal_file PORN_REMOVAL_FILE`: Porn removal classifier output file (default: porn_removal.bin)
-  * `--porn_removal_side {sl,tl}`: Whether the porn removal should be applied at the source or at the target language. (default: sl)
-  * `--noisy_examples_file_sl NOISY_EXAMPLES_FILE_SL`: File with noisy text in the SL. These are used to estimate the perplexity of noisy text. (default: None)
-  * `--noisy_examples_file_tl NOISY_EXAMPLES_FILE_TL`: File with noisy text in the TL. These are used to estimate the perplexity of noisy text. (default: None)
-  * `--lm_dev_size LM_DEV_SIZE`: Number of sentences to be removed from clean text before training LMs. These are used to estimate the perplexity of clean text. (default: 2000)
-  * `--lm_file_sl LM_FILE_SL`: SL language model output file. (default: None)
-  * `--lm_file_tl LM_FILE_TL`: TL language model output file. (default: None)
-  * `--lm_training_file_sl LM_TRAINING_FILE_SL`: SL text from which the SL LM is trained. If this parameter is not specified, SL LM is trained from the SL side of the input file, after removing --lm_dev_size sentences. (default: None)
-  * `--lm_training_file_tl LM_TRAINING_FILE_TL`: TL text from which the TL LM is trained. If this parameter is not specified, TL LM is trained from the TL side of the input file, after removing --lm_dev_size sentences. (default: None)
-  * `--lm_clean_examples_file_sl LM_CLEAN_EXAMPLES_FILE_SL`: File with clean text in the SL. Used to estimate the perplexity of clean text. This option must be used together with --lm_training_file_sl and both files must not have common sentences. This option replaces --lm_dev_size. (default: None)
-  * `--lm_clean_examples_file_tl LM_CLEAN_EXAMPLES_FILE_TL`: File with clean text in the TL. Used to estimate the perplexity of clean text. This option must be used together with --lm_training_file_tl and both files must not have common sentences. This option replaces --lm_dev_size. (default: None)
-* Logging:
-  * `-q, --quiet`: Silent logging mode (default: False)
-  * `--debug`: Debug logging mode (default: False)
-  * `--logfile LOGFILE`: Store log to a file (default: \<\_io.TextIOWrapper name='<stderr>' mode='w' encoding='UTF-8'>)
-
-### Example
-
-```bash
-bicleaner-ai-train \
-          --parallel_train corpus.en-cs.train \
-          --parallel_dev corpus.en-cs.dev \
-          --mono_train mono.en-cs \
-          -m models/en-cs \
-          -s en \
-          -t cs \
-          -F wordfreqs-cs.gz \
-          --lm_file_sl models/en-cs/lm.en  --lm_file_tl models/en-cs/lm.cs \
-          --porn_removal_train porn-removal.txt.en  --porn_removal_file models/en-cs/porn-model.en \
-```
-
-This will train a lite classifier for English-Czech using the corpus `corpus.en-cs.train`, the `corpus.en-cs.dev` as development set and the monolingual corpus `mono.en-cs` to train the vocabulary embeddings.
-All the model files created during training, the language model files, the porn removal file, and the `metadata.yaml` will be stored in the model directory `models/en-cs`.
-
-To train full models you would need to use `--classifier_type xlmr` and `--mono_train` is not needed.
-
-### Synthetic noise
-By default the training will use `rand_ratio`, `womit_ratio` and `freq_ratio` options with a value of 3.
-Both `womit_ratio` and `freq_ratio` will use Sacremoses tokenizer by default.
-So, for languages that are not supported by this tokenizer or are poorly supported, `source_tokenizer_command` and/or `target_tokenizer_command` should be provided.
-Also note that, if a tokenizer command is used, the word frequencies need to be tokenized in the same way to allow noise based on frequency work correctly.
-
-If no tokenization is available for your languages, you can disable these noise option that use tokenization and use fuzzy mathing noise: `--womit_ratio 0 --freq_ratio 0 --fuzzy_ratio 6`.
+#### Multilingual models
+There are multilingual full models available.
+They can work with, potentially, any language (currently only paired with English) that XLMR [supports](https://github.com/facebookresearch/fairseq/tree/main/examples/xlmr#introduction).
+To see a further explaination on how to train a multilingual model or how our models perform, take a look [here](docs/training/multilingual.md) and [here](docs/training/multilingual.md#performance).
+
+**WARNING**: multilingual models will disable hardrules that expect language parameter.
+You can, however, overwrite the language code in the model configuration with `-s`/`--source_lang` or `-t`/`--target_lang` options during classify. For example when scoring English-Icelandic data, use:
+```
+bicleaner-ai-classify \
+    --scol 1 --tcol 2 \
+    -t is \
+    corpus.en-is.tsv \
+    corpus.en-is.classified.tsv \
+    bitextor/bicleaner-ai-full-en-xx
+```
+
+### Usage
+
+<details>
+<summary>Full description of the command-line parameters:</summary>
+
+```
+usage: bicleaner-ai-classify [-h] [-s SOURCE_LANG] [-t TARGET_LANG] [-S SOURCE_TOKENIZER_COMMAND] [-T TARGET_TOKENIZER_COMMAND] [--header] [--scol SCOL] [--tcol TCOL] [-b BLOCK_SIZE] [-p PROCESSES] [--batch_size BATCH_SIZE]
+                             [--tmp_dir TMP_DIR] [--score_only] [--calibrated] [--raw_output] [--lm_threshold LM_THRESHOLD] [--disable_hardrules] [--disable_lm_filter] [--disable_porn_removal] [--disable_minimal_length]
+                             [--run_all_rules] [--rules_config RULES_CONFIG] [--offline] [--auth_token AUTH_TOKEN] [-q] [--debug] [--logfile LOGFILE] [-v]
+                             input [output] model
+
+positional arguments:
+  input                 Tab-separated files to be classified
+  output                Output of the classification (default: <_io.TextIOWrapper name='<stdout>' mode='w' encoding='utf-8'>)
+  model                 Path to model directory or HuggingFace Hub model identifier (such as 'bitextor/bicleaner-ai-full-en-fr')
+
+options:
+  -h, --help            show this help message and exit
+
+Optional:
+  -s SOURCE_LANG, --source_lang SOURCE_LANG
+                        Overwrite model config source language (default: None)
+  -t TARGET_LANG, --target_lang TARGET_LANG
+                        Overwrite model config target language (default: None)
+  -S SOURCE_TOKENIZER_COMMAND, --source_tokenizer_command SOURCE_TOKENIZER_COMMAND
+                        Source language (SL) tokenizer full command (default: None)
+  -T TARGET_TOKENIZER_COMMAND, --target_tokenizer_command TARGET_TOKENIZER_COMMAND
+                        Target language (TL) tokenizer full command (default: None)
+  --header              Input file will be expected to have a header, and the output will have a header as well (default: False)
+  --scol SCOL           Source sentence column (starting in 1). The name of the field is expected instead of the position if --header is set (default: 3)
+  --tcol TCOL           Target sentence column (starting in 1). The name of the field is expected instead of the position if --header is set (default: 4)
+  -b BLOCK_SIZE, --block_size BLOCK_SIZE
+                        Sentence pairs per block (default: 10000)
+  -p PROCESSES, --processes PROCESSES
+                        Option no longer available, please set BICLEANER_AI_THREADS environment variable (default: None)
+  --batch_size BATCH_SIZE
+                        Sentence pairs per block (default: 32)
+  --tmp_dir TMP_DIR     Temporary directory where creating the temporary files of this program (default: /tmp)
+  --score_only          Only output one column which is the bicleaner score (default: False)
+  --calibrated          Output calibrated scores (default: False)
+  --raw_output          Return raw output without computing positive class probability. (default: False)
+  --lm_threshold LM_THRESHOLD
+                        Threshold for language model fluency scoring. All TUs whose LM fluency score falls below the threshold will are removed (classifier score set to 0), unless the option --keep_lm_result set. (default: 0.5)
+  --disable_hardrules   Disables the bicleaner_hardrules filtering (only bicleaner_classify is applied) (default: False)
+  --disable_lm_filter   Disables LM filtering (default: False)
+  --disable_porn_removal
+                        Don't apply porn removal (default: False)
+  --disable_minimal_length
+                        Don't apply minimal length rule (default: False)
+  --run_all_rules       Run all rules of Hardrules instead of stopping at first discard (default: False)
+  --rules_config RULES_CONFIG
+                        Hardrules configuration file (default: None)
+  --offline             Don't try to download the model, instead try directly to load from local storage (default: False)
+  --auth_token AUTH_TOKEN
+                        Auth token for the Hugging Face Hub (default: None)
+
+Logging:
+  -q, --quiet           Silent logging mode (default: False)
+  --debug               Debug logging mode (default: False)
+  --logfile LOGFILE     Store log to a file (default: <_io.TextIOWrapper name='<stderr>' mode='w' encoding='utf-8'>)
+  -v, --version         Show version of the package and exit
+```
+
+</details>
+
+## Training models
+Bicleaner AI provides a command-line tool to train your own model, in case available models do not fit your needs.
+Please go to our [training documentation](docs/training) for a quick start and further details.
 
 ## Setting the number of threads
 To set the maximum number of threads/processes to be used during training or classifying, `--processes` option is no longer available.
 You will need to set `BICLEANER_AI_THREADS` environment variable to the desired value.
 For example:
 ```
 BICLEANER_AI_THREADS=12 bicleaner-ai-classify ...
@@ -1065,12 +947,38 @@
 | model | speed CPUx1 | speed GPUx1 |
 | ----- | ----------- | ----------- |
 | full | 1.78 rows/sec | 200 rows/sec |
 | lite | 600 rows/sec | 10,000 rows/sec |
 
 * CPU: Intel Core i9-9960X single core (lite model batch 16, full model batch 1)
 * GPU: Nvidia V100 (lite model batch 2048, full model batch 16)
+
+## Citation
+
+> J. Zaragoza-Bernabeu, M. Bañón, G. Ramírez-Sánchez, S. Ortiz-Rojas, \
+> "[Bicleaner AI: Bicleaner Goes Neural](https://aclanthology.org/2022.lrec-1.87/)", \
+> in *Proceedings of the 13th Language Resources and Evaluation Conference*. \
+> Marseille, France: Language Resources and Evaluation Conference, June 2022
+
+```latex
+@inproceedings{zaragoza-bernabeu-etal-2022-bicleaner,
+    title = {"Bicleaner {AI}: Bicleaner Goes Neural"},
+    author = {"Zaragoza-Bernabeu, Jaume  and
+      Ram{\'\i}rez-S{\'a}nchez, Gema  and
+      Ba{\~n}{\'o}n, Marta  and
+      Ortiz Rojas, Sergio"},
+    booktitle = {"Proceedings of the Thirteenth Language Resources and Evaluation Conference"},
+    month = jun,
+    year = {"2022"},
+    address = {"Marseille, France"},
+    publisher = {"European Language Resources Association"},
+    url = {"https://aclanthology.org/2022.lrec-1.87"},
+    pages = {"824--831"},
+    abstract = {"This paper describes the experiments carried out during the development of the latest version of Bicleaner, named Bicleaner AI, a tool that aims at detecting noisy sentences in parallel corpora. The tool, which now implements a new neural classifier, uses state-of-the-art techniques based on pre-trained transformer-based language models fine-tuned on a binary classification task. After that, parallel corpus filtering is performed, discarding the sentences that have lower probability of being mutual translations. Our experiments, based on the training of neural machine translation (NMT) with corpora filtered using Bicleaner AI for two different scenarios, show significant improvements in translation quality compared to the previous version of the tool which implemented a classifier based on Extremely Randomized Trees."},
+}
+```
+
 ___
 
 ![Connecting Europe Facility](https://www.paracrawl.eu/images/logo_en_cef273x39.png)
 
 All documents and software contained in this repository reflect only the authors' view. The Innovation and Networks Executive Agency of the European Union is not responsible for any use that may be made of the information it contains.
```

### Comparing `bicleaner-ai-2.3.2/src/bicleaner_ai.egg-info/SOURCES.txt` & `bicleaner_ai-3.0.0/src/bicleaner_ai.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 LICENSE
 README.md
 pyproject.toml
 src/bicleaner_ai/__init__.py
 src/bicleaner_ai/bicleaner_ai_classifier.py
 src/bicleaner_ai/bicleaner_ai_download.py
 src/bicleaner_ai/bicleaner_ai_download_hf.py
+src/bicleaner_ai/bicleaner_ai_generate_train.py
 src/bicleaner_ai/bicleaner_ai_train.py
 src/bicleaner_ai/calibrate.py
 src/bicleaner_ai/classify.py
 src/bicleaner_ai/datagen.py
 src/bicleaner_ai/decomposable_attention.py
 src/bicleaner_ai/layers.py
 src/bicleaner_ai/losses.py
 src/bicleaner_ai/metrics.py
 src/bicleaner_ai/models.py
 src/bicleaner_ai/models_util.py
+src/bicleaner_ai/noise_generation.py
 src/bicleaner_ai/tokenizer.py
 src/bicleaner_ai/training.py
 src/bicleaner_ai/util.py
 src/bicleaner_ai/word_freqs_list.py
 src/bicleaner_ai/word_freqs_zipf.py
 src/bicleaner_ai/word_freqs_zipf_double_linked.py
 src/bicleaner_ai.egg-info/PKG-INFO
```

