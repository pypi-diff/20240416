# Comparing `tmp/flowchat-1.1.4.tar.gz` & `tmp/flowchat-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flowchat-1.1.4.tar", last modified: Sun Apr 14 20:18:45 2024, max compression
+gzip compressed data, was "flowchat-1.2.0.tar", last modified: Tue Apr 16 02:26:16 2024, max compression
```

## Comparing `flowchat-1.1.4.tar` & `flowchat-1.2.0.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 flatypus   (501) staff       (20)        0 2024-04-14 20:18:45.257724 flowchat-1.1.4/
--rw-r--r--   0 flatypus   (501) staff       (20)     1068 2024-03-05 00:02:48.000000 flowchat-1.1.4/LICENSE
--rw-r--r--   0 flatypus   (501) staff       (20)     7676 2024-04-14 20:18:45.257537 flowchat-1.1.4/PKG-INFO
--rw-r--r--   0 flatypus   (501) staff       (20)     6705 2024-04-14 20:10:37.000000 flowchat-1.1.4/README.md
-drwxr-xr-x   0 flatypus   (501) staff       (20)        0 2024-04-14 20:18:45.254590 flowchat-1.1.4/flowchat/
--rw-r--r--   0 flatypus   (501) staff       (20)      185 2024-04-14 20:12:59.000000 flowchat-1.1.4/flowchat/__init__.py
--rw-r--r--   0 flatypus   (501) staff       (20)      590 2024-03-08 00:59:53.000000 flowchat-1.1.4/flowchat/autodedent.py
--rw-r--r--   0 flatypus   (501) staff       (20)    11790 2024-04-14 20:15:39.000000 flowchat-1.1.4/flowchat/chain.py
-drwxr-xr-x   0 flatypus   (501) staff       (20)        0 2024-04-14 20:18:45.255480 flowchat-1.1.4/flowchat/private/
--rw-r--r--   0 flatypus   (501) staff       (20)        0 2023-11-08 02:00:20.000000 flowchat-1.1.4/flowchat/private/__init__.py
--rw-r--r--   0 flatypus   (501) staff       (20)      309 2024-03-08 00:59:53.000000 flowchat-1.1.4/flowchat/private/_private_helpers.py
-drwxr-xr-x   0 flatypus   (501) staff       (20)        0 2024-04-14 20:18:45.257312 flowchat-1.1.4/flowchat.egg-info/
--rw-r--r--   0 flatypus   (501) staff       (20)     7676 2024-04-14 20:18:45.000000 flowchat-1.1.4/flowchat.egg-info/PKG-INFO
--rw-r--r--   0 flatypus   (501) staff       (20)      437 2024-04-14 20:18:45.000000 flowchat-1.1.4/flowchat.egg-info/SOURCES.txt
--rw-r--r--   0 flatypus   (501) staff       (20)        1 2024-04-14 20:18:45.000000 flowchat-1.1.4/flowchat.egg-info/dependency_links.txt
--rw-r--r--   0 flatypus   (501) staff       (20)       44 2024-04-14 20:18:45.000000 flowchat-1.1.4/flowchat.egg-info/requires.txt
--rw-r--r--   0 flatypus   (501) staff       (20)        9 2024-04-14 20:18:45.000000 flowchat-1.1.4/flowchat.egg-info/top_level.txt
--rw-r--r--   0 flatypus   (501) staff       (20)      153 2023-11-25 09:49:08.000000 flowchat-1.1.4/pyproject.toml
--rw-r--r--   0 flatypus   (501) staff       (20)       38 2024-04-14 20:18:45.257765 flowchat-1.1.4/setup.cfg
--rw-r--r--   0 flatypus   (501) staff       (20)     1389 2024-04-14 20:18:18.000000 flowchat-1.1.4/setup.py
-drwxr-xr-x   0 flatypus   (501) staff       (20)        0 2024-04-14 20:18:45.256898 flowchat-1.1.4/tests/
--rw-r--r--   0 flatypus   (501) staff       (20)     2041 2023-11-25 09:35:06.000000 flowchat-1.1.4/tests/test_autodedent.py
--rw-r--r--   0 flatypus   (501) staff       (20)     4106 2024-03-08 00:59:53.000000 flowchat-1.1.4/tests/test_chaining.py
--rw-r--r--   0 flatypus   (501) staff       (20)     1344 2023-11-25 07:32:30.000000 flowchat-1.1.4/tests/test_config.py
--rw-r--r--   0 flatypus   (501) staff       (20)     4796 2024-03-08 00:59:53.000000 flowchat-1.1.4/tests/test_pull.py
--rw-r--r--   0 flatypus   (501) staff       (20)     1214 2023-11-25 10:45:06.000000 flowchat-1.1.4/tests/test_stream.py
+drwxr-xr-x   0 flatypus   (501) staff       (20)        0 2024-04-16 02:26:16.787717 flowchat-1.2.0/
+-rw-r--r--   0 flatypus   (501) staff       (20)     1068 2024-03-05 00:02:48.000000 flowchat-1.2.0/LICENSE
+-rw-r--r--   0 flatypus   (501) staff       (20)     7664 2024-04-16 02:26:16.787505 flowchat-1.2.0/PKG-INFO
+-rw-r--r--   0 flatypus   (501) staff       (20)     6705 2024-04-14 20:10:37.000000 flowchat-1.2.0/README.md
+drwxr-xr-x   0 flatypus   (501) staff       (20)        0 2024-04-16 02:26:16.784116 flowchat-1.2.0/flowchat/
+-rw-r--r--   0 flatypus   (501) staff       (20)      185 2024-04-14 20:12:59.000000 flowchat-1.2.0/flowchat/__init__.py
+-rw-r--r--   0 flatypus   (501) staff       (20)      590 2024-03-08 00:59:53.000000 flowchat-1.2.0/flowchat/autodedent.py
+-rw-r--r--   0 flatypus   (501) staff       (20)    11197 2024-04-16 02:23:59.000000 flowchat-1.2.0/flowchat/chain.py
+drwxr-xr-x   0 flatypus   (501) staff       (20)        0 2024-04-16 02:26:16.785193 flowchat-1.2.0/flowchat/private/
+-rw-r--r--   0 flatypus   (501) staff       (20)        0 2023-11-08 02:00:20.000000 flowchat-1.2.0/flowchat/private/__init__.py
+-rw-r--r--   0 flatypus   (501) staff       (20)     5242 2024-04-16 02:23:27.000000 flowchat-1.2.0/flowchat/private/_private_helpers.py
+-rw-r--r--   0 flatypus   (501) staff       (20)      670 2024-04-15 23:52:59.000000 flowchat-1.2.0/flowchat/types.py
+drwxr-xr-x   0 flatypus   (501) staff       (20)        0 2024-04-16 02:26:16.787219 flowchat-1.2.0/flowchat.egg-info/
+-rw-r--r--   0 flatypus   (501) staff       (20)     7664 2024-04-16 02:26:16.000000 flowchat-1.2.0/flowchat.egg-info/PKG-INFO
+-rw-r--r--   0 flatypus   (501) staff       (20)      455 2024-04-16 02:26:16.000000 flowchat-1.2.0/flowchat.egg-info/SOURCES.txt
+-rw-r--r--   0 flatypus   (501) staff       (20)        1 2024-04-16 02:26:16.000000 flowchat-1.2.0/flowchat.egg-info/dependency_links.txt
+-rw-r--r--   0 flatypus   (501) staff       (20)       32 2024-04-16 02:26:16.000000 flowchat-1.2.0/flowchat.egg-info/requires.txt
+-rw-r--r--   0 flatypus   (501) staff       (20)        9 2024-04-16 02:26:16.000000 flowchat-1.2.0/flowchat.egg-info/top_level.txt
+-rw-r--r--   0 flatypus   (501) staff       (20)      153 2023-11-25 09:49:08.000000 flowchat-1.2.0/pyproject.toml
+-rw-r--r--   0 flatypus   (501) staff       (20)       38 2024-04-16 02:26:16.787773 flowchat-1.2.0/setup.cfg
+-rw-r--r--   0 flatypus   (501) staff       (20)     1391 2024-04-16 02:26:01.000000 flowchat-1.2.0/setup.py
+drwxr-xr-x   0 flatypus   (501) staff       (20)        0 2024-04-16 02:26:16.786661 flowchat-1.2.0/tests/
+-rw-r--r--   0 flatypus   (501) staff       (20)     2041 2023-11-25 09:35:06.000000 flowchat-1.2.0/tests/test_autodedent.py
+-rw-r--r--   0 flatypus   (501) staff       (20)     4250 2024-04-16 02:25:51.000000 flowchat-1.2.0/tests/test_chaining.py
+-rw-r--r--   0 flatypus   (501) staff       (20)     1344 2023-11-25 07:32:30.000000 flowchat-1.2.0/tests/test_config.py
+-rw-r--r--   0 flatypus   (501) staff       (20)     4765 2024-04-15 23:12:53.000000 flowchat-1.2.0/tests/test_pull.py
+-rw-r--r--   0 flatypus   (501) staff       (20)     1214 2023-11-25 10:45:06.000000 flowchat-1.2.0/tests/test_stream.py
```

### Comparing `flowchat-1.1.4/LICENSE` & `flowchat-1.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `flowchat-1.1.4/PKG-INFO` & `flowchat-1.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flowchat
-Version: 1.1.4
+Version: 1.2.0
 Summary: Streamlining the process of multi-prompting LLMs with chains
 Home-page: https://github.com/flatypus/flowchat
 Author: Hinson Chan
 Author-email: <yhc3141@gmail.com>
 Maintainer: Hinson Chan
 Maintainer-email: <yhc3141@gmail.com>
 License: MIT
@@ -15,17 +15,17 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: openai
-Requires-Dist: retry
-Requires-Dist: wrapt_timeout_decorator
 Requires-Dist: Pillow
+Requires-Dist: tiktoken
+Requires-Dist: requests
 
 # flowchat - clean, readable, logical code.
 
 [![PyPI version](https://img.shields.io/pypi/v/flowchat.svg)](https://pypi.org/project/flowchat/)
 [![License](https://img.shields.io/pypi/l/flowchat?logoColor=blue)](LICENSE.txt)
 ![Downloads](https://img.shields.io/pypi/dm/flowchat?logoColor=blue)
```

### Comparing `flowchat-1.1.4/README.md` & `flowchat-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `flowchat-1.1.4/flowchat/autodedent.py` & `flowchat-1.2.0/flowchat/autodedent.py`

 * *Files identical despite different names*

### Comparing `flowchat-1.1.4/flowchat/chain.py` & `flowchat-1.2.0/flowchat/chain.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,23 @@
 from .autodedent import autodedent
-from .private._private_helpers import encode_image
-from PIL.Image import Image as PILImage
-from retry import retry
-from typing import List, Optional, TypedDict, Union, Callable, Dict, Literal, Any, Generator
+from .private._private_helpers import encode_image, CountStreamTokens
+from .types import *
+from typing import List, Optional, TypedDict, Union, Callable, Dict, Any, Generator
 from typing_extensions import Unpack, NotRequired
-from wrapt_timeout_decorator.wrapt_timeout_decorator import timeout
 import json
 import logging
 import openai
 import os
 
+
 logging.basicConfig(
     level=logging.WARNING,
     format='[%(asctime)s] %(levelname)s: %(message)s'
 )
 
-Message = TypedDict('Message', {'role': str, 'content': str | List[Any]})
-ResponseFormat = TypedDict(
-    'ResponseFormat', {'type': Literal['text', 'json_object']})
-ImageFormat = TypedDict('ImageFormat', {
-    'url': str | PILImage,
-    'format_type': str,
-    'detail': Literal['low', 'high']
-})
-
 
 # use total=False to make fields non-required
 class RequestParams(TypedDict, total=False):
     model: NotRequired[str]
     frequency_penalty: NotRequired[Union[float, int]]
     logit_bias: NotRequired[Dict[str, Union[float, int]]]
     max_tokens: NotRequired[Union[float, int]]
@@ -36,14 +26,19 @@
     response_format: NotRequired[ResponseFormat]
     seed: NotRequired[int]
     stop: NotRequired[Union[str, List[str]]]
     temperature: NotRequired[Union[float, int]]
     top_p: NotRequired[Union[float, int]]
 
 
+class Usage(TypedDict):
+    prompt_tokens: int
+    completion_tokens: int
+
+
 class Chain:
     def __init__(self, model: str, api_key: str = "", environ_key: str = "OPENAI_API_KEY") -> None:
         super().__init__()
 
         if type(model) is not str:
             raise TypeError(
                 f"Model argument must be a string, not {type(model)}"
@@ -72,79 +67,78 @@
             )
         openai.api_key = api_key
 
         self.model = model
         self.system: Message | None = None
         self.user_prompt: List[Message] = []
         self.model_response = None
-        self.prompt_tokens = 0
-        self.completion_tokens = 0
-
-    def _query_api(self, function: Callable[[Any], Any], *args: Any, max_query_time: int | None = None, **kwargs: Any) -> Any:
-        """Call the API for max_query_time seconds, and if it times out, it will retry."""
-        timeouted_function = timeout(
-            dec_timeout=max_query_time, use_signals=False)(function)
-        return timeouted_function(*args, **kwargs)
-
-    def _try_query_and_parse(self, function: Callable[[Any], Any], json_schema: Any, *args: Any, max_query_time: int | None = None, stream: bool = False, **kwargs: Any) -> Any:
-        """Query and try to parse the response, and if it fails, it will retry."""
-        completion = self._query_api(
-            function, *args, max_query_time=max_query_time, stream=stream, **kwargs)
-
-        if completion is None:
-            return None
-
-        if stream:
-            return completion
-
-        message = completion.choices[0].message.content
-
-        if not json_schema is None:
-            open_bracket = message.find('{')
-            close_bracket = message.rfind('}')
-            message = message[open_bracket:close_bracket+1]
-            try:
-                message = json.loads(message)
-            except json.JSONDecodeError:
-                raise Exception(
-                    "Response was not in the expected JSON format. Please try again. Check that you haven't accidentally lowered the max_tokens parameter so that the response is truncated."
-                )
-
-        self.prompt_tokens += completion.usage.prompt_tokens
-        self.completion_tokens += completion.usage.completion_tokens
-
-        return message
+        self.usage: Usage = {
+            "prompt_tokens": 0,
+            "completion_tokens": 0
+        }
+
+    def _add_token_count(self, prompt_tokens: int, completion_tokens: int) -> None:
+        """Add token counts to the chain's total token count."""
+        self.usage["prompt_tokens"] += prompt_tokens
+        self.usage["completion_tokens"] += completion_tokens
+
+    def _get_completion(self, **params: Any) -> CreateResponse:
+        """Get a completion from OpenAI's API."""
+        return openai.chat.completions.create(**params)  # type: ignore
 
     def _ask(
         self,
         system: Message | None,
         user_messages: List[Message],
         json_schema: Optional[dict[Any, Any]] = None,
-        max_query_time: Optional[int] = None,
-        tries: int = -1,
         stream: bool = False,
-        **params: Any
+        **params: Unpack[RequestParams]
     ) -> Any:
         """Ask a question to the chatbot with a system prompt and return the response."""
+        model = params.get("model", self.model)
 
         messages = [
             system,
             *user_messages
         ] if system else user_messages
 
-        message = retry(delay=1, logger=logging.getLogger(), tries=tries)(self._try_query_and_parse)(
-            openai.chat.completions.create,  # type: ignore
-            json_schema=json_schema,
-            messages=messages,
-            max_query_time=max_query_time,
-            stream=stream,
-            **params
+        completion = self._get_completion(
+            messages=messages, stream=stream, **params
         )
 
-        return message
+        if completion is None:
+            return None
+
+        if stream and isinstance(completion, Stream):
+            return CountStreamTokens(model, messages).count(completion, self._add_token_count)
+
+        elif isinstance(completion, ChatCompletion):
+            message = completion.choices[0].message.content
+            if message is None:
+                raise Exception("Response was empty. Please try again.")
+
+            if not json_schema is None:
+                open_bracket = message.find('{')
+                close_bracket = message.rfind('}')
+                message = message[open_bracket:close_bracket+1]
+                try:
+                    message = json.loads(message)
+                except json.JSONDecodeError:
+                    raise Exception(
+                        "Response was not in the expected JSON format. Please try again. Check that you haven't accidentally lowered the max_tokens parameter so that the response is truncated."
+                    )
+            print(completion)
+
+            if completion.usage is not None:
+                self._add_token_count(
+                    completion.usage.prompt_tokens,
+                    completion.usage.completion_tokens
+                )
+
+            return message
 
     def _format_images(self, image: str | ImageFormat | Any) -> dict[str, str]:
         """Format whatever image format we receive into the specific format that OpenAI's API expects."""
         if isinstance(image, str):
             return {"url": image}
         elif not isinstance(image, dict):
             # not string or dict so assume PIL image
@@ -235,15 +229,15 @@
                 {"role": role, "content": [
                     {"type": "text", "text": prompt},
                     *images
                 ]}
             )
         return self
 
-    def pull(self, json_schema: Optional[dict[Any, Any]] = None, max_query_time: Optional[int] = None, tries: int = -1, **params: Unpack[RequestParams]) -> 'Chain':
+    def pull(self, json_schema: Optional[dict[Any, Any]] = None, **params: Unpack[RequestParams]) -> 'Chain':
         """Makes a request to the LLM and sets the response."""
 
         params['model'] = params.get('model', self.model)
 
         if len(self.user_prompt) == 0:
             raise ValueError(
                 "User prompt is empty. Please set a user prompt before pulling."
@@ -255,67 +249,65 @@
             self.user_prompt[-1]['content'] += autodedent(
                 "You must respond in the following example JSON format. Remember to enclose the entire JSON object in curly braces:",
                 json.dumps(json_schema, indent=4)
             )
 
         response = self._ask(
             self.system, self.user_prompt,
-            json_schema=json_schema, max_query_time=max_query_time,
-            tries=tries, **params
+            json_schema=json_schema, **params
         )
 
         self.model_response = response
         return self
 
     def stream(
-        self,
-        plain_text_stream: bool = False,
-        max_query_time: Optional[int] = None,
+        self, plain_text_stream: bool = False,
         **params: Unpack[RequestParams]
-
     ) -> Generator[str, None, None]:
         """Returns a generator that yields responses from the LLM."""
         params['model'] = params.get('model', self.model)
 
         if len(self.user_prompt) == 0:
             raise ValueError(
                 "User prompt is empty. Please set a user prompt before pulling."
             )
 
         return (
             response.choices[0].delta.content if plain_text_stream else response
             for response in self._ask(
                 self.system, self.user_prompt,
-                json_schema=None, max_query_time=max_query_time,
+                json_schema=None,
                 stream=True, **params
             )
         )
 
     def last(self) -> Any:
         """Return the chain's last model response."""
         if self.model_response is None:
             raise ValueError(
                 "Model response is empty. Please pull a response before calling last()."
             )
         return self.model_response
 
-    def token_usage(self) -> tuple[int, int]:
+    def token_usage(self) -> Usage:
         """Return the number of tokens used"""
-        return self.prompt_tokens, self.completion_tokens
+        return self.usage
 
     def log(self) -> 'Chain':
         """Log the chain's system prompt, user prompt, and model response."""
         print('='*60)
         print(f"System: {self.system}")
         print(f"User: {self.user_prompt}")
         print(f"Text: {self.model_response}")
         print('='*60)
         print("\n")
         return self
 
     def log_tokens(self) -> 'Chain':
         """Log the number of tokens used"""
-        prompt, completion = self.token_usage()
+        usage = self.token_usage()
+        prompt = usage["prompt_tokens"]
+        completion = usage["completion_tokens"]
         print(f"Prompt tokens: {prompt}")
         print(f"Completion tokens: {completion}")
         print(f"Total tokens: {prompt + completion}")
         return self
```

### Comparing `flowchat-1.1.4/flowchat.egg-info/PKG-INFO` & `flowchat-1.2.0/flowchat.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flowchat
-Version: 1.1.4
+Version: 1.2.0
 Summary: Streamlining the process of multi-prompting LLMs with chains
 Home-page: https://github.com/flatypus/flowchat
 Author: Hinson Chan
 Author-email: <yhc3141@gmail.com>
 Maintainer: Hinson Chan
 Maintainer-email: <yhc3141@gmail.com>
 License: MIT
@@ -15,17 +15,17 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: openai
-Requires-Dist: retry
-Requires-Dist: wrapt_timeout_decorator
 Requires-Dist: Pillow
+Requires-Dist: tiktoken
+Requires-Dist: requests
 
 # flowchat - clean, readable, logical code.
 
 [![PyPI version](https://img.shields.io/pypi/v/flowchat.svg)](https://pypi.org/project/flowchat/)
 [![License](https://img.shields.io/pypi/l/flowchat?logoColor=blue)](LICENSE.txt)
 ![Downloads](https://img.shields.io/pypi/dm/flowchat?logoColor=blue)
```

### Comparing `flowchat-1.1.4/setup.py` & `flowchat-1.2.0/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 from setuptools import setup, find_packages
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
-VERSION = '1.1.4'
+VERSION = '1.2.0'
 DESCRIPTION = 'Streamlining the process of multi-prompting LLMs with chains'
 
 setup(
     name="flowchat",
     version=VERSION,
     author="Hinson Chan",
     author_email="<yhc3141@gmail.com>",
     maintainer="Hinson Chan",
     maintainer_email="<yhc3141@gmail.com>",
     description=DESCRIPTION,
     long_description=long_description,
     long_description_content_type='text/markdown',
     packages=find_packages(),
-    install_requires=["openai", "retry", "wrapt_timeout_decorator", "Pillow"],
+    install_requires=[
+        "openai", "Pillow", "tiktoken", "requests"
+    ],
     setup_requires=['pytest-runner', 'flake8'],
     tests_require=['pytest'],
     classifiers=[
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
         'Programming Language :: Python :: 3',
         'Topic :: Scientific/Engineering :: Artificial Intelligence',
```

### Comparing `flowchat-1.1.4/tests/test_autodedent.py` & `flowchat-1.2.0/tests/test_autodedent.py`

 * *Files identical despite different names*

### Comparing `flowchat-1.1.4/tests/test_chaining.py` & `flowchat-1.2.0/tests/test_chaining.py`

 * *Files 6% similar despite different names*

```diff
@@ -84,24 +84,31 @@
         (Chain(model="gpt-3.5-turbo").link("How are you?").log())
         captured = capsys.readouterr()
         assert captured.out == f"{self.equal_barrier}\nSystem: {None}\nUser: {[{'role': 'user', 'content': 'How are you?'}]}\nText: {None}\n{self.equal_barrier}\n\n\n"
 
     def test_token_usage(self):
         # test that the token_usage method works as expected
         chain = Chain(model="gpt-3.5-turbo")
-        chain.prompt_tokens = 1
-        chain.completion_tokens = 2
+        chain.usage = {
+            "prompt_tokens":  1,
+            "completion_tokens":  2
+        }
         usage = chain.token_usage()
-        assert usage == (1, 2)
+        assert usage == {
+            "prompt_tokens":  1,
+            "completion_tokens":  2
+        }
 
     def test_log_tokens(self, capsys):
         # test that the log_tokens method works as expected
         chain = Chain(model="gpt-3.5-turbo")
-        chain.prompt_tokens = 1
-        chain.completion_tokens = 2
+        chain.usage = {
+            "prompt_tokens":  1,
+            "completion_tokens":  2
+        }
         chain.log_tokens()
         captured = capsys.readouterr()
         assert captured.out == f"Prompt tokens: 1\nCompletion tokens: 2\nTotal tokens: 3\n"
 
     def test_empty_link(self):
         # test that the link method raises a ValueError when called with no arguments
         chain = Chain(model="gpt-3.5-turbo")
```

### Comparing `flowchat-1.1.4/tests/test_config.py` & `flowchat-1.2.0/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `flowchat-1.1.4/tests/test_pull.py` & `flowchat-1.2.0/tests/test_pull.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
         self.chain.pull(model='new-model', max_tokens=100)
         expected_params = {
             'max_tokens': 100,
             'model': 'new-model'
         }
         self.chain._ask.assert_called_with(
             self.chain.system, self.chain.user_prompt,
-            json_schema=None, max_query_time=None, tries=-1,
+            json_schema=None,
             **expected_params
         )
 
     def test_pull_with_json_schema(self):
         with patch('json.dumps') as mock_json_dumps:
             mock_json_dumps.return_value = '{}'
             schema = {'type': 'object'}
```

### Comparing `flowchat-1.1.4/tests/test_stream.py` & `flowchat-1.2.0/tests/test_stream.py`

 * *Files identical despite different names*

