# Comparing `tmp/llm2vec-0.1.2.tar.gz` & `tmp/llm2vec-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "llm2vec-0.1.2.tar", last modified: Thu Apr  4 21:59:15 2024, max compression
+gzip compressed data, was "llm2vec-0.1.3.tar", last modified: Tue Apr 16 16:57:16 2024, max compression
```

## Comparing `llm2vec-0.1.2.tar` & `llm2vec-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,22 @@
-drwxr-xr-x   0 vaibhav.adlakha   (502) staff       (20)        0 2024-04-04 21:59:15.035776 llm2vec-0.1.2/
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)     1067 2024-04-04 20:24:53.000000 llm2vec-0.1.2/LICENSE
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)     4920 2024-04-04 21:59:15.035931 llm2vec-0.1.2/PKG-INFO
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)     4470 2024-04-04 20:25:54.000000 llm2vec-0.1.2/README.md
-drwxr-xr-x   0 vaibhav.adlakha   (502) staff       (20)        0 2024-04-04 21:59:15.031611 llm2vec-0.1.2/llm2vec/
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)       28 2024-04-04 20:24:53.000000 llm2vec-0.1.2/llm2vec/__init__.py
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)    10405 2024-04-04 21:59:01.000000 llm2vec-0.1.2/llm2vec/llm2vec.py
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)       22 2024-04-04 21:58:58.000000 llm2vec-0.1.2/llm2vec/version.py
-drwxr-xr-x   0 vaibhav.adlakha   (502) staff       (20)        0 2024-04-04 21:59:15.035366 llm2vec-0.1.2/llm2vec.egg-info/
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)     4920 2024-04-04 21:59:14.000000 llm2vec-0.1.2/llm2vec.egg-info/PKG-INFO
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)      278 2024-04-04 21:59:14.000000 llm2vec-0.1.2/llm2vec.egg-info/SOURCES.txt
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)        1 2024-04-04 21:59:14.000000 llm2vec-0.1.2/llm2vec.egg-info/dependency_links.txt
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)        1 2024-04-04 20:26:27.000000 llm2vec-0.1.2/llm2vec.egg-info/not-zip-safe
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)       43 2024-04-04 21:59:14.000000 llm2vec-0.1.2/llm2vec.egg-info/requires.txt
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)        8 2024-04-04 21:59:14.000000 llm2vec-0.1.2/llm2vec.egg-info/top_level.txt
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)       79 2024-04-04 21:59:15.036602 llm2vec-0.1.2/setup.cfg
--rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)     1024 2024-04-04 20:24:53.000000 llm2vec-0.1.2/setup.py
+drwxr-xr-x   0 vaibhav.adlakha   (502) staff       (20)        0 2024-04-16 16:57:16.572394 llm2vec-0.1.3/
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)     1067 2024-04-08 21:09:47.000000 llm2vec-0.1.3/LICENSE
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)     6536 2024-04-16 16:57:16.572627 llm2vec-0.1.3/PKG-INFO
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)     6086 2024-04-16 16:56:44.000000 llm2vec-0.1.3/README.md
+drwxr-xr-x   0 vaibhav.adlakha   (502) staff       (20)        0 2024-04-16 16:57:16.562083 llm2vec-0.1.3/llm2vec/
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)       29 2024-04-16 16:56:44.000000 llm2vec-0.1.3/llm2vec/__init__.py
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)    14576 2024-04-16 16:56:44.000000 llm2vec-0.1.3/llm2vec/llm2vec.py
+drwxr-xr-x   0 vaibhav.adlakha   (502) staff       (20)        0 2024-04-16 16:57:16.571452 llm2vec-0.1.3/llm2vec/models/
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)      130 2024-04-16 16:56:44.000000 llm2vec-0.1.3/llm2vec/models/__init__.py
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)     7620 2024-04-16 16:56:44.000000 llm2vec-0.1.3/llm2vec/models/attn_mask_utils.py
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)     7348 2024-04-16 16:56:44.000000 llm2vec-0.1.3/llm2vec/models/bidirectional_llama.py
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)    10038 2024-04-16 16:56:44.000000 llm2vec-0.1.3/llm2vec/models/bidirectional_mistral.py
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)       22 2024-04-16 16:57:09.000000 llm2vec-0.1.3/llm2vec/version.py
+drwxr-xr-x   0 vaibhav.adlakha   (502) staff       (20)        0 2024-04-16 16:57:16.566650 llm2vec-0.1.3/llm2vec.egg-info/
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)     6536 2024-04-16 16:57:16.000000 llm2vec-0.1.3/llm2vec.egg-info/PKG-INFO
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)      417 2024-04-16 16:57:16.000000 llm2vec-0.1.3/llm2vec.egg-info/SOURCES.txt
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)        1 2024-04-16 16:57:16.000000 llm2vec-0.1.3/llm2vec.egg-info/dependency_links.txt
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)        1 2024-04-16 16:57:16.000000 llm2vec-0.1.3/llm2vec.egg-info/not-zip-safe
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)       43 2024-04-16 16:57:16.000000 llm2vec-0.1.3/llm2vec.egg-info/requires.txt
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)        8 2024-04-16 16:57:16.000000 llm2vec-0.1.3/llm2vec.egg-info/top_level.txt
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)       79 2024-04-16 16:57:16.573459 llm2vec-0.1.3/setup.cfg
+-rw-r--r--   0 vaibhav.adlakha   (502) staff       (20)     1024 2024-04-16 16:56:44.000000 llm2vec-0.1.3/setup.py
```

### Comparing `llm2vec-0.1.2/LICENSE` & `llm2vec-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `llm2vec-0.1.2/setup.py` & `llm2vec-0.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     python_requires=">=3.8",
     packages=find_packages(include=[f"{package_name}*"]),
     install_requires=[
         "numpy",
         "tqdm",
         "torch",
         "peft",
-        "transformers>=4.38.1"
+        "transformers>=4.39.1"
     ],
     classifiers=[
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
         "License :: OSI Approved :: MIT License",
     ],
     license='MIT',
```

