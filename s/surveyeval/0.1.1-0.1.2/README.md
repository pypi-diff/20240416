# Comparing `tmp/surveyeval-0.1.1.tar.gz` & `tmp/surveyeval-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "surveyeval-0.1.1.tar", last modified: Sun Apr 14 17:29:13 2024, max compression
+gzip compressed data, was "surveyeval-0.1.2.tar", last modified: Tue Apr 16 20:26:36 2024, max compression
```

## Comparing `surveyeval-0.1.1.tar` & `surveyeval-0.1.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 crobert    (501) staff       (20)        0 2024-04-14 17:29:13.907072 surveyeval-0.1.1/
--rw-r--r--   0 crobert    (501) staff       (20)    11357 2023-11-29 20:42:10.000000 surveyeval-0.1.1/LICENSE
--rw-r--r--   0 crobert    (501) staff       (20)    11787 2024-04-14 17:29:13.906796 surveyeval-0.1.1/PKG-INFO
--rw-r--r--   0 crobert    (501) staff       (20)    10430 2024-04-14 15:10:57.000000 surveyeval-0.1.1/README.rst
--rw-r--r--   0 crobert    (501) staff       (20)       38 2024-04-14 17:29:13.907132 surveyeval-0.1.1/setup.cfg
--rw-r--r--   0 crobert    (501) staff       (20)     2044 2024-04-14 15:16:06.000000 surveyeval-0.1.1/setup.py
-drwxr-xr-x   0 crobert    (501) staff       (20)        0 2024-04-14 17:29:13.901405 surveyeval-0.1.1/src/
-drwxr-xr-x   0 crobert    (501) staff       (20)        0 2024-04-14 17:29:13.904550 surveyeval-0.1.1/src/surveyeval/
--rw-r--r--   0 crobert    (501) staff       (20)     1058 2024-04-14 15:10:57.000000 surveyeval-0.1.1/src/surveyeval/__init__.py
--rw-r--r--   0 crobert    (501) staff       (20)    49441 2024-04-14 15:33:38.000000 surveyeval-0.1.1/src/surveyeval/core_evaluation_lenses.py
--rw-r--r--   0 crobert    (501) staff       (20)    33231 2024-04-14 16:03:22.000000 surveyeval-0.1.1/src/surveyeval/evaluation_engine.py
--rw-r--r--   0 crobert    (501) staff       (20)    56480 2024-04-14 15:27:21.000000 surveyeval-0.1.1/src/surveyeval/survey_parser.py
-drwxr-xr-x   0 crobert    (501) staff       (20)        0 2024-04-14 17:29:13.906387 surveyeval-0.1.1/src/surveyeval.egg-info/
--rw-r--r--   0 crobert    (501) staff       (20)    11787 2024-04-14 17:29:13.000000 surveyeval-0.1.1/src/surveyeval.egg-info/PKG-INFO
--rw-r--r--   0 crobert    (501) staff       (20)      352 2024-04-14 17:29:13.000000 surveyeval-0.1.1/src/surveyeval.egg-info/SOURCES.txt
--rw-r--r--   0 crobert    (501) staff       (20)        1 2024-04-14 17:29:13.000000 surveyeval-0.1.1/src/surveyeval.egg-info/dependency_links.txt
--rw-r--r--   0 crobert    (501) staff       (20)      505 2024-04-14 17:29:13.000000 surveyeval-0.1.1/src/surveyeval.egg-info/requires.txt
--rw-r--r--   0 crobert    (501) staff       (20)       11 2024-04-14 17:29:13.000000 surveyeval-0.1.1/src/surveyeval.egg-info/top_level.txt
+drwxr-xr-x   0 crobert    (501) staff       (20)        0 2024-04-16 20:26:36.824059 surveyeval-0.1.2/
+-rw-r--r--   0 crobert    (501) staff       (20)    11357 2023-11-29 20:42:10.000000 surveyeval-0.1.2/LICENSE
+-rw-r--r--   0 crobert    (501) staff       (20)    11786 2024-04-16 20:26:36.823788 surveyeval-0.1.2/PKG-INFO
+-rw-r--r--   0 crobert    (501) staff       (20)    10430 2024-04-14 15:10:57.000000 surveyeval-0.1.2/README.rst
+-rw-r--r--   0 crobert    (501) staff       (20)       38 2024-04-16 20:26:36.824112 surveyeval-0.1.2/setup.cfg
+-rw-r--r--   0 crobert    (501) staff       (20)     2043 2024-04-16 20:26:26.000000 surveyeval-0.1.2/setup.py
+drwxr-xr-x   0 crobert    (501) staff       (20)        0 2024-04-16 20:26:36.817239 surveyeval-0.1.2/src/
+drwxr-xr-x   0 crobert    (501) staff       (20)        0 2024-04-16 20:26:36.820910 surveyeval-0.1.2/src/surveyeval/
+-rw-r--r--   0 crobert    (501) staff       (20)     1058 2024-04-14 15:10:57.000000 surveyeval-0.1.2/src/surveyeval/__init__.py
+-rw-r--r--   0 crobert    (501) staff       (20)    49441 2024-04-14 15:33:38.000000 surveyeval-0.1.2/src/surveyeval/core_evaluation_lenses.py
+-rw-r--r--   0 crobert    (501) staff       (20)    33231 2024-04-14 16:03:22.000000 surveyeval-0.1.2/src/surveyeval/evaluation_engine.py
+-rw-r--r--   0 crobert    (501) staff       (20)    56480 2024-04-14 15:27:21.000000 surveyeval-0.1.2/src/surveyeval/survey_parser.py
+drwxr-xr-x   0 crobert    (501) staff       (20)        0 2024-04-16 20:26:36.823313 surveyeval-0.1.2/src/surveyeval.egg-info/
+-rw-r--r--   0 crobert    (501) staff       (20)    11786 2024-04-16 20:26:36.000000 surveyeval-0.1.2/src/surveyeval.egg-info/PKG-INFO
+-rw-r--r--   0 crobert    (501) staff       (20)      352 2024-04-16 20:26:36.000000 surveyeval-0.1.2/src/surveyeval.egg-info/SOURCES.txt
+-rw-r--r--   0 crobert    (501) staff       (20)        1 2024-04-16 20:26:36.000000 surveyeval-0.1.2/src/surveyeval.egg-info/dependency_links.txt
+-rw-r--r--   0 crobert    (501) staff       (20)      504 2024-04-16 20:26:36.000000 surveyeval-0.1.2/src/surveyeval.egg-info/requires.txt
+-rw-r--r--   0 crobert    (501) staff       (20)       11 2024-04-16 20:26:36.000000 surveyeval-0.1.2/src/surveyeval.egg-info/top_level.txt
```

### Comparing `surveyeval-0.1.1/LICENSE` & `surveyeval-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `surveyeval-0.1.1/PKG-INFO` & `surveyeval-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: surveyeval
-Version: 0.1.1
+Version: 0.1.2
 Summary: A toolkit for survey evaluation
 Home-page: https://github.com/higherbar-ai/survey-eval
 Author: Christopher Robert
 Author-email: crobert@higherbar.ai
 License: Apache 2.0
 Project-URL: Documentation, https://surveyeval.readthedocs.io/
 Requires-Python: >=3.10
@@ -30,15 +30,15 @@
 Requires-Dist: tabula-py~=2.9.0
 Requires-Dist: pypdf~=4.0.1
 Requires-Dist: pytesseract~=0.3.10
 Requires-Dist: tokenizers
 Requires-Dist: docx
 Requires-Dist: mammoth
 Requires-Dist: markdownify
-Requires-Dist: kor~=0.13.0
+Requires-Dist: kor~=1.0.0
 Requires-Dist: scrapy~=2.11.1
 Requires-Dist: ipywidgets
 Requires-Dist: chromadb
 Requires-Dist: pyxform
 Requires-Dist: lxml
 Requires-Dist: requests~=2.31.0
 Requires-Dist: tqdm~=4.65.0
```

### Comparing `surveyeval-0.1.1/README.rst` & `surveyeval-0.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `surveyeval-0.1.1/setup.py` & `surveyeval-0.1.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from setuptools import setup
 
 with open('README.rst') as file:
     readme = file.read()
 
 setup(
     name='surveyeval',
-    version='0.1.1',
+    version='0.1.2',
     packages=['surveyeval'],
     python_requires='>=3.10',
     install_requires=[
         'bs4~=0.0.1',
         'tiktoken~=0.5.2',
         'openai~=1.10.0',
         'langchain~=0.1.13',
@@ -44,15 +44,15 @@
         'tabula-py~=2.9.0',
         'pypdf~=4.0.1',
         'pytesseract~=0.3.10',
         'tokenizers',
         'docx',
         'mammoth',
         'markdownify',
-        'kor~=0.13.0',
+        'kor~=1.0.0',
         'scrapy~=2.11.1',
         'ipywidgets',
         'chromadb',
         'pyxform',
         'lxml',
         'requests~=2.31.0',
         'tqdm~=4.65.0',
```

### Comparing `surveyeval-0.1.1/src/surveyeval/__init__.py` & `surveyeval-0.1.2/src/surveyeval/__init__.py`

 * *Files identical despite different names*

### Comparing `surveyeval-0.1.1/src/surveyeval/core_evaluation_lenses.py` & `surveyeval-0.1.2/src/surveyeval/core_evaluation_lenses.py`

 * *Files identical despite different names*

### Comparing `surveyeval-0.1.1/src/surveyeval/evaluation_engine.py` & `surveyeval-0.1.2/src/surveyeval/evaluation_engine.py`

 * *Files identical despite different names*

### Comparing `surveyeval-0.1.1/src/surveyeval/survey_parser.py` & `surveyeval-0.1.2/src/surveyeval/survey_parser.py`

 * *Files identical despite different names*

### Comparing `surveyeval-0.1.1/src/surveyeval.egg-info/PKG-INFO` & `surveyeval-0.1.2/src/surveyeval.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: surveyeval
-Version: 0.1.1
+Version: 0.1.2
 Summary: A toolkit for survey evaluation
 Home-page: https://github.com/higherbar-ai/survey-eval
 Author: Christopher Robert
 Author-email: crobert@higherbar.ai
 License: Apache 2.0
 Project-URL: Documentation, https://surveyeval.readthedocs.io/
 Requires-Python: >=3.10
@@ -30,15 +30,15 @@
 Requires-Dist: tabula-py~=2.9.0
 Requires-Dist: pypdf~=4.0.1
 Requires-Dist: pytesseract~=0.3.10
 Requires-Dist: tokenizers
 Requires-Dist: docx
 Requires-Dist: mammoth
 Requires-Dist: markdownify
-Requires-Dist: kor~=0.13.0
+Requires-Dist: kor~=1.0.0
 Requires-Dist: scrapy~=2.11.1
 Requires-Dist: ipywidgets
 Requires-Dist: chromadb
 Requires-Dist: pyxform
 Requires-Dist: lxml
 Requires-Dist: requests~=2.31.0
 Requires-Dist: tqdm~=4.65.0
```

