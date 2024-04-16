# Comparing `tmp/gtsystem-0.1.1.tar.gz` & `tmp/gtsystem-0.1.2.tar.gz`

## Comparing `gtsystem-0.1.1.tar` & `gtsystem-0.1.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gtsystem-0.1.1/gtsystem/__init__.py
--rw-r--r--   0        0        0     3593 2020-02-02 00:00:00.000000 gtsystem-0.1.1/gtsystem/anthropic.py
--rw-r--r--   0        0        0    10040 2020-02-02 00:00:00.000000 gtsystem-0.1.1/gtsystem/bedrock.py
--rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 gtsystem-0.1.1/gtsystem/benchmark.py
--rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 gtsystem-0.1.1/gtsystem/chat.py
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 gtsystem-0.1.1/gtsystem/groq.py
--rw-r--r--   0        0        0     3467 2020-02-02 00:00:00.000000 gtsystem-0.1.1/gtsystem/instrument.py
--rw-r--r--   0        0        0     2053 2020-02-02 00:00:00.000000 gtsystem-0.1.1/gtsystem/leaderboard.py
--rw-r--r--   0        0        0     2129 2020-02-02 00:00:00.000000 gtsystem-0.1.1/gtsystem/ollama.py
--rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 gtsystem-0.1.1/gtsystem/openai.py
--rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 gtsystem-0.1.1/gtsystem/render.py
--rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 gtsystem-0.1.1/gtsystem/tasks.py
--rw-r--r--   0        0        0     3100 2020-02-02 00:00:00.000000 gtsystem-0.1.1/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 gtsystem-0.1.1/LICENSE
--rw-r--r--   0        0        0     6824 2020-02-02 00:00:00.000000 gtsystem-0.1.1/README.md
--rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 gtsystem-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     8167 2020-02-02 00:00:00.000000 gtsystem-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gtsystem-0.1.2/gtsystem/__init__.py
+-rw-r--r--   0        0        0     3593 2020-02-02 00:00:00.000000 gtsystem-0.1.2/gtsystem/anthropic.py
+-rw-r--r--   0        0        0    10040 2020-02-02 00:00:00.000000 gtsystem-0.1.2/gtsystem/bedrock.py
+-rw-r--r--   0        0        0      824 2020-02-02 00:00:00.000000 gtsystem-0.1.2/gtsystem/benchmark.py
+-rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 gtsystem-0.1.2/gtsystem/chat.py
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 gtsystem-0.1.2/gtsystem/groq.py
+-rw-r--r--   0        0        0     3467 2020-02-02 00:00:00.000000 gtsystem-0.1.2/gtsystem/instrument.py
+-rw-r--r--   0        0        0     2053 2020-02-02 00:00:00.000000 gtsystem-0.1.2/gtsystem/leaderboard.py
+-rw-r--r--   0        0        0     2129 2020-02-02 00:00:00.000000 gtsystem-0.1.2/gtsystem/ollama.py
+-rw-r--r--   0        0        0     2813 2020-02-02 00:00:00.000000 gtsystem-0.1.2/gtsystem/openai.py
+-rw-r--r--   0        0        0     1244 2020-02-02 00:00:00.000000 gtsystem-0.1.2/gtsystem/render.py
+-rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 gtsystem-0.1.2/gtsystem/tasks.py
+-rw-r--r--   0        0        0     3100 2020-02-02 00:00:00.000000 gtsystem-0.1.2/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 gtsystem-0.1.2/LICENSE
+-rw-r--r--   0        0        0     8030 2020-02-02 00:00:00.000000 gtsystem-0.1.2/README.md
+-rw-r--r--   0        0        0     1426 2020-02-02 00:00:00.000000 gtsystem-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     9373 2020-02-02 00:00:00.000000 gtsystem-0.1.2/PKG-INFO
```

### Comparing `gtsystem-0.1.1/gtsystem/anthropic.py` & `gtsystem-0.1.2/gtsystem/anthropic.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     if reset:
         CHAT_CONTEXT.reset_context()
     
     if system != "":
         CHAT_CONTEXT.set_system(system)
     
     if image_url != "":
-        CHAT_CONTEXT.add_image_message(image_url=image_url, prompt=prompt)
+        CHAT_CONTEXT.add_image_message(prompt=prompt, image_url=image_url)
     else:
         CHAT_CONTEXT.add_message("user", prompt)
 
     message  = anthropic.Anthropic().messages.create(
         model=model,
         system=CHAT_CONTEXT.get_system(),
         temperature=temperature,
```

### Comparing `gtsystem-0.1.1/gtsystem/bedrock.py` & `gtsystem-0.1.2/gtsystem/bedrock.py`

 * *Files identical despite different names*

### Comparing `gtsystem-0.1.1/gtsystem/benchmark.py` & `gtsystem-0.1.2/gtsystem/benchmark.py`

 * *Files identical despite different names*

### Comparing `gtsystem-0.1.1/gtsystem/groq.py` & `gtsystem-0.1.2/gtsystem/groq.py`

 * *Files identical despite different names*

### Comparing `gtsystem-0.1.1/gtsystem/instrument.py` & `gtsystem-0.1.2/gtsystem/instrument.py`

 * *Files identical despite different names*

### Comparing `gtsystem-0.1.1/gtsystem/leaderboard.py` & `gtsystem-0.1.2/gtsystem/leaderboard.py`

 * *Files identical despite different names*

### Comparing `gtsystem-0.1.1/gtsystem/ollama.py` & `gtsystem-0.1.2/gtsystem/ollama.py`

 * *Files identical despite different names*

### Comparing `gtsystem-0.1.1/gtsystem/openai.py` & `gtsystem-0.1.2/gtsystem/openai.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,39 +1,76 @@
 from openai import OpenAI
-
+from .chat import GptChat
 from .instrument import metrics
+
 OPENAI = None
 
 def init():
     global OPENAI
     OPENAI = OpenAI()
 
-def _gpt_text(prompt, system='', temperature=0.0, topP=1, tokens=512, model=""):
+CHAT_CONTEXT = GptChat()
+
+def _gpt_chat(prompt, system='', temperature=0.0, topP=1, tokens=512, image_url="", model="", reset=False):
     if OPENAI is None:
         init()
 
+    if reset:
+        CHAT_CONTEXT.reset_context()
+    
+    if system != "":
+        CHAT_CONTEXT.add_message("system", system)
+    
+    if image_url != "":
+        CHAT_CONTEXT.add_image_message(prompt=prompt, image_url=image_url)
+    else:
+        CHAT_CONTEXT.add_message("user", prompt)
+
     response = OPENAI.chat.completions.create(
-    model=model,
-    messages=[
-        {
-        "role": "system",
-        "content": system
-        },
-        {
-        "role": "user",
-        "content": prompt
-        }
-    ],
-    temperature=temperature,
-    top_p=topP,
-    max_tokens=tokens,
+        model=model,
+        messages=CHAT_CONTEXT.get_messages(),
+        temperature=temperature,
+        top_p=topP,
+        max_tokens=tokens,
     )
     response_text = response.choices[0].message.content.strip()
     return response_text
 
+@metrics.track
+def gpt4_chat(prompt, system='', temperature=0.0, topP=1, tokens=4096, image_url="", reset=False):
+    return _gpt_chat(prompt, system=system, temperature=temperature, 
+                topP=topP, tokens=tokens, model="gpt-4-turbo", image_url=image_url, reset=reset)
+
+@metrics.track
+def gpt3_chat(prompt, system='', temperature=0.0, topP=1, tokens=4096, reset=False):
+    return _gpt_chat(prompt, system=system, temperature=temperature, 
+                topP=topP, tokens=tokens, model="gpt-3.5-turbo", reset=reset)
+
+def _gpt_text(prompt, system='', temperature=0.0, topP=1, tokens=512, model=""):
+    if OPENAI is None:
+        init()
+
+    response = OPENAI.chat.completions.create(
+        model=model,
+        messages=[
+            {
+            "role": "system",
+            "content": system
+            },
+            {
+            "role": "user",
+            "content": prompt
+            }
+        ],
+        temperature=temperature,
+        top_p=topP,
+        max_tokens=tokens,
+    )
+    response_text = response.choices[0].message.content.strip()
+    return response_text
 
 @metrics.track
 def gpt3_text(prompt, system='', temperature=0.0, topP=1, tokens=512):
     return _gpt_text(prompt, system=system, temperature=temperature, 
                 topP=topP, tokens=tokens, model="gpt-3.5-turbo")
 
 @metrics.track
```

### Comparing `gtsystem-0.1.1/gtsystem/render.py` & `gtsystem-0.1.2/gtsystem/render.py`

 * *Files identical despite different names*

### Comparing `gtsystem-0.1.1/gtsystem/tasks.py` & `gtsystem-0.1.2/gtsystem/tasks.py`

 * *Files identical despite different names*

### Comparing `gtsystem-0.1.1/.gitignore` & `gtsystem-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `gtsystem-0.1.1/LICENSE` & `gtsystem-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `gtsystem-0.1.1/README.md` & `gtsystem-0.1.2/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -10,43 +10,67 @@
 The get started using `gtsystem` package follow these steps.
 
 **Step 1.** Install gtsystem package using `pip install gtsystem`
 
 **Step 2.** Open a Jupyter notebook and try this sample.
 
 ```python
-from gtsystem import openai, bedrock, ollama
+from gtsystem import openai, bedrock, anthropic, ollama, instrument
 prompt = 'How many faces does a tetrahedron have?'
-openai.gpt_text(prompt)
-bedrock.llama_text(prompt)
-bedrock.claude_text(prompt)
+openai.text(prompt)
+bedrock.text(prompt)
+anthropic.text(prompt)
 ollama.mistral_text(prompt)
+instrument.metrics.stats()
 ```
 
+Note: To install the dependencies and setup each of the vendor APIs you can continue reading [here](https://github.com/GenaiTechne/gtsystem?tab=readme-ov-file#installing-dependencies).
+
 ## Features and Notebook Samples
 
 The `gtsystem` package source is available in this [repository on GitHub](https://github.com/GenaiTechne/gtsystem).
 
 You can read more about the vision behind gtsystem on the [GenAI Techne substack post](https://genaitechne.substack.com/p/excelling-in-the-craft-of-generative).
 
 [![](https://raw.githubusercontent.com/GenaiTechne/gtsystem/main/gtsystem-features.jpg)](https://genaitechne.substack.com/p/excelling-in-the-craft-of-generative)
 
 You can learn `gtsystem` API by following along the [notebook samples](https://github.com/GenaiTechne/gtsystem/tree/main/notebooks) included in the `gtsystem` repo. This samples are documented on the [GenAI Techne Substack](https://genaitechne.substack.com/).
 
+0. **Review model leaderboard:** Use `00-leaderboard.ipynb` for reviewing model leaderboard, filter by ranking, vendors, models to decide which one to explore.
+
 1. **Evaluate models using one line of code:** Refer `01-evaluate.ipynb` for single statement prompt evaluations across multiple models including OpenAI GPT, Bedrock hosted Claude or Llama.
 
 2. **Render LLM responses:** Use `02-render.ipynb` for well formatted rendering of the model responses including markdown tables.
 
 3. **Load evaluation tasks from Excel:** Try `03-tasks.ipynb` for automating evaluation tasks - find, list, load prompts by task, including optimal parameter values for temperature and TopP.
 
 4. **Instrument speed and size (cost) of response:** Reuse `04-instrument.ipynb` for instrumenting and comparing multiple models across latency and size of response.
 
-4. **Benchmark quality of response:** Use `05-benchmark.ipynb` for automated benchmarking quality of responses from models like Llama and Claude using GPT-4 as an LLM evaluator.
+5. **Benchmark quality of response:** Use `05-benchmark.ipynb` for automated benchmarking quality of responses from models like Llama and Claude using GPT-4 as an LLM evaluator.
+
+6. **Run models on your laptop:** Get `06-ollama.ipynb` to run models like Mistral, Llama, and CodeLlama locally on your laptop and compare models hosted on Cloud or proprietary model APIs.
+
+7. **Low code sample:** Check out simple `07-low-code-sample.ipynb` to appreciate how much can be done with just simple GTSystem APIs.
+
+8. **Go from prototype to production:** Start with `08-prototype-to-production.ipynb` to go from prototyping using best models, then exploring local models on laptop, finally comparing fastest vendors like Groq in one seamless workflow.
+
+9. **Visual chat on Bedrock:** Explore `09-chat-bedrock.ipynb` for visual chat using Bedrock hosted models.
 
-5. **Run models on your laptop:** Get `06-ollama.ipynb` to run models like Mistral, Llama, and CodeLlama locally on your laptop and compare models hosted on Cloud or proprietary model APIs.
+10. **Visual chat on Anthropic:** Explore `10-chat-anthropic.ipynb` for visual chat using Anthropic hosted models.
+
+## What's New
+
+### 2024-04-15 (Release 0.1.2)
+
+- Multimodal Chat using OpenAI.
+
+### 2024-04-14 (Release 0.1.1)
+
+- Multimodal Chat using Anthropic/Claude.
+- Multimodal Chat using Bedrock/Claude.
 
 ## Installing Dependencies
 
 You can install following dependencies to work with `gtsystem` based on your needs. Start with our `requirements.txt` or create your own. Then run `pip install -r requirements.txt` within your environment.
 
 ```
 # Python capabilities
@@ -62,14 +86,17 @@
 boto3
 awscli
 botocore
 
 # OpenAI for GPT models
 openai
 
+# Anthropic models
+anthropic
+
 # Ollama for LLMs running on your laptop
 ollama
 
 # Groq for open models on fast Groq LPUs
 groq
 ```
```

### Comparing `gtsystem-0.1.1/pyproject.toml` & `gtsystem-0.1.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "gtsystem"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="GenAI Techne", email="team@genaitechne.com" },
 ]
 description = "GenAI Techne System (gtsystem) is a low code Python package for crafting GenAI applications quickly"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `gtsystem-0.1.1/PKG-INFO` & `gtsystem-0.1.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: gtsystem
-Version: 0.1.1
+Version: 0.1.2
 Summary: GenAI Techne System (gtsystem) is a low code Python package for crafting GenAI applications quickly
 Project-URL: Homepage, https://github.com/GenaiTechne/gtsystem
 Project-URL: Issues, https://github.com/GenaiTechne/gtsystem/issues
 Author-email: GenAI Techne <team@genaitechne.com>
 License-File: LICENSE
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Framework :: Jupyter
@@ -40,43 +40,67 @@
 The get started using `gtsystem` package follow these steps.
 
 **Step 1.** Install gtsystem package using `pip install gtsystem`
 
 **Step 2.** Open a Jupyter notebook and try this sample.
 
 ```python
-from gtsystem import openai, bedrock, ollama
+from gtsystem import openai, bedrock, anthropic, ollama, instrument
 prompt = 'How many faces does a tetrahedron have?'
-openai.gpt_text(prompt)
-bedrock.llama_text(prompt)
-bedrock.claude_text(prompt)
+openai.text(prompt)
+bedrock.text(prompt)
+anthropic.text(prompt)
 ollama.mistral_text(prompt)
+instrument.metrics.stats()
 ```
 
+Note: To install the dependencies and setup each of the vendor APIs you can continue reading [here](https://github.com/GenaiTechne/gtsystem?tab=readme-ov-file#installing-dependencies).
+
 ## Features and Notebook Samples
 
 The `gtsystem` package source is available in this [repository on GitHub](https://github.com/GenaiTechne/gtsystem).
 
 You can read more about the vision behind gtsystem on the [GenAI Techne substack post](https://genaitechne.substack.com/p/excelling-in-the-craft-of-generative).
 
 [![](https://raw.githubusercontent.com/GenaiTechne/gtsystem/main/gtsystem-features.jpg)](https://genaitechne.substack.com/p/excelling-in-the-craft-of-generative)
 
 You can learn `gtsystem` API by following along the [notebook samples](https://github.com/GenaiTechne/gtsystem/tree/main/notebooks) included in the `gtsystem` repo. This samples are documented on the [GenAI Techne Substack](https://genaitechne.substack.com/).
 
+0. **Review model leaderboard:** Use `00-leaderboard.ipynb` for reviewing model leaderboard, filter by ranking, vendors, models to decide which one to explore.
+
 1. **Evaluate models using one line of code:** Refer `01-evaluate.ipynb` for single statement prompt evaluations across multiple models including OpenAI GPT, Bedrock hosted Claude or Llama.
 
 2. **Render LLM responses:** Use `02-render.ipynb` for well formatted rendering of the model responses including markdown tables.
 
 3. **Load evaluation tasks from Excel:** Try `03-tasks.ipynb` for automating evaluation tasks - find, list, load prompts by task, including optimal parameter values for temperature and TopP.
 
 4. **Instrument speed and size (cost) of response:** Reuse `04-instrument.ipynb` for instrumenting and comparing multiple models across latency and size of response.
 
-4. **Benchmark quality of response:** Use `05-benchmark.ipynb` for automated benchmarking quality of responses from models like Llama and Claude using GPT-4 as an LLM evaluator.
+5. **Benchmark quality of response:** Use `05-benchmark.ipynb` for automated benchmarking quality of responses from models like Llama and Claude using GPT-4 as an LLM evaluator.
+
+6. **Run models on your laptop:** Get `06-ollama.ipynb` to run models like Mistral, Llama, and CodeLlama locally on your laptop and compare models hosted on Cloud or proprietary model APIs.
+
+7. **Low code sample:** Check out simple `07-low-code-sample.ipynb` to appreciate how much can be done with just simple GTSystem APIs.
+
+8. **Go from prototype to production:** Start with `08-prototype-to-production.ipynb` to go from prototyping using best models, then exploring local models on laptop, finally comparing fastest vendors like Groq in one seamless workflow.
+
+9. **Visual chat on Bedrock:** Explore `09-chat-bedrock.ipynb` for visual chat using Bedrock hosted models.
 
-5. **Run models on your laptop:** Get `06-ollama.ipynb` to run models like Mistral, Llama, and CodeLlama locally on your laptop and compare models hosted on Cloud or proprietary model APIs.
+10. **Visual chat on Anthropic:** Explore `10-chat-anthropic.ipynb` for visual chat using Anthropic hosted models.
+
+## What's New
+
+### 2024-04-15 (Release 0.1.2)
+
+- Multimodal Chat using OpenAI.
+
+### 2024-04-14 (Release 0.1.1)
+
+- Multimodal Chat using Anthropic/Claude.
+- Multimodal Chat using Bedrock/Claude.
 
 ## Installing Dependencies
 
 You can install following dependencies to work with `gtsystem` based on your needs. Start with our `requirements.txt` or create your own. Then run `pip install -r requirements.txt` within your environment.
 
 ```
 # Python capabilities
@@ -92,14 +116,17 @@
 boto3
 awscli
 botocore
 
 # OpenAI for GPT models
 openai
 
+# Anthropic models
+anthropic
+
 # Ollama for LLMs running on your laptop
 ollama
 
 # Groq for open models on fast Groq LPUs
 groq
 ```
```

