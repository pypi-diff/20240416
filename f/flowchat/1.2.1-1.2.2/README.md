# Comparing `tmp/flowchat-1.2.1.tar.gz` & `tmp/flowchat-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flowchat-1.2.1.tar", last modified: Tue Apr 16 02:45:47 2024, max compression
+gzip compressed data, was "flowchat-1.2.2.tar", last modified: Tue Apr 16 03:31:11 2024, max compression
```

## Comparing `flowchat-1.2.1.tar` & `flowchat-1.2.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 flatypus   (501) staff       (20)        0 2024-04-16 02:45:47.553590 flowchat-1.2.1/
--rw-r--r--   0 flatypus   (501) staff       (20)     1068 2024-03-05 00:02:48.000000 flowchat-1.2.1/LICENSE
--rw-r--r--   0 flatypus   (501) staff       (20)     7664 2024-04-16 02:45:47.553359 flowchat-1.2.1/PKG-INFO
--rw-r--r--   0 flatypus   (501) staff       (20)     6705 2024-04-14 20:10:37.000000 flowchat-1.2.1/README.md
-drwxr-xr-x   0 flatypus   (501) staff       (20)        0 2024-04-16 02:45:47.549507 flowchat-1.2.1/flowchat/
--rw-r--r--   0 flatypus   (501) staff       (20)      185 2024-04-16 02:26:44.000000 flowchat-1.2.1/flowchat/__init__.py
--rw-r--r--   0 flatypus   (501) staff       (20)      590 2024-03-08 00:59:53.000000 flowchat-1.2.1/flowchat/autodedent.py
--rw-r--r--   0 flatypus   (501) staff       (20)    11213 2024-04-16 02:44:33.000000 flowchat-1.2.1/flowchat/chain.py
-drwxr-xr-x   0 flatypus   (501) staff       (20)        0 2024-04-16 02:45:47.550834 flowchat-1.2.1/flowchat/private/
--rw-r--r--   0 flatypus   (501) staff       (20)        0 2023-11-08 02:00:20.000000 flowchat-1.2.1/flowchat/private/__init__.py
--rw-r--r--   0 flatypus   (501) staff       (20)     5258 2024-04-16 02:44:33.000000 flowchat-1.2.1/flowchat/private/_private_helpers.py
--rw-r--r--   0 flatypus   (501) staff       (20)      670 2024-04-16 02:44:31.000000 flowchat-1.2.1/flowchat/types.py
-drwxr-xr-x   0 flatypus   (501) staff       (20)        0 2024-04-16 02:45:47.553045 flowchat-1.2.1/flowchat.egg-info/
--rw-r--r--   0 flatypus   (501) staff       (20)     7664 2024-04-16 02:45:47.000000 flowchat-1.2.1/flowchat.egg-info/PKG-INFO
--rw-r--r--   0 flatypus   (501) staff       (20)      455 2024-04-16 02:45:47.000000 flowchat-1.2.1/flowchat.egg-info/SOURCES.txt
--rw-r--r--   0 flatypus   (501) staff       (20)        1 2024-04-16 02:45:47.000000 flowchat-1.2.1/flowchat.egg-info/dependency_links.txt
--rw-r--r--   0 flatypus   (501) staff       (20)       32 2024-04-16 02:45:47.000000 flowchat-1.2.1/flowchat.egg-info/requires.txt
--rw-r--r--   0 flatypus   (501) staff       (20)        9 2024-04-16 02:45:47.000000 flowchat-1.2.1/flowchat.egg-info/top_level.txt
--rw-r--r--   0 flatypus   (501) staff       (20)      153 2023-11-25 09:49:08.000000 flowchat-1.2.1/pyproject.toml
--rw-r--r--   0 flatypus   (501) staff       (20)       38 2024-04-16 02:45:47.553647 flowchat-1.2.1/setup.cfg
--rw-r--r--   0 flatypus   (501) staff       (20)     1391 2024-04-16 02:45:36.000000 flowchat-1.2.1/setup.py
-drwxr-xr-x   0 flatypus   (501) staff       (20)        0 2024-04-16 02:45:47.552482 flowchat-1.2.1/tests/
--rw-r--r--   0 flatypus   (501) staff       (20)     2041 2023-11-25 09:35:06.000000 flowchat-1.2.1/tests/test_autodedent.py
--rw-r--r--   0 flatypus   (501) staff       (20)     4250 2024-04-16 02:44:31.000000 flowchat-1.2.1/tests/test_chaining.py
--rw-r--r--   0 flatypus   (501) staff       (20)     1344 2023-11-25 07:32:30.000000 flowchat-1.2.1/tests/test_config.py
--rw-r--r--   0 flatypus   (501) staff       (20)     4765 2024-04-16 02:44:31.000000 flowchat-1.2.1/tests/test_pull.py
--rw-r--r--   0 flatypus   (501) staff       (20)     1214 2023-11-25 10:45:06.000000 flowchat-1.2.1/tests/test_stream.py
+drwxr-xr-x   0 flatypus   (501) staff       (20)        0 2024-04-16 03:31:11.984276 flowchat-1.2.2/
+-rw-r--r--   0 flatypus   (501) staff       (20)     1068 2024-03-05 00:02:48.000000 flowchat-1.2.2/LICENSE
+-rw-r--r--   0 flatypus   (501) staff       (20)     7664 2024-04-16 03:31:11.984085 flowchat-1.2.2/PKG-INFO
+-rw-r--r--   0 flatypus   (501) staff       (20)     6705 2024-04-14 20:10:37.000000 flowchat-1.2.2/README.md
+drwxr-xr-x   0 flatypus   (501) staff       (20)        0 2024-04-16 03:31:11.980628 flowchat-1.2.2/flowchat/
+-rw-r--r--   0 flatypus   (501) staff       (20)       81 2024-04-16 03:29:58.000000 flowchat-1.2.2/flowchat/__init__.py
+-rw-r--r--   0 flatypus   (501) staff       (20)      590 2024-03-08 00:59:53.000000 flowchat-1.2.2/flowchat/autodedent.py
+-rw-r--r--   0 flatypus   (501) staff       (20)    10525 2024-04-16 03:29:01.000000 flowchat-1.2.2/flowchat/chain.py
+drwxr-xr-x   0 flatypus   (501) staff       (20)        0 2024-04-16 03:31:11.981680 flowchat-1.2.2/flowchat/private/
+-rw-r--r--   0 flatypus   (501) staff       (20)        0 2023-11-08 02:00:20.000000 flowchat-1.2.2/flowchat/private/__init__.py
+-rw-r--r--   0 flatypus   (501) staff       (20)     5258 2024-04-16 02:52:28.000000 flowchat-1.2.2/flowchat/private/_private_helpers.py
+-rw-r--r--   0 flatypus   (501) staff       (20)     1355 2024-04-16 03:28:44.000000 flowchat-1.2.2/flowchat/types.py
+drwxr-xr-x   0 flatypus   (501) staff       (20)        0 2024-04-16 03:31:11.983784 flowchat-1.2.2/flowchat.egg-info/
+-rw-r--r--   0 flatypus   (501) staff       (20)     7664 2024-04-16 03:31:11.000000 flowchat-1.2.2/flowchat.egg-info/PKG-INFO
+-rw-r--r--   0 flatypus   (501) staff       (20)      455 2024-04-16 03:31:11.000000 flowchat-1.2.2/flowchat.egg-info/SOURCES.txt
+-rw-r--r--   0 flatypus   (501) staff       (20)        1 2024-04-16 03:31:11.000000 flowchat-1.2.2/flowchat.egg-info/dependency_links.txt
+-rw-r--r--   0 flatypus   (501) staff       (20)       32 2024-04-16 03:31:11.000000 flowchat-1.2.2/flowchat.egg-info/requires.txt
+-rw-r--r--   0 flatypus   (501) staff       (20)        9 2024-04-16 03:31:11.000000 flowchat-1.2.2/flowchat.egg-info/top_level.txt
+-rw-r--r--   0 flatypus   (501) staff       (20)      153 2023-11-25 09:49:08.000000 flowchat-1.2.2/pyproject.toml
+-rw-r--r--   0 flatypus   (501) staff       (20)       38 2024-04-16 03:31:11.984323 flowchat-1.2.2/setup.cfg
+-rw-r--r--   0 flatypus   (501) staff       (20)     1391 2024-04-16 03:30:55.000000 flowchat-1.2.2/setup.py
+drwxr-xr-x   0 flatypus   (501) staff       (20)        0 2024-04-16 03:31:11.983322 flowchat-1.2.2/tests/
+-rw-r--r--   0 flatypus   (501) staff       (20)     2041 2023-11-25 09:35:06.000000 flowchat-1.2.2/tests/test_autodedent.py
+-rw-r--r--   0 flatypus   (501) staff       (20)     4250 2024-04-16 02:44:31.000000 flowchat-1.2.2/tests/test_chaining.py
+-rw-r--r--   0 flatypus   (501) staff       (20)     1344 2023-11-25 07:32:30.000000 flowchat-1.2.2/tests/test_config.py
+-rw-r--r--   0 flatypus   (501) staff       (20)     4765 2024-04-16 02:44:31.000000 flowchat-1.2.2/tests/test_pull.py
+-rw-r--r--   0 flatypus   (501) staff       (20)     1214 2023-11-25 10:45:06.000000 flowchat-1.2.2/tests/test_stream.py
```

### Comparing `flowchat-1.2.1/LICENSE` & `flowchat-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `flowchat-1.2.1/PKG-INFO` & `flowchat-1.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flowchat
-Version: 1.2.1
+Version: 1.2.2
 Summary: Streamlining the process of multi-prompting LLMs with chains
 Home-page: https://github.com/flatypus/flowchat
 Author: Hinson Chan
 Author-email: <yhc3141@gmail.com>
 Maintainer: Hinson Chan
 Maintainer-email: <yhc3141@gmail.com>
 License: MIT
```

### Comparing `flowchat-1.2.1/README.md` & `flowchat-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `flowchat-1.2.1/flowchat/autodedent.py` & `flowchat-1.2.2/flowchat/autodedent.py`

 * *Files identical despite different names*

### Comparing `flowchat-1.2.1/flowchat/chain.py` & `flowchat-1.2.2/flowchat/chain.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,44 +1,24 @@
 from .autodedent import autodedent
 from .private._private_helpers import encode_image, CountStreamTokens
 from .types import *
-from typing import List, Optional, TypedDict, Union, Callable, Dict, Any, Generator
-from typing_extensions import Unpack, NotRequired
+from typing import List, Optional, Union, Callable, Any, Generator
+from typing_extensions import Unpack
 import json
 import logging
 import openai
 import os
 
 
 logging.basicConfig(
     level=logging.WARNING,
     format='[%(asctime)s] %(levelname)s: %(message)s'
 )
 
 
-# use total=False to make fields non-required
-class RequestParams(TypedDict, total=False):
-    model: NotRequired[str]
-    frequency_penalty: NotRequired[Union[float, int]]
-    logit_bias: NotRequired[Dict[str, Union[float, int]]]
-    max_tokens: NotRequired[Union[float, int]]
-    n: NotRequired[Union[float, int]]
-    presence_penalty: NotRequired[Union[float, int]]
-    response_format: NotRequired[ResponseFormat]
-    seed: NotRequired[int]
-    stop: NotRequired[Union[str, List[str]]]
-    temperature: NotRequired[Union[float, int]]
-    top_p: NotRequired[Union[float, int]]
-
-
-class Usage(TypedDict):
-    prompt_tokens: int
-    completion_tokens: int
-
-
 class Chain:
     def __init__(self, model: str, api_key: str = "", environ_key: str = "OPENAI_API_KEY") -> None:
         super().__init__()
 
         if type(model) is not str:
             raise TypeError(
                 f"Model argument must be a string, not {type(model)}"
```

### Comparing `flowchat-1.2.1/flowchat/private/_private_helpers.py` & `flowchat-1.2.2/flowchat/private/_private_helpers.py`

 * *Files identical despite different names*

### Comparing `flowchat-1.2.1/flowchat.egg-info/PKG-INFO` & `flowchat-1.2.2/flowchat.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flowchat
-Version: 1.2.1
+Version: 1.2.2
 Summary: Streamlining the process of multi-prompting LLMs with chains
 Home-page: https://github.com/flatypus/flowchat
 Author: Hinson Chan
 Author-email: <yhc3141@gmail.com>
 Maintainer: Hinson Chan
 Maintainer-email: <yhc3141@gmail.com>
 License: MIT
```

### Comparing `flowchat-1.2.1/setup.py` & `flowchat-1.2.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
-VERSION = '1.2.1'
+VERSION = '1.2.2'
 DESCRIPTION = 'Streamlining the process of multi-prompting LLMs with chains'
 
 setup(
     name="flowchat",
     version=VERSION,
     author="Hinson Chan",
     author_email="<yhc3141@gmail.com>",
```

### Comparing `flowchat-1.2.1/tests/test_autodedent.py` & `flowchat-1.2.2/tests/test_autodedent.py`

 * *Files identical despite different names*

### Comparing `flowchat-1.2.1/tests/test_chaining.py` & `flowchat-1.2.2/tests/test_chaining.py`

 * *Files identical despite different names*

### Comparing `flowchat-1.2.1/tests/test_config.py` & `flowchat-1.2.2/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `flowchat-1.2.1/tests/test_pull.py` & `flowchat-1.2.2/tests/test_pull.py`

 * *Files identical despite different names*

### Comparing `flowchat-1.2.1/tests/test_stream.py` & `flowchat-1.2.2/tests/test_stream.py`

 * *Files identical despite different names*

