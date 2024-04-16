# Comparing `tmp/cyril1-0.1.2.tar.gz` & `tmp/cyril1-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cyril1-0.1.2.tar", max compression
+gzip compressed data, was "cyril1-0.1.3.tar", max compression
```

## Comparing `cyril1-0.1.2.tar` & `cyril1-0.1.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1772 2024-04-11 21:27:46.843321 cyril1-0.1.2/README.md
--rw-r--r--   0        0        0       22 2024-04-15 21:00:24.544479 cyril1-0.1.2/cyril/__init__.py
--rw-r--r--   0        0        0      182 2024-04-13 20:22:16.238516 cyril1-0.1.2/cyril/__main__.py
--rw-r--r--   0        0        0        0 2024-04-07 13:29:32.008325 cyril1-0.1.2/cyril/commands/__init__.py
--rw-r--r--   0        0        0      687 2024-04-15 20:33:35.021459 cyril1-0.1.2/cyril/commands/ask.py
--rw-r--r--   0        0        0     1108 2024-04-15 20:33:35.017460 cyril1-0.1.2/cyril/commands/bash.py
--rw-r--r--   0        0        0     2512 2024-04-15 20:33:35.025458 cyril1-0.1.2/cyril/commands/keyboard.py
--rw-r--r--   0        0        0     3296 2024-04-12 17:14:23.545563 cyril1-0.1.2/cyril/commands/register.py
--rw-r--r--   0        0        0     1405 2024-04-15 20:33:35.033457 cyril1-0.1.2/cyril/commands/terraform.py
--rw-r--r--   0        0        0      701 2024-04-12 20:24:22.573602 cyril1-0.1.2/cyril/config.py
--rw-r--r--   0        0        0        0 2024-04-07 18:39:39.652273 cyril1-0.1.2/cyril/load_env/__init__.py
--rw-r--r--   0        0        0      884 2024-04-12 07:47:51.152528 cyril1-0.1.2/cyril/load_env/load.py
--rw-r--r--   0        0        0        0 2024-04-07 19:21:38.624029 cyril1-0.1.2/cyril/operators/__init__.py
--rw-r--r--   0        0        0      283 2024-04-12 20:27:50.806588 cyril1-0.1.2/cyril/operators/abc.py
--rw-r--r--   0        0        0     2831 2024-04-13 21:02:17.987531 cyril1-0.1.2/cyril/operators/gemini.py
--rw-r--r--   0        0        0     1068 2024-04-12 20:25:37.510022 cyril1-0.1.2/cyril/operators/gemini_API.py
--rw-r--r--   0        0        0     1118 2024-04-12 20:45:17.957111 cyril1-0.1.2/cyril/operators/open_ai.py
--rw-r--r--   0        0        0       96 2024-04-13 17:03:45.742361 cyril1-0.1.2/cyril/scripts/format.sh
--rw-r--r--   0        0        0       90 2024-04-13 17:02:40.394707 cyril1-0.1.2/cyril/scripts/lint.sh
--rw-r--r--   0        0        0      435 2024-04-13 17:06:22.237799 cyril1-0.1.2/cyril/scripts/test.sh
--rw-r--r--   0        0        0     1252 2024-04-15 21:14:07.461497 cyril1-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     2686 1970-01-01 00:00:00.000000 cyril1-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1773 2024-04-15 21:17:23.225881 cyril1-0.1.3/README.md
+-rw-r--r--   0        0        0       22 2024-04-15 21:17:57.121948 cyril1-0.1.3/cyril/__init__.py
+-rw-r--r--   0        0        0      182 2024-04-13 20:22:16.238516 cyril1-0.1.3/cyril/__main__.py
+-rw-r--r--   0        0        0        0 2024-04-07 13:29:32.008325 cyril1-0.1.3/cyril/commands/__init__.py
+-rw-r--r--   0        0        0      687 2024-04-15 20:33:35.021459 cyril1-0.1.3/cyril/commands/ask.py
+-rw-r--r--   0        0        0     1108 2024-04-15 20:33:35.017460 cyril1-0.1.3/cyril/commands/bash.py
+-rw-r--r--   0        0        0     2512 2024-04-15 20:33:35.025458 cyril1-0.1.3/cyril/commands/keyboard.py
+-rw-r--r--   0        0        0     3296 2024-04-12 17:14:23.545563 cyril1-0.1.3/cyril/commands/register.py
+-rw-r--r--   0        0        0     1405 2024-04-15 20:33:35.033457 cyril1-0.1.3/cyril/commands/terraform.py
+-rw-r--r--   0        0        0      701 2024-04-12 20:24:22.573602 cyril1-0.1.3/cyril/config.py
+-rw-r--r--   0        0        0        0 2024-04-07 18:39:39.652273 cyril1-0.1.3/cyril/load_env/__init__.py
+-rw-r--r--   0        0        0      884 2024-04-12 07:47:51.152528 cyril1-0.1.3/cyril/load_env/load.py
+-rw-r--r--   0        0        0        0 2024-04-07 19:21:38.624029 cyril1-0.1.3/cyril/operators/__init__.py
+-rw-r--r--   0        0        0      283 2024-04-12 20:27:50.806588 cyril1-0.1.3/cyril/operators/abc.py
+-rw-r--r--   0        0        0     2831 2024-04-13 21:02:17.987531 cyril1-0.1.3/cyril/operators/gemini.py
+-rw-r--r--   0        0        0     1068 2024-04-12 20:25:37.510022 cyril1-0.1.3/cyril/operators/gemini_API.py
+-rw-r--r--   0        0        0     1118 2024-04-12 20:45:17.957111 cyril1-0.1.3/cyril/operators/open_ai.py
+-rw-r--r--   0        0        0       96 2024-04-13 17:03:45.742361 cyril1-0.1.3/cyril/scripts/format.sh
+-rw-r--r--   0        0        0       90 2024-04-13 17:02:40.394707 cyril1-0.1.3/cyril/scripts/lint.sh
+-rw-r--r--   0        0        0      435 2024-04-13 17:06:22.237799 cyril1-0.1.3/cyril/scripts/test.sh
+-rw-r--r--   0        0        0     1252 2024-04-15 21:17:57.141948 cyril1-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2687 1970-01-01 00:00:00.000000 cyril1-0.1.3/PKG-INFO
```

### Comparing `cyril1-0.1.2/README.md` & `cyril1-0.1.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -23,15 +23,15 @@
 * **Judgement-Free Zone:** Ask anything, no matter how silly or complex. Cyril won't judge, just guide.
 
 ## Installation
 
 <div class="termy">
 
 ```console
-$ pip install cyril
+$ pip install cyril1
 
 ---> 100%
 ```
 
 </div>
 
 You will also need either
```

### Comparing `cyril1-0.1.2/cyril/commands/ask.py` & `cyril1-0.1.3/cyril/commands/ask.py`

 * *Files identical despite different names*

### Comparing `cyril1-0.1.2/cyril/commands/bash.py` & `cyril1-0.1.3/cyril/commands/bash.py`

 * *Files identical despite different names*

### Comparing `cyril1-0.1.2/cyril/commands/keyboard.py` & `cyril1-0.1.3/cyril/commands/keyboard.py`

 * *Files identical despite different names*

### Comparing `cyril1-0.1.2/cyril/commands/register.py` & `cyril1-0.1.3/cyril/commands/register.py`

 * *Files identical despite different names*

### Comparing `cyril1-0.1.2/cyril/commands/terraform.py` & `cyril1-0.1.3/cyril/commands/terraform.py`

 * *Files identical despite different names*

### Comparing `cyril1-0.1.2/cyril/config.py` & `cyril1-0.1.3/cyril/config.py`

 * *Files identical despite different names*

### Comparing `cyril1-0.1.2/cyril/load_env/load.py` & `cyril1-0.1.3/cyril/load_env/load.py`

 * *Files identical despite different names*

### Comparing `cyril1-0.1.2/cyril/operators/gemini.py` & `cyril1-0.1.3/cyril/operators/gemini.py`

 * *Files identical despite different names*

### Comparing `cyril1-0.1.2/cyril/operators/gemini_API.py` & `cyril1-0.1.3/cyril/operators/gemini_API.py`

 * *Files identical despite different names*

### Comparing `cyril1-0.1.2/cyril/operators/open_ai.py` & `cyril1-0.1.3/cyril/operators/open_ai.py`

 * *Files identical despite different names*

### Comparing `cyril1-0.1.2/pyproject.toml` & `cyril1-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cyril1"
-version = "0.1.2"
+version = "0.1.3"
 description = ""
 authors = ["Raphael Obadia <o.raphou@gmail.com>"]
 readme = "README.md"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Topic :: Software Development :: Build Tools",
```

### Comparing `cyril1-0.1.2/PKG-INFO` & `cyril1-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cyril1
-Version: 0.1.2
+Version: 0.1.3
 Summary: 
 Author: Raphael Obadia
 Author-email: o.raphou@gmail.com
 Requires-Python: >=3.9
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
@@ -48,15 +48,15 @@
 * **Judgement-Free Zone:** Ask anything, no matter how silly or complex. Cyril won't judge, just guide.
 
 ## Installation
 
 <div class="termy">
 
 ```console
-$ pip install cyril
+$ pip install cyril1
 
 ---> 100%
 ```
 
 </div>
 
 You will also need either
```

