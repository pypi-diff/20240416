# Comparing `tmp/cyril1-0.1.3.tar.gz` & `tmp/cyril1-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cyril1-0.1.3.tar", max compression
+gzip compressed data, was "cyril1-0.1.4.tar", max compression
```

## Comparing `cyril1-0.1.3.tar` & `cyril1-0.1.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1773 2024-04-15 21:17:23.225881 cyril1-0.1.3/README.md
--rw-r--r--   0        0        0       22 2024-04-15 21:17:57.121948 cyril1-0.1.3/cyril/__init__.py
--rw-r--r--   0        0        0      182 2024-04-13 20:22:16.238516 cyril1-0.1.3/cyril/__main__.py
--rw-r--r--   0        0        0        0 2024-04-07 13:29:32.008325 cyril1-0.1.3/cyril/commands/__init__.py
--rw-r--r--   0        0        0      687 2024-04-15 20:33:35.021459 cyril1-0.1.3/cyril/commands/ask.py
--rw-r--r--   0        0        0     1108 2024-04-15 20:33:35.017460 cyril1-0.1.3/cyril/commands/bash.py
--rw-r--r--   0        0        0     2512 2024-04-15 20:33:35.025458 cyril1-0.1.3/cyril/commands/keyboard.py
--rw-r--r--   0        0        0     3296 2024-04-12 17:14:23.545563 cyril1-0.1.3/cyril/commands/register.py
--rw-r--r--   0        0        0     1405 2024-04-15 20:33:35.033457 cyril1-0.1.3/cyril/commands/terraform.py
--rw-r--r--   0        0        0      701 2024-04-12 20:24:22.573602 cyril1-0.1.3/cyril/config.py
--rw-r--r--   0        0        0        0 2024-04-07 18:39:39.652273 cyril1-0.1.3/cyril/load_env/__init__.py
--rw-r--r--   0        0        0      884 2024-04-12 07:47:51.152528 cyril1-0.1.3/cyril/load_env/load.py
--rw-r--r--   0        0        0        0 2024-04-07 19:21:38.624029 cyril1-0.1.3/cyril/operators/__init__.py
--rw-r--r--   0        0        0      283 2024-04-12 20:27:50.806588 cyril1-0.1.3/cyril/operators/abc.py
--rw-r--r--   0        0        0     2831 2024-04-13 21:02:17.987531 cyril1-0.1.3/cyril/operators/gemini.py
--rw-r--r--   0        0        0     1068 2024-04-12 20:25:37.510022 cyril1-0.1.3/cyril/operators/gemini_API.py
--rw-r--r--   0        0        0     1118 2024-04-12 20:45:17.957111 cyril1-0.1.3/cyril/operators/open_ai.py
--rw-r--r--   0        0        0       96 2024-04-13 17:03:45.742361 cyril1-0.1.3/cyril/scripts/format.sh
--rw-r--r--   0        0        0       90 2024-04-13 17:02:40.394707 cyril1-0.1.3/cyril/scripts/lint.sh
--rw-r--r--   0        0        0      435 2024-04-13 17:06:22.237799 cyril1-0.1.3/cyril/scripts/test.sh
--rw-r--r--   0        0        0     1252 2024-04-15 21:17:57.141948 cyril1-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     2687 1970-01-01 00:00:00.000000 cyril1-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0     1964 2024-04-16 20:41:28.378655 cyril1-0.1.4/README.md
+-rw-r--r--   0        0        0       22 2024-04-16 20:41:28.382655 cyril1-0.1.4/cyril/__init__.py
+-rw-r--r--   0        0        0      182 2024-04-13 20:22:16.238516 cyril1-0.1.4/cyril/__main__.py
+-rw-r--r--   0        0        0        0 2024-04-07 13:29:32.008325 cyril1-0.1.4/cyril/commands/__init__.py
+-rw-r--r--   0        0        0      687 2024-04-15 20:33:35.021459 cyril1-0.1.4/cyril/commands/ask.py
+-rw-r--r--   0        0        0     1108 2024-04-15 20:33:35.017460 cyril1-0.1.4/cyril/commands/bash.py
+-rw-r--r--   0        0        0     2512 2024-04-15 20:33:35.025458 cyril1-0.1.4/cyril/commands/keyboard.py
+-rw-r--r--   0        0        0     3296 2024-04-12 17:14:23.545563 cyril1-0.1.4/cyril/commands/register.py
+-rw-r--r--   0        0        0     1405 2024-04-15 20:33:35.033457 cyril1-0.1.4/cyril/commands/terraform.py
+-rw-r--r--   0        0        0      701 2024-04-12 20:24:22.573602 cyril1-0.1.4/cyril/config.py
+-rw-r--r--   0        0        0        0 2024-04-07 18:39:39.652273 cyril1-0.1.4/cyril/load_env/__init__.py
+-rw-r--r--   0        0        0      884 2024-04-12 07:47:51.152528 cyril1-0.1.4/cyril/load_env/load.py
+-rw-r--r--   0        0        0        0 2024-04-07 19:21:38.624029 cyril1-0.1.4/cyril/operators/__init__.py
+-rw-r--r--   0        0        0      283 2024-04-12 20:27:50.806588 cyril1-0.1.4/cyril/operators/abc.py
+-rw-r--r--   0        0        0     2831 2024-04-13 21:02:17.987531 cyril1-0.1.4/cyril/operators/gemini.py
+-rw-r--r--   0        0        0     1068 2024-04-12 20:25:37.510022 cyril1-0.1.4/cyril/operators/gemini_API.py
+-rw-r--r--   0        0        0     1118 2024-04-12 20:45:17.957111 cyril1-0.1.4/cyril/operators/open_ai.py
+-rw-r--r--   0        0        0       96 2024-04-13 17:03:45.742361 cyril1-0.1.4/cyril/scripts/format.sh
+-rw-r--r--   0        0        0       90 2024-04-13 17:02:40.394707 cyril1-0.1.4/cyril/scripts/lint.sh
+-rw-r--r--   0        0        0      435 2024-04-13 17:06:22.237799 cyril1-0.1.4/cyril/scripts/test.sh
+-rw-r--r--   0        0        0     1300 2024-04-16 20:41:28.370655 cyril1-0.1.4/pyproject.toml
+-rw-r--r--   0        0        0     2978 1970-01-01 00:00:00.000000 cyril1-0.1.4/PKG-INFO
```

### Comparing `cyril1-0.1.3/README.md` & `cyril1-0.1.4/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,18 +1,15 @@
 <p align="center">
   <center> Cyril </center>
 <p align="center">
     <em>Cyril, your best colleague is sitting next to you to assist you.</em>
 
 ---
-
-**Documentation**: Docu what?</a>
-
-**Source Code**: Todo</a>
-
+[![PyPI version](https://badge.fury.io/py/cyril1.svg)](https://badge.fury.io/py/cyril1)
+[![Downloads](https://pepy.tech/badge/cyril1)](https://pepy.tech/project/cyril1)
 ---
 
 Imagine a good colleague, a friend, a genius who assists you every minute. A Terraform question? Ask Cyril! A Bash question? Ask Cyril! You have a question about life in general or about keyboards! Just ASK!
 
 **Cyril** is there for you, he is your lover, your best friend, your teacher, your god. HE WILL always be available for you.
 
 The key features are:
@@ -37,21 +34,23 @@
 You will also need either
 * OpenAi API key
 * Gemini API key
 * GCP project_id with an accès to Gemini **AND** ADC with gcloud cli installed
 
 Export the API key as an environment variable:
 * export CYRIL_OPEN_API=***
-* export CYRIL_GEMINI=*** 
+* export CYRIL_GEMINI=*** # Not Implemented Yet
 * export PROJECT_ID=***
 
 ## Example
 * Open a terminal
 ``` console
 $ cyril ask "What is the meaning of life?"
 
 $ cyril bash "How to list all files in a directory?"
 
 $ cyril terraform "How to create a new resource in Terraform?"
+
+$cyril keyboard "What is the best mechanical keyboard switch?"
 ```
```

### Comparing `cyril1-0.1.3/cyril/commands/ask.py` & `cyril1-0.1.4/cyril/commands/ask.py`

 * *Files identical despite different names*

### Comparing `cyril1-0.1.3/cyril/commands/bash.py` & `cyril1-0.1.4/cyril/commands/bash.py`

 * *Files identical despite different names*

### Comparing `cyril1-0.1.3/cyril/commands/keyboard.py` & `cyril1-0.1.4/cyril/commands/keyboard.py`

 * *Files identical despite different names*

### Comparing `cyril1-0.1.3/cyril/commands/register.py` & `cyril1-0.1.4/cyril/commands/register.py`

 * *Files identical despite different names*

### Comparing `cyril1-0.1.3/cyril/commands/terraform.py` & `cyril1-0.1.4/cyril/commands/terraform.py`

 * *Files identical despite different names*

### Comparing `cyril1-0.1.3/cyril/config.py` & `cyril1-0.1.4/cyril/config.py`

 * *Files identical despite different names*

### Comparing `cyril1-0.1.3/cyril/load_env/load.py` & `cyril1-0.1.4/cyril/load_env/load.py`

 * *Files identical despite different names*

### Comparing `cyril1-0.1.3/cyril/operators/gemini.py` & `cyril1-0.1.4/cyril/operators/gemini.py`

 * *Files identical despite different names*

### Comparing `cyril1-0.1.3/cyril/operators/gemini_API.py` & `cyril1-0.1.4/cyril/operators/gemini_API.py`

 * *Files identical despite different names*

### Comparing `cyril1-0.1.3/cyril/operators/open_ai.py` & `cyril1-0.1.4/cyril/operators/open_ai.py`

 * *Files identical despite different names*

### Comparing `cyril1-0.1.3/pyproject.toml` & `cyril1-0.1.4/pyproject.toml`

 * *Files 25% similar despite different names*

```diff
@@ -1,21 +1,23 @@
 [tool.poetry]
 name = "cyril1"
-version = "0.1.3"
+version = "0.1.4"
 description = ""
 authors = ["Raphael Obadia <o.raphou@gmail.com>"]
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Topic :: Software Development :: Build Tools",
 ]
 packages = [
     { include = "cyril" }
 ]
+repository = "https://github.com/RaphOb/Cyril"
+
 
 [tool.poetry.dependencies]
 python = ">=3.9"
 ruff = "^0.3.5"
 black = "^24.3.0"
 typer = "^0.12.1"
 pydantic-settings = "^2.2.1"
```

### Comparing `cyril1-0.1.3/PKG-INFO` & `cyril1-0.1.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: cyril1
-Version: 0.1.3
+Version: 0.1.4
 Summary: 
+Home-page: https://github.com/RaphOb/Cyril
 Author: Raphael Obadia
 Author-email: o.raphou@gmail.com
 Requires-Python: >=3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -17,27 +18,25 @@
 Requires-Dist: halo (>=0.0.31,<0.0.32)
 Requires-Dist: httpx (>=0.27.0,<0.28.0)
 Requires-Dist: openai (>=1.16.2,<2.0.0)
 Requires-Dist: pydantic-settings (>=2.2.1,<3.0.0)
 Requires-Dist: requests (>=2.31.0,<3.0.0)
 Requires-Dist: ruff (>=0.3.5,<0.4.0)
 Requires-Dist: typer (>=0.12.1,<0.13.0)
+Project-URL: Repository, https://github.com/RaphOb/Cyril
 Description-Content-Type: text/markdown
 
 <p align="center">
   <center> Cyril </center>
 <p align="center">
     <em>Cyril, your best colleague is sitting next to you to assist you.</em>
 
 ---
-
-**Documentation**: Docu what?</a>
-
-**Source Code**: Todo</a>
-
+[![PyPI version](https://badge.fury.io/py/cyril1.svg)](https://badge.fury.io/py/cyril1)
+[![Downloads](https://pepy.tech/badge/cyril1)](https://pepy.tech/project/cyril1)
 ---
 
 Imagine a good colleague, a friend, a genius who assists you every minute. A Terraform question? Ask Cyril! A Bash question? Ask Cyril! You have a question about life in general or about keyboards! Just ASK!
 
 **Cyril** is there for you, he is your lover, your best friend, your teacher, your god. HE WILL always be available for you.
 
 The key features are:
@@ -62,22 +61,24 @@
 You will also need either
 * OpenAi API key
 * Gemini API key
 * GCP project_id with an accès to Gemini **AND** ADC with gcloud cli installed
 
 Export the API key as an environment variable:
 * export CYRIL_OPEN_API=***
-* export CYRIL_GEMINI=*** 
+* export CYRIL_GEMINI=*** # Not Implemented Yet
 * export PROJECT_ID=***
 
 ## Example
 * Open a terminal
 ``` console
 $ cyril ask "What is the meaning of life?"
 
 $ cyril bash "How to list all files in a directory?"
 
 $ cyril terraform "How to create a new resource in Terraform?"
+
+$cyril keyboard "What is the best mechanical keyboard switch?"
 ```
```

