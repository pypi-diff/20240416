# Comparing `tmp/bicleaner_ai-3.0.0.tar.gz` & `tmp/bicleaner_ai-3.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bicleaner_ai-3.0.0.tar", last modified: Tue Apr 16 14:12:40 2024, max compression
+gzip compressed data, was "bicleaner_ai-3.0.1.tar", last modified: Tue Apr 16 15:13:58 2024, max compression
```

## Comparing `bicleaner_ai-3.0.0.tar` & `bicleaner_ai-3.0.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:12:40.500031 bicleaner_ai-3.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-04-16 14:12:34.000000 bicleaner_ai-3.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    57475 2024-04-16 14:12:40.500031 bicleaner_ai-3.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15362 2024-04-16 14:12:34.000000 bicleaner_ai-3.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-04-16 14:12:34.000000 bicleaner_ai-3.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 14:12:40.500031 bicleaner_ai-3.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:12:40.492031 bicleaner_ai-3.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:12:40.500031 bicleaner_ai-3.0.0/src/bicleaner_ai/
--rwxr-xr-x   0 runner    (1001) docker     (127)      112 2024-04-16 14:12:34.000000 bicleaner_ai-3.0.0/src/bicleaner_ai/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4586 2024-04-16 14:12:34.000000 bicleaner_ai-3.0.0/src/bicleaner_ai/bicleaner_ai_classifier.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4458 2024-04-16 14:12:34.000000 bicleaner_ai-3.0.0/src/bicleaner_ai/bicleaner_ai_download.py
--rwxr-xr-x   0 runner    (1001) docker     (127)      642 2024-04-16 14:12:34.000000 bicleaner_ai-3.0.0/src/bicleaner_ai/bicleaner_ai_download_hf.py
--rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-04-16 14:12:34.000000 bicleaner_ai-3.0.0/src/bicleaner_ai/bicleaner_ai_generate_train.py
--rwxr-xr-x   0 runner    (1001) docker     (127)    13857 2024-04-16 14:12:34.000000 bicleaner_ai-3.0.0/src/bicleaner_ai/bicleaner_ai_train.py
--rw-r--r--   0 runner    (1001) docker     (127)     2964 2024-04-16 14:12:34.000000 bicleaner_ai-3.0.0/src/bicleaner_ai/calibrate.py
--rw-r--r--   0 runner    (1001) docker     (127)    15330 2024-04-16 14:12:34.000000 bicleaner_ai-3.0.0/src/bicleaner_ai/classify.py
--rw-r--r--   0 runner    (1001) docker     (127)     6479 2024-04-16 14:12:34.000000 bicleaner_ai-3.0.0/src/bicleaner_ai/datagen.py
--rw-r--r--   0 runner    (1001) docker     (127)     7456 2024-04-16 14:12:34.000000 bicleaner_ai-3.0.0/src/bicleaner_ai/decomposable_attention.py
--rw-r--r--   0 runner    (1001) docker     (127)     3927 2024-04-16 14:12:34.000000 bicleaner_ai-3.0.0/src/bicleaner_ai/layers.py
--rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-04-16 14:12:34.000000 bicleaner_ai-3.0.0/src/bicleaner_ai/losses.py
--rw-r--r--   0 runner    (1001) docker     (127)     6372 2024-04-16 14:12:34.000000 bicleaner_ai-3.0.0/src/bicleaner_ai/metrics.py
--rw-r--r--   0 runner    (1001) docker     (127)    25856 2024-04-16 14:12:34.000000 bicleaner_ai-3.0.0/src/bicleaner_ai/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     4101 2024-04-16 14:12:34.000000 bicleaner_ai-3.0.0/src/bicleaner_ai/models_util.py
--rw-r--r--   0 runner    (1001) docker     (127)    12203 2024-04-16 14:12:34.000000 bicleaner_ai-3.0.0/src/bicleaner_ai/noise_generation.py
--rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-16 14:12:34.000000 bicleaner_ai-3.0.0/src/bicleaner_ai/tokenizer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4744 2024-04-16 14:12:34.000000 bicleaner_ai-3.0.0/src/bicleaner_ai/training.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     4249 2024-04-16 14:12:34.000000 bicleaner_ai-3.0.0/src/bicleaner_ai/util.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1351 2024-04-16 14:12:34.000000 bicleaner_ai-3.0.0/src/bicleaner_ai/word_freqs_list.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     3123 2024-04-16 14:12:34.000000 bicleaner_ai-3.0.0/src/bicleaner_ai/word_freqs_zipf.py
--rwxr-xr-x   0 runner    (1001) docker     (127)     1082 2024-04-16 14:12:34.000000 bicleaner_ai-3.0.0/src/bicleaner_ai/word_freqs_zipf_double_linked.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:12:40.500031 bicleaner_ai-3.0.0/src/bicleaner_ai.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    57475 2024-04-16 14:12:40.000000 bicleaner_ai-3.0.0/src/bicleaner_ai.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-04-16 14:12:40.000000 bicleaner_ai-3.0.0/src/bicleaner_ai.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 14:12:40.000000 bicleaner_ai-3.0.0/src/bicleaner_ai.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-16 14:12:40.000000 bicleaner_ai-3.0.0/src/bicleaner_ai.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-16 14:12:40.000000 bicleaner_ai-3.0.0/src/bicleaner_ai.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-16 14:12:40.000000 bicleaner_ai-3.0.0/src/bicleaner_ai.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:13:57.996266 bicleaner_ai-3.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    35147 2024-04-16 15:13:53.000000 bicleaner_ai-3.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    57475 2024-04-16 15:13:57.996266 bicleaner_ai-3.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15362 2024-04-16 15:13:53.000000 bicleaner_ai-3.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2161 2024-04-16 15:13:53.000000 bicleaner_ai-3.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 15:13:57.996266 bicleaner_ai-3.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:13:57.992266 bicleaner_ai-3.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:13:57.996266 bicleaner_ai-3.0.1/src/bicleaner_ai/
+-rwxr-xr-x   0 runner    (1001) docker     (127)      112 2024-04-16 15:13:53.000000 bicleaner_ai-3.0.1/src/bicleaner_ai/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4586 2024-04-16 15:13:53.000000 bicleaner_ai-3.0.1/src/bicleaner_ai/bicleaner_ai_classifier.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4458 2024-04-16 15:13:53.000000 bicleaner_ai-3.0.1/src/bicleaner_ai/bicleaner_ai_download.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)      642 2024-04-16 15:13:53.000000 bicleaner_ai-3.0.1/src/bicleaner_ai/bicleaner_ai_download_hf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2624 2024-04-16 15:13:53.000000 bicleaner_ai-3.0.1/src/bicleaner_ai/bicleaner_ai_generate_train.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)    13857 2024-04-16 15:13:53.000000 bicleaner_ai-3.0.1/src/bicleaner_ai/bicleaner_ai_train.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2964 2024-04-16 15:13:53.000000 bicleaner_ai-3.0.1/src/bicleaner_ai/calibrate.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15330 2024-04-16 15:13:53.000000 bicleaner_ai-3.0.1/src/bicleaner_ai/classify.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6479 2024-04-16 15:13:53.000000 bicleaner_ai-3.0.1/src/bicleaner_ai/datagen.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7456 2024-04-16 15:13:53.000000 bicleaner_ai-3.0.1/src/bicleaner_ai/decomposable_attention.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3927 2024-04-16 15:13:53.000000 bicleaner_ai-3.0.1/src/bicleaner_ai/layers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2283 2024-04-16 15:13:53.000000 bicleaner_ai-3.0.1/src/bicleaner_ai/losses.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6372 2024-04-16 15:13:53.000000 bicleaner_ai-3.0.1/src/bicleaner_ai/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25856 2024-04-16 15:13:53.000000 bicleaner_ai-3.0.1/src/bicleaner_ai/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4101 2024-04-16 15:13:53.000000 bicleaner_ai-3.0.1/src/bicleaner_ai/models_util.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12203 2024-04-16 15:13:53.000000 bicleaner_ai-3.0.1/src/bicleaner_ai/noise_generation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1214 2024-04-16 15:13:53.000000 bicleaner_ai-3.0.1/src/bicleaner_ai/tokenizer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4744 2024-04-16 15:13:53.000000 bicleaner_ai-3.0.1/src/bicleaner_ai/training.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     4249 2024-04-16 15:13:53.000000 bicleaner_ai-3.0.1/src/bicleaner_ai/util.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1351 2024-04-16 15:13:53.000000 bicleaner_ai-3.0.1/src/bicleaner_ai/word_freqs_list.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     3123 2024-04-16 15:13:53.000000 bicleaner_ai-3.0.1/src/bicleaner_ai/word_freqs_zipf.py
+-rwxr-xr-x   0 runner    (1001) docker     (127)     1082 2024-04-16 15:13:53.000000 bicleaner_ai-3.0.1/src/bicleaner_ai/word_freqs_zipf_double_linked.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:13:57.996266 bicleaner_ai-3.0.1/src/bicleaner_ai.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    57475 2024-04-16 15:13:57.000000 bicleaner_ai-3.0.1/src/bicleaner_ai.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1035 2024-04-16 15:13:57.000000 bicleaner_ai-3.0.1/src/bicleaner_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 15:13:57.000000 bicleaner_ai-3.0.1/src/bicleaner_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-16 15:13:57.000000 bicleaner_ai-3.0.1/src/bicleaner_ai.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      323 2024-04-16 15:13:57.000000 bicleaner_ai-3.0.1/src/bicleaner_ai.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-16 15:13:57.000000 bicleaner_ai-3.0.1/src/bicleaner_ai.egg-info/top_level.txt
```

### Comparing `bicleaner_ai-3.0.0/LICENSE` & `bicleaner_ai-3.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `bicleaner_ai-3.0.0/PKG-INFO` & `bicleaner_ai-3.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bicleaner-ai
-Version: 3.0.0
+Version: 3.0.1
 Summary: Parallel corpus classifier, indicating the likelihood of a pair of sentences being mutual translations or not (neural version)
 Author-email: Prompsit Language Engineering <info@prompsit.com>
 Maintainer-email: Jaume Zaragoza <jzaragoza@prompsit.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
@@ -694,15 +694,15 @@
 Requires-Dist: scikit-learn>=0.22.1
 Requires-Dist: PyYAML>=5.1.2
 Requires-Dist: numpy
 Requires-Dist: pytest
 Requires-Dist: toolwrapper
 Requires-Dist: joblib
 Requires-Dist: sacremoses
-Requires-Dist: bicleaner-hardrules==2.10.3
+Requires-Dist: bicleaner-hardrules==2.10.4
 Requires-Dist: sentencepiece
 Requires-Dist: protobuf==3.20.3
 Requires-Dist: tensorflow<2.16,>=2.6.5
 Requires-Dist: bicleaner-ai-glove==0.2.1
 Requires-Dist: fuzzywuzzy
 Requires-Dist: python-Levenshtein
 Requires-Dist: transformers==4.36.1
```

### Comparing `bicleaner_ai-3.0.0/README.md` & `bicleaner_ai-3.0.1/README.md`

 * *Files identical despite different names*

### Comparing `bicleaner_ai-3.0.0/pyproject.toml` & `bicleaner_ai-3.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "bicleaner-ai"
-version = "3.0.0"
+version = "3.0.1"
 license = {file = "LICENSE"}
 authors = [
     { "name" = "Prompsit Language Engineering", "email" = "info@prompsit.com" }
 ]
 maintainers = [
     { "name" = "Jaume Zaragoza", "email" = "jzaragoza@prompsit.com" }
 ]
@@ -15,15 +15,15 @@
     "scikit-learn>=0.22.1",
     "PyYAML>=5.1.2",
     "numpy",
     "pytest",
     "toolwrapper",
     "joblib",
     "sacremoses",
-    "bicleaner-hardrules==2.10.3",
+    "bicleaner-hardrules==2.10.4",
     "sentencepiece",
     "protobuf==3.20.3",
     "tensorflow>=2.6.5,<2.16",
     "bicleaner-ai-glove==0.2.1",
     "fuzzywuzzy",
     "python-Levenshtein",
     "transformers==4.36.1",
```

### Comparing `bicleaner_ai-3.0.0/src/bicleaner_ai/bicleaner_ai_classifier.py` & `bicleaner_ai-3.0.1/src/bicleaner_ai/bicleaner_ai_classifier.py`

 * *Files identical despite different names*

### Comparing `bicleaner_ai-3.0.0/src/bicleaner_ai/bicleaner_ai_download.py` & `bicleaner_ai-3.0.1/src/bicleaner_ai/bicleaner_ai_download.py`

 * *Files identical despite different names*

### Comparing `bicleaner_ai-3.0.0/src/bicleaner_ai/bicleaner_ai_download_hf.py` & `bicleaner_ai-3.0.1/src/bicleaner_ai/bicleaner_ai_download_hf.py`

 * *Files identical despite different names*

### Comparing `bicleaner_ai-3.0.0/src/bicleaner_ai/bicleaner_ai_generate_train.py` & `bicleaner_ai-3.0.1/src/bicleaner_ai/bicleaner_ai_generate_train.py`

 * *Files identical despite different names*

### Comparing `bicleaner_ai-3.0.0/src/bicleaner_ai/bicleaner_ai_train.py` & `bicleaner_ai-3.0.1/src/bicleaner_ai/bicleaner_ai_train.py`

 * *Files identical despite different names*

### Comparing `bicleaner_ai-3.0.0/src/bicleaner_ai/calibrate.py` & `bicleaner_ai-3.0.1/src/bicleaner_ai/calibrate.py`

 * *Files identical despite different names*

### Comparing `bicleaner_ai-3.0.0/src/bicleaner_ai/classify.py` & `bicleaner_ai-3.0.1/src/bicleaner_ai/classify.py`

 * *Files identical despite different names*

### Comparing `bicleaner_ai-3.0.0/src/bicleaner_ai/datagen.py` & `bicleaner_ai-3.0.1/src/bicleaner_ai/datagen.py`

 * *Files identical despite different names*

### Comparing `bicleaner_ai-3.0.0/src/bicleaner_ai/decomposable_attention.py` & `bicleaner_ai-3.0.1/src/bicleaner_ai/decomposable_attention.py`

 * *Files identical despite different names*

### Comparing `bicleaner_ai-3.0.0/src/bicleaner_ai/layers.py` & `bicleaner_ai-3.0.1/src/bicleaner_ai/layers.py`

 * *Files identical despite different names*

### Comparing `bicleaner_ai-3.0.0/src/bicleaner_ai/losses.py` & `bicleaner_ai-3.0.1/src/bicleaner_ai/losses.py`

 * *Files identical despite different names*

### Comparing `bicleaner_ai-3.0.0/src/bicleaner_ai/metrics.py` & `bicleaner_ai-3.0.1/src/bicleaner_ai/metrics.py`

 * *Files identical despite different names*

### Comparing `bicleaner_ai-3.0.0/src/bicleaner_ai/models.py` & `bicleaner_ai-3.0.1/src/bicleaner_ai/models.py`

 * *Files identical despite different names*

### Comparing `bicleaner_ai-3.0.0/src/bicleaner_ai/models_util.py` & `bicleaner_ai-3.0.1/src/bicleaner_ai/models_util.py`

 * *Files identical despite different names*

### Comparing `bicleaner_ai-3.0.0/src/bicleaner_ai/noise_generation.py` & `bicleaner_ai-3.0.1/src/bicleaner_ai/noise_generation.py`

 * *Files identical despite different names*

### Comparing `bicleaner_ai-3.0.0/src/bicleaner_ai/tokenizer.py` & `bicleaner_ai-3.0.1/src/bicleaner_ai/tokenizer.py`

 * *Files identical despite different names*

### Comparing `bicleaner_ai-3.0.0/src/bicleaner_ai/training.py` & `bicleaner_ai-3.0.1/src/bicleaner_ai/training.py`

 * *Files identical despite different names*

### Comparing `bicleaner_ai-3.0.0/src/bicleaner_ai/util.py` & `bicleaner_ai-3.0.1/src/bicleaner_ai/util.py`

 * *Files identical despite different names*

### Comparing `bicleaner_ai-3.0.0/src/bicleaner_ai/word_freqs_list.py` & `bicleaner_ai-3.0.1/src/bicleaner_ai/word_freqs_list.py`

 * *Files identical despite different names*

### Comparing `bicleaner_ai-3.0.0/src/bicleaner_ai/word_freqs_zipf.py` & `bicleaner_ai-3.0.1/src/bicleaner_ai/word_freqs_zipf.py`

 * *Files identical despite different names*

### Comparing `bicleaner_ai-3.0.0/src/bicleaner_ai/word_freqs_zipf_double_linked.py` & `bicleaner_ai-3.0.1/src/bicleaner_ai/word_freqs_zipf_double_linked.py`

 * *Files identical despite different names*

### Comparing `bicleaner_ai-3.0.0/src/bicleaner_ai.egg-info/PKG-INFO` & `bicleaner_ai-3.0.1/src/bicleaner_ai.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bicleaner-ai
-Version: 3.0.0
+Version: 3.0.1
 Summary: Parallel corpus classifier, indicating the likelihood of a pair of sentences being mutual translations or not (neural version)
 Author-email: Prompsit Language Engineering <info@prompsit.com>
 Maintainer-email: Jaume Zaragoza <jzaragoza@prompsit.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <http://fsf.org/>
@@ -694,15 +694,15 @@
 Requires-Dist: scikit-learn>=0.22.1
 Requires-Dist: PyYAML>=5.1.2
 Requires-Dist: numpy
 Requires-Dist: pytest
 Requires-Dist: toolwrapper
 Requires-Dist: joblib
 Requires-Dist: sacremoses
-Requires-Dist: bicleaner-hardrules==2.10.3
+Requires-Dist: bicleaner-hardrules==2.10.4
 Requires-Dist: sentencepiece
 Requires-Dist: protobuf==3.20.3
 Requires-Dist: tensorflow<2.16,>=2.6.5
 Requires-Dist: bicleaner-ai-glove==0.2.1
 Requires-Dist: fuzzywuzzy
 Requires-Dist: python-Levenshtein
 Requires-Dist: transformers==4.36.1
```

### Comparing `bicleaner_ai-3.0.0/src/bicleaner_ai.egg-info/SOURCES.txt` & `bicleaner_ai-3.0.1/src/bicleaner_ai.egg-info/SOURCES.txt`

 * *Files identical despite different names*

