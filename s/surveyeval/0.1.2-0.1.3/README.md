# Comparing `tmp/surveyeval-0.1.2.tar.gz` & `tmp/surveyeval-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "surveyeval-0.1.2.tar", last modified: Tue Apr 16 20:26:36 2024, max compression
+gzip compressed data, was "surveyeval-0.1.3.tar", last modified: Tue Apr 16 20:56:30 2024, max compression
```

## Comparing `surveyeval-0.1.2.tar` & `surveyeval-0.1.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 crobert    (501) staff       (20)        0 2024-04-16 20:26:36.824059 surveyeval-0.1.2/
--rw-r--r--   0 crobert    (501) staff       (20)    11357 2023-11-29 20:42:10.000000 surveyeval-0.1.2/LICENSE
--rw-r--r--   0 crobert    (501) staff       (20)    11786 2024-04-16 20:26:36.823788 surveyeval-0.1.2/PKG-INFO
--rw-r--r--   0 crobert    (501) staff       (20)    10430 2024-04-14 15:10:57.000000 surveyeval-0.1.2/README.rst
--rw-r--r--   0 crobert    (501) staff       (20)       38 2024-04-16 20:26:36.824112 surveyeval-0.1.2/setup.cfg
--rw-r--r--   0 crobert    (501) staff       (20)     2043 2024-04-16 20:26:26.000000 surveyeval-0.1.2/setup.py
-drwxr-xr-x   0 crobert    (501) staff       (20)        0 2024-04-16 20:26:36.817239 surveyeval-0.1.2/src/
-drwxr-xr-x   0 crobert    (501) staff       (20)        0 2024-04-16 20:26:36.820910 surveyeval-0.1.2/src/surveyeval/
--rw-r--r--   0 crobert    (501) staff       (20)     1058 2024-04-14 15:10:57.000000 surveyeval-0.1.2/src/surveyeval/__init__.py
--rw-r--r--   0 crobert    (501) staff       (20)    49441 2024-04-14 15:33:38.000000 surveyeval-0.1.2/src/surveyeval/core_evaluation_lenses.py
--rw-r--r--   0 crobert    (501) staff       (20)    33231 2024-04-14 16:03:22.000000 surveyeval-0.1.2/src/surveyeval/evaluation_engine.py
--rw-r--r--   0 crobert    (501) staff       (20)    56480 2024-04-14 15:27:21.000000 surveyeval-0.1.2/src/surveyeval/survey_parser.py
-drwxr-xr-x   0 crobert    (501) staff       (20)        0 2024-04-16 20:26:36.823313 surveyeval-0.1.2/src/surveyeval.egg-info/
--rw-r--r--   0 crobert    (501) staff       (20)    11786 2024-04-16 20:26:36.000000 surveyeval-0.1.2/src/surveyeval.egg-info/PKG-INFO
--rw-r--r--   0 crobert    (501) staff       (20)      352 2024-04-16 20:26:36.000000 surveyeval-0.1.2/src/surveyeval.egg-info/SOURCES.txt
--rw-r--r--   0 crobert    (501) staff       (20)        1 2024-04-16 20:26:36.000000 surveyeval-0.1.2/src/surveyeval.egg-info/dependency_links.txt
--rw-r--r--   0 crobert    (501) staff       (20)      504 2024-04-16 20:26:36.000000 surveyeval-0.1.2/src/surveyeval.egg-info/requires.txt
--rw-r--r--   0 crobert    (501) staff       (20)       11 2024-04-16 20:26:36.000000 surveyeval-0.1.2/src/surveyeval.egg-info/top_level.txt
+drwxr-xr-x   0 crobert    (501) staff       (20)        0 2024-04-16 20:56:30.363758 surveyeval-0.1.3/
+-rw-r--r--   0 crobert    (501) staff       (20)    11357 2023-11-29 20:42:10.000000 surveyeval-0.1.3/LICENSE
+-rw-r--r--   0 crobert    (501) staff       (20)    11786 2024-04-16 20:56:30.363467 surveyeval-0.1.3/PKG-INFO
+-rw-r--r--   0 crobert    (501) staff       (20)    10430 2024-04-14 15:10:57.000000 surveyeval-0.1.3/README.rst
+-rw-r--r--   0 crobert    (501) staff       (20)       38 2024-04-16 20:56:30.363808 surveyeval-0.1.3/setup.cfg
+-rw-r--r--   0 crobert    (501) staff       (20)     2043 2024-04-16 20:56:22.000000 surveyeval-0.1.3/setup.py
+drwxr-xr-x   0 crobert    (501) staff       (20)        0 2024-04-16 20:56:30.357399 surveyeval-0.1.3/src/
+drwxr-xr-x   0 crobert    (501) staff       (20)        0 2024-04-16 20:56:30.361071 surveyeval-0.1.3/src/surveyeval/
+-rw-r--r--   0 crobert    (501) staff       (20)     1058 2024-04-14 15:10:57.000000 surveyeval-0.1.3/src/surveyeval/__init__.py
+-rw-r--r--   0 crobert    (501) staff       (20)    49441 2024-04-14 15:33:38.000000 surveyeval-0.1.3/src/surveyeval/core_evaluation_lenses.py
+-rw-r--r--   0 crobert    (501) staff       (20)    33231 2024-04-14 16:03:22.000000 surveyeval-0.1.3/src/surveyeval/evaluation_engine.py
+-rw-r--r--   0 crobert    (501) staff       (20)    56480 2024-04-14 15:27:21.000000 surveyeval-0.1.3/src/surveyeval/survey_parser.py
+drwxr-xr-x   0 crobert    (501) staff       (20)        0 2024-04-16 20:56:30.363043 surveyeval-0.1.3/src/surveyeval.egg-info/
+-rw-r--r--   0 crobert    (501) staff       (20)    11786 2024-04-16 20:56:30.000000 surveyeval-0.1.3/src/surveyeval.egg-info/PKG-INFO
+-rw-r--r--   0 crobert    (501) staff       (20)      352 2024-04-16 20:56:30.000000 surveyeval-0.1.3/src/surveyeval.egg-info/SOURCES.txt
+-rw-r--r--   0 crobert    (501) staff       (20)        1 2024-04-16 20:56:30.000000 surveyeval-0.1.3/src/surveyeval.egg-info/dependency_links.txt
+-rw-r--r--   0 crobert    (501) staff       (20)      504 2024-04-16 20:56:30.000000 surveyeval-0.1.3/src/surveyeval.egg-info/requires.txt
+-rw-r--r--   0 crobert    (501) staff       (20)       11 2024-04-16 20:56:30.000000 surveyeval-0.1.3/src/surveyeval.egg-info/top_level.txt
```

### Comparing `surveyeval-0.1.2/LICENSE` & `surveyeval-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `surveyeval-0.1.2/PKG-INFO` & `surveyeval-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: surveyeval
-Version: 0.1.2
+Version: 0.1.3
 Summary: A toolkit for survey evaluation
 Home-page: https://github.com/higherbar-ai/survey-eval
 Author: Christopher Robert
 Author-email: crobert@higherbar.ai
 License: Apache 2.0
 Project-URL: Documentation, https://surveyeval.readthedocs.io/
 Requires-Python: >=3.10
 License-File: LICENSE
 Requires-Dist: bs4~=0.0.1
 Requires-Dist: tiktoken~=0.5.2
 Requires-Dist: openai~=1.10.0
-Requires-Dist: langchain~=0.1.13
+Requires-Dist: langchain~=0.1.15
 Requires-Dist: langchain-openai~=0.0.5
 Requires-Dist: langchain-community~=0.0.17
 Requires-Dist: unstructured[local-inference]
 Requires-Dist: tensorboard>2.12.2
 Requires-Dist: uvicorn[standard]~=0.22.0
 Requires-Dist: pydantic~=1.10.8
 Requires-Dist: markdown~=3.4.3
```

### Comparing `surveyeval-0.1.2/README.rst` & `surveyeval-0.1.3/README.rst`

 * *Files identical despite different names*

### Comparing `surveyeval-0.1.2/setup.py` & `surveyeval-0.1.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -15,22 +15,22 @@
 from setuptools import setup
 
 with open('README.rst') as file:
     readme = file.read()
 
 setup(
     name='surveyeval',
-    version='0.1.2',
+    version='0.1.3',
     packages=['surveyeval'],
     python_requires='>=3.10',
     install_requires=[
         'bs4~=0.0.1',
         'tiktoken~=0.5.2',
         'openai~=1.10.0',
-        'langchain~=0.1.13',
+        'langchain~=0.1.15',
         'langchain-openai~=0.0.5',
         'langchain-community~=0.0.17',
         'unstructured[local-inference]',
         'tensorboard>2.12.2',
         'uvicorn[standard]~=0.22.0',
         'pydantic~=1.10.8',
         'markdown~=3.4.3',
```

### Comparing `surveyeval-0.1.2/src/surveyeval/__init__.py` & `surveyeval-0.1.3/src/surveyeval/__init__.py`

 * *Files identical despite different names*

### Comparing `surveyeval-0.1.2/src/surveyeval/core_evaluation_lenses.py` & `surveyeval-0.1.3/src/surveyeval/core_evaluation_lenses.py`

 * *Files identical despite different names*

### Comparing `surveyeval-0.1.2/src/surveyeval/evaluation_engine.py` & `surveyeval-0.1.3/src/surveyeval/evaluation_engine.py`

 * *Files identical despite different names*

### Comparing `surveyeval-0.1.2/src/surveyeval/survey_parser.py` & `surveyeval-0.1.3/src/surveyeval/survey_parser.py`

 * *Files identical despite different names*

### Comparing `surveyeval-0.1.2/src/surveyeval.egg-info/PKG-INFO` & `surveyeval-0.1.3/src/surveyeval.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: surveyeval
-Version: 0.1.2
+Version: 0.1.3
 Summary: A toolkit for survey evaluation
 Home-page: https://github.com/higherbar-ai/survey-eval
 Author: Christopher Robert
 Author-email: crobert@higherbar.ai
 License: Apache 2.0
 Project-URL: Documentation, https://surveyeval.readthedocs.io/
 Requires-Python: >=3.10
 License-File: LICENSE
 Requires-Dist: bs4~=0.0.1
 Requires-Dist: tiktoken~=0.5.2
 Requires-Dist: openai~=1.10.0
-Requires-Dist: langchain~=0.1.13
+Requires-Dist: langchain~=0.1.15
 Requires-Dist: langchain-openai~=0.0.5
 Requires-Dist: langchain-community~=0.0.17
 Requires-Dist: unstructured[local-inference]
 Requires-Dist: tensorboard>2.12.2
 Requires-Dist: uvicorn[standard]~=0.22.0
 Requires-Dist: pydantic~=1.10.8
 Requires-Dist: markdown~=3.4.3
```

