# Comparing `tmp/gradio_awsbedrock_multimodalchatbot-0.0.1.tar.gz` & `tmp/gradio_awsbedrock_multimodalchatbot-0.0.2.tar.gz`

## Comparing `gradio_awsbedrock_multimodalchatbot-0.0.1.tar` & `gradio_awsbedrock_multimodalchatbot-0.0.2.tar`

### file list

```diff
@@ -1,24 +1,25 @@
--rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 gradio_awsbedrock_multimodalchatbot-0.0.1/backend/gradio_awsBedrock_multimodalChatbot/__init__.py
--rw-r--r--   0        0        0    11240 2020-02-02 00:00:00.000000 gradio_awsbedrock_multimodalchatbot-0.0.1/backend/gradio_awsBedrock_multimodalChatbot/multimodalchatbot.py
--rw-r--r--   0        0        0    26428 2020-02-02 00:00:00.000000 gradio_awsbedrock_multimodalchatbot-0.0.1/backend/gradio_awsBedrock_multimodalChatbot/multimodalchatbot.pyi
--rw-r--r--   0        0        0   766349 2020-02-02 00:00:00.000000 gradio_awsbedrock_multimodalchatbot-0.0.1/backend/gradio_awsBedrock_multimodalChatbot/templates/component/index.js
--rw-r--r--   0        0        0  1483905 2020-02-02 00:00:00.000000 gradio_awsbedrock_multimodalchatbot-0.0.1/backend/gradio_awsBedrock_multimodalChatbot/templates/component/style.css
--rw-r--r--   0        0        0     2374 2020-02-02 00:00:00.000000 gradio_awsbedrock_multimodalchatbot-0.0.1/backend/gradio_awsBedrock_multimodalChatbot/templates/component/assets/worker-43d19264.js
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gradio_awsbedrock_multimodalchatbot-0.0.1/demo/__init__.py
--rw-r--r--   0        0        0     2810 2020-02-02 00:00:00.000000 gradio_awsbedrock_multimodalchatbot-0.0.1/demo/app.py
--rw-r--r--   0        0        0     2392 2020-02-02 00:00:00.000000 gradio_awsbedrock_multimodalchatbot-0.0.1/demo/bedrock_utils.py
--rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 gradio_awsbedrock_multimodalchatbot-0.0.1/demo/css.css
--rw-r--r--   0        0        0    15559 2020-02-02 00:00:00.000000 gradio_awsbedrock_multimodalchatbot-0.0.1/demo/space.py
--rw-r--r--   0        0        0     3821 2020-02-02 00:00:00.000000 gradio_awsbedrock_multimodalchatbot-0.0.1/frontend/Index.svelte
--rw-r--r--   0        0        0    59659 2020-02-02 00:00:00.000000 gradio_awsbedrock_multimodalchatbot-0.0.1/frontend/package-lock.json
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 gradio_awsbedrock_multimodalchatbot-0.0.1/frontend/package.json
--rw-r--r--   0        0        0    13218 2020-02-02 00:00:00.000000 gradio_awsbedrock_multimodalchatbot-0.0.1/frontend/shared/ChatBot.svelte
--rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 gradio_awsbedrock_multimodalchatbot-0.0.1/frontend/shared/Copy.svelte
--rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 gradio_awsbedrock_multimodalchatbot-0.0.1/frontend/shared/LikeDislike.svelte
--rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 gradio_awsbedrock_multimodalchatbot-0.0.1/frontend/shared/Pending.svelte
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 gradio_awsbedrock_multimodalchatbot-0.0.1/frontend/shared/autorender.d.ts
--rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 gradio_awsbedrock_multimodalchatbot-0.0.1/frontend/shared/utils.ts
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 gradio_awsbedrock_multimodalchatbot-0.0.1/.gitignore
--rw-r--r--   0        0        0    14337 2020-02-02 00:00:00.000000 gradio_awsbedrock_multimodalchatbot-0.0.1/README.md
--rw-r--r--   0        0        0     1943 2020-02-02 00:00:00.000000 gradio_awsbedrock_multimodalchatbot-0.0.1/pyproject.toml
--rw-r--r--   0        0        0    15581 2020-02-02 00:00:00.000000 gradio_awsbedrock_multimodalchatbot-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 gradio_awsbedrock_multimodalchatbot-0.0.2/backend/gradio_awsBedrock_multimodalChatbot/__init__.py
+-rw-r--r--   0        0        0    11240 2020-02-02 00:00:00.000000 gradio_awsbedrock_multimodalchatbot-0.0.2/backend/gradio_awsBedrock_multimodalChatbot/multimodalchatbot.py
+-rw-r--r--   0        0        0    26428 2020-02-02 00:00:00.000000 gradio_awsbedrock_multimodalchatbot-0.0.2/backend/gradio_awsBedrock_multimodalChatbot/multimodalchatbot.pyi
+-rw-r--r--   0        0        0   766349 2020-02-02 00:00:00.000000 gradio_awsbedrock_multimodalchatbot-0.0.2/backend/gradio_awsBedrock_multimodalChatbot/templates/component/index.js
+-rw-r--r--   0        0        0  1483905 2020-02-02 00:00:00.000000 gradio_awsbedrock_multimodalchatbot-0.0.2/backend/gradio_awsBedrock_multimodalChatbot/templates/component/style.css
+-rw-r--r--   0        0        0     2374 2020-02-02 00:00:00.000000 gradio_awsbedrock_multimodalchatbot-0.0.2/backend/gradio_awsBedrock_multimodalChatbot/templates/component/assets/worker-43d19264.js
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 gradio_awsbedrock_multimodalchatbot-0.0.2/demo/__init__.py
+-rw-r--r--   0        0        0     2810 2020-02-02 00:00:00.000000 gradio_awsbedrock_multimodalchatbot-0.0.2/demo/app.py
+-rw-r--r--   0        0        0     2392 2020-02-02 00:00:00.000000 gradio_awsbedrock_multimodalchatbot-0.0.2/demo/bedrock_utils.py
+-rw-r--r--   0        0        0     2543 2020-02-02 00:00:00.000000 gradio_awsbedrock_multimodalchatbot-0.0.2/demo/css.css
+-rw-r--r--   0        0        0     1283 2020-02-02 00:00:00.000000 gradio_awsbedrock_multimodalchatbot-0.0.2/demo/requirements.txt
+-rw-r--r--   0        0        0    15657 2020-02-02 00:00:00.000000 gradio_awsbedrock_multimodalchatbot-0.0.2/demo/space.py
+-rw-r--r--   0        0        0     3821 2020-02-02 00:00:00.000000 gradio_awsbedrock_multimodalchatbot-0.0.2/frontend/Index.svelte
+-rw-r--r--   0        0        0    59659 2020-02-02 00:00:00.000000 gradio_awsbedrock_multimodalchatbot-0.0.2/frontend/package-lock.json
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 gradio_awsbedrock_multimodalchatbot-0.0.2/frontend/package.json
+-rw-r--r--   0        0        0    13218 2020-02-02 00:00:00.000000 gradio_awsbedrock_multimodalchatbot-0.0.2/frontend/shared/ChatBot.svelte
+-rw-r--r--   0        0        0     1394 2020-02-02 00:00:00.000000 gradio_awsbedrock_multimodalchatbot-0.0.2/frontend/shared/Copy.svelte
+-rw-r--r--   0        0        0      882 2020-02-02 00:00:00.000000 gradio_awsbedrock_multimodalchatbot-0.0.2/frontend/shared/LikeDislike.svelte
+-rw-r--r--   0        0        0     1082 2020-02-02 00:00:00.000000 gradio_awsbedrock_multimodalchatbot-0.0.2/frontend/shared/Pending.svelte
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 gradio_awsbedrock_multimodalchatbot-0.0.2/frontend/shared/autorender.d.ts
+-rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 gradio_awsbedrock_multimodalchatbot-0.0.2/frontend/shared/utils.ts
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 gradio_awsbedrock_multimodalchatbot-0.0.2/.gitignore
+-rw-r--r--   0        0        0    14435 2020-02-02 00:00:00.000000 gradio_awsbedrock_multimodalchatbot-0.0.2/README.md
+-rw-r--r--   0        0        0     2142 2020-02-02 00:00:00.000000 gradio_awsbedrock_multimodalchatbot-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0    15641 2020-02-02 00:00:00.000000 gradio_awsbedrock_multimodalchatbot-0.0.2/PKG-INFO
```

### Comparing `gradio_awsbedrock_multimodalchatbot-0.0.1/backend/gradio_awsBedrock_multimodalChatbot/multimodalchatbot.py` & `gradio_awsbedrock_multimodalchatbot-0.0.2/backend/gradio_awsBedrock_multimodalChatbot/multimodalchatbot.py`

 * *Files identical despite different names*

### Comparing `gradio_awsbedrock_multimodalchatbot-0.0.1/backend/gradio_awsBedrock_multimodalChatbot/multimodalchatbot.pyi` & `gradio_awsbedrock_multimodalchatbot-0.0.2/backend/gradio_awsBedrock_multimodalChatbot/multimodalchatbot.pyi`

 * *Files identical despite different names*

### Comparing `gradio_awsbedrock_multimodalchatbot-0.0.1/backend/gradio_awsBedrock_multimodalChatbot/templates/component/index.js` & `gradio_awsbedrock_multimodalchatbot-0.0.2/backend/gradio_awsBedrock_multimodalChatbot/templates/component/index.js`

 * *Files identical despite different names*

### Comparing `gradio_awsbedrock_multimodalchatbot-0.0.1/backend/gradio_awsBedrock_multimodalChatbot/templates/component/style.css` & `gradio_awsbedrock_multimodalchatbot-0.0.2/backend/gradio_awsBedrock_multimodalChatbot/templates/component/style.css`

 * *Files identical despite different names*

### Comparing `gradio_awsbedrock_multimodalchatbot-0.0.1/backend/gradio_awsBedrock_multimodalChatbot/templates/component/assets/worker-43d19264.js` & `gradio_awsbedrock_multimodalchatbot-0.0.2/backend/gradio_awsBedrock_multimodalChatbot/templates/component/assets/worker-43d19264.js`

 * *Files identical despite different names*

### Comparing `gradio_awsbedrock_multimodalchatbot-0.0.1/demo/app.py` & `gradio_awsbedrock_multimodalchatbot-0.0.2/demo/app.py`

 * *Files identical despite different names*

### Comparing `gradio_awsbedrock_multimodalchatbot-0.0.1/demo/bedrock_utils.py` & `gradio_awsbedrock_multimodalchatbot-0.0.2/demo/bedrock_utils.py`

 * *Files identical despite different names*

### Comparing `gradio_awsbedrock_multimodalchatbot-0.0.1/demo/css.css` & `gradio_awsbedrock_multimodalchatbot-0.0.2/demo/css.css`

 * *Files identical despite different names*

### Comparing `gradio_awsbedrock_multimodalchatbot-0.0.1/demo/space.py` & `gradio_awsbedrock_multimodalchatbot-0.0.2/demo/space.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     ),
 ) as demo:
     gr.Markdown(
 """
 # `gradio_awsBedrock_multimodalChatbot`
 
 <div style="display: flex; gap: 7px;">
-<img alt="Static Badge" src="https://img.shields.io/badge/version%20-%200.0.1%20-%20orange">  
+<a href="https://pypi.org/project/gradio_awsBedrock_multimodalChatbot/" target="_blank"><img alt="PyPI - Version" src="https://img.shields.io/pypi/v/gradio_awsBedrock_multimodalChatbot"></a>  
 </div>
 
 This component enables multi-modal input for the Anthropic Claude v3 suite of models available from Amazon Bedrock
 """, elem_classes=["md-custom"], header_links=True)
     app.render()
     gr.Markdown(
 """
```

### Comparing `gradio_awsbedrock_multimodalchatbot-0.0.1/frontend/Index.svelte` & `gradio_awsbedrock_multimodalchatbot-0.0.2/frontend/Index.svelte`

 * *Files identical despite different names*

### Comparing `gradio_awsbedrock_multimodalchatbot-0.0.1/frontend/package-lock.json` & `gradio_awsbedrock_multimodalchatbot-0.0.2/frontend/package-lock.json`

 * *Files identical despite different names*

### Comparing `gradio_awsbedrock_multimodalchatbot-0.0.1/frontend/package.json` & `gradio_awsbedrock_multimodalchatbot-0.0.2/frontend/package.json`

 * *Files identical despite different names*

### Comparing `gradio_awsbedrock_multimodalchatbot-0.0.1/frontend/shared/ChatBot.svelte` & `gradio_awsbedrock_multimodalchatbot-0.0.2/frontend/shared/ChatBot.svelte`

 * *Files identical despite different names*

### Comparing `gradio_awsbedrock_multimodalchatbot-0.0.1/frontend/shared/Copy.svelte` & `gradio_awsbedrock_multimodalchatbot-0.0.2/frontend/shared/Copy.svelte`

 * *Files identical despite different names*

### Comparing `gradio_awsbedrock_multimodalchatbot-0.0.1/frontend/shared/LikeDislike.svelte` & `gradio_awsbedrock_multimodalchatbot-0.0.2/frontend/shared/LikeDislike.svelte`

 * *Files identical despite different names*

### Comparing `gradio_awsbedrock_multimodalchatbot-0.0.1/frontend/shared/Pending.svelte` & `gradio_awsbedrock_multimodalchatbot-0.0.2/frontend/shared/Pending.svelte`

 * *Files identical despite different names*

### Comparing `gradio_awsbedrock_multimodalchatbot-0.0.1/frontend/shared/utils.ts` & `gradio_awsbedrock_multimodalchatbot-0.0.2/frontend/shared/utils.ts`

 * *Files identical despite different names*

### Comparing `gradio_awsbedrock_multimodalchatbot-0.0.1/README.md` & `gradio_awsbedrock_multimodalchatbot-0.0.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 
 # `gradio_awsBedrock_multimodalChatbot`
-<img alt="Static Badge" src="https://img.shields.io/badge/version%20-%200.0.1%20-%20orange">  
+<a href="https://pypi.org/project/gradio_awsBedrock_multimodalChatbot/" target="_blank"><img alt="PyPI - Version" src="https://img.shields.io/pypi/v/gradio_awsBedrock_multimodalChatbot"></a>  
 
 This component enables multi-modal input for the Anthropic Claude v3 suite of models available from Amazon Bedrock
 
 ## Installation
 
 ```bash
 pip install gradio_awsBedrock_multimodalChatbot
```

### Comparing `gradio_awsbedrock_multimodalchatbot-0.0.1/pyproject.toml` & `gradio_awsbedrock_multimodalchatbot-0.0.2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -4,20 +4,20 @@
   "hatch-requirements-txt",
   "hatch-fancy-pypi-readme>=22.5.0",
 ]
 build-backend = "hatchling.build"
 
 [project]
 name = "gradio_awsBedrock_multimodalChatbot"
-version = "0.0.1"
+version = "0.0.2"
 description = "This component enables multi-modal input for the Anthropic Claude v3 suite of models available from Amazon Bedrock"
 readme = "README.md"
 license = "MIT"
 requires-python = ">=3.8"
-authors = [{ name = "Dakota Smith", email = "dakota.smith52@outlook.com" }]
+authors = [{ name = "Jedijamez", email = "" }]
 keywords = ["gradio-custom-component", "gradio-template-Chatbot", "AWS", "Bedrock", "Amazon Bedrock", "Anthropic", "LLM", "Chatbot", "Multimodal", "Claude", "Claude v3"]
 # Add dependencies here
 dependencies = ["gradio>=4.0,<5.0"]
 classifiers = [
   'Development Status :: 3 - Alpha',
   'License :: OSI Approved :: Apache Software License',
   'Operating System :: OS Independent',
@@ -32,11 +32,11 @@
   'Topic :: Scientific/Engineering :: Visualization',
 ]
 
 [project.optional-dependencies]
 dev = ["build", "twine"]
 
 [tool.hatch.build]
-artifacts = ["/backend/gradio_multimodalchatbot/templates", "*.pyi", "backend/gradio_multimodalchatbot/templates", "backend/gradio_multimodalchatbot/templates", "backend/gradio_multimodalchatbot/templates", "backend/gradio_multimodalchatbot/templates", "backend/gradio_multimodalchatbot/templates", "backend/gradio_multimodalchatbot/templates", "backend/gradio_multimodalchatbot/templates", "backend/gradio_multimodalchatbot/templates", "backend/gradio_awsBedrock_multimodalChatbot/templates"]
+artifacts = ["/backend/gradio_multimodalchatbot/templates", "*.pyi", "backend/gradio_multimodalchatbot/templates", "backend/gradio_multimodalchatbot/templates", "backend/gradio_multimodalchatbot/templates", "backend/gradio_multimodalchatbot/templates", "backend/gradio_multimodalchatbot/templates", "backend/gradio_multimodalchatbot/templates", "backend/gradio_multimodalchatbot/templates", "backend/gradio_multimodalchatbot/templates", "backend/gradio_awsBedrock_multimodalChatbot/templates", "backend/gradio_awsBedrock_multimodalChatbot/templates", "backend/gradio_awsBedrock_multimodalChatbot/templates", "backend/gradio_awsBedrock_multimodalChatbot/templates", "backend/gradio_awsBedrock_multimodalChatbot/templates"]
 
 [tool.hatch.build.targets.wheel]
 packages = ["/backend/gradio_multimodalchatbot"]
```

### Comparing `gradio_awsbedrock_multimodalchatbot-0.0.1/PKG-INFO` & `gradio_awsbedrock_multimodalchatbot-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.3
 Name: gradio_awsBedrock_multimodalChatbot
-Version: 0.0.1
+Version: 0.0.2
 Summary: This component enables multi-modal input for the Anthropic Claude v3 suite of models available from Amazon Bedrock
-Author-email: Dakota Smith <dakota.smith52@outlook.com>
+Author: Jedijamez
 License-Expression: MIT
 Keywords: AWS,Amazon Bedrock,Anthropic,Bedrock,Chatbot,Claude,Claude v3,LLM,Multimodal,gradio-custom-component,gradio-template-Chatbot
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
@@ -22,15 +22,15 @@
 Provides-Extra: dev
 Requires-Dist: build; extra == 'dev'
 Requires-Dist: twine; extra == 'dev'
 Description-Content-Type: text/markdown
 
 
 # `gradio_awsBedrock_multimodalChatbot`
-<img alt="Static Badge" src="https://img.shields.io/badge/version%20-%200.0.1%20-%20orange">  
+<a href="https://pypi.org/project/gradio_awsBedrock_multimodalChatbot/" target="_blank"><img alt="PyPI - Version" src="https://img.shields.io/pypi/v/gradio_awsBedrock_multimodalChatbot"></a>  
 
 This component enables multi-modal input for the Anthropic Claude v3 suite of models available from Amazon Bedrock
 
 ## Installation
 
 ```bash
 pip install gradio_awsBedrock_multimodalChatbot
```

