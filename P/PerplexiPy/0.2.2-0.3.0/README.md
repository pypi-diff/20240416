# Comparing `tmp/PerplexiPy-0.2.2-py3-none-any.whl.zip` & `tmp/PerplexiPy-0.3.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,12 +1,12 @@
-Zip file size: 9305 bytes, number of entries: 10
--rw-r--r--  2.0 unx     8810 b- defN 24-Mar-24 20:07 perplexipy/__init__.py
--rw-r--r--  2.0 unx     2347 b- defN 24-Mar-25 04:50 perplexipy/codex.py
+Zip file size: 10763 bytes, number of entries: 10
+-rw-r--r--  2.0 unx     9067 b- defN 24-Apr-16 02:09 perplexipy/__init__.py
+-rw-r--r--  2.0 unx     6928 b- defN 24-Apr-16 02:09 perplexipy/codex.py
 -rw-r--r--  2.0 unx      283 b- defN 24-Mar-01 20:13 perplexipy/errors.py
--rw-r--r--  2.0 unx      684 b- defN 24-Mar-24 20:04 perplexipy/responses.py
--rw-r--r--  2.0 unx     1514 b- defN 24-Mar-25 04:53 PerplexiPy-0.2.2.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx     6259 b- defN 24-Mar-25 04:53 PerplexiPy-0.2.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Mar-25 04:53 PerplexiPy-0.2.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       49 b- defN 24-Mar-25 04:53 PerplexiPy-0.2.2.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       11 b- defN 24-Mar-25 04:53 PerplexiPy-0.2.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      813 b- defN 24-Mar-25 04:53 PerplexiPy-0.2.2.dist-info/RECORD
-10 files, 20862 bytes uncompressed, 7913 bytes compressed:  62.1%
+-rw-r--r--  2.0 unx      684 b- defN 24-Apr-13 17:06 perplexipy/responses.py
+-rw-r--r--  2.0 unx     1514 b- defN 24-Apr-16 02:11 PerplexiPy-0.3.0.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx     6289 b- defN 24-Apr-16 02:11 PerplexiPy-0.3.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-16 02:11 PerplexiPy-0.3.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       49 b- defN 24-Apr-16 02:11 PerplexiPy-0.3.0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       11 b- defN 24-Apr-16 02:11 PerplexiPy-0.3.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      813 b- defN 24-Apr-16 02:11 PerplexiPy-0.3.0.dist-info/RECORD
+10 files, 25730 bytes uncompressed, 9371 bytes compressed:  63.6%
```

## zipnote {}

```diff
@@ -6,26 +6,26 @@
 
 Filename: perplexipy/errors.py
 Comment: 
 
 Filename: perplexipy/responses.py
 Comment: 
 
-Filename: PerplexiPy-0.2.2.dist-info/LICENSE.txt
+Filename: PerplexiPy-0.3.0.dist-info/LICENSE.txt
 Comment: 
 
-Filename: PerplexiPy-0.2.2.dist-info/METADATA
+Filename: PerplexiPy-0.3.0.dist-info/METADATA
 Comment: 
 
-Filename: PerplexiPy-0.2.2.dist-info/WHEEL
+Filename: PerplexiPy-0.3.0.dist-info/WHEEL
 Comment: 
 
-Filename: PerplexiPy-0.2.2.dist-info/entry_points.txt
+Filename: PerplexiPy-0.3.0.dist-info/entry_points.txt
 Comment: 
 
-Filename: PerplexiPy-0.2.2.dist-info/top_level.txt
+Filename: PerplexiPy-0.3.0.dist-info/top_level.txt
 Comment: 
 
-Filename: PerplexiPy-0.2.2.dist-info/RECORD
+Filename: PerplexiPy-0.3.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## perplexipy/__init__.py

```diff
@@ -1,10 +1,12 @@
 # See: https://github.com/CIME-Software/perplexipy/blob/master/LICENSE.txt
 
 
+from collections import OrderedDict
+
 import importlib.metadata
 
 
 __VERSION__ = importlib.metadata.version('PerplexiPy')
 
 
 """
@@ -134,14 +136,18 @@
             raise PerplexityClientError('query cannot be None or empty')
 
         messages = [ { 'role': self._role, 'content': query, }, ]
 
         response = self._client.chat.completions.create(
             model = self.model,
             messages = messages,
+            # TODO: check the OpenAI documentation to see how this is used.
+            # See:  https://docs.mistral.ai/platform/guardrailing/
+            # No guardrailing.
+            # safe_mode = False,
         )
 
         result = response.choices[0].message.content
 
         return result
 
 
@@ -240,23 +246,23 @@
         information attributes are:
 
         - `parameterCount`
         - `contextLength`
         - `modelType`
         - `availability`
         """
-        supportedModels = {
+        supportedModels = OrderedDict({
             'codellama-70b-instruct': ModelInfo('70B', 16384, 'chat completion', 'open source',),
             'mistral-7b-instruct': ModelInfo('7B', 16384, 'chat completion', 'open source',),
             'mixtral-8x7b-instruct': ModelInfo('8x7B', 16384, 'chat completion', 'open source',),
             'sonar-medium-chat': ModelInfo('8x7B', 16348, 'chat completion', 'Perplexity',),
             'sonar-medium-online': ModelInfo('8x7B', 12000, 'chat completion', 'Perplexity',),
             'sonar-small-chat': ModelInfo('7B', 16384, 'chat completion', 'Perplexity',),
             'sonar-small-online': ModelInfo('7B', 12000, 'chat completion', 'Perplexity',),
-        }
+        })
 
         return supportedModels
 
 
     @property
     def model(self) -> str:
         """
```

## perplexipy/codex.py

```diff
@@ -1,29 +1,65 @@
 # See: https://github.com/CIME-Software/perplexipy/blob/master/LICENSE.txt
 
 
+from prompt_toolkit import HTML
+from prompt_toolkit import PromptSession
+from prompt_toolkit import print_formatted_text as printF
+from prompt_toolkit.enums import EditingMode
+
 from perplexipy import PerplexityClient
 from perplexipy import __VERSION__
 
 import os
 import select
 import sys
 
 import click
 
 
+# *** constants ***
+
+ARG_REPL = 'repl'
+"""
+@private
+"""
+
+DEFAULT_LLM = 'mixtral-8x7b-instruct'
+DEFAULT_VIM_EDIT_MODE = True
+"""
+@private
+"""
+
+QUERY_CRISP = 'Concise, code only reply to this prompt: '
+"""
+@private
+"""
+
+QUERY_DETAILED = 'Give me a concise coding example and include URL references in reply this prompt: '
+"""
+@private
+"""
+
+
+# *** globals ***
+
+_client = PerplexityClient(key = os.environ['PERPLEXITY_API_KEY'])
+_client.model = DEFAULT_LLM
+_queryCodeStyle = True
+
+
 # *** implementation ***
 
 def _die(msg: str, exitCode: int = 99):
     click.echo(msg)
     sys.exit(99)
 
 
 def _helpUser() -> str:
-    return "Syntax: codex 'your coding question here in single quotes'\n"
+    return "Syntax: codex repl | 'your coding question here in single quotes'\n"
 
 
 def codexCore(userQuery: str) -> str:
     """
     Send a user query to the model for processing.
 
     Arguments
@@ -31,19 +67,22 @@
         userQuery
     A string with the user query, most often a programming question.
 
     Returns
     -------
     The result of the query, or `None` if the query was empty.
     """
+    global _client
+
     result = None
     if userQuery:
-        client = PerplexityClient(key = os.environ['PERPLEXITY_API_KEY'])
-        client.model = 'codellama-70b-instruct'
-        result = client.query(userQuery)
+        if not _client:
+            _client = PerplexityClient(key = os.environ['PERPLEXITY_API_KEY'])
+            _client.model = DEFAULT_LLM
+        result = _client.query(userQuery)
 
     return result
 
 
 def _stdinHasData() -> bool:
     """
     Checks if there's data pending to be processed off `stdin`.  It's a
@@ -60,14 +99,145 @@
     result = ''
     for line in sys.stdin:
         result += line
 
     return result
 
 
+def _activeModel(modelID: int = 0) -> str:
+    if modelID:
+        try:
+            ref = modelID-1
+            model = list(_client.models.keys())[ref]
+            _client.model = model
+        except:
+            click.secho('Invalid model ID = %s' % modelID, bg = 'red', fg = 'white')
+
+    click.secho('Active model: %s\n' % _client.model, fg = 'green', bold = True)
+
+
+def _REPLHello():
+    click.clear()
+    printF(HTML('PerplexiPy <b><ansigreen>codex playground - coding, scripting, and sysops assistant</ansigreen></b>'))
+    _activeModel()
+    printF(HTML('Enter <b>/help</b> for commands list'))
+    print()
+
+
+def _helpREPL():
+    print("""
+/active [modelID] - display active model or set active to modelID
+/clear - clear the screen
+/exit - end codex and return to the command prompt
+/help - this commands list help
+/mode [mode] - display or set the editing mode to vi or emacs
+/models - list available models; n = modelID
+/quit - alias for /exit
+/style [style] - display or set query style to code or human
+? - alias for /help
+""")
+
+
+def _displayModels() -> str:
+    _activeModel()
+    print('Available models:\n')
+    n = 1
+    for model in _client.models.keys():
+        print('%2d - %s' % (n, model))
+        n += 1
+    print()
+
+
+def _editingMode(session: PromptSession, mode = None):
+    if mode:
+        mode = mode.lower()
+        newEditingMode = EditingMode.EMACS if mode == 'emacs' else EditingMode.VI
+        session = PromptSession(editing_mode = newEditingMode)
+
+    editingMode = str(session.editing_mode).replace('EditingMode.', '').lower()
+    click.secho('Editing mode = %s' % editingMode, fg = 'bright_blue')
+
+    return session
+
+
+def _queryStyle(newStyle: str = None):
+    global _queryCodeStyle
+
+    if newStyle:
+        if 'human' == newStyle:
+            _queryCodeStyle = False
+        else:
+            _queryCodeStyle = True
+
+    click.secho('Coding query style = %s' % _queryCodeStyle, fg = 'bright_blue')
+
+
+def _makeQuery(userQuery: str) -> str:
+    if _queryCodeStyle:
+        userQuery = QUERY_DETAILED+userQuery
+
+    return codexCore(userQuery)
+
+
+def _runREPL() -> str:
+    """
+    Run a REPL loop for sending queries to the AI provider.
+
+    Returns
+    -------
+    The word "REPL" to signal to the `codex` command that it received valid
+    input.
+    """
+    _REPLHello()
+    session = PromptSession(vi_mode = True)
+    _editingMode(session)
+    while True:
+        userQuery = session.prompt('Ask anything (/exit to end): ')
+        if userQuery[0] in ('/', '?', ':'):
+            parts = userQuery.split(' ')
+            command = parts[0]
+            if command in ('/exit', '/quit', ':q', '/q'):
+                sys.exit(0)
+            elif command == '/active':
+                if len(parts) > 1:
+                    try:
+                        _activeModel(int(parts[1]))
+                    except:
+                        _activeModel()
+                else:
+                    _activeModel()
+            elif command == '/clear':
+                click.clear()
+                _editingMode(session)
+            elif command in ('/help', '?'):
+                _helpREPL()
+            elif command == '/mode':
+                if len(parts) > 1:
+                    try:
+                        session = _editingMode(session, parts[1])
+                    except:
+                        pass
+                else:
+                    _editingMode(session)
+            elif command == '/models':
+                _displayModels()
+            elif command == '/style':
+                if len(parts) > 1:
+                    _queryStyle(parts[1])
+                else:
+                    _queryStyle()
+            continue
+        result = _makeQuery(userQuery)
+        print('%s' % result)
+        print('--------------------------------------------------')
+        print()
+
+    return 'REPL'
+
+
 @click.command('codex')
 @click.version_option(__VERSION__, prog_name = 'codex')
 @click.argument('tokens', nargs = -1, type = click.STRING)
 def codex(tokens: list) -> str:
     """
     Process a command line query and display the result to the console.
 
@@ -81,18 +251,21 @@
     -------
     A string with the response to the query, after displaying it to the
     console.
     """
     result = None
     userQuery = None
     if len(tokens):
-        userQuery = 'Concise, code only answer to this question: '+' '.join(tokens)
+        if len(tokens) == 1 and tokens[0].lower() == ARG_REPL:
+            userQuery = _runREPL()
+        else:
+            userQuery = QUERY_CRISP+''.join(tokens)
     elif _stdinHasData():
         userQuery = _assembleInput()
-        userQuery = 'Give me a concise coding example to answer this question: '+userQuery
+        userQuery = QUERY_DETAILED+userQuery
 
     if userQuery:
         result = codexCore(userQuery)
         click.echo(result)
     else:
         _die(_helpUser(), 1)
```

## Comparing `PerplexiPy-0.2.2.dist-info/LICENSE.txt` & `PerplexiPy-0.3.0.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `PerplexiPy-0.2.2.dist-info/METADATA` & `PerplexiPy-0.3.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PerplexiPy
-Version: 0.2.2
+Version: 0.3.0
 Summary: PerplexiPy - A robust Perplexity AI API client
 Author-email: CIME Software Ltd <perplexipy@cime.net>
 License: BSD-3
 Project-URL: homepage, https://cime-software.github.io/perplexipy/
 Project-URL: Documentation, https://cime-software.github.io/perplexipy/
 Project-URL: Bug Tracker, https://github.com/CIME-Software/perplexipy/issues
 Project-URL: Source, https://github.com/CIME-Software/perplexipy
@@ -17,17 +17,18 @@
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 Requires-Dist: click
 Requires-Dist: openai (>=1.12.0)
+Requires-Dist: prompt-toolkit
 Requires-Dist: python-dotenv
 
-% perplexipy(3) Version 0.2.2 | Perplexity AI high level API documentation
+% perplexipy(3) Version 0.3.0 | Perplexity AI high level API documentation
 
 Name
 ====
 
 **PerplexiPy** - Perplexity AI high level library
```

### html2text {}

```diff
@@ -1,39 +1,39 @@
-Metadata-Version: 2.1 Name: PerplexiPy Version: 0.2.2 Summary: PerplexiPy - A
+Metadata-Version: 2.1 Name: PerplexiPy Version: 0.3.0 Summary: PerplexiPy - A
 robust Perplexity AI API client Author-email: CIME Software Ltd
 cime.net> License: BSD-3 Project-URL: homepage, https://cime-
 software.github.io/perplexipy/ Project-URL: Documentation, https://cime-
 software.github.io/perplexipy/ Project-URL: Bug Tracker, https://github.com/
 CIME-Software/perplexipy/issues Project-URL: Source, https://github.com/CIME-
 Software/perplexipy Classifier: Development Status :: 4 - Beta Classifier:
 Intended Audience :: Developers Classifier: License :: OSI Approved :: BSD
 License Classifier: Operating System :: OS Independent Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Python: >=3.9 Description-Content-Type: text/markdown License-File:
 LICENSE.txt Requires-Dist: click Requires-Dist: openai (>=1.12.0) Requires-
-Dist: python-dotenv % perplexipy(3) Version 0.2.2 | Perplexity AI high level
-API documentation Name ==== **PerplexiPy** - Perplexity AI high level library
-Synopsis ======== ```python client = PerplexityClient() \ print(client.query
-('What is the meaning of 42?') \ for result in client.queryStreamable('List of
-all US presidents'): \ print(result) ``` Description =========== **PerplexiPy**
-is a high-level, convenience library for interacting with the Perplexity API
-from any Python 3.9+ application. The library aims to simplify interactions
-with Perplexity models by encapsulating all the implementation details of the
-lower level OpenAI API. All interaction between the code and this library
-occurs in the form of string and native Python objects, not OpenAPI / Swagger
-mapped objects. **PerplexiPy** implements a combination of the Perplexity AI
-and the OpenAI outputs. API semantics follow the "literate programming"
-workflow, and attempt to make the resulting code as simple to follow as
-possible. _P_e_r_p_l_e_x_i_t_y_ _A_I is an AI-powered search engine that uses natural
-language processing and machine learning to provide accurate and comprehensive
-answers to end-user queries. It can be argued that it outperforms OpenAI's
-offerings in accuracy and responsiveness. **PerplexiPy** enables the creation
-of Python programs and tools that leverage the power of Perplexity AI.
+Dist: prompt-toolkit Requires-Dist: python-dotenv % perplexipy(3) Version 0.3.0
+| Perplexity AI high level API documentation Name ==== **PerplexiPy** -
+Perplexity AI high level library Synopsis ======== ```python client =
+PerplexityClient() \ print(client.query('What is the meaning of 42?') \ for
+result in client.queryStreamable('List of all US presidents'): \ print(result)
+``` Description =========== **PerplexiPy** is a high-level, convenience library
+for interacting with the Perplexity API from any Python 3.9+ application. The
+library aims to simplify interactions with Perplexity models by encapsulating
+all the implementation details of the lower level OpenAI API. All interaction
+between the code and this library occurs in the form of string and native
+Python objects, not OpenAPI / Swagger mapped objects. **PerplexiPy** implements
+a combination of the Perplexity AI and the OpenAI outputs. API semantics follow
+the "literate programming" workflow, and attempt to make the resulting code as
+simple to follow as possible. _P_e_r_p_l_e_x_i_t_y_ _A_I is an AI-powered search engine that
+uses natural language processing and machine learning to provide accurate and
+comprehensive answers to end-user queries. It can be argued that it outperforms
+OpenAI's offerings in accuracy and responsiveness. **PerplexiPy** enables the
+creation of Python programs and tools that leverage the power of Perplexity AI.
 Documentation ============= These documents encompass all information about
 **PerplexiPy**: - This README file, hosted in the **[perplexipy](https://
 github.com/CIME-Software/perplexipy)** GitHub repository project on GitHub and
 exported to the PyPI project page - A `man` page autogenerated from this README
 file, `perplexipy.3` - The complete **PerplexiPy API reference** on GitHub
 Pages - https://cime-software.github.io/perplexipy/perplexipy.html - The
 _P_e_r_p_l_e_x_i_P_y_-_t_u_t_o_r_i_a_l_._i_p_y_n_b tutorial notebook The `man` page can be generated
```

## Comparing `PerplexiPy-0.2.2.dist-info/RECORD` & `PerplexiPy-0.3.0.dist-info/RECORD`

 * *Files 23% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-perplexipy/__init__.py,sha256=ZrZuH_l_3Nt-Gy_4vHKBQ1NEiEc4C4UupCd_VcXODgY,8810
-perplexipy/codex.py,sha256=Y1ICzyX8zJep3o1m9UlucWdSMwUXH_s5GE5hQwW6LDY,2347
+perplexipy/__init__.py,sha256=YHI3TDJUnV8BIKHKojbwSo75NKX9i9xq4jmChr2EZH4,9067
+perplexipy/codex.py,sha256=saBLfO-9Cc5QJ2lkJELeBXIXuQRJUgqjt8wojxZaOeo,6928
 perplexipy/errors.py,sha256=YM4dVV9q2aLm_ZJdhyCjhejLXdo8mEffx93zlP_7lOs,283
 perplexipy/responses.py,sha256=1OrBpZxGHaVvlE5x9ZtdQhoXP5RbmKOXtHGt6Nm7g2I,684
-PerplexiPy-0.2.2.dist-info/LICENSE.txt,sha256=j9TykfeJa2xvP5Wmggfxaz8pTnedQO9BQX5PbJkh8Yc,1514
-PerplexiPy-0.2.2.dist-info/METADATA,sha256=mfshjqpw9fZDETI5OVDYverQJ1TKsB7vG47oLziLPis,6259
-PerplexiPy-0.2.2.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-PerplexiPy-0.2.2.dist-info/entry_points.txt,sha256=tRB7D5Ao_Rptera8eLiPoF9ecAvHbf5lFSYYaGs9Cfw,49
-PerplexiPy-0.2.2.dist-info/top_level.txt,sha256=JS_DtYqartG2-vkrCiFr0aeoy4Dg6my7DlmUA90wKhA,11
-PerplexiPy-0.2.2.dist-info/RECORD,,
+PerplexiPy-0.3.0.dist-info/LICENSE.txt,sha256=j9TykfeJa2xvP5Wmggfxaz8pTnedQO9BQX5PbJkh8Yc,1514
+PerplexiPy-0.3.0.dist-info/METADATA,sha256=yf4RRV8F98VQvr24AozVgbup9ghbaujAHPW1P_PGF04,6289
+PerplexiPy-0.3.0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+PerplexiPy-0.3.0.dist-info/entry_points.txt,sha256=tRB7D5Ao_Rptera8eLiPoF9ecAvHbf5lFSYYaGs9Cfw,49
+PerplexiPy-0.3.0.dist-info/top_level.txt,sha256=JS_DtYqartG2-vkrCiFr0aeoy4Dg6my7DlmUA90wKhA,11
+PerplexiPy-0.3.0.dist-info/RECORD,,
```

