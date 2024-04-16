# Comparing `tmp/postfinancex-0.0.1.tar.gz` & `tmp/postfinancex-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "postfinancex-0.0.1.tar", max compression
+gzip compressed data, was "postfinancex-0.0.2.tar", max compression
```

## Comparing `postfinancex-0.0.1.tar` & `postfinancex-0.0.2.tar`

### file list

```diff
@@ -1,8 +1,14 @@
--rw-r--r--   0        0        0     1494 2024-04-12 16:26:18.496679 postfinancex-0.0.1/LICENSE
--rw-r--r--   0        0        0      923 2024-04-13 15:10:41.269686 postfinancex-0.0.1/README.md
--rw-r--r--   0        0        0       47 2024-04-12 15:27:47.839565 postfinancex-0.0.1/postfinance/__init__.py
--rw-r--r--   0        0        0     1456 2024-04-13 14:54:45.220013 postfinancex-0.0.1/postfinance/agent.py
--rw-r--r--   0        0        0     3215 2024-04-13 14:08:02.821552 postfinancex-0.0.1/postfinance/models.py
--rw-r--r--   0        0        0    15614 2024-04-13 14:31:39.411708 postfinancex-0.0.1/postfinance/prompts.py
--rw-r--r--   0        0        0      564 2024-04-12 17:09:50.766904 postfinancex-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     1533 1970-01-01 00:00:00.000000 postfinancex-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0     1494 2024-04-12 16:26:18.496679 postfinancex-0.0.2/LICENSE
+-rw-r--r--   0        0        0      923 2024-04-13 15:10:41.269686 postfinancex-0.0.2/README.md
+-rw-r--r--   0        0        0      222 2024-04-16 00:54:00.166029 postfinancex-0.0.2/postfinance/__init__.py
+-rw-r--r--   0        0        0     3426 2024-04-16 03:31:21.698476 postfinancex-0.0.2/postfinance/agents.py
+-rw-r--r--   0        0        0        0 2024-04-15 09:30:16.578796 postfinancex-0.0.2/postfinance/langchain/__init__.py
+-rw-r--r--   0        0        0     2599 2024-04-15 00:18:14.909252 postfinancex-0.0.2/postfinance/langchain/embeddings.py
+-rw-r--r--   0        0        0        0 2024-04-16 01:02:12.975627 postfinancex-0.0.2/postfinance/langchain/llms.py
+-rw-r--r--   0        0        0     4721 2024-04-14 13:46:39.816449 postfinancex-0.0.2/postfinance/langchain/storage.py
+-rw-r--r--   0        0        0       59 2024-04-14 14:24:09.328883 postfinancex-0.0.2/postfinance/langchain/vectorstores.py
+-rw-r--r--   0        0        0     3653 2024-04-16 00:52:55.886409 postfinancex-0.0.2/postfinance/models.py
+-rw-r--r--   0        0        0     8047 2024-04-16 02:32:25.644407 postfinancex-0.0.2/postfinance/output_parsers.py
+-rw-r--r--   0        0        0    16768 2024-04-16 00:29:23.895001 postfinancex-0.0.2/postfinance/prompts.py
+-rw-r--r--   0        0        0      564 2024-04-16 03:27:27.442524 postfinancex-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     1533 1970-01-01 00:00:00.000000 postfinancex-0.0.2/PKG-INFO
```

### Comparing `postfinancex-0.0.1/LICENSE` & `postfinancex-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `postfinancex-0.0.1/README.md` & `postfinancex-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `postfinancex-0.0.1/postfinance/models.py` & `postfinancex-0.0.2/postfinance/models.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,54 +1,74 @@
-from typing import List
+from enum import Enum
+from typing import Any, Dict, List, Optional
 
 from ibm_watsonx_ai.foundation_models import Model
-from ibm_watsonx_ai.foundation_models.utils.enums import (
-    DecodingMethods,
-    ModelTypes,
-)
+from ibm_watsonx_ai.foundation_models.utils.enums import ModelTypes
 from ibm_watsonx_ai.metanames import GenTextParamsMetaNames
 
 
-def list_models(task: str) -> List[str]:
-    """List supported models.
+class TaskTypes(Enum):
+
+    TRANSLATION = "translation"
+    ANNOTATION = "annotation"
+    CHAT = "chat"
+
+
+def get_model(
+    task: str | TaskTypes,
+    model: str,
+    params: Optional[Dict[str, Any]] = None,
+    api_key: str = "lHMtCMCF5jiwPqgFPeOCDsqoUU4Rm_vIuqSXJmjgIXSQ",
+    url: str = "https://us-south.ml.cloud.ibm.com",
+    project_id: str = "38a37d7d-4ab7-4349-935c-936add66c7f5",
+) -> Model:
+    if model not in list_supported_models(task):
+        raise ValueError(f'Unsupported model: "{model}" for task "{task}"')
+    params = params or get_default_params()
+    return Model(
+        model_id=model,
+        params=params,
+        credentials={
+            "apikey": api_key,
+            "url": url,
+        },
+        project_id=project_id,
+    )
+
+
+def list_supported_models(task: str | TaskTypes) -> List[str]:
+    """List supported models for a specific task.
 
     Reference:
         [1] https://ibm.github.io/watsonx-ai-python-sdk/fm_model.html#ibm_watsonx_ai.foundation_models.utils.enums.ModelTypes
         [2] https://dataplatform.cloud.ibm.com/docs/content/wsj/analyze-data/fm-models.html?context=wx&audience=wdp
     """
-    if task == "translate":
+    if task == TaskTypes.TRANSLATION.value or task == TaskTypes.TRANSLATION:
         return [
             # "ibm/granite-20b-multilingual",
             "mistralai/mixtral-8x7b-instruct-v01",
             ModelTypes.MIXTRAL_8X7B_INSTRUCT_V01_Q.value,
         ]
-    if task == "annotate":
+    if task == TaskTypes.ANNOTATION.value or task == TaskTypes.ANNOTATION:
         return [
             "mistralai/mixtral-8x7b-instruct-v01",
             ModelTypes.MIXTRAL_8X7B_INSTRUCT_V01_Q.value,
             # ModelTypes.LLAMA_2_70B_CHAT.value,
         ]
-    if task == "chat":
+    if task == TaskTypes.CHAT.value or task == TaskTypes.CHAT:
         return [
             "mistralai/mixtral-8x7b-instruct-v01",
             ModelTypes.MIXTRAL_8X7B_INSTRUCT_V01_Q.value,
             # ModelTypes.LLAMA_2_70B_CHAT.value,
         ]
     raise ValueError(f'Unsupported task: "{task}"')
 
 
-def list_decoding_methods() -> List[str]:
-    return [
-        DecodingMethods.GREEDY.value,
-        DecodingMethods.SAMPLE.value,
-    ]
-
-
-def list_params() -> List[str]:
-    """
+def get_default_params() -> Dict[str, Any]:
+    """Get default model parameters.
 
     >>> GenTextParamsMetaNames().show()
     >>> ---------------------  -----  --------
         META_PROP NAME         TYPE   REQUIRED
         DECODING_METHOD        str    N
         LENGTH_PENALTY         dict   N
         TEMPERATURE            float  N
@@ -64,36 +84,17 @@
         RETURN_OPTIONS         dict   N
         ---------------------  -----  --------
 
     Reference:
         [1] https://ibm.github.io/watsonx-ai-python-sdk/fm_model.html#metanames.GenTextParamsMetaNames
         [2] https://dataplatform.cloud.ibm.com/docs/content/wsj/analyze-data/fm-model-parameters.html?context=wx
     """
-    return [
-        GenTextParamsMetaNames.DECODING_METHOD,
-        GenTextParamsMetaNames.TEMPERATURE,
-        GenTextParamsMetaNames.TOP_P,
-        GenTextParamsMetaNames.TOP_K,
-        GenTextParamsMetaNames.RANDOM_SEED,
-        GenTextParamsMetaNames.REPETITION_PENALTY,
-        GenTextParamsMetaNames.MIN_NEW_TOKENS,
-        GenTextParamsMetaNames.MAX_NEW_TOKENS,
-    ]
-
-
-def get_model(
-    task: str,
-    model: str,
-    params: dict,
-    api_key: str,
-) -> Model:
-    if model not in list_models(task):
-        raise ValueError(f'Unsupported model: "{model}" for task "{task}"')
-    return Model(
-        model_id=model,
-        params=params,
-        credentials={
-            "apikey": api_key,
-            "url": "https://us-south.ml.cloud.ibm.com",
-        },
-        project_id="38a37d7d-4ab7-4349-935c-936add66c7f5",
-    )
+    return {
+        GenTextParamsMetaNames.DECODING_METHOD: "sample",
+        GenTextParamsMetaNames.TEMPERATURE: 0.1,
+        GenTextParamsMetaNames.TOP_P: 1.0,
+        GenTextParamsMetaNames.TOP_K: 50,
+        GenTextParamsMetaNames.RANDOM_SEED: 42,
+        GenTextParamsMetaNames.REPETITION_PENALTY: 1.0,
+        GenTextParamsMetaNames.MIN_NEW_TOKENS: 0,
+        GenTextParamsMetaNames.MAX_NEW_TOKENS: 1000,
+    }
```

### Comparing `postfinancex-0.0.1/postfinance/prompts.py` & `postfinancex-0.0.2/postfinance/prompts.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,10 @@
-TRANSLATE_PROMPT_TEMPLATE = """Detect the language of the following transcript and translate it from the detected language to English.
+from .models import TaskTypes
+
+TRANSLATE_PROMPT_TEMPLATE = """Detect the language of the following transcript. In addition, translate the transcript from the detected language to English.
 
 Transcript:
 ```
 **Skript 01 - Anfrage zu Gebühren und Zinsen auf Kontoauszügen**
 
 **Call-Center-Mitarbeiter (CCM):** "Grüezi, hie isch de [Mitarbeitername] vo de [Bankname] Chundebetreuig. Wie cha ich Ihne hütt hälfe?"
 
@@ -37,18 +39,18 @@
 **K:** "Danke, Ihne au. Uf Wiederhöre."
 
 **CCM:** "Uf Wiederhöre!"
 ```
 
 Output:
 ```
-Detected Language: 
+Language:
 Swiss German
 
-Translated Transcript in English:
+Translation:
 **Script 01 - Inquiry About Fees and Interest on Account Statements**
 
 **Call-Center Employee (CCE):** "Hello, this is [Employee Name] from [Bank Name] Customer Service. How can I help you today?"
 
 **Customer (C):** "Hello, I'm [Customer Name]. I've reviewed my account statement and I have some questions about the fees and interest that are listed."
 
 **CCE:** "Sure, I can certainly help you with that. Could you please give me your account number and your date of birth so I can verify your identity and check your account?"
@@ -83,18 +85,31 @@
 ```
 
 Transcript:
 ```
 {content}
 ```
 
-Output:"""
+Output:
+"""
+
 
+ANNOTATE_PROMPT_TEMPLATE = """Summarize the following transcript in one sentence. In addition, given the transcript, extract the customer's requests, questions or problems as well as the call-center employee's corresponding response. Extraction should be detailed and cite the related content in the transcript. Citation should be enclosed within the round brakets following the extration. Extraction from the customer's messages should be classified into one of three classes: Request, Question, Problem. 
 
-ANNOTATE_PROMPT_TEMPLATE = """Summarize the following transcript in one sentence. In addition, given the transcript, extract the customer's questions or problems as well as the call-center employee' answers or solutions. Extraction should be detailed and cite the related content in the transcript.
+Definitions of three classes Request, Question, Problem:
+```
+Class name: Request
+Description: The customer is requesting something. They might say they are needing information about something to be sent to their email address or mail address.
+
+Class name: Question
+Description: The customer is asking a technical question or a how-to question about the products or services.
+
+Class name: Problem
+Description: The customer is describing a problem they are having. They might say they are trying something, but it's not working. They might say they are getting an error or unexpected results.
+```
 
 Transcipt:
 ```
 **Script 01 - Inquiry About Fees and Interest on Account Statements**
 
 **Call-Center Employee (CCE):** "Hello, this is [Employee Name] from [Bank Name] Customer Service. How can I help you today?"
 
@@ -132,31 +147,34 @@
 ```
 
 Output:
 ```
 Summary:
 The customer called to inquire about unexpected fees and interest charges on their bank account statement, and the call-center employee explained the charges and discussed potential ways to avoid them in the future.
 
-Customer's Questions or Problems:
-1. The customer questioned the 'Account Management Fee' and 'Overdraft Interest' listed on their account statement, expressing confusion over their existence since they believed their account should not have any fees and they had not overspent their account balance ("There is a fee listed with the title 'Account Management Fee' and another one called 'Overdraft Interest.' I thought that I didn’t have any fees, and I don’t understand what the overdraft interest is.").
-
-2. The customer was certain they never exceeded their account balance and needed clarification on the recorded overdraft ("Ah, that makes sense. But I am actually quite sure that I never spent more than what was in my account.").
-
-3. The customer asked for ways to avoid these fees in the future ("Okay, I must have overlooked that. And can I do something to avoid these fees?").
-
-4. The customer requested information about different account models that might not carry the same fees ("That sounds reasonable. I will think about switching accounts. Can you send me information about the different account models?").
-
-Call-Center Employee's Answers or Solutions:
-1. The call-center employee clarified that the 'Account Management Fee' is a standard fee for account administration, dependent on the account model, and 'Overdraft Interest' is charged when the account balance goes negative, even briefly ("The account management fee is a standardized fee that we charge for the administration of your account. The amount of this fee can vary depending on your account model. As for the overdraft interest: this is an interest we charge if you spend more money than is available in your account, so if you overdraw your account.").
-
-2. Upon further review, the employee confirmed that the customer's account was indeed briefly overdrawn, which led to the overdraft charge ("I can check that again for you. One moment please... Yes, I see there was a brief moment when your account was slightly overdrawn. That could explain the overdraft interest.").
-
-3. The employee suggested regularly monitoring the account to avoid overdrafts and discussed the possibility of switching to a different account model to reduce or eliminate the management fee ("For the account management fee, if you want an account model with lower or no fees, we could talk about switching accounts. For the overdraft interest, I recommend you regularly check your account and make sure there is enough money available before making larger expenses.").
-
-4. The employee agreed to send information on different account models via email and confirmed that they had the correct email address on file ("Certainly, I can send you an overview by email. Is your email address up to date with us?").
+Customer's requests, questions or problems:
+Customer's Question: 
+The customer questioned the 'Account Management Fee' and 'Overdraft Interest' listed on their account statement, expressing confusion over their existence since they believed their account should not have any fees and they had not overspent their account balance ("There is a fee listed with the title 'Account Management Fee' and another one called 'Overdraft Interest.' I thought that I didn’t have any fees, and I don’t understand what the overdraft interest is.").
+Call-Center Employee's Response:
+The call-center employee clarified that the 'Account Management Fee' is a standard fee for account administration, dependent on the account model, and 'Overdraft Interest' is charged when the account balance goes negative, even briefly ("The account management fee is a standardized fee that we charge for the administration of your account. The amount of this fee can vary depending on your account model. As for the overdraft interest: this is an interest we charge if you spend more money than is available in your account, so if you overdraw your account.").
+
+Customer's Problem: 
+The customer was certain they never exceeded their account balance and needed clarification on the recorded overdraft ("Ah, that makes sense. But I am actually quite sure that I never spent more than what was in my account.").
+Call-Center Employee's Response:
+Upon further review, the employee confirmed that the customer's account was indeed briefly overdrawn, which led to the overdraft charge ("I can check that again for you. One moment please... Yes, I see there was a brief moment when your account was slightly overdrawn. That could explain the overdraft interest.").
+
+Customer's Question: 
+The customer asked for ways to avoid these fees in the future ("Okay, I must have overlooked that. And can I do something to avoid these fees?").
+Call-Center Employee's Response:
+The employee suggested regularly monitoring the account to avoid overdrafts and discussed the possibility of switching to a different account model to reduce or eliminate the management fee ("For the account management fee, if you want an account model with lower or no fees, we could talk about switching accounts. For the overdraft interest, I recommend you regularly check your account and make sure there is enough money available before making larger expenses.").
+
+Customer's Request:
+The customer requested information about different account models that might not carry the same fees ("That sounds reasonable. I will think about switching accounts. Can you send me information about the different account models?").
+Call-Center Employee's Response:
+The employee agreed to send information on different account models via email and confirmed that they had the correct email address on file ("Certainly, I can send you an overview by email. Is your email address up to date with us?").
 ```
 
 Transcipt:
 ```
 {content}
 ```
 
@@ -200,35 +218,33 @@
 **CCE:** "I'm glad I could help. I will send you the information right away. If there is anything else, we are here for you. Have a nice day, [Customer Name]!"
 
 **C:** "Thank you, you too. Goodbye."
 
 **CCE:** "Goodbye!"
 ```
 
-Conversation: 
+Dialogue: 
 ```
 Assistant: How could I help you?
 User: How to avoid account management fees?
 Assistant: To avoid account management fees, you may consider switching to a different account model that may have lower or no fees associated with it ("For the account management fee, if you want an account model with lower or no fees, we could talk about switching accounts").
 User: What is the overdraft interest?
 Assistant: The overdraft interest is an interest charge applied when you spend more money than is available in your account, essentially when your account balance goes negative ("As for the overdraft interest: this is an interest we charge if you spend more money than is available in your account, so if you overdraw your account").
 ```
 
 Transcript:
 ```
 {content}
 ```
 
-Conversation:
-```
-{messages}
-```"""
+Answer:
+"""
 
 
-def get_prompt_template(task: str) -> str:
-    if task == "translate":
-        return TRANSLATE_PROMPT_TEMPLATE
-    if task == "annotate":
-        return ANNOTATE_PROMPT_TEMPLATE
-    if task == "chat":
-        return CHAT_PROMPT_TEMPLATE
+def get_prompt(task: str | TaskTypes, **kwargs) -> str:
+    if task == TaskTypes.TRANSLATION.value or task == TaskTypes.TRANSLATION:
+        return TRANSLATE_PROMPT_TEMPLATE.format(**kwargs)
+    if task == TaskTypes.ANNOTATION.value or task == TaskTypes.ANNOTATION:
+        return ANNOTATE_PROMPT_TEMPLATE.format(**kwargs)
+    if task == TaskTypes.CHAT.value or task == TaskTypes.CHAT:
+        return CHAT_PROMPT_TEMPLATE.format(**kwargs)
     raise ValueError(f'Unsupported task: "{task}"')
```

### Comparing `postfinancex-0.0.1/pyproject.toml` & `postfinancex-0.0.2/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "postfinancex"
-version = "0.0.1"
+version = "0.0.2"
 description = "🤖 PostFinance LLM agent powered by IBM watsonx.ai ✨ PostFinance X IBM watsonx.ai"
 packages = [
     {include = "postfinance"}
 ]
 authors = ["Yi ZHANG <yizhang.dev@gmail.com>"]
 license = "BSD-3-Clause"
 readme = "README.md"
```

### Comparing `postfinancex-0.0.1/PKG-INFO` & `postfinancex-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: postfinancex
-Version: 0.0.1
+Version: 0.0.2
 Summary: 🤖 PostFinance LLM agent powered by IBM watsonx.ai ✨ PostFinance X IBM watsonx.ai
 Home-page: https://pypi.org/project/postfinancex
 License: BSD-3-Clause
 Author: Yi ZHANG
 Author-email: yizhang.dev@gmail.com
 Requires-Python: >=3.12,<4.0
 Classifier: License :: OSI Approved :: BSD License
```

