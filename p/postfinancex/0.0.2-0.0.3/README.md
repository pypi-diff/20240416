# Comparing `tmp/postfinancex-0.0.2.tar.gz` & `tmp/postfinancex-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "postfinancex-0.0.2.tar", max compression
+gzip compressed data, was "postfinancex-0.0.3.tar", max compression
```

## Comparing `postfinancex-0.0.2.tar` & `postfinancex-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,15 @@
--rw-r--r--   0        0        0     1494 2024-04-12 16:26:18.496679 postfinancex-0.0.2/LICENSE
--rw-r--r--   0        0        0      923 2024-04-13 15:10:41.269686 postfinancex-0.0.2/README.md
--rw-r--r--   0        0        0      222 2024-04-16 00:54:00.166029 postfinancex-0.0.2/postfinance/__init__.py
--rw-r--r--   0        0        0     3426 2024-04-16 03:31:21.698476 postfinancex-0.0.2/postfinance/agents.py
--rw-r--r--   0        0        0        0 2024-04-15 09:30:16.578796 postfinancex-0.0.2/postfinance/langchain/__init__.py
--rw-r--r--   0        0        0     2599 2024-04-15 00:18:14.909252 postfinancex-0.0.2/postfinance/langchain/embeddings.py
--rw-r--r--   0        0        0        0 2024-04-16 01:02:12.975627 postfinancex-0.0.2/postfinance/langchain/llms.py
--rw-r--r--   0        0        0     4721 2024-04-14 13:46:39.816449 postfinancex-0.0.2/postfinance/langchain/storage.py
--rw-r--r--   0        0        0       59 2024-04-14 14:24:09.328883 postfinancex-0.0.2/postfinance/langchain/vectorstores.py
--rw-r--r--   0        0        0     3653 2024-04-16 00:52:55.886409 postfinancex-0.0.2/postfinance/models.py
--rw-r--r--   0        0        0     8047 2024-04-16 02:32:25.644407 postfinancex-0.0.2/postfinance/output_parsers.py
--rw-r--r--   0        0        0    16768 2024-04-16 00:29:23.895001 postfinancex-0.0.2/postfinance/prompts.py
--rw-r--r--   0        0        0      564 2024-04-16 03:27:27.442524 postfinancex-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     1533 1970-01-01 00:00:00.000000 postfinancex-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1494 2024-04-12 16:26:18.496679 postfinancex-0.0.3/LICENSE
+-rw-r--r--   0        0        0      923 2024-04-16 17:38:59.033315 postfinancex-0.0.3/README.md
+-rw-r--r--   0        0        0      222 2024-04-16 00:54:00.166029 postfinancex-0.0.3/postfinance/__init__.py
+-rw-r--r--   0        0        0     5326 2024-04-16 17:06:55.783461 postfinancex-0.0.3/postfinance/agents.py
+-rw-r--r--   0        0        0     2094 2024-04-16 16:27:34.174963 postfinancex-0.0.3/postfinance/input_parsers.py
+-rw-r--r--   0        0        0        0 2024-04-15 09:30:16.578796 postfinancex-0.0.3/postfinance/langchain/__init__.py
+-rw-r--r--   0        0        0     2599 2024-04-15 00:18:14.909252 postfinancex-0.0.3/postfinance/langchain/embeddings.py
+-rw-r--r--   0        0        0        0 2024-04-16 01:02:12.975627 postfinancex-0.0.3/postfinance/langchain/llms.py
+-rw-r--r--   0        0        0     4721 2024-04-14 13:46:39.816449 postfinancex-0.0.3/postfinance/langchain/storage.py
+-rw-r--r--   0        0        0       59 2024-04-14 14:24:09.328883 postfinancex-0.0.3/postfinance/langchain/vectorstores.py
+-rw-r--r--   0        0        0     3716 2024-04-16 17:16:08.729777 postfinancex-0.0.3/postfinance/models.py
+-rw-r--r--   0        0        0     6790 2024-04-16 15:55:57.740472 postfinancex-0.0.3/postfinance/output_parsers.py
+-rw-r--r--   0        0        0    14430 2024-04-16 17:15:12.175360 postfinancex-0.0.3/postfinance/prompts.py
+-rw-r--r--   0        0        0      667 2024-04-16 17:36:22.921913 postfinancex-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     1721 1970-01-01 00:00:00.000000 postfinancex-0.0.3/PKG-INFO
```

### Comparing `postfinancex-0.0.2/LICENSE` & `postfinancex-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `postfinancex-0.0.2/README.md` & `postfinancex-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `postfinancex-0.0.2/postfinance/langchain/embeddings.py` & `postfinancex-0.0.3/postfinance/langchain/embeddings.py`

 * *Files identical despite different names*

### Comparing `postfinancex-0.0.2/postfinance/langchain/storage.py` & `postfinancex-0.0.3/postfinance/langchain/storage.py`

 * *Files identical despite different names*

### Comparing `postfinancex-0.0.2/postfinance/models.py` & `postfinancex-0.0.3/postfinance/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     api_key: str = "lHMtCMCF5jiwPqgFPeOCDsqoUU4Rm_vIuqSXJmjgIXSQ",
     url: str = "https://us-south.ml.cloud.ibm.com",
     project_id: str = "38a37d7d-4ab7-4349-935c-936add66c7f5",
 ) -> Model:
     if model not in list_supported_models(task):
         raise ValueError(f'Unsupported model: "{model}" for task "{task}"')
     params = params or get_default_params()
+    print(params)
     return Model(
         model_id=model,
         params=params,
         credentials={
             "apikey": api_key,
             "url": url,
         },
@@ -54,15 +55,16 @@
             ModelTypes.MIXTRAL_8X7B_INSTRUCT_V01_Q.value,
             # ModelTypes.LLAMA_2_70B_CHAT.value,
         ]
     if task == TaskTypes.CHAT.value or task == TaskTypes.CHAT:
         return [
             "mistralai/mixtral-8x7b-instruct-v01",
             ModelTypes.MIXTRAL_8X7B_INSTRUCT_V01_Q.value,
-            # ModelTypes.LLAMA_2_70B_CHAT.value,
+            ModelTypes.LLAMA_2_70B_CHAT.value,
+            ModelTypes.LLAMA_2_13B_CHAT.value,
         ]
     raise ValueError(f'Unsupported task: "{task}"')
 
 
 def get_default_params() -> Dict[str, Any]:
     """Get default model parameters.
 
@@ -86,15 +88,15 @@
 
     Reference:
         [1] https://ibm.github.io/watsonx-ai-python-sdk/fm_model.html#metanames.GenTextParamsMetaNames
         [2] https://dataplatform.cloud.ibm.com/docs/content/wsj/analyze-data/fm-model-parameters.html?context=wx
     """
     return {
         GenTextParamsMetaNames.DECODING_METHOD: "sample",
-        GenTextParamsMetaNames.TEMPERATURE: 0.1,
+        GenTextParamsMetaNames.TEMPERATURE: 0.0,
         GenTextParamsMetaNames.TOP_P: 1.0,
         GenTextParamsMetaNames.TOP_K: 50,
         GenTextParamsMetaNames.RANDOM_SEED: 42,
         GenTextParamsMetaNames.REPETITION_PENALTY: 1.0,
         GenTextParamsMetaNames.MIN_NEW_TOKENS: 0,
         GenTextParamsMetaNames.MAX_NEW_TOKENS: 1000,
     }
```

### Comparing `postfinancex-0.0.2/postfinance/output_parsers.py` & `postfinancex-0.0.3/postfinance/output_parsers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,78 +1,29 @@
 import json
 import re
 from typing import Callable
 
+from .input_parsers import (
+    NO_MATCH,
+    _transcript_markdown_to_json,
+    _transcript_markdown_to_text,
+)
 from .models import TaskTypes
 
-NO_MATCH = "NO MATCH"
-
 
 def get_output_parser(task: str | TaskTypes) -> Callable:
     if task == TaskTypes.TRANSLATION.value or task == TaskTypes.TRANSLATION:
         return translation_json_output_parser
     if task == TaskTypes.ANNOTATION.value or task == TaskTypes.ANNOTATION:
         return annotation_json_output_parser
+    if task == TaskTypes.CHAT.value or task == TaskTypes.CHAT:
+        return chat_str_output_parser
     raise ValueError(f'Unsupported task: "{task}"')
 
 
-def _transcript_to_markdown(transcript: str) -> str:
-    return transcript
-
-
-def _transcript_markdown_to_text(markdown: str) -> str:
-    # Remove Markdown bold formatting with double asterisks (**)
-    text = re.sub(r"\*\*(.*?)\*\*", r"\1", markdown)
-    # Remove empty lines
-    text = "\n".join(
-        [line.strip() for line in text.split("\n") if line.strip() != ""]
-    )
-    return text
-
-
-def _transcript_markdown_to_json(
-    markdown: str,
-    dumps: bool = False,
-) -> dict | str:
-    # Pattern to find the title enclosed in double asterisks (**)
-    title_pattern = r"\*\*(.*)\*\*\n"
-    # Pattern to find the dialogue
-    dialogue_pattern = r"\n\*\*(.*?):\*\* \"(.*?)\""
-
-    title_match = re.search(title_pattern, markdown, re.DOTALL)
-    dialogue = re.findall(dialogue_pattern, markdown, re.S)
-
-    title = title_match.group(1).strip() if title_match else NO_MATCH
-    dialogue = [
-        {"role": role.strip(), "content": content.strip()}
-        for role, content in dialogue
-    ]
-
-    data = {
-        "title": title,
-        "dialogue": dialogue,
-    }
-    return json.dumps(data, indent=4) if dumps else data
-
-
-def transcript_json_input_parser(
-    input: str,
-    dumps: bool = False,
-) -> dict | str:
-    markdown = _transcript_to_markdown(input)
-    data = {
-        "transcript": {
-            "markdown": markdown,
-            "text": _transcript_markdown_to_text(markdown),
-            "json": _transcript_markdown_to_json(markdown),
-        },
-    }
-    return json.dumps(data, indent=4) if dumps else data
-
-
 def _unblock(output: str) -> str:
     # Pattern to find the output enclosed in triple backticks (```)
     pattern = r"```(.*?)```"
     match = re.search(pattern, output, re.DOTALL)
     return match.group(1).strip() if match else NO_MATCH
 
 
@@ -246,7 +197,11 @@
         "summary": summary,
         "annotation": {
             "markdown": _annotation_to_markdown(annotation),
             "json": _annotation_to_json(annotation),
         },
     }
     return json.dumps(data, indent=4) if dumps else data
+
+
+def chat_str_output_parser(output: str, dumps: bool = False) -> str:
+    return output
```

### Comparing `postfinancex-0.0.2/postfinance/prompts.py` & `postfinancex-0.0.3/postfinance/prompts.py`

 * *Files 13% similar despite different names*

```diff
@@ -176,71 +176,37 @@
 Transcipt:
 ```
 {content}
 ```
 
 Output:"""
 
-
-CHAT_PROMPT_TEMPLATE = """You are a virtual assistant. Given the following transcript and the current conversation between a user and the assistant, answer any user query by using information from the transcript. The response should be detailed and cite the related content in the transcript.
+# TODO: Optimize the prompt template for chat task
+# https://dataplatform.cloud.ibm.com/docs/content/wsj/analyze-data/fm-prompt-samples.html?context=wx&audience=wdp#dialog
+CHAT_PROMPT_TEMPLATE = """You are a virtual assistant. Given the following transcript and the conversation history between a user and the assistant, your task is to answer any user query according to the information from the transcript. Your response should be detailed and cite the related content in the transcript. Citation should be enclosed within the round brakets following the response.
 
 Transcript:
 ```
-**Script 01 - Inquiry About Fees and Interest on Account Statements**
-
-**Call-Center Employee (CCE):** "Hello, this is [Employee Name] from [Bank Name] Customer Service. How can I help you today?"
-
-**Customer (C):** "Hello, I'm [Customer Name]. I've reviewed my account statement and I have some questions about the fees and interest that are listed."
-
-**CCE:** "Sure, I can certainly help you with that. Could you please give me your account number and your date of birth so I can verify your identity and check your account?"
-
-**C:** "Of course, my account number is [Number] and my birthdate is [Date]. It’s specifically about a few fees that I don’t quite understand."
-
-**CCE:** "Okay, let me take a look at that. One moment please... Alright, I have your account open now. Can you tell me which fees you are referring to?"
-
-**C:** "There is a fee listed with the title 'Account Management Fee' and another one called 'Overdraft Interest.' I thought that I didn’t have any fees, and I don’t understand what the overdraft interest is."
-
-**CCE:** "I can explain that. The account management fee is a standardized fee that we charge for the administration of your account. The amount of this fee can vary depending on your account model. As for the overdraft interest: this is an interest we charge if you spend more money than is available in your account, so if you overdraw your account."
-
-**C:** "Ah, that makes sense. But I am actually quite sure that I never spent more than what was in my account."
-
-**CCE:** "I can check that again for you. One moment please... Yes, I see there was a brief moment when your account was slightly overdrawn. That could explain the overdraft interest."
-
-**C:** "Okay, I must have overlooked that. And can I do something to avoid these fees?"
-
-**CCE:** "For the account management fee, if you want an account model with lower or no fees, we could talk about switching accounts. For the overdraft interest, I recommend you regularly check your account and make sure there is enough money available before making larger expenses."
-
-**C:** "That sounds reasonable. I will think about switching accounts. Can you send me information about the different account models?"
-
-**CCE:** "Certainly, I can send you an overview by email. Is your email address up to date with us?"
-
-**C:** "Yes, it is. Thank you for your help and explanations."
-
-**CCE:** "I'm glad I could help. I will send you the information right away. If there is anything else, we are here for you. Have a nice day, [Customer Name]!"
-
-**C:** "Thank you, you too. Goodbye."
-
-**CCE:** "Goodbye!"
+{content}
 ```
 
-Dialogue: 
-```
+Dialogue:
 Assistant: How could I help you?
+
 User: How to avoid account management fees?
+
 Assistant: To avoid account management fees, you may consider switching to a different account model that may have lower or no fees associated with it ("For the account management fee, if you want an account model with lower or no fees, we could talk about switching accounts").
+
 User: What is the overdraft interest?
+
 Assistant: The overdraft interest is an interest charge applied when you spend more money than is available in your account, essentially when your account balance goes negative ("As for the overdraft interest: this is an interest we charge if you spend more money than is available in your account, so if you overdraw your account").
-```
 
-Transcript:
-```
-{content}
-```
+{dialogue}
 
-Answer:
+Assistant:
 """
 
 
 def get_prompt(task: str | TaskTypes, **kwargs) -> str:
     if task == TaskTypes.TRANSLATION.value or task == TaskTypes.TRANSLATION:
         return TRANSLATE_PROMPT_TEMPLATE.format(**kwargs)
     if task == TaskTypes.ANNOTATION.value or task == TaskTypes.ANNOTATION:
```

### Comparing `postfinancex-0.0.2/pyproject.toml` & `postfinancex-0.0.3/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 [tool.poetry]
 name = "postfinancex"
-version = "0.0.2"
-description = "🤖 PostFinance LLM agent powered by IBM watsonx.ai ✨ PostFinance X IBM watsonx.ai"
+version = "0.0.3"
+description = "PostFinanceX Virtual Assistant powered by IBM watsonx.ai ✨ PostFinance X IBM watsonx.ai"
 packages = [
     {include = "postfinance"}
 ]
 authors = ["Yi ZHANG <yizhang.dev@gmail.com>"]
 license = "BSD-3-Clause"
 readme = "README.md"
 homepage = "https://pypi.org/project/postfinancex"
 repository = "https://github.com/imyizhang/postfinancex"
 
 [tool.poetry.dependencies]
 python = "^3.12"
 ibm-watsonx-ai = "^0.2.4"
+pymongo = "^4.6.3"
+dnspython = "^2.6.1"
+langchain-community = "^0.0.33"
+langchain-core = "^0.1.43"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `postfinancex-0.0.2/PKG-INFO` & `postfinancex-0.0.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,20 +1,24 @@
 Metadata-Version: 2.1
 Name: postfinancex
-Version: 0.0.2
-Summary: 🤖 PostFinance LLM agent powered by IBM watsonx.ai ✨ PostFinance X IBM watsonx.ai
+Version: 0.0.3
+Summary: PostFinanceX Virtual Assistant powered by IBM watsonx.ai ✨ PostFinance X IBM watsonx.ai
 Home-page: https://pypi.org/project/postfinancex
 License: BSD-3-Clause
 Author: Yi ZHANG
 Author-email: yizhang.dev@gmail.com
 Requires-Python: >=3.12,<4.0
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.12
+Requires-Dist: dnspython (>=2.6.1,<3.0.0)
 Requires-Dist: ibm-watsonx-ai (>=0.2.4,<0.3.0)
+Requires-Dist: langchain-community (>=0.0.33,<0.0.34)
+Requires-Dist: langchain-core (>=0.1.43,<0.2.0)
+Requires-Dist: pymongo (>=4.6.3,<5.0.0)
 Project-URL: Repository, https://github.com/imyizhang/postfinancex
 Description-Content-Type: text/markdown
 
 # PostFinanceX
 
 [![GitHub][github_badge]][github_link] [![PyPI][pypi_badge]][pypi_link]
```

