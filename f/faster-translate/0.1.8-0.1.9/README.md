# Comparing `tmp/faster_translate-0.1.8.tar.gz` & `tmp/faster_translate-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "faster_translate-0.1.8.tar", last modified: Sun Apr 14 19:05:04 2024, max compression
+gzip compressed data, was "faster_translate-0.1.9.tar", last modified: Tue Apr 16 13:56:14 2024, max compression
```

## Comparing `faster_translate-0.1.8.tar` & `faster_translate-0.1.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxr-x   0 sawradip  (1000) sawradip  (1000)        0 2024-04-14 19:05:04.081675 faster_translate-0.1.8/
--rw-rw-r--   0 sawradip  (1000) sawradip  (1000)     1069 2024-04-13 18:30:01.000000 faster_translate-0.1.8/LICENSE
--rw-r--r--   0 sawradip  (1000) sawradip  (1000)     4786 2024-04-14 19:05:04.081675 faster_translate-0.1.8/PKG-INFO
--rw-rw-r--   0 sawradip  (1000) sawradip  (1000)     2974 2024-04-13 18:30:01.000000 faster_translate-0.1.8/README.md
-drwxrwxr-x   0 sawradip  (1000) sawradip  (1000)        0 2024-04-14 19:05:04.081675 faster_translate-0.1.8/faster_translate/
--rw-rw-r--   0 sawradip  (1000) sawradip  (1000)       75 2024-04-13 18:35:30.000000 faster_translate-0.1.8/faster_translate/__init__.py
--rw-rw-r--   0 sawradip  (1000) sawradip  (1000)     7356 2024-04-14 19:00:54.000000 faster_translate-0.1.8/faster_translate/model.py
--rw-rw-r--   0 sawradip  (1000) sawradip  (1000)     2244 2024-04-14 18:54:44.000000 faster_translate-0.1.8/faster_translate/utils.py
-drwxrwxr-x   0 sawradip  (1000) sawradip  (1000)        0 2024-04-14 19:05:04.081675 faster_translate-0.1.8/faster_translate.egg-info/
--rw-r--r--   0 sawradip  (1000) sawradip  (1000)     4786 2024-04-14 19:05:04.000000 faster_translate-0.1.8/faster_translate.egg-info/PKG-INFO
--rw-rw-r--   0 sawradip  (1000) sawradip  (1000)      312 2024-04-14 19:05:04.000000 faster_translate-0.1.8/faster_translate.egg-info/SOURCES.txt
--rw-rw-r--   0 sawradip  (1000) sawradip  (1000)        1 2024-04-14 19:05:04.000000 faster_translate-0.1.8/faster_translate.egg-info/dependency_links.txt
--rw-rw-r--   0 sawradip  (1000) sawradip  (1000)       91 2024-04-14 19:05:04.000000 faster_translate-0.1.8/faster_translate.egg-info/requires.txt
--rw-rw-r--   0 sawradip  (1000) sawradip  (1000)       17 2024-04-14 19:05:04.000000 faster_translate-0.1.8/faster_translate.egg-info/top_level.txt
--rw-rw-r--   0 sawradip  (1000) sawradip  (1000)      676 2024-04-14 19:04:59.000000 faster_translate-0.1.8/pyproject.toml
--rw-rw-r--   0 sawradip  (1000) sawradip  (1000)       38 2024-04-14 19:05:04.081675 faster_translate-0.1.8/setup.cfg
+drwxrwxr-x   0 sawradip  (1000) sawradip  (1000)        0 2024-04-16 13:56:14.198938 faster_translate-0.1.9/
+-rw-rw-r--   0 sawradip  (1000) sawradip  (1000)     1069 2024-04-13 18:30:01.000000 faster_translate-0.1.9/LICENSE
+-rw-r--r--   0 sawradip  (1000) sawradip  (1000)     4786 2024-04-16 13:56:14.198938 faster_translate-0.1.9/PKG-INFO
+-rw-rw-r--   0 sawradip  (1000) sawradip  (1000)     2974 2024-04-13 18:30:01.000000 faster_translate-0.1.9/README.md
+drwxrwxr-x   0 sawradip  (1000) sawradip  (1000)        0 2024-04-16 13:56:14.198938 faster_translate-0.1.9/faster_translate/
+-rw-rw-r--   0 sawradip  (1000) sawradip  (1000)       75 2024-04-13 18:35:30.000000 faster_translate-0.1.9/faster_translate/__init__.py
+-rw-rw-r--   0 sawradip  (1000) sawradip  (1000)     8362 2024-04-16 13:48:33.000000 faster_translate-0.1.9/faster_translate/model.py
+-rw-rw-r--   0 sawradip  (1000) sawradip  (1000)     2327 2024-04-16 13:51:04.000000 faster_translate-0.1.9/faster_translate/utils.py
+drwxrwxr-x   0 sawradip  (1000) sawradip  (1000)        0 2024-04-16 13:56:14.198938 faster_translate-0.1.9/faster_translate.egg-info/
+-rw-r--r--   0 sawradip  (1000) sawradip  (1000)     4786 2024-04-16 13:56:14.000000 faster_translate-0.1.9/faster_translate.egg-info/PKG-INFO
+-rw-rw-r--   0 sawradip  (1000) sawradip  (1000)      312 2024-04-16 13:56:14.000000 faster_translate-0.1.9/faster_translate.egg-info/SOURCES.txt
+-rw-rw-r--   0 sawradip  (1000) sawradip  (1000)        1 2024-04-16 13:56:14.000000 faster_translate-0.1.9/faster_translate.egg-info/dependency_links.txt
+-rw-rw-r--   0 sawradip  (1000) sawradip  (1000)       91 2024-04-16 13:56:14.000000 faster_translate-0.1.9/faster_translate.egg-info/requires.txt
+-rw-rw-r--   0 sawradip  (1000) sawradip  (1000)       17 2024-04-16 13:56:14.000000 faster_translate-0.1.9/faster_translate.egg-info/top_level.txt
+-rw-rw-r--   0 sawradip  (1000) sawradip  (1000)      676 2024-04-16 13:55:54.000000 faster_translate-0.1.9/pyproject.toml
+-rw-rw-r--   0 sawradip  (1000) sawradip  (1000)       38 2024-04-16 13:56:14.198938 faster_translate-0.1.9/setup.cfg
```

### Comparing `faster_translate-0.1.8/LICENSE` & `faster_translate-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `faster_translate-0.1.8/PKG-INFO` & `faster_translate-0.1.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: faster_translate
-Version: 0.1.8
+Version: 0.1.9
 Summary: A simple translation utility using Hugging Face models.
 Author-email: Sawradip Saha <sawradip0@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Sawradip Saha
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `faster_translate-0.1.8/README.md` & `faster_translate-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `faster_translate-0.1.8/faster_translate/model.py` & `faster_translate-0.1.9/faster_translate/model.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import os
 import json
 import subprocess
 import ctranslate2
 from tqdm.auto import tqdm
 from tokenizers import Tokenizer
 from tokenizers.models import BPE
+from transformers import AutoTokenizer
 from tokenizers.pre_tokenizers import Whitespace
 from tokenizers.trainers import BpeTrainer
 
 from .utils import download_model_hf, _MODELS
 
 
 def is_cuda_available():
@@ -24,45 +25,55 @@
         return True
 
     return False
 
 device_name = "cuda" if is_cuda_available() else "cpu"
 
 class TranslateModel:
-    def __init__(self, model_dir, source_token_list = None, tokenizer_filename = None, normalizer_func=None, device = device_name):
+    def __init__(self, model_dir, source_token_list = None, tokenizer_filename = None, tokenizer_repo = None, normalizer_func=None, device = device_name):
         self.model_dir = model_dir
         self.translator = ctranslate2.Translator(model_dir, device=device)
         
         if normalizer_func is None:
             self.normalizer_func = lambda x: x
         elif isinstance(normalizer_func, str):
             self.normalizer_func = self.get_text_normalizer(normalizer_func)
         else:
             self.normalizer_func = normalizer_func
             
-            
-        if source_token_list is None:
-            source_token_list = self.get_token_list(tokenizer_filename)
-        self.source_tokenizer = self.get_bpe_tokenizer(source_token_list)
-        
+        self.source_tokenizer = self.get_hf_tokenizer(tokenizer_repo)
+        if self.source_tokenizer is None:
+            if source_token_list is None:
+                source_token_list = self.get_token_list(tokenizer_filename)
+            self.source_tokenizer = self.get_bpe_tokenizer(source_token_list)
+        
+    def get_hf_tokenizer(self, tokenizer_repo):
+        if tokenizer_repo is not None:
+            return  AutoTokenizer.from_pretrained(tokenizer_repo)
+        elif os.path.isfile(os.path.join(self.model_dir, 'tokenizer_config.json')):
+            return  AutoTokenizer.from_pretrained(self.model_dir)
+        else:
+            return None       
+         
     def get_token_list(self, tokenizer_filename):
+        
         if tokenizer_filename is not None:
             tokenizer_filepath  = os.path.join(self.model_dir, tokenizer_filename)
         elif os.path.isfile(os.path.join(self.model_dir, "source_vocabulary.json")):
             tokenizer_filepath  = os.path.join(self.model_dir, "source_vocabulary.json")
         elif os.path.isfile(os.path.join(self.model_dir, "shared_vocabulary.json")):
             tokenizer_filepath  = os.path.join(self.model_dir, "shared_vocabulary.json")
         else:
             raise Exception("Vocabulary file was not found.")
         
-            # self.source_tokenizer_json = os.path.join(model_dir, "source_vocabulary.json")
         with open(tokenizer_filepath, 'r', encoding='utf-8') as file:
             source_token_list = json.load(file)
         return source_token_list
     
+
         
     def get_bpe_tokenizer(self, token_list):
         
         # Initialize a tokenizer
         tokenizer = Tokenizer(BPE(unk_token="<unk>"))
         tokenizer.pre_tokenizer = Whitespace()
         
@@ -70,16 +81,20 @@
         trainer = BpeTrainer(special_tokens=token_list, vocab_size=len(token_list), min_frequency=1)
         tokenizer.train_from_iterator(token_list, trainer=trainer)
         
         return tokenizer
     
     
     def source_tokenize_batch(self, text_batch):
-        text_batch = [f" {text}".replace(" ", "▁") for text in text_batch]
-        tokenized_batch = [encoded.tokens for encoded in self.source_tokenizer.encode_batch(text_batch)]
+        if isinstance(self.source_tokenizer, Tokenizer):
+            text_batch = [f" {text}".replace(" ", "▁") for text in text_batch]
+            tokenized_batch = [encoded.tokens for encoded in self.source_tokenizer.encode_batch(text_batch)]
+        else:
+            tokenized_batch = [self.source_tokenizer.convert_ids_to_tokens(
+                                    input_id_list) for input_id_list in self.source_tokenizer(text_batch)["input_ids"]]
         return tokenized_batch
     
     
     def get_text_normalizer(self, normalizer_func_name):
         if normalizer_func_name == "buetnlpnormalizer":
             try:
                 from normalizer import normalize
@@ -89,18 +104,20 @@
             normalizer_func = lambda texts: [normalize(text) for text in texts]
         else:
             raise Exception(f"{normalizer_func_name} not supported yet.")
         return normalizer_func
         
         
     def detokenize_single(self, tokens):
-        # Concatenate, replace special prefix, and handle edge cases
-        concatenated = ''.join(tokens)
-        proper_string = concatenated.replace('▁', ' ').strip()
-        proper_string = proper_string.replace(' ,', ',').replace(' .', '.').replace(" '", "'").replace(" :", ":")
+        if isinstance(self.source_tokenizer, Tokenizer):
+            concatenated = ''.join(tokens)
+            proper_string = concatenated.replace('▁', ' ').strip()
+            proper_string = proper_string.replace(' ,', ',').replace(' .', '.').replace(" '", "'").replace(" :", ":")
+        else:
+            proper_string = self.source_tokenizer.decode(self.source_tokenizer.convert_tokens_to_ids(tokens), skip_special_tokens=True)
         return proper_string
     
     
     def detokenize_batch(self, token_batch):
         translated_decoded_batch = [self.detokenize_single(pred.hypotheses[0]) for pred in token_batch]
         return translated_decoded_batch
     
@@ -140,29 +157,30 @@
             with open(file_path, 'w') as file:
                 file.write(translated_str)
                 
         return translated_results
     
     
     @classmethod
-    def from_pretrained(cls, model_name_or_path, save_path=None, revision=None, token=None, **kwargs):
+    def from_pretrained(cls, model_name_or_path, save_path=None, revision=None, token=None, tokenizer_repo = None, **kwargs):
         """
         This is for loading any pre converted translation model from huggingface.
     
 
         Parameters:
         - model_identifier: The name of the Hugging Face repository (e.g., "sawradip/faster-translate-banglanmt-bn2en-t5") or a local directory path.
         - save_path: The local path where the repository should be downloaded. If None, uses the default cache directory. Ignored if model_identifier is a local directory.
         - revision: The specific repository revision to download. If None, the latest version is downloaded. Ignored if model_identifier is a local directory.
         - token: An optional Hugging Face authentication token for private repositories. Ignored if model_identifier is a local directory.
         """
         
         if model_name_or_path in _MODELS:
             model_args = _MODELS[model_name_or_path]
             kwargs["normalizer_func"] = model_args.get("normalizer_func")
+            kwargs["tokenizer_repo"] = tokenizer_repo if tokenizer_repo else model_args.get("tokenizer_repo")
             
         # Check if model_identifier is a local directory
         if os.path.isdir(model_name_or_path):
             print(f"Loading model from local directory: {model_name_or_path}")
             model_path = model_name_or_path
         else:
             # Download the model using the utility function from faster_translate/utils.py
```

### Comparing `faster_translate-0.1.8/faster_translate/utils.py` & `faster_translate-0.1.9/faster_translate/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 from huggingface_hub import HfApi, snapshot_download
 import os
 
 _MODELS = {
     "banglanmt_bn2en": {
         "model_repo": "sawradip/faster-translate-banglanmt-bn2en-t5",
-        "normalizer_func":"buetnlpnormalizer"
+        "normalizer_func":"buetnlpnormalizer",
     },
     "banglanmt_en2bn": {
-        "model_repo": "sawradip/faster-translate-banglanmt-en2bn-t5"
+        "model_repo": "sawradip/faster-translate-banglanmt-en2bn-t5",
+        
     },
-    "banglabertv1_en2bn": {
-        "model_repo": "sawradip/faster-translate-banglabart-en2bn-v1"
+    "bangla_mbartv1_en2bn": {
+        "model_repo": "sawradip/faster-translate-banglabart-en2bn-v1",
+        "tokenizer_repo": "facebook/mbart-large-50-many-to-many-mmt"
     }
 }
 def upload_model_hf(repo_name, folder_path, token ):
     """
     Upload all files from a folder to a Hugging Face repository.
 
     Parameters:
```

### Comparing `faster_translate-0.1.8/faster_translate.egg-info/PKG-INFO` & `faster_translate-0.1.9/faster_translate.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: faster_translate
-Version: 0.1.8
+Version: 0.1.9
 Summary: A simple translation utility using Hugging Face models.
 Author-email: Sawradip Saha <sawradip0@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Sawradip Saha
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `faster_translate-0.1.8/pyproject.toml` & `faster_translate-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "faster_translate"
-version = "0.1.8"
+version = "0.1.9"
 description = "A simple translation utility using Hugging Face models."
 readme = "README.md"
 authors = [{name = "Sawradip Saha", email = "sawradip0@gmail.com"}]
 license = {file = "LICENSE"}
 keywords = ["translation", "huggingface", "nlp"]
 classifiers = [
     "Programming Language :: Python :: 3",
```

