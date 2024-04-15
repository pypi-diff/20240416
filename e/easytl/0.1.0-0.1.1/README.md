# Comparing `tmp/easytl-0.1.0.tar.gz` & `tmp/easytl-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easytl-0.1.0.tar", last modified: Wed Apr 10 05:59:40 2024, max compression
+gzip compressed data, was "easytl-0.1.1.tar", last modified: Mon Apr 15 03:51:21 2024, max compression
```

## Comparing `easytl-0.1.0.tar` & `easytl-0.1.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 05:59:40.220667 easytl-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 05:59:40.216667 easytl-0.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 05:59:40.220667 easytl-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-10 05:59:26.000000 easytl-0.1.0/.github/workflows/workflow.yml
--rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-04-10 05:59:26.000000 easytl-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    26526 2024-04-10 05:59:26.000000 easytl-0.1.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     6552 2024-04-10 05:59:40.220667 easytl-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     5813 2024-04-10 05:59:26.000000 easytl-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      846 2024-04-10 05:59:26.000000 easytl-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 05:59:40.220667 easytl-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 05:59:40.216667 easytl-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 05:59:40.220667 easytl-0.1.0/src/easytl/
--rw-r--r--   0 runner    (1001) docker     (127)      859 2024-04-10 05:59:26.000000 easytl-0.1.0/src/easytl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-04-10 05:59:26.000000 easytl-0.1.0/src/easytl/classes.py
--rw-r--r--   0 runner    (1001) docker     (127)    10289 2024-04-10 05:59:26.000000 easytl-0.1.0/src/easytl/deepl_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    39632 2024-04-10 05:59:26.000000 easytl-0.1.0/src/easytl/easytl.py
--rw-r--r--   0 runner    (1001) docker     (127)     2050 2024-04-10 05:59:26.000000 easytl-0.1.0/src/easytl/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)    14139 2024-04-10 05:59:26.000000 easytl-0.1.0/src/easytl/gemini_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    15670 2024-04-10 05:59:26.000000 easytl-0.1.0/src/easytl/openai_service.py
--rw-r--r--   0 runner    (1001) docker     (127)    22559 2024-04-10 05:59:26.000000 easytl-0.1.0/src/easytl/util.py
--rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-10 05:59:26.000000 easytl-0.1.0/src/easytl/version.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 05:59:40.220667 easytl-0.1.0/src/easytl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     6552 2024-04-10 05:59:40.000000 easytl-0.1.0/src/easytl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-10 05:59:40.000000 easytl-0.1.0/src/easytl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 05:59:40.000000 easytl-0.1.0/src/easytl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-10 05:59:40.000000 easytl-0.1.0/src/easytl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-10 05:59:40.000000 easytl-0.1.0/src/easytl.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 03:51:21.177182 easytl-0.1.1/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 03:51:21.173182 easytl-0.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 03:51:21.177182 easytl-0.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)      729 2024-04-15 03:51:10.000000 easytl-0.1.1/.github/workflows/workflow.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     3100 2024-04-15 03:51:10.000000 easytl-0.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    26526 2024-04-15 03:51:10.000000 easytl-0.1.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6552 2024-04-15 03:51:21.177182 easytl-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     5813 2024-04-15 03:51:10.000000 easytl-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      846 2024-04-15 03:51:10.000000 easytl-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 03:51:21.177182 easytl-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 03:51:21.173182 easytl-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 03:51:21.177182 easytl-0.1.1/src/easytl/
+-rw-r--r--   0 runner    (1001) docker     (127)      895 2024-04-15 03:51:10.000000 easytl-0.1.1/src/easytl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1943 2024-04-15 03:51:10.000000 easytl-0.1.1/src/easytl/classes.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10289 2024-04-15 03:51:10.000000 easytl-0.1.1/src/easytl/deepl_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    39632 2024-04-15 03:51:10.000000 easytl-0.1.1/src/easytl/easytl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2086 2024-04-15 03:51:10.000000 easytl-0.1.1/src/easytl/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14139 2024-04-15 03:51:10.000000 easytl-0.1.1/src/easytl/gemini_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15670 2024-04-15 03:51:10.000000 easytl-0.1.1/src/easytl/openai_service.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22559 2024-04-15 03:51:10.000000 easytl-0.1.1/src/easytl/util.py
+-rw-r--r--   0 runner    (1001) docker     (127)      202 2024-04-15 03:51:10.000000 easytl-0.1.1/src/easytl/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 03:51:21.177182 easytl-0.1.1/src/easytl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     6552 2024-04-15 03:51:21.000000 easytl-0.1.1/src/easytl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-15 03:51:21.000000 easytl-0.1.1/src/easytl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 03:51:21.000000 easytl-0.1.1/src/easytl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-15 03:51:21.000000 easytl-0.1.1/src/easytl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-15 03:51:21.000000 easytl-0.1.1/src/easytl.egg-info/top_level.txt
```

### Comparing `easytl-0.1.0/.github/workflows/workflow.yml` & `easytl-0.1.1/.github/workflows/workflow.yml`

 * *Files identical despite different names*

### Comparing `easytl-0.1.0/.gitignore` & `easytl-0.1.1/.gitignore`

 * *Files identical despite different names*

### Comparing `easytl-0.1.0/LICENSE.md` & `easytl-0.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `easytl-0.1.0/PKG-INFO` & `easytl-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easytl
-Version: 0.1.0
+Version: 0.1.1
 Summary: Wrapper for OpenAI, DeepL, and Gemini APIs for easy translation of text.
 Author-email: Bikatr7 <Tetralon07@gmail.com>
 Project-URL: Homepage, https://github.com/Bikatr7/EasyTL
 Project-URL: Issues, https://github.com/Bikatr7/EasyTL/issues
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
 Classifier: Operating System :: OS Independent
```

### Comparing `easytl-0.1.0/README.md` & `easytl-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `easytl-0.1.0/pyproject.toml` & `easytl-0.1.1/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     "deepl==1.16.1",
     "openai==1.13.3",
     "backoff==2.2.1",
     "tiktoken==0.6.0"
 ]
 
 name = "easytl"
-version = "v0.1.0"
+version = "v0.1.1"
 authors = [
   { name="Bikatr7", email="Tetralon07@gmail.com" },
 ]
 description = "Wrapper for OpenAI, DeepL, and Gemini APIs for easy translation of text."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `easytl-0.1.0/src/easytl/__init__.py` & `easytl-0.1.1/src/easytl/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,10 +7,10 @@
 __author__ = "Bikatr7 <Tetralon07@gmail.com>"
 
 from .easytl import EasyTL
 from .classes import Language, SplitSentences, Formality, GlossaryInfo, ModelTranslationMessage, SystemTranslationMessage, Message
 from .util import MODEL_COSTS, ALLOWED_GEMINI_MODELS, ALLOWED_OPENAI_MODELS
 
 from .exceptions import DeepLException, GoogleAPIError, OpenAIError, EasyTLException, InvalidAPIKeyException, InvalidEasyTLSettings
-from .exceptions import AuthenticationError, InternalServerError, RateLimitError, APITimeoutError
+from .exceptions import AuthenticationError, InternalServerError, RateLimitError, APITimeoutError, APIConnectionError, APIStatusError
 from .exceptions import AuthorizationException, QuotaExceededException
 from .exceptions import GoogleAuthError
```

### Comparing `easytl-0.1.0/src/easytl/classes.py` & `easytl-0.1.1/src/easytl/classes.py`

 * *Files identical despite different names*

### Comparing `easytl-0.1.0/src/easytl/deepl_service.py` & `easytl-0.1.1/src/easytl/deepl_service.py`

 * *Files identical despite different names*

### Comparing `easytl-0.1.0/src/easytl/easytl.py` & `easytl-0.1.1/src/easytl/easytl.py`

 * *Files identical despite different names*

### Comparing `easytl-0.1.0/src/easytl/exceptions.py` & `easytl-0.1.1/src/easytl/exceptions.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 ## google generic exception
 from google.api_core.exceptions import GoogleAPIError
 
 ## openai generic exception
 from openai import OpenAIError
 
 ## service specific exceptions
-from openai import AuthenticationError, InternalServerError, RateLimitError, APITimeoutError
+from openai import AuthenticationError, InternalServerError, RateLimitError, APITimeoutError, APIConnectionError, APIStatusError
 from deepl.exceptions import AuthorizationException, QuotaExceededException
 from google.auth.exceptions import GoogleAuthError
 
 class EasyTLException(Exception):
 
     """
```

### Comparing `easytl-0.1.0/src/easytl/gemini_service.py` & `easytl-0.1.1/src/easytl/gemini_service.py`

 * *Files identical despite different names*

### Comparing `easytl-0.1.0/src/easytl/openai_service.py` & `easytl-0.1.1/src/easytl/openai_service.py`

 * *Files identical despite different names*

### Comparing `easytl-0.1.0/src/easytl/util.py` & `easytl-0.1.1/src/easytl/util.py`

 * *Files identical despite different names*

### Comparing `easytl-0.1.0/src/easytl.egg-info/PKG-INFO` & `easytl-0.1.1/src/easytl.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easytl
-Version: 0.1.0
+Version: 0.1.1
 Summary: Wrapper for OpenAI, DeepL, and Gemini APIs for easy translation of text.
 Author-email: Bikatr7 <Tetralon07@gmail.com>
 Project-URL: Homepage, https://github.com/Bikatr7/EasyTL
 Project-URL: Issues, https://github.com/Bikatr7/EasyTL/issues
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v2 or later (LGPLv2+)
 Classifier: Operating System :: OS Independent
```

