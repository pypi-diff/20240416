# Comparing `tmp/notdiamond-0.1.2b0.tar.gz` & `tmp/notdiamond-0.1.3b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "notdiamond-0.1.2b0.tar", max compression
+gzip compressed data, was "notdiamond-0.1.3b0.tar", max compression
```

## Comparing `notdiamond-0.1.2b0.tar` & `notdiamond-0.1.3b0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     4667 2024-04-09 10:12:26.438700 notdiamond-0.1.2b0/README.md
--rw-r--r--   0        0        0        0 2024-04-02 07:43:11.001993 notdiamond-0.1.2b0/notdiamond/__init__.py
--rw-r--r--   0        0        0      440 2024-04-02 07:43:11.002696 notdiamond-0.1.2b0/notdiamond/exceptions.py
--rw-r--r--   0        0        0        0 2024-04-02 07:43:11.002740 notdiamond-0.1.2b0/notdiamond/llms/__init__.py
--rw-r--r--   0        0        0    31309 2024-04-13 13:31:19.750433 notdiamond-0.1.2b0/notdiamond/llms/llm.py
--rw-r--r--   0        0        0     4432 2024-04-13 12:29:10.520716 notdiamond-0.1.2b0/notdiamond/llms/provider.py
--rw-r--r--   0        0        0     3350 2024-04-13 13:31:28.950135 notdiamond-0.1.2b0/notdiamond/llms/providers.py
--rw-r--r--   0        0        0    11540 2024-04-13 13:31:19.751412 notdiamond-0.1.2b0/notdiamond/llms/request.py
--rw-r--r--   0        0        0        0 2024-04-02 07:43:11.004168 notdiamond-0.1.2b0/notdiamond/metrics/__init__.py
--rw-r--r--   0        0        0     1155 2024-04-02 11:25:39.891484 notdiamond-0.1.2b0/notdiamond/metrics/metric.py
--rw-r--r--   0        0        0     1100 2024-04-06 09:04:10.351693 notdiamond-0.1.2b0/notdiamond/metrics/request.py
--rw-r--r--   0        0        0        0 2024-04-02 07:43:11.004898 notdiamond-0.1.2b0/notdiamond/prompts/__init__.py
--rw-r--r--   0        0        0      147 2024-04-02 07:43:11.005796 notdiamond-0.1.2b0/notdiamond/prompts/hash.py
--rw-r--r--   0        0        0     7782 2024-04-06 09:04:10.351913 notdiamond-0.1.2b0/notdiamond/prompts/prompt.py
--rw-r--r--   0        0        0     1881 2024-04-06 09:04:10.352179 notdiamond-0.1.2b0/notdiamond/settings.py
--rw-r--r--   0        0        0      972 2024-04-02 07:43:11.007948 notdiamond-0.1.2b0/notdiamond/types.py
--rw-r--r--   0        0        0     1479 2024-04-13 13:55:02.082427 notdiamond-0.1.2b0/pyproject.toml
--rw-r--r--   0        0        0     5822 1970-01-01 00:00:00.000000 notdiamond-0.1.2b0/PKG-INFO
+-rw-r--r--   0        0        0     4667 2024-04-09 10:12:26.438700 notdiamond-0.1.3b0/README.md
+-rw-r--r--   0        0        0        0 2024-04-02 07:43:11.001993 notdiamond-0.1.3b0/notdiamond/__init__.py
+-rw-r--r--   0        0        0      440 2024-04-02 07:43:11.002696 notdiamond-0.1.3b0/notdiamond/exceptions.py
+-rw-r--r--   0        0        0        0 2024-04-02 07:43:11.002740 notdiamond-0.1.3b0/notdiamond/llms/__init__.py
+-rw-r--r--   0        0        0    31309 2024-04-16 07:37:25.829978 notdiamond-0.1.3b0/notdiamond/llms/llm.py
+-rw-r--r--   0        0        0     4432 2024-04-13 12:29:10.520716 notdiamond-0.1.3b0/notdiamond/llms/provider.py
+-rw-r--r--   0        0        0     3638 2024-04-16 07:39:04.865174 notdiamond-0.1.3b0/notdiamond/llms/providers.py
+-rw-r--r--   0        0        0    11540 2024-04-13 13:31:19.751412 notdiamond-0.1.3b0/notdiamond/llms/request.py
+-rw-r--r--   0        0        0        0 2024-04-02 07:43:11.004168 notdiamond-0.1.3b0/notdiamond/metrics/__init__.py
+-rw-r--r--   0        0        0     1155 2024-04-02 11:25:39.891484 notdiamond-0.1.3b0/notdiamond/metrics/metric.py
+-rw-r--r--   0        0        0     1100 2024-04-06 09:04:10.351693 notdiamond-0.1.3b0/notdiamond/metrics/request.py
+-rw-r--r--   0        0        0        0 2024-04-02 07:43:11.004898 notdiamond-0.1.3b0/notdiamond/prompts/__init__.py
+-rw-r--r--   0        0        0      147 2024-04-02 07:43:11.005796 notdiamond-0.1.3b0/notdiamond/prompts/hash.py
+-rw-r--r--   0        0        0     7782 2024-04-06 09:04:10.351913 notdiamond-0.1.3b0/notdiamond/prompts/prompt.py
+-rw-r--r--   0        0        0     1933 2024-04-16 07:39:04.865490 notdiamond-0.1.3b0/notdiamond/settings.py
+-rw-r--r--   0        0        0      972 2024-04-02 07:43:11.007948 notdiamond-0.1.3b0/notdiamond/types.py
+-rw-r--r--   0        0        0     1458 2024-04-16 16:10:20.724515 notdiamond-0.1.3b0/pyproject.toml
+-rw-r--r--   0        0        0     5779 1970-01-01 00:00:00.000000 notdiamond-0.1.3b0/PKG-INFO
```

### Comparing `notdiamond-0.1.2b0/README.md` & `notdiamond-0.1.3b0/README.md`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.2b0/notdiamond/llms/llm.py` & `notdiamond-0.1.3b0/notdiamond/llms/llm.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.2b0/notdiamond/llms/provider.py` & `notdiamond-0.1.3b0/notdiamond/llms/provider.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.2b0/notdiamond/llms/providers.py` & `notdiamond-0.1.3b0/notdiamond/llms/providers.py`

 * *Files 15% similar despite different names*

```diff
@@ -12,16 +12,18 @@
         GPT_3_5_TURBO (NDLLMProvider): refers to 'gpt-3.5-turbo' model by OpenAI
         GPT_4 (NDLLMProvider): refers to 'gpt-4' model by OpenAI
         GPT_4_1106_PREVIEW (NDLLMProvider): refers to 'gpt-4-1106-preview' model by OpenAI
         GPT_4_TURBO_PREVIEW (NDLLMProvider): refers to 'gpt-4-turbo-preview' model by OpenAI
         CLAUDE_2_1 (NDLLMProvider): refers to 'claude-2.1' model by Anthropic
         CLAUDE_3_OPUS_20240229 (NDLLMProvider): refers to 'claude-3-opus-20240229' model by Anthropic
         CLAUDE_3_SONNET_20240229 (NDLLMProvider): refers to 'claude-3-sonnet-20240229' model by Anthropic
+        CLAUDE_3_HAIKU_20240307 (NDLLMProvider): refers to 'claude-3-haiku-20240307' model by Anthropic
         GEMINI_PRO (NDLLMProvider): refers to 'gemini-pro' model by Google
         COMMAND (NDLLMProvider): refers to 'command' model by Cohere
+        COMMAND_R (NDLLMProvider): refers to 'command-r' model by Cohere
         MISTRAL_LARGE_LATEST (NDLLMProvider): refers to 'mistral-large-latest' model by Mistral AI
         MISTRAL_MEDIUM_LATEST (NDLLMProvider): refers to 'mistral-medium-latest' model by Mistral AI
         MISTRAL_SMALL_LATEST (NDLLMProvider): refers to 'mistral-small-latest' model by Mistral AI
         OPEN_MISTRAL_7B (NDLLMProvider): refers to 'open-mistral-7b' model by Mistral AI
         OPEN_MIXTRAL_8X7B (NDLLMProvider): refers to 'open-mixtral-8x7b' model by Mistral AI
         CODELLAMA_34B_INSTRUCT_HF (NDLLMProvider): refers to 'CodeLlama-34b-Instruct-hf' model served via TogetherAI
         PHIND_CODELLAMA_34B_V2 (NDLLMProvider): refers to 'Phind-CodeLlama-34B-v2' model served via TogetherAI
@@ -36,16 +38,18 @@
     GPT_3_5_TURBO = ("openai", "gpt-3.5-turbo")
     GPT_4 = ("openai", "gpt-4")
     GPT_4_1106_PREVIEW = ("openai", "gpt-4-1106-preview")
     GPT_4_TURBO_PREVIEW = ("openai", "gpt-4-turbo-preview")
     CLAUDE_2_1 = ("anthropic", "claude-2.1")
     CLAUDE_3_OPUS_20240229 = ("anthropic", "claude-3-opus-20240229")
     CLAUDE_3_SONNET_20240229 = ("anthropic", "claude-3-sonnet-20240229")
+    CLAUDE_3_HAIKU_20240307 = ("anthropic", "claude-3-haiku-20240307")
     GEMINI_PRO = ("google", "gemini-pro")
     COMMAND = ("cohere", "command")
+    COMMAND_R = ("cohere", "command-r")
     MISTRAL_LARGE_LATEST = ("mistral", "mistral-large-latest")
     MISTRAL_MEDIUM_LATEST = ("mistral", "mistral-medium-latest")
     MISTRAL_SMALL_LATEST = ("mistral", "mistral-small-latest")
     OPEN_MISTRAL_7B = ("mistral", "open-mistral-7b")
     OPEN_MIXTRAL_8X7B = ("mistral", "open-mixtral-8x7b")
     CODELLAMA_34B_INSTRUCT_HF = ("togetherai", "CodeLlama-34b-Instruct-hf")
     PHIND_CODELLAMA_34B_V2 = ("togetherai", "Phind-CodeLlama-34B-v2")
```

### Comparing `notdiamond-0.1.2b0/notdiamond/llms/request.py` & `notdiamond-0.1.3b0/notdiamond/llms/request.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.2b0/notdiamond/metrics/metric.py` & `notdiamond-0.1.3b0/notdiamond/metrics/metric.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.2b0/notdiamond/metrics/request.py` & `notdiamond-0.1.3b0/notdiamond/metrics/request.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.2b0/notdiamond/prompts/prompt.py` & `notdiamond-0.1.3b0/notdiamond/prompts/prompt.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.2b0/notdiamond/settings.py` & `notdiamond-0.1.3b0/notdiamond/settings.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,19 +26,20 @@
         "api_key": OPENAI_API_KEY,
     },
     "anthropic": {
         "models": [
             "claude-2.1",
             "claude-3-opus-20240229",
             "claude-3-sonnet-20240229",
+            "claude-3-haiku-20240307",
         ],
         "api_key": ANTHROPIC_API_KEY,
     },
     "google": {"models": ["gemini-pro"], "api_key": GOOGLE_API_KEY},
-    "cohere": {"models": ["command"], "api_key": COHERE_API_KEY},
+    "cohere": {"models": ["command", "command-r"], "api_key": COHERE_API_KEY},
     "mistral": {
         "models": [
             "mistral-large-latest",
             "mistral-medium-latest",
             "mistral-small-latest",
             "open-mistral-7b",
             "open-mixtral-8x7b",
```

### Comparing `notdiamond-0.1.2b0/notdiamond/types.py` & `notdiamond-0.1.3b0/notdiamond/types.py`

 * *Files identical despite different names*

### Comparing `notdiamond-0.1.2b0/pyproject.toml` & `notdiamond-0.1.3b0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 [tool.poetry]
 name = "notdiamond"
-version = "0.1.2-beta"
+version = "0.1.3-beta"
 description = "Not Diamond Python Library"
 authors = ["Not Diamond <t5@notdiamond.ai>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9.0"
 langchain = ">=0.1.10"
-anthropic = "^0.20.0"
 langchain-google-genai = ">=0.0.2"
-litellm = "^1.32.4"
+litellm = "^1.34.40"
 langchain-openai = "^0.0.5"
 python-dotenv = "^1.0.1"
 openai = ">=1.0.0"
 ppdeep = "^20200505"
-langchain-anthropic = "^0.1.4"
+langchain-anthropic = "^0.1.8"
 langchain-community = "^0.0.28"
 langchain-mistralai = "^0.0.5"
 together = "^0.2.11"
 langchain-together = "^0.0.2.post1"
 aiohttp = "^3.9.3"
-langchain-cohere = "^0.1.1"
+langchain-cohere = "^0.1.2"
 
 [tool.poetry.group.test.dependencies]
 pytest = "^8.0.0"
 pytest-asyncio = "^0.23.6"
 
 [tool.poetry.group.dev.dependencies]
 ruff = "^0.3.1"
```

### Comparing `notdiamond-0.1.2b0/PKG-INFO` & `notdiamond-0.1.3b0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,30 +1,29 @@
 Metadata-Version: 2.1
 Name: notdiamond
-Version: 0.1.2b0
+Version: 0.1.3b0
 Summary: Not Diamond Python Library
 Author: Not Diamond
 Author-email: t5@notdiamond.ai
 Requires-Python: >=3.9.0,<4.0.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: aiohttp (>=3.9.3,<4.0.0)
-Requires-Dist: anthropic (>=0.20.0,<0.21.0)
 Requires-Dist: langchain (>=0.1.10)
-Requires-Dist: langchain-anthropic (>=0.1.4,<0.2.0)
-Requires-Dist: langchain-cohere (>=0.1.1,<0.2.0)
+Requires-Dist: langchain-anthropic (>=0.1.8,<0.2.0)
+Requires-Dist: langchain-cohere (>=0.1.2,<0.2.0)
 Requires-Dist: langchain-community (>=0.0.28,<0.0.29)
 Requires-Dist: langchain-google-genai (>=0.0.2)
 Requires-Dist: langchain-mistralai (>=0.0.5,<0.0.6)
 Requires-Dist: langchain-openai (>=0.0.5,<0.0.6)
 Requires-Dist: langchain-together (>=0.0.2.post1,<0.0.3)
-Requires-Dist: litellm (>=1.32.4,<2.0.0)
+Requires-Dist: litellm (>=1.34.40,<2.0.0)
 Requires-Dist: openai (>=1.0.0)
 Requires-Dist: ppdeep (>=20200505,<20200506)
 Requires-Dist: python-dotenv (>=1.0.1,<2.0.0)
 Requires-Dist: together (>=0.2.11,<0.3.0)
 Description-Content-Type: text/markdown
 
 # Getting started with Not Diamond
```

