# Comparing `tmp/flowchat-1.2.0.tar.gz` & `tmp/flowchat-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flowchat-1.2.0.tar", last modified: Tue Apr 16 02:26:16 2024, max compression
+gzip compressed data, was "flowchat-1.2.1.tar", last modified: Tue Apr 16 02:45:47 2024, max compression
```

## Comparing `flowchat-1.2.0.tar` & `flowchat-1.2.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 flatypus   (501) staff       (20)        0 2024-04-16 02:26:16.787717 flowchat-1.2.0/
--rw-r--r--   0 flatypus   (501) staff       (20)     1068 2024-03-05 00:02:48.000000 flowchat-1.2.0/LICENSE
--rw-r--r--   0 flatypus   (501) staff       (20)     7664 2024-04-16 02:26:16.787505 flowchat-1.2.0/PKG-INFO
--rw-r--r--   0 flatypus   (501) staff       (20)     6705 2024-04-14 20:10:37.000000 flowchat-1.2.0/README.md
-drwxr-xr-x   0 flatypus   (501) staff       (20)        0 2024-04-16 02:26:16.784116 flowchat-1.2.0/flowchat/
--rw-r--r--   0 flatypus   (501) staff       (20)      185 2024-04-14 20:12:59.000000 flowchat-1.2.0/flowchat/__init__.py
--rw-r--r--   0 flatypus   (501) staff       (20)      590 2024-03-08 00:59:53.000000 flowchat-1.2.0/flowchat/autodedent.py
--rw-r--r--   0 flatypus   (501) staff       (20)    11197 2024-04-16 02:23:59.000000 flowchat-1.2.0/flowchat/chain.py
-drwxr-xr-x   0 flatypus   (501) staff       (20)        0 2024-04-16 02:26:16.785193 flowchat-1.2.0/flowchat/private/
--rw-r--r--   0 flatypus   (501) staff       (20)        0 2023-11-08 02:00:20.000000 flowchat-1.2.0/flowchat/private/__init__.py
--rw-r--r--   0 flatypus   (501) staff       (20)     5242 2024-04-16 02:23:27.000000 flowchat-1.2.0/flowchat/private/_private_helpers.py
--rw-r--r--   0 flatypus   (501) staff       (20)      670 2024-04-15 23:52:59.000000 flowchat-1.2.0/flowchat/types.py
-drwxr-xr-x   0 flatypus   (501) staff       (20)        0 2024-04-16 02:26:16.787219 flowchat-1.2.0/flowchat.egg-info/
--rw-r--r--   0 flatypus   (501) staff       (20)     7664 2024-04-16 02:26:16.000000 flowchat-1.2.0/flowchat.egg-info/PKG-INFO
--rw-r--r--   0 flatypus   (501) staff       (20)      455 2024-04-16 02:26:16.000000 flowchat-1.2.0/flowchat.egg-info/SOURCES.txt
--rw-r--r--   0 flatypus   (501) staff       (20)        1 2024-04-16 02:26:16.000000 flowchat-1.2.0/flowchat.egg-info/dependency_links.txt
--rw-r--r--   0 flatypus   (501) staff       (20)       32 2024-04-16 02:26:16.000000 flowchat-1.2.0/flowchat.egg-info/requires.txt
--rw-r--r--   0 flatypus   (501) staff       (20)        9 2024-04-16 02:26:16.000000 flowchat-1.2.0/flowchat.egg-info/top_level.txt
--rw-r--r--   0 flatypus   (501) staff       (20)      153 2023-11-25 09:49:08.000000 flowchat-1.2.0/pyproject.toml
--rw-r--r--   0 flatypus   (501) staff       (20)       38 2024-04-16 02:26:16.787773 flowchat-1.2.0/setup.cfg
--rw-r--r--   0 flatypus   (501) staff       (20)     1391 2024-04-16 02:26:01.000000 flowchat-1.2.0/setup.py
-drwxr-xr-x   0 flatypus   (501) staff       (20)        0 2024-04-16 02:26:16.786661 flowchat-1.2.0/tests/
--rw-r--r--   0 flatypus   (501) staff       (20)     2041 2023-11-25 09:35:06.000000 flowchat-1.2.0/tests/test_autodedent.py
--rw-r--r--   0 flatypus   (501) staff       (20)     4250 2024-04-16 02:25:51.000000 flowchat-1.2.0/tests/test_chaining.py
--rw-r--r--   0 flatypus   (501) staff       (20)     1344 2023-11-25 07:32:30.000000 flowchat-1.2.0/tests/test_config.py
--rw-r--r--   0 flatypus   (501) staff       (20)     4765 2024-04-15 23:12:53.000000 flowchat-1.2.0/tests/test_pull.py
--rw-r--r--   0 flatypus   (501) staff       (20)     1214 2023-11-25 10:45:06.000000 flowchat-1.2.0/tests/test_stream.py
+drwxr-xr-x   0 flatypus   (501) staff       (20)        0 2024-04-16 02:45:47.553590 flowchat-1.2.1/
+-rw-r--r--   0 flatypus   (501) staff       (20)     1068 2024-03-05 00:02:48.000000 flowchat-1.2.1/LICENSE
+-rw-r--r--   0 flatypus   (501) staff       (20)     7664 2024-04-16 02:45:47.553359 flowchat-1.2.1/PKG-INFO
+-rw-r--r--   0 flatypus   (501) staff       (20)     6705 2024-04-14 20:10:37.000000 flowchat-1.2.1/README.md
+drwxr-xr-x   0 flatypus   (501) staff       (20)        0 2024-04-16 02:45:47.549507 flowchat-1.2.1/flowchat/
+-rw-r--r--   0 flatypus   (501) staff       (20)      185 2024-04-16 02:26:44.000000 flowchat-1.2.1/flowchat/__init__.py
+-rw-r--r--   0 flatypus   (501) staff       (20)      590 2024-03-08 00:59:53.000000 flowchat-1.2.1/flowchat/autodedent.py
+-rw-r--r--   0 flatypus   (501) staff       (20)    11213 2024-04-16 02:44:33.000000 flowchat-1.2.1/flowchat/chain.py
+drwxr-xr-x   0 flatypus   (501) staff       (20)        0 2024-04-16 02:45:47.550834 flowchat-1.2.1/flowchat/private/
+-rw-r--r--   0 flatypus   (501) staff       (20)        0 2023-11-08 02:00:20.000000 flowchat-1.2.1/flowchat/private/__init__.py
+-rw-r--r--   0 flatypus   (501) staff       (20)     5258 2024-04-16 02:44:33.000000 flowchat-1.2.1/flowchat/private/_private_helpers.py
+-rw-r--r--   0 flatypus   (501) staff       (20)      670 2024-04-16 02:44:31.000000 flowchat-1.2.1/flowchat/types.py
+drwxr-xr-x   0 flatypus   (501) staff       (20)        0 2024-04-16 02:45:47.553045 flowchat-1.2.1/flowchat.egg-info/
+-rw-r--r--   0 flatypus   (501) staff       (20)     7664 2024-04-16 02:45:47.000000 flowchat-1.2.1/flowchat.egg-info/PKG-INFO
+-rw-r--r--   0 flatypus   (501) staff       (20)      455 2024-04-16 02:45:47.000000 flowchat-1.2.1/flowchat.egg-info/SOURCES.txt
+-rw-r--r--   0 flatypus   (501) staff       (20)        1 2024-04-16 02:45:47.000000 flowchat-1.2.1/flowchat.egg-info/dependency_links.txt
+-rw-r--r--   0 flatypus   (501) staff       (20)       32 2024-04-16 02:45:47.000000 flowchat-1.2.1/flowchat.egg-info/requires.txt
+-rw-r--r--   0 flatypus   (501) staff       (20)        9 2024-04-16 02:45:47.000000 flowchat-1.2.1/flowchat.egg-info/top_level.txt
+-rw-r--r--   0 flatypus   (501) staff       (20)      153 2023-11-25 09:49:08.000000 flowchat-1.2.1/pyproject.toml
+-rw-r--r--   0 flatypus   (501) staff       (20)       38 2024-04-16 02:45:47.553647 flowchat-1.2.1/setup.cfg
+-rw-r--r--   0 flatypus   (501) staff       (20)     1391 2024-04-16 02:45:36.000000 flowchat-1.2.1/setup.py
+drwxr-xr-x   0 flatypus   (501) staff       (20)        0 2024-04-16 02:45:47.552482 flowchat-1.2.1/tests/
+-rw-r--r--   0 flatypus   (501) staff       (20)     2041 2023-11-25 09:35:06.000000 flowchat-1.2.1/tests/test_autodedent.py
+-rw-r--r--   0 flatypus   (501) staff       (20)     4250 2024-04-16 02:44:31.000000 flowchat-1.2.1/tests/test_chaining.py
+-rw-r--r--   0 flatypus   (501) staff       (20)     1344 2023-11-25 07:32:30.000000 flowchat-1.2.1/tests/test_config.py
+-rw-r--r--   0 flatypus   (501) staff       (20)     4765 2024-04-16 02:44:31.000000 flowchat-1.2.1/tests/test_pull.py
+-rw-r--r--   0 flatypus   (501) staff       (20)     1214 2023-11-25 10:45:06.000000 flowchat-1.2.1/tests/test_stream.py
```

### Comparing `flowchat-1.2.0/LICENSE` & `flowchat-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `flowchat-1.2.0/PKG-INFO` & `flowchat-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flowchat
-Version: 1.2.0
+Version: 1.2.1
 Summary: Streamlining the process of multi-prompting LLMs with chains
 Home-page: https://github.com/flatypus/flowchat
 Author: Hinson Chan
 Author-email: <yhc3141@gmail.com>
 Maintainer: Hinson Chan
 Maintainer-email: <yhc3141@gmail.com>
 License: MIT
```

### Comparing `flowchat-1.2.0/README.md` & `flowchat-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `flowchat-1.2.0/flowchat/autodedent.py` & `flowchat-1.2.1/flowchat/autodedent.py`

 * *Files identical despite different names*

### Comparing `flowchat-1.2.0/flowchat/chain.py` & `flowchat-1.2.1/flowchat/chain.py`

 * *Files 0% similar despite different names*

```diff
@@ -105,15 +105,15 @@
             messages=messages, stream=stream, **params
         )
 
         if completion is None:
             return None
 
         if stream and isinstance(completion, Stream):
-            return CountStreamTokens(model, messages).count(completion, self._add_token_count)
+            return CountStreamTokens(model, messages).wrap_stream_and_count(completion, self._add_token_count)
 
         elif isinstance(completion, ChatCompletion):
             message = completion.choices[0].message.content
             if message is None:
                 raise Exception("Response was empty. Please try again.")
 
             if not json_schema is None:
```

### Comparing `flowchat-1.2.0/flowchat/private/_private_helpers.py` & `flowchat-1.2.1/flowchat/private/_private_helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -130,15 +130,15 @@
         tokens += 3  # every reply is primed with <|start|>assistant<|message|>
 
         return tokens
 
     def _count_output_tokens(self, message: str):
         return len(self.encoding.encode(message))
 
-    def count(self, generator: StreamChatCompletion, callback: Callable[[int, int], None]):
+    def wrap_stream_and_count(self, generator: StreamChatCompletion, callback: Callable[[int, int], None]):
         for response in generator:
             content = response.choices[0].delta.content
             yield response
 
             if content is None:
                 output_message = "".join(self.collect_tokens)
                 prompt_tokens = self._count_input_tokens()
```

### Comparing `flowchat-1.2.0/flowchat/types.py` & `flowchat-1.2.1/flowchat/types.py`

 * *Files identical despite different names*

### Comparing `flowchat-1.2.0/flowchat.egg-info/PKG-INFO` & `flowchat-1.2.1/flowchat.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flowchat
-Version: 1.2.0
+Version: 1.2.1
 Summary: Streamlining the process of multi-prompting LLMs with chains
 Home-page: https://github.com/flatypus/flowchat
 Author: Hinson Chan
 Author-email: <yhc3141@gmail.com>
 Maintainer: Hinson Chan
 Maintainer-email: <yhc3141@gmail.com>
 License: MIT
```

### Comparing `flowchat-1.2.0/setup.py` & `flowchat-1.2.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
-VERSION = '1.2.0'
+VERSION = '1.2.1'
 DESCRIPTION = 'Streamlining the process of multi-prompting LLMs with chains'
 
 setup(
     name="flowchat",
     version=VERSION,
     author="Hinson Chan",
     author_email="<yhc3141@gmail.com>",
```

### Comparing `flowchat-1.2.0/tests/test_autodedent.py` & `flowchat-1.2.1/tests/test_autodedent.py`

 * *Files identical despite different names*

### Comparing `flowchat-1.2.0/tests/test_chaining.py` & `flowchat-1.2.1/tests/test_chaining.py`

 * *Files identical despite different names*

### Comparing `flowchat-1.2.0/tests/test_config.py` & `flowchat-1.2.1/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `flowchat-1.2.0/tests/test_pull.py` & `flowchat-1.2.1/tests/test_pull.py`

 * *Files identical despite different names*

### Comparing `flowchat-1.2.0/tests/test_stream.py` & `flowchat-1.2.1/tests/test_stream.py`

 * *Files identical despite different names*

