# Comparing `tmp/openphrasebank-0.1.0.tar.gz` & `tmp/openphrasebank-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openphrasebank-0.1.0.tar", last modified: Mon Apr 15 21:46:42 2024, max compression
+gzip compressed data, was "openphrasebank-0.1.1.tar", last modified: Tue Apr 16 17:39:56 2024, max compression
```

## Comparing `openphrasebank-0.1.0.tar` & `openphrasebank-0.1.1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:46:42.086077 openphrasebank-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-15 21:46:36.000000 openphrasebank-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9459 2024-04-15 21:46:42.086077 openphrasebank-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8743 2024-04-15 21:46:36.000000 openphrasebank-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:46:42.082077 openphrasebank-0.1.0/openphrasebank/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:46:42.086077 openphrasebank-0.1.0/openphrasebank/openphrasebank.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9459 2024-04-15 21:46:42.000000 openphrasebank-0.1.0/openphrasebank/openphrasebank.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-15 21:46:42.000000 openphrasebank-0.1.0/openphrasebank/openphrasebank.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 21:46:42.000000 openphrasebank-0.1.0/openphrasebank/openphrasebank.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-15 21:46:42.000000 openphrasebank-0.1.0/openphrasebank/openphrasebank.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-15 21:46:42.000000 openphrasebank-0.1.0/openphrasebank/openphrasebank.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 21:46:42.000000 openphrasebank-0.1.0/openphrasebank/openphrasebank.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 21:46:42.086077 openphrasebank-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1315 2024-04-15 21:46:36.000000 openphrasebank-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 21:46:42.086077 openphrasebank-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-04-15 21:46:36.000000 openphrasebank-0.1.0/tests/test_core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:39:56.248480 openphrasebank-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-16 17:39:50.000000 openphrasebank-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    10443 2024-04-16 17:39:56.248480 openphrasebank-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     9781 2024-04-16 17:39:50.000000 openphrasebank-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:39:56.244480 openphrasebank-0.1.1/openphrasebank/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:39:56.248480 openphrasebank-0.1.1/openphrasebank/openphrasebank.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    10443 2024-04-16 17:39:56.000000 openphrasebank-0.1.1/openphrasebank/openphrasebank.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      365 2024-04-16 17:39:56.000000 openphrasebank-0.1.1/openphrasebank/openphrasebank.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 17:39:56.000000 openphrasebank-0.1.1/openphrasebank/openphrasebank.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-16 17:39:56.000000 openphrasebank-0.1.1/openphrasebank/openphrasebank.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-16 17:39:56.000000 openphrasebank-0.1.1/openphrasebank/openphrasebank.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 17:39:56.000000 openphrasebank-0.1.1/openphrasebank/openphrasebank.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 17:39:56.248480 openphrasebank-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1260 2024-04-16 17:39:50.000000 openphrasebank-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 17:39:56.244480 openphrasebank-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     2059 2024-04-16 17:39:50.000000 openphrasebank-0.1.1/tests/test_core.py
```

### Comparing `openphrasebank-0.1.0/LICENSE` & `openphrasebank-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `openphrasebank-0.1.0/PKG-INFO` & `openphrasebank-0.1.1/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: openphrasebank
-Version: 0.1.0
-Summary: PhraseBank is a utility designed to help users build customized phrasebanks from various texts or corpora.
-Home-page: https://github.com/liuh886/open_phrasebank
+Version: 0.1.1
+Summary: Customize phrasebanks from various texts or corpora.
+Home-page: https://github.com/liuh886/open-phrasebank
 Author: Zhihao
 Author-email: liuzhihao109@foxmial.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
@@ -16,74 +16,69 @@
 Requires-Dist: tqdm
 Requires-Dist: datasets
 Provides-Extra: spacy
 Requires-Dist: spacy>=3.0; extra == "spacy"
 Requires-Dist: en_core_web_sm; extra == "spacy"
 
 
-
 # Open Phrasebank
 
 <!-- start why-use-phrase-bank -->
 
-[![Documentation Status](https://readthedocs.org/projects/open-phrasebank/badge/?version=latest)](https://open-phrasebank.readthedocs.io/en/latest/?badge=latest)
-![PyPI - Version](https://img.shields.io/pypi/v/openphrasebank)
+Building your own phrasebank. ✨
 
+![Documentation Status](https://readthedocs.org/projects/open-phrasebank/badge/?version=latest) ![PyPI - Version](https://img.shields.io/pypi/v/openphrasebank) [![GitHub Action](https://github.com/liuh886/open-phrasebank/actions/workflows/lint.yml/badge.svg)](https://github.com/liuh886/open-phrasebank/actions/workflows/lint.yml) ![GitHub License](https://img.shields.io/github/license/liuh886/open-phrasebank) ![Docker Pulls](https://img.shields.io/docker/pulls/liuh886/open-phrasebank)
 
-Building your own phrasebank.
 
-This repository provides an accessible **phrase bank**, which is a collection of frequently used phrases that can be utilized, for example, in the auto-complete function of an IDE. (Note: This library does not provide IDE or auto-complete functions but offers a ready-to-use phrase bank)
+This repository provides an accessible **phrase bank**, which is a collection of frequently used phrases that can be utilized, for example, in the auto-complete function of an IDE. (Note: This library does not provide IDE or auto-complete functions but offers ready-to-use phrasebanks)
 
 Moreover, this repository includes features for constructing a phrase bank from a provided text or an open corpus.
 
 ## Why Use Phrase Bank
   
-### Case 1 - Typing in Flow
+### Boosting Typing Experience with Phrasebank 🚀
 
 ![](https://i.imgur.com/MGDIqly.gif)
 
-Boosting typing experience with phrasebank.🚀
-
 
-### Case 2 - Academic Writing
-
-  
+### Academic Writing 🕵️‍♀
 
 You can further customize the phrasebank according to your needs, e.g. for certain disciplines, for certain styles (descriptive, analytical, persuasive and critical), for certain sections (abstract, body text), as long as you can find good ingredients.
 
-
 <!-- end why-use-phrase-bank -->
 
 
 ## Open Phrasebanks
 <!-- start open-phrase-bank -->
 
 ### Academic Phrasebank
 
 Elsevier OA CC-BY contains 40k articles from Elsevier's journals, including from Arts, Business, STEM to Social Sciences[^1]. 
 
-| No. | Phrasebank                                                                                                                 | Source                                                                                                               | N-gram Length | Lines | Comments                                                                |
-| --- | -------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------- | ------------- | ----- | ----------------------------------------------------------------------- |
-| 1   | 📍[academic_phrasebank](https://github.com/liuh886/open_phrasebank/blob/main/phrasebanks/academic_phrasebank.txt)          | Book - [Academic Phrasebank](https://github.com/liuh886/open_phrasebank/blob/main/data/Academic_Phrasebank.pdf) 2014 | 2-5           | 2,190 | Extract from pdf (Zhihao, 2024)                                         |
-| 2   | 📍[elsevier_phrasebank](https://github.com/liuh886/open_phrasebank/blob/main/phrasebanks/elsevier_phrasebank.txt)          | Corpus - [Elsevier OA CC-BY](https://elsevier.digitalcommonsdata.com/datasets/zm33cdndxs/2) 2020                     | 2-6           | 3,792 | Extract by n-gram frequency (Zhihao, 2024)                              |
-| 3   | 📍[bawe_1000.csv](https://github.com/liuh886/open_phrasebank/blob/main/phrasebanks/bawe_ngrams.csv)                        | Corpus - [British Academic Written English](https://app.sketchengine.eu/#dashboard?corpname=preloaded%2Fbawe2) 2019  | 4-6           | 1,000 | Due to inaccessible, only most frequent  1000 list here. (Zhihao, 2024) |
-| 4   | 📍academic_word_list                                                                                                       | [Academic Word List Coxhead (2000)](https://www.uefap.com/vocab/select/awl.htm)                                      | 1             | 570   | The 570 word for academic English (exclude frequent 2000 words)         |
-| 5   | 📍[elsevier_awl](https://github.com/liuh886/open_phrasebank/blob/main/phrasebanks/elsevier_phrasebank.txt)                 | 2                                                                                                                    | 2-6           | 994   | The Elsevier phrasebank that contains  AWL (Zhihao, 2024)               |
-| 6   | 📍[elsevier_ENVI_EART](https://github.com/liuh886/open_phrasebank/blob/main/phrasebanks/elsevier_phrasebank_ENVI_EART.txt) | 2                                                                                                                    | 2-7           | 3,700 | Environment & Earth Science 3700 collection (Zhihao 2024)               |
-| 7   | 📍[elsevier_PSYC_SOCI](https://github.com/liuh886/open_phrasebank/blob/main/phrasebanks/elsevier_phrasebank_PSYC_SOCI.txt) | 2                                                                                                                    | 2-7           | 3,700 | Social Science & Psychology 3700 collection (Zhihao 2024)               |
-| 8   | 📍 [elsevier_MEDI](https://github.com/liuh886/open_phrasebank/blob/main/phrasebanks/elsevier_phrasebank_MEDI.txt)          | 2                                                                                                                    | 2-7           | 3,700 | Medicine 3700 collection (Zhihao 2024)                                  |
+| No. | Phrasebank                                                                                                                           | Source                                                                                                                                                                  | N of grams | Lines | Comments                                                                               |
+| --- | ------------------------------------------------------------------------------------------------------------------------------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------- | ----- | -------------------------------------------------------------------------------------- |
+| 1   | 📍[academic_phrasebank](https://raw.githubusercontent.com/liuh886/open-phrasebank/main/phrasebanks/academic_phrasebank.txt)          | Book [Academic Phrasebank](https://github.com/liuh886/open-phrasebank/blob/main/data/Academic_Phrasebank.pdf) 2014                                                      | 2-5           | 2,190 | Extract from pdf (Zhihao, 2024)                                                        |
+| 2   | 📍[elsevier_phrasebank](https://raw.githubusercontent.com/liuh886/open-phrasebank/main/phrasebanks/elsevier_phrasebank.txt)          | Corpus [Elsevier OA CC-BY](https://elsevier.digitalcommonsdata.com/datasets/zm33cdndxs/2) 2020                                                                          | 2-6           | 3,792 | Extract by n-gram (Zhihao 2024) |
+| 3   | 📍[bawe_1000.csv](https://raw.githubusercontent.com/liuh886/open-phrasebank/main/phrasebanks/bawe_ngrams.csv)                        | Corpus [British Academic Written English](https://www.coventry.ac.uk/research/research-directories/current-projects/2015/british-academic-written-english-corpus-bawe/) | 4-6           | 1,000 | Due to inaccessible, only most frequent  1000 list here. (Zhihao, 2024)                |
+| 4   | 📍academic_word_list                                                                                                                 | [Academic Word List Coxhead (2000)](https://www.uefap.com/vocab/select/awl.htm)                                                                                         | 1             | 570   | The 570 word for academic English (exclude frequent 2000 words)                        |
+| 5   | 📍[elsevier_awl](https://raw.githubusercontent.com/liuh886/open-phrasebank/main/phrasebanks/elsevier_phrasebank.txt)                 | 2,4                                                                                                                                                                     | 2-6           | 994   | The Elsevier phrasebank that contains  AWL (Zhihao, 2024)                              |
+| 6   | 📍[elsevier_ENVI_EART](https://raw.githubusercontent.com/liuh886/open-phrasebank/main/phrasebanks/elsevier_phrasebank_ENVI_EART.txt) | 2                                                                                                                                                                       | 2-7           | 3,700 | Environment & Earth Science 3700 collection (Zhihao 2024)                              |
+| 7   | 📍[elsevier_PSYC_SOCI](https://raw.githubusercontent.com/liuh886/open-phrasebank/main/phrasebanks/elsevier_phrasebank_PSYC_SOCI.txt) | 2                                                                                                                                                                       | 2-7           | 3,700 | Social Science & Psychology 3700 collection (Zhihao 2024)                              |
+| 8   | 📍[elsevier_MEDI](https://raw.githubusercontent.com/liuh886/open-phrasebank/main/phrasebanks/elsevier_phrasebank_MEDI.txt)           | 2                                                                                                                                                                       | 2-7           | 3,700 | Medicine 3700 collection (Zhihao 2024)                                                 |
 
-[^1]:Over 20 diciplines [orieg/elsevier-oa-cc-by · Datasets at Hugging Face](https://huggingface.co/datasets/orieg/elsevier-oa-cc-by)
+
+
+[^1]:Over 20 disciplines [orieg/elsevier-oa-cc-by · Datasets at Hugging Face](https://huggingface.co/datasets/orieg/elsevier-oa-cc-by)
 
 
 ### English Frequent Phrasebank
 
 | No. | Phrasebank                                                                                                                              | Source              | N-gram Length | Lines  | Comments                                                      |
 | --- | --------------------------------------------------------------------------------------------------------------------------------------- | ------------------- | ------------- | ------ | ------------------------------------------------------------- |
-| 1   | 📍[google-10000-english.txt](https://github.com/first20hours/google-10000-english/blob/master/google-10000-english.txt)                 | Google Books Corpus | 1             | 10,000 | The 10,000 most common English words from Google Books Corpus |
+| 1   | 📍[google-10000-english](https://raw.githubusercontent.com/first20hours/google-10000-english/master/google-10000-english-no-swears.txt)               | Google Books Corpus | 1             | 10,000 | The 10,000 most common English words from Google Books Corpus |
 | 2   | 📍[Wordlist 1200.txt](https://raw.githubusercontent.com/ManiacDC/TypingAid/master/Wordlists/Wordlist%201200%20frequency%20weighted.txt) | Internet            | 1             | 2,000  | The 2,000 most common English words                           |
 <!-- end open-phrase-bank -->
 
 
 ## Quickstart
 
 <!-- start quickstart -->
@@ -100,33 +95,33 @@
 <!-- start custom -->
 ## Get a Self-defined Phrasebank in 3 Steps
 
 ![](https://i.imgur.com/qssU2VP.png)
 
 Below is an example based on n-gram frequency. [More examples, e.g. extract from PDF, are available in documents](https://open-phrasebank.readthedocs.io/en/latest/quickstart/index.html).
 
-### Step 1 - Load and Tokenize the Data
+### 1️⃣ Load and Tokenize the Data
 ``` python
 import openphrasebank as opb
 
 tokens_gen = opb.load_and_tokenize_data (dataset_name="orieg/elsevier-oa-cc-by", 
                                          subject_areas=['PSYC','SOCI'],
                                          keys=['title', 'abstract','body_text'],
                                          save_cache=True,
                                          cache_file='temp_tokens.json')
 ```
 
-### Step 2 - Generate N-grams
+### 2️⃣ Generate N-grams
 
 ``` python
 n_values = [1,2,3,4,5,6,7,8]
 opb.generate_multiple_ngrams(tokens_gen, n_values)
 ```
 
-### Step 3 - Filter and save
+### 3️⃣ Filter and save
 
 ``` python
 # Define the top limits for each n-gram length
 top_limits = {1: 2000, 2: 2000, 3: 1000, 4: 300, 5: 200, 6: 200, 7: 200, 8: 200}
 
 # Filter the frequent n-grams and store the results in a dictionary
 phrases = {}
@@ -148,14 +143,15 @@
 ## How to Contribute
 
 You can either contribute the phrasebank or the code. Check out our [contributing](https://open-phrasebank.readthedocs.io/en/latest/contributing.html). 
 
 <!-- start issues -->
 ### Known Issues
 
-
-| Phrasebank          |                                                                                                                    |
+| Phrasebank          | Issues                                                                                                             |
 | ------------------- | ------------------------------------------------------------------------------------------------------------------ |
 | academic_phrasebank | Due to the table in the PDF file not being properly handled, many sentences were not extracted correctly. (zhihao) |
 | elsevier_phrasebank |                                                                                                                    |
 
 <!-- end issues -->
+
+[![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/F1F7WYJ6B)
```

### Comparing `openphrasebank-0.1.0/README.md` & `openphrasebank-0.1.1/openphrasebank/openphrasebank.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,68 +1,84 @@
+Metadata-Version: 2.1
+Name: openphrasebank
+Version: 0.1.1
+Summary: Customize phrasebanks from various texts or corpora.
+Home-page: https://github.com/liuh886/open-phrasebank
+Author: Zhihao
+Author-email: liuzhihao109@foxmial.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.8
+Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: nltk
+Requires-Dist: pymupdf
+Requires-Dist: tqdm
+Requires-Dist: datasets
+Provides-Extra: spacy
+Requires-Dist: spacy>=3.0; extra == "spacy"
+Requires-Dist: en_core_web_sm; extra == "spacy"
 
 
 # Open Phrasebank
 
 <!-- start why-use-phrase-bank -->
 
-[![Documentation Status](https://readthedocs.org/projects/open-phrasebank/badge/?version=latest)](https://open-phrasebank.readthedocs.io/en/latest/?badge=latest)
-![PyPI - Version](https://img.shields.io/pypi/v/openphrasebank)
+Building your own phrasebank. ✨
 
+![Documentation Status](https://readthedocs.org/projects/open-phrasebank/badge/?version=latest) ![PyPI - Version](https://img.shields.io/pypi/v/openphrasebank) [![GitHub Action](https://github.com/liuh886/open-phrasebank/actions/workflows/lint.yml/badge.svg)](https://github.com/liuh886/open-phrasebank/actions/workflows/lint.yml) ![GitHub License](https://img.shields.io/github/license/liuh886/open-phrasebank) ![Docker Pulls](https://img.shields.io/docker/pulls/liuh886/open-phrasebank)
 
-Building your own phrasebank.
 
-This repository provides an accessible **phrase bank**, which is a collection of frequently used phrases that can be utilized, for example, in the auto-complete function of an IDE. (Note: This library does not provide IDE or auto-complete functions but offers a ready-to-use phrase bank)
+This repository provides an accessible **phrase bank**, which is a collection of frequently used phrases that can be utilized, for example, in the auto-complete function of an IDE. (Note: This library does not provide IDE or auto-complete functions but offers ready-to-use phrasebanks)
 
 Moreover, this repository includes features for constructing a phrase bank from a provided text or an open corpus.
 
 ## Why Use Phrase Bank
   
-### Case 1 - Typing in Flow
+### Boosting Typing Experience with Phrasebank 🚀
 
 ![](https://i.imgur.com/MGDIqly.gif)
 
-Boosting typing experience with phrasebank.🚀
 
-
-### Case 2 - Academic Writing
-
-  
+### Academic Writing 🕵️‍♀
 
 You can further customize the phrasebank according to your needs, e.g. for certain disciplines, for certain styles (descriptive, analytical, persuasive and critical), for certain sections (abstract, body text), as long as you can find good ingredients.
 
-
 <!-- end why-use-phrase-bank -->
 
 
 ## Open Phrasebanks
 <!-- start open-phrase-bank -->
 
 ### Academic Phrasebank
 
 Elsevier OA CC-BY contains 40k articles from Elsevier's journals, including from Arts, Business, STEM to Social Sciences[^1]. 
 
-| No. | Phrasebank                                                                                                                 | Source                                                                                                               | N-gram Length | Lines | Comments                                                                |
-| --- | -------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------- | ------------- | ----- | ----------------------------------------------------------------------- |
-| 1   | 📍[academic_phrasebank](https://github.com/liuh886/open_phrasebank/blob/main/phrasebanks/academic_phrasebank.txt)          | Book - [Academic Phrasebank](https://github.com/liuh886/open_phrasebank/blob/main/data/Academic_Phrasebank.pdf) 2014 | 2-5           | 2,190 | Extract from pdf (Zhihao, 2024)                                         |
-| 2   | 📍[elsevier_phrasebank](https://github.com/liuh886/open_phrasebank/blob/main/phrasebanks/elsevier_phrasebank.txt)          | Corpus - [Elsevier OA CC-BY](https://elsevier.digitalcommonsdata.com/datasets/zm33cdndxs/2) 2020                     | 2-6           | 3,792 | Extract by n-gram frequency (Zhihao, 2024)                              |
-| 3   | 📍[bawe_1000.csv](https://github.com/liuh886/open_phrasebank/blob/main/phrasebanks/bawe_ngrams.csv)                        | Corpus - [British Academic Written English](https://app.sketchengine.eu/#dashboard?corpname=preloaded%2Fbawe2) 2019  | 4-6           | 1,000 | Due to inaccessible, only most frequent  1000 list here. (Zhihao, 2024) |
-| 4   | 📍academic_word_list                                                                                                       | [Academic Word List Coxhead (2000)](https://www.uefap.com/vocab/select/awl.htm)                                      | 1             | 570   | The 570 word for academic English (exclude frequent 2000 words)         |
-| 5   | 📍[elsevier_awl](https://github.com/liuh886/open_phrasebank/blob/main/phrasebanks/elsevier_phrasebank.txt)                 | 2                                                                                                                    | 2-6           | 994   | The Elsevier phrasebank that contains  AWL (Zhihao, 2024)               |
-| 6   | 📍[elsevier_ENVI_EART](https://github.com/liuh886/open_phrasebank/blob/main/phrasebanks/elsevier_phrasebank_ENVI_EART.txt) | 2                                                                                                                    | 2-7           | 3,700 | Environment & Earth Science 3700 collection (Zhihao 2024)               |
-| 7   | 📍[elsevier_PSYC_SOCI](https://github.com/liuh886/open_phrasebank/blob/main/phrasebanks/elsevier_phrasebank_PSYC_SOCI.txt) | 2                                                                                                                    | 2-7           | 3,700 | Social Science & Psychology 3700 collection (Zhihao 2024)               |
-| 8   | 📍 [elsevier_MEDI](https://github.com/liuh886/open_phrasebank/blob/main/phrasebanks/elsevier_phrasebank_MEDI.txt)          | 2                                                                                                                    | 2-7           | 3,700 | Medicine 3700 collection (Zhihao 2024)                                  |
+| No. | Phrasebank                                                                                                                           | Source                                                                                                                                                                  | N of grams | Lines | Comments                                                                               |
+| --- | ------------------------------------------------------------------------------------------------------------------------------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------- | ----- | -------------------------------------------------------------------------------------- |
+| 1   | 📍[academic_phrasebank](https://raw.githubusercontent.com/liuh886/open-phrasebank/main/phrasebanks/academic_phrasebank.txt)          | Book [Academic Phrasebank](https://github.com/liuh886/open-phrasebank/blob/main/data/Academic_Phrasebank.pdf) 2014                                                      | 2-5           | 2,190 | Extract from pdf (Zhihao, 2024)                                                        |
+| 2   | 📍[elsevier_phrasebank](https://raw.githubusercontent.com/liuh886/open-phrasebank/main/phrasebanks/elsevier_phrasebank.txt)          | Corpus [Elsevier OA CC-BY](https://elsevier.digitalcommonsdata.com/datasets/zm33cdndxs/2) 2020                                                                          | 2-6           | 3,792 | Extract by n-gram (Zhihao 2024) |
+| 3   | 📍[bawe_1000.csv](https://raw.githubusercontent.com/liuh886/open-phrasebank/main/phrasebanks/bawe_ngrams.csv)                        | Corpus [British Academic Written English](https://www.coventry.ac.uk/research/research-directories/current-projects/2015/british-academic-written-english-corpus-bawe/) | 4-6           | 1,000 | Due to inaccessible, only most frequent  1000 list here. (Zhihao, 2024)                |
+| 4   | 📍academic_word_list                                                                                                                 | [Academic Word List Coxhead (2000)](https://www.uefap.com/vocab/select/awl.htm)                                                                                         | 1             | 570   | The 570 word for academic English (exclude frequent 2000 words)                        |
+| 5   | 📍[elsevier_awl](https://raw.githubusercontent.com/liuh886/open-phrasebank/main/phrasebanks/elsevier_phrasebank.txt)                 | 2,4                                                                                                                                                                     | 2-6           | 994   | The Elsevier phrasebank that contains  AWL (Zhihao, 2024)                              |
+| 6   | 📍[elsevier_ENVI_EART](https://raw.githubusercontent.com/liuh886/open-phrasebank/main/phrasebanks/elsevier_phrasebank_ENVI_EART.txt) | 2                                                                                                                                                                       | 2-7           | 3,700 | Environment & Earth Science 3700 collection (Zhihao 2024)                              |
+| 7   | 📍[elsevier_PSYC_SOCI](https://raw.githubusercontent.com/liuh886/open-phrasebank/main/phrasebanks/elsevier_phrasebank_PSYC_SOCI.txt) | 2                                                                                                                                                                       | 2-7           | 3,700 | Social Science & Psychology 3700 collection (Zhihao 2024)                              |
+| 8   | 📍[elsevier_MEDI](https://raw.githubusercontent.com/liuh886/open-phrasebank/main/phrasebanks/elsevier_phrasebank_MEDI.txt)           | 2                                                                                                                                                                       | 2-7           | 3,700 | Medicine 3700 collection (Zhihao 2024)                                                 |
 
-[^1]:Over 20 diciplines [orieg/elsevier-oa-cc-by · Datasets at Hugging Face](https://huggingface.co/datasets/orieg/elsevier-oa-cc-by)
+
+
+[^1]:Over 20 disciplines [orieg/elsevier-oa-cc-by · Datasets at Hugging Face](https://huggingface.co/datasets/orieg/elsevier-oa-cc-by)
 
 
 ### English Frequent Phrasebank
 
 | No. | Phrasebank                                                                                                                              | Source              | N-gram Length | Lines  | Comments                                                      |
 | --- | --------------------------------------------------------------------------------------------------------------------------------------- | ------------------- | ------------- | ------ | ------------------------------------------------------------- |
-| 1   | 📍[google-10000-english.txt](https://github.com/first20hours/google-10000-english/blob/master/google-10000-english.txt)                 | Google Books Corpus | 1             | 10,000 | The 10,000 most common English words from Google Books Corpus |
+| 1   | 📍[google-10000-english](https://raw.githubusercontent.com/first20hours/google-10000-english/master/google-10000-english-no-swears.txt)               | Google Books Corpus | 1             | 10,000 | The 10,000 most common English words from Google Books Corpus |
 | 2   | 📍[Wordlist 1200.txt](https://raw.githubusercontent.com/ManiacDC/TypingAid/master/Wordlists/Wordlist%201200%20frequency%20weighted.txt) | Internet            | 1             | 2,000  | The 2,000 most common English words                           |
 <!-- end open-phrase-bank -->
 
 
 ## Quickstart
 
 <!-- start quickstart -->
@@ -79,33 +95,33 @@
 <!-- start custom -->
 ## Get a Self-defined Phrasebank in 3 Steps
 
 ![](https://i.imgur.com/qssU2VP.png)
 
 Below is an example based on n-gram frequency. [More examples, e.g. extract from PDF, are available in documents](https://open-phrasebank.readthedocs.io/en/latest/quickstart/index.html).
 
-### Step 1 - Load and Tokenize the Data
+### 1️⃣ Load and Tokenize the Data
 ``` python
 import openphrasebank as opb
 
 tokens_gen = opb.load_and_tokenize_data (dataset_name="orieg/elsevier-oa-cc-by", 
                                          subject_areas=['PSYC','SOCI'],
                                          keys=['title', 'abstract','body_text'],
                                          save_cache=True,
                                          cache_file='temp_tokens.json')
 ```
 
-### Step 2 - Generate N-grams
+### 2️⃣ Generate N-grams
 
 ``` python
 n_values = [1,2,3,4,5,6,7,8]
 opb.generate_multiple_ngrams(tokens_gen, n_values)
 ```
 
-### Step 3 - Filter and save
+### 3️⃣ Filter and save
 
 ``` python
 # Define the top limits for each n-gram length
 top_limits = {1: 2000, 2: 2000, 3: 1000, 4: 300, 5: 200, 6: 200, 7: 200, 8: 200}
 
 # Filter the frequent n-grams and store the results in a dictionary
 phrases = {}
@@ -127,14 +143,15 @@
 ## How to Contribute
 
 You can either contribute the phrasebank or the code. Check out our [contributing](https://open-phrasebank.readthedocs.io/en/latest/contributing.html). 
 
 <!-- start issues -->
 ### Known Issues
 
-
-| Phrasebank          |                                                                                                                    |
+| Phrasebank          | Issues                                                                                                             |
 | ------------------- | ------------------------------------------------------------------------------------------------------------------ |
 | academic_phrasebank | Due to the table in the PDF file not being properly handled, many sentences were not extracted correctly. (zhihao) |
 | elsevier_phrasebank |                                                                                                                    |
 
-<!-- end issues -->
+<!-- end issues -->
+
+[![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/F1F7WYJ6B)
```

### Comparing `openphrasebank-0.1.0/openphrasebank/openphrasebank.egg-info/PKG-INFO` & `openphrasebank-0.1.1/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,89 +1,63 @@
-Metadata-Version: 2.1
-Name: openphrasebank
-Version: 0.1.0
-Summary: PhraseBank is a utility designed to help users build customized phrasebanks from various texts or corpora.
-Home-page: https://github.com/liuh886/open_phrasebank
-Author: Zhihao
-Author-email: liuzhihao109@foxmial.com
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.8
-Description-Content-Type: text/markdown
-License-File: LICENSE
-Requires-Dist: nltk
-Requires-Dist: pymupdf
-Requires-Dist: tqdm
-Requires-Dist: datasets
-Provides-Extra: spacy
-Requires-Dist: spacy>=3.0; extra == "spacy"
-Requires-Dist: en_core_web_sm; extra == "spacy"
-
-
 
 # Open Phrasebank
 
 <!-- start why-use-phrase-bank -->
 
-[![Documentation Status](https://readthedocs.org/projects/open-phrasebank/badge/?version=latest)](https://open-phrasebank.readthedocs.io/en/latest/?badge=latest)
-![PyPI - Version](https://img.shields.io/pypi/v/openphrasebank)
+Building your own phrasebank. ✨
 
+![Documentation Status](https://readthedocs.org/projects/open-phrasebank/badge/?version=latest) ![PyPI - Version](https://img.shields.io/pypi/v/openphrasebank) [![GitHub Action](https://github.com/liuh886/open-phrasebank/actions/workflows/lint.yml/badge.svg)](https://github.com/liuh886/open-phrasebank/actions/workflows/lint.yml) ![GitHub License](https://img.shields.io/github/license/liuh886/open-phrasebank) ![Docker Pulls](https://img.shields.io/docker/pulls/liuh886/open-phrasebank)
 
-Building your own phrasebank.
 
-This repository provides an accessible **phrase bank**, which is a collection of frequently used phrases that can be utilized, for example, in the auto-complete function of an IDE. (Note: This library does not provide IDE or auto-complete functions but offers a ready-to-use phrase bank)
+This repository provides an accessible **phrase bank**, which is a collection of frequently used phrases that can be utilized, for example, in the auto-complete function of an IDE. (Note: This library does not provide IDE or auto-complete functions but offers ready-to-use phrasebanks)
 
 Moreover, this repository includes features for constructing a phrase bank from a provided text or an open corpus.
 
 ## Why Use Phrase Bank
   
-### Case 1 - Typing in Flow
+### Boosting Typing Experience with Phrasebank 🚀
 
 ![](https://i.imgur.com/MGDIqly.gif)
 
-Boosting typing experience with phrasebank.🚀
-
 
-### Case 2 - Academic Writing
-
-  
+### Academic Writing 🕵️‍♀
 
 You can further customize the phrasebank according to your needs, e.g. for certain disciplines, for certain styles (descriptive, analytical, persuasive and critical), for certain sections (abstract, body text), as long as you can find good ingredients.
 
-
 <!-- end why-use-phrase-bank -->
 
 
 ## Open Phrasebanks
 <!-- start open-phrase-bank -->
 
 ### Academic Phrasebank
 
 Elsevier OA CC-BY contains 40k articles from Elsevier's journals, including from Arts, Business, STEM to Social Sciences[^1]. 
 
-| No. | Phrasebank                                                                                                                 | Source                                                                                                               | N-gram Length | Lines | Comments                                                                |
-| --- | -------------------------------------------------------------------------------------------------------------------------- | -------------------------------------------------------------------------------------------------------------------- | ------------- | ----- | ----------------------------------------------------------------------- |
-| 1   | 📍[academic_phrasebank](https://github.com/liuh886/open_phrasebank/blob/main/phrasebanks/academic_phrasebank.txt)          | Book - [Academic Phrasebank](https://github.com/liuh886/open_phrasebank/blob/main/data/Academic_Phrasebank.pdf) 2014 | 2-5           | 2,190 | Extract from pdf (Zhihao, 2024)                                         |
-| 2   | 📍[elsevier_phrasebank](https://github.com/liuh886/open_phrasebank/blob/main/phrasebanks/elsevier_phrasebank.txt)          | Corpus - [Elsevier OA CC-BY](https://elsevier.digitalcommonsdata.com/datasets/zm33cdndxs/2) 2020                     | 2-6           | 3,792 | Extract by n-gram frequency (Zhihao, 2024)                              |
-| 3   | 📍[bawe_1000.csv](https://github.com/liuh886/open_phrasebank/blob/main/phrasebanks/bawe_ngrams.csv)                        | Corpus - [British Academic Written English](https://app.sketchengine.eu/#dashboard?corpname=preloaded%2Fbawe2) 2019  | 4-6           | 1,000 | Due to inaccessible, only most frequent  1000 list here. (Zhihao, 2024) |
-| 4   | 📍academic_word_list                                                                                                       | [Academic Word List Coxhead (2000)](https://www.uefap.com/vocab/select/awl.htm)                                      | 1             | 570   | The 570 word for academic English (exclude frequent 2000 words)         |
-| 5   | 📍[elsevier_awl](https://github.com/liuh886/open_phrasebank/blob/main/phrasebanks/elsevier_phrasebank.txt)                 | 2                                                                                                                    | 2-6           | 994   | The Elsevier phrasebank that contains  AWL (Zhihao, 2024)               |
-| 6   | 📍[elsevier_ENVI_EART](https://github.com/liuh886/open_phrasebank/blob/main/phrasebanks/elsevier_phrasebank_ENVI_EART.txt) | 2                                                                                                                    | 2-7           | 3,700 | Environment & Earth Science 3700 collection (Zhihao 2024)               |
-| 7   | 📍[elsevier_PSYC_SOCI](https://github.com/liuh886/open_phrasebank/blob/main/phrasebanks/elsevier_phrasebank_PSYC_SOCI.txt) | 2                                                                                                                    | 2-7           | 3,700 | Social Science & Psychology 3700 collection (Zhihao 2024)               |
-| 8   | 📍 [elsevier_MEDI](https://github.com/liuh886/open_phrasebank/blob/main/phrasebanks/elsevier_phrasebank_MEDI.txt)          | 2                                                                                                                    | 2-7           | 3,700 | Medicine 3700 collection (Zhihao 2024)                                  |
+| No. | Phrasebank                                                                                                                           | Source                                                                                                                                                                  | N of grams | Lines | Comments                                                                               |
+| --- | ------------------------------------------------------------------------------------------------------------------------------------ | ----------------------------------------------------------------------------------------------------------------------------------------------------------------------- | ------------- | ----- | -------------------------------------------------------------------------------------- |
+| 1   | 📍[academic_phrasebank](https://raw.githubusercontent.com/liuh886/open-phrasebank/main/phrasebanks/academic_phrasebank.txt)          | Book [Academic Phrasebank](https://github.com/liuh886/open-phrasebank/blob/main/data/Academic_Phrasebank.pdf) 2014                                                      | 2-5           | 2,190 | Extract from pdf (Zhihao, 2024)                                                        |
+| 2   | 📍[elsevier_phrasebank](https://raw.githubusercontent.com/liuh886/open-phrasebank/main/phrasebanks/elsevier_phrasebank.txt)          | Corpus [Elsevier OA CC-BY](https://elsevier.digitalcommonsdata.com/datasets/zm33cdndxs/2) 2020                                                                          | 2-6           | 3,792 | Extract by n-gram (Zhihao 2024) |
+| 3   | 📍[bawe_1000.csv](https://raw.githubusercontent.com/liuh886/open-phrasebank/main/phrasebanks/bawe_ngrams.csv)                        | Corpus [British Academic Written English](https://www.coventry.ac.uk/research/research-directories/current-projects/2015/british-academic-written-english-corpus-bawe/) | 4-6           | 1,000 | Due to inaccessible, only most frequent  1000 list here. (Zhihao, 2024)                |
+| 4   | 📍academic_word_list                                                                                                                 | [Academic Word List Coxhead (2000)](https://www.uefap.com/vocab/select/awl.htm)                                                                                         | 1             | 570   | The 570 word for academic English (exclude frequent 2000 words)                        |
+| 5   | 📍[elsevier_awl](https://raw.githubusercontent.com/liuh886/open-phrasebank/main/phrasebanks/elsevier_phrasebank.txt)                 | 2,4                                                                                                                                                                     | 2-6           | 994   | The Elsevier phrasebank that contains  AWL (Zhihao, 2024)                              |
+| 6   | 📍[elsevier_ENVI_EART](https://raw.githubusercontent.com/liuh886/open-phrasebank/main/phrasebanks/elsevier_phrasebank_ENVI_EART.txt) | 2                                                                                                                                                                       | 2-7           | 3,700 | Environment & Earth Science 3700 collection (Zhihao 2024)                              |
+| 7   | 📍[elsevier_PSYC_SOCI](https://raw.githubusercontent.com/liuh886/open-phrasebank/main/phrasebanks/elsevier_phrasebank_PSYC_SOCI.txt) | 2                                                                                                                                                                       | 2-7           | 3,700 | Social Science & Psychology 3700 collection (Zhihao 2024)                              |
+| 8   | 📍[elsevier_MEDI](https://raw.githubusercontent.com/liuh886/open-phrasebank/main/phrasebanks/elsevier_phrasebank_MEDI.txt)           | 2                                                                                                                                                                       | 2-7           | 3,700 | Medicine 3700 collection (Zhihao 2024)                                                 |
+
+
 
-[^1]:Over 20 diciplines [orieg/elsevier-oa-cc-by · Datasets at Hugging Face](https://huggingface.co/datasets/orieg/elsevier-oa-cc-by)
+[^1]:Over 20 disciplines [orieg/elsevier-oa-cc-by · Datasets at Hugging Face](https://huggingface.co/datasets/orieg/elsevier-oa-cc-by)
 
 
 ### English Frequent Phrasebank
 
 | No. | Phrasebank                                                                                                                              | Source              | N-gram Length | Lines  | Comments                                                      |
 | --- | --------------------------------------------------------------------------------------------------------------------------------------- | ------------------- | ------------- | ------ | ------------------------------------------------------------- |
-| 1   | 📍[google-10000-english.txt](https://github.com/first20hours/google-10000-english/blob/master/google-10000-english.txt)                 | Google Books Corpus | 1             | 10,000 | The 10,000 most common English words from Google Books Corpus |
+| 1   | 📍[google-10000-english](https://raw.githubusercontent.com/first20hours/google-10000-english/master/google-10000-english-no-swears.txt)               | Google Books Corpus | 1             | 10,000 | The 10,000 most common English words from Google Books Corpus |
 | 2   | 📍[Wordlist 1200.txt](https://raw.githubusercontent.com/ManiacDC/TypingAid/master/Wordlists/Wordlist%201200%20frequency%20weighted.txt) | Internet            | 1             | 2,000  | The 2,000 most common English words                           |
 <!-- end open-phrase-bank -->
 
 
 ## Quickstart
 
 <!-- start quickstart -->
@@ -100,33 +74,33 @@
 <!-- start custom -->
 ## Get a Self-defined Phrasebank in 3 Steps
 
 ![](https://i.imgur.com/qssU2VP.png)
 
 Below is an example based on n-gram frequency. [More examples, e.g. extract from PDF, are available in documents](https://open-phrasebank.readthedocs.io/en/latest/quickstart/index.html).
 
-### Step 1 - Load and Tokenize the Data
+### 1️⃣ Load and Tokenize the Data
 ``` python
 import openphrasebank as opb
 
 tokens_gen = opb.load_and_tokenize_data (dataset_name="orieg/elsevier-oa-cc-by", 
                                          subject_areas=['PSYC','SOCI'],
                                          keys=['title', 'abstract','body_text'],
                                          save_cache=True,
                                          cache_file='temp_tokens.json')
 ```
 
-### Step 2 - Generate N-grams
+### 2️⃣ Generate N-grams
 
 ``` python
 n_values = [1,2,3,4,5,6,7,8]
 opb.generate_multiple_ngrams(tokens_gen, n_values)
 ```
 
-### Step 3 - Filter and save
+### 3️⃣ Filter and save
 
 ``` python
 # Define the top limits for each n-gram length
 top_limits = {1: 2000, 2: 2000, 3: 1000, 4: 300, 5: 200, 6: 200, 7: 200, 8: 200}
 
 # Filter the frequent n-grams and store the results in a dictionary
 phrases = {}
@@ -148,14 +122,15 @@
 ## How to Contribute
 
 You can either contribute the phrasebank or the code. Check out our [contributing](https://open-phrasebank.readthedocs.io/en/latest/contributing.html). 
 
 <!-- start issues -->
 ### Known Issues
 
-
-| Phrasebank          |                                                                                                                    |
+| Phrasebank          | Issues                                                                                                             |
 | ------------------- | ------------------------------------------------------------------------------------------------------------------ |
 | academic_phrasebank | Due to the table in the PDF file not being properly handled, many sentences were not extracted correctly. (zhihao) |
 | elsevier_phrasebank |                                                                                                                    |
 
 <!-- end issues -->
+
+[![ko-fi](https://ko-fi.com/img/githubbutton_sm.svg)](https://ko-fi.com/F1F7WYJ6B)
```

### Comparing `openphrasebank-0.1.0/setup.py` & `openphrasebank-0.1.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,18 +1,18 @@
-from setuptools import setup, find_packages 
+from setuptools import setup, find_packages
 
 setup(
     name="openphrasebank",
-    version="0.1.0",
+    version="0.1.1",
     author="Zhihao",
     author_email="liuzhihao109@foxmial.com",
-    description="PhraseBank is a utility designed to help users build customized phrasebanks from various texts or corpora.",
+    description="Customize phrasebanks from various texts or corpora.",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
-    url="https://github.com/liuh886/open_phrasebank",
+    url="https://github.com/liuh886/open-phrasebank",
     install_requires=[
         'nltk', 
         'pymupdf',
         'tqdm',  
         'datasets', # Huggingface datasets
     ],
     extras_require={
```

### Comparing `openphrasebank-0.1.0/tests/test_core.py` & `openphrasebank-0.1.1/tests/test_core.py`

 * *Files identical despite different names*

