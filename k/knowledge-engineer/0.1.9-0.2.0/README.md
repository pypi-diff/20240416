# Comparing `tmp/knowledge_engineer-0.1.9.tar.gz` & `tmp/knowledge_engineer-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "knowledge_engineer-0.1.9.tar", last modified: Mon Mar 11 05:32:54 2024, max compression
+gzip compressed data, was "knowledge_engineer-0.2.0.tar", last modified: Tue Apr 16 16:31:47 2024, max compression
```

## Comparing `knowledge_engineer-0.1.9.tar` & `knowledge_engineer-0.2.0.tar`

### file list

```diff
@@ -1,23 +1,24 @@
-drwxrwxr-x   0 jerry     (1000) jerry     (1000)        0 2024-03-11 05:32:54.227841 knowledge_engineer-0.1.9/
--rw-rw-r--   0 jerry     (1000) jerry     (1000)     1071 2024-02-14 05:51:20.000000 knowledge_engineer-0.1.9/LICENSE
--rw-r--r--   0 jerry     (1000) jerry     (1000)     2290 2024-03-11 05:32:54.227841 knowledge_engineer-0.1.9/PKG-INFO
--rw-rw-r--   0 jerry     (1000) jerry     (1000)     1827 2024-02-21 04:47:15.000000 knowledge_engineer-0.1.9/README.md
-drwxrwxr-x   0 jerry     (1000) jerry     (1000)        0 2024-03-11 05:32:54.227841 knowledge_engineer-0.1.9/knowledge_engineer/
--rw-rw-r--   0 jerry     (1000) jerry     (1000)     2432 2024-03-06 01:06:20.000000 knowledge_engineer-0.1.9/knowledge_engineer/AI_API_Costs.py
--rw-rw-r--   0 jerry     (1000) jerry     (1000)        0 2024-02-14 05:51:20.000000 knowledge_engineer-0.1.9/knowledge_engineer/__init__.py
--rw-rw-r--   0 jerry     (1000) jerry     (1000)    15111 2024-03-11 05:19:05.000000 knowledge_engineer-0.1.9/knowledge_engineer/ai.py
--rw-rw-r--   0 jerry     (1000) jerry     (1000)     3771 2024-03-11 05:19:06.000000 knowledge_engineer-0.1.9/knowledge_engineer/create_new_process.py
--rw-rw-r--   0 jerry     (1000) jerry     (1000)     8985 2024-03-05 11:05:42.000000 knowledge_engineer-0.1.9/knowledge_engineer/db.py
--rw-rw-r--   0 jerry     (1000) jerry     (1000)     9259 2024-03-05 23:36:30.000000 knowledge_engineer-0.1.9/knowledge_engineer/ke.py
--rw-rw-r--   0 jerry     (1000) jerry     (1000)     8217 2024-03-05 00:26:02.000000 knowledge_engineer-0.1.9/knowledge_engineer/line_statement.py
--rw-rw-r--   0 jerry     (1000) jerry     (1000)     4934 2024-03-09 04:27:18.000000 knowledge_engineer-0.1.9/knowledge_engineer/logger.py
--rw-rw-r--   0 jerry     (1000) jerry     (1000)     4436 2024-03-05 23:36:30.000000 knowledge_engineer-0.1.9/knowledge_engineer/step.py
--rw-rw-r--   0 jerry     (1000) jerry     (1000)      360 2024-03-05 12:27:53.000000 knowledge_engineer-0.1.9/knowledge_engineer/version.py
-drwxrwxr-x   0 jerry     (1000) jerry     (1000)        0 2024-03-11 05:32:54.227841 knowledge_engineer-0.1.9/knowledge_engineer.egg-info/
--rw-r--r--   0 jerry     (1000) jerry     (1000)     2290 2024-03-11 05:32:54.000000 knowledge_engineer-0.1.9/knowledge_engineer.egg-info/PKG-INFO
--rw-rw-r--   0 jerry     (1000) jerry     (1000)      560 2024-03-11 05:32:54.000000 knowledge_engineer-0.1.9/knowledge_engineer.egg-info/SOURCES.txt
--rw-rw-r--   0 jerry     (1000) jerry     (1000)        1 2024-03-11 05:32:54.000000 knowledge_engineer-0.1.9/knowledge_engineer.egg-info/dependency_links.txt
--rw-rw-r--   0 jerry     (1000) jerry     (1000)       66 2024-03-11 05:32:54.000000 knowledge_engineer-0.1.9/knowledge_engineer.egg-info/entry_points.txt
--rw-rw-r--   0 jerry     (1000) jerry     (1000)       19 2024-03-11 05:32:54.000000 knowledge_engineer-0.1.9/knowledge_engineer.egg-info/top_level.txt
--rw-rw-r--   0 jerry     (1000) jerry     (1000)      104 2024-02-14 05:51:20.000000 knowledge_engineer-0.1.9/pyproject.toml
--rw-rw-r--   0 jerry     (1000) jerry     (1000)      645 2024-03-11 05:32:54.231842 knowledge_engineer-0.1.9/setup.cfg
+drwxrwxr-x   0 jerry     (1000) jerry     (1000)        0 2024-04-16 16:31:47.594835 knowledge_engineer-0.2.0/
+-rw-rw-r--   0 jerry     (1000) jerry     (1000)     1071 2024-04-03 04:15:47.000000 knowledge_engineer-0.2.0/LICENSE
+-rw-r--r--   0 jerry     (1000) jerry     (1000)     2482 2024-04-16 16:31:47.594835 knowledge_engineer-0.2.0/PKG-INFO
+-rw-rw-r--   0 jerry     (1000) jerry     (1000)     1827 2024-04-03 04:15:47.000000 knowledge_engineer-0.2.0/README.md
+drwxrwxr-x   0 jerry     (1000) jerry     (1000)        0 2024-04-16 16:31:47.590835 knowledge_engineer-0.2.0/knowledge_engineer/
+-rw-rw-r--   0 jerry     (1000) jerry     (1000)     2432 2024-04-03 04:15:47.000000 knowledge_engineer-0.2.0/knowledge_engineer/AI_API_Costs.py
+-rw-rw-r--   0 jerry     (1000) jerry     (1000)        0 2024-04-03 04:15:47.000000 knowledge_engineer-0.2.0/knowledge_engineer/__init__.py
+-rw-rw-r--   0 jerry     (1000) jerry     (1000)    15290 2024-04-03 04:15:47.000000 knowledge_engineer-0.2.0/knowledge_engineer/ai.py
+-rw-rw-r--   0 jerry     (1000) jerry     (1000)     3771 2024-04-03 04:38:09.000000 knowledge_engineer-0.2.0/knowledge_engineer/create_new_process.py
+-rw-rw-r--   0 jerry     (1000) jerry     (1000)     8985 2024-04-03 04:15:47.000000 knowledge_engineer-0.2.0/knowledge_engineer/db.py
+-rw-rw-r--   0 jerry     (1000) jerry     (1000)     9259 2024-04-03 04:15:47.000000 knowledge_engineer-0.2.0/knowledge_engineer/ke.py
+-rw-rw-r--   0 jerry     (1000) jerry     (1000)     8217 2024-04-03 04:15:47.000000 knowledge_engineer-0.2.0/knowledge_engineer/line_statement.py
+-rw-rw-r--   0 jerry     (1000) jerry     (1000)     6240 2024-04-03 04:15:47.000000 knowledge_engineer-0.2.0/knowledge_engineer/logger.py
+-rw-rw-r--   0 jerry     (1000) jerry     (1000)     4436 2024-04-03 04:15:47.000000 knowledge_engineer-0.2.0/knowledge_engineer/step.py
+-rw-rw-r--   0 jerry     (1000) jerry     (1000)      360 2024-04-03 04:15:47.000000 knowledge_engineer-0.2.0/knowledge_engineer/version.py
+drwxrwxr-x   0 jerry     (1000) jerry     (1000)        0 2024-04-16 16:31:47.594835 knowledge_engineer-0.2.0/knowledge_engineer.egg-info/
+-rw-r--r--   0 jerry     (1000) jerry     (1000)     2482 2024-04-16 16:31:47.000000 knowledge_engineer-0.2.0/knowledge_engineer.egg-info/PKG-INFO
+-rw-rw-r--   0 jerry     (1000) jerry     (1000)      601 2024-04-16 16:31:47.000000 knowledge_engineer-0.2.0/knowledge_engineer.egg-info/SOURCES.txt
+-rw-rw-r--   0 jerry     (1000) jerry     (1000)        1 2024-04-16 16:31:47.000000 knowledge_engineer-0.2.0/knowledge_engineer.egg-info/dependency_links.txt
+-rw-rw-r--   0 jerry     (1000) jerry     (1000)       66 2024-04-16 16:31:47.000000 knowledge_engineer-0.2.0/knowledge_engineer.egg-info/entry_points.txt
+-rw-rw-r--   0 jerry     (1000) jerry     (1000)       70 2024-04-16 16:31:47.000000 knowledge_engineer-0.2.0/knowledge_engineer.egg-info/requires.txt
+-rw-rw-r--   0 jerry     (1000) jerry     (1000)       19 2024-04-16 16:31:47.000000 knowledge_engineer-0.2.0/knowledge_engineer.egg-info/top_level.txt
+-rw-rw-r--   0 jerry     (1000) jerry     (1000)      737 2024-04-16 16:22:25.000000 knowledge_engineer-0.2.0/pyproject.toml
+-rw-rw-r--   0 jerry     (1000) jerry     (1000)      627 2024-04-16 16:31:47.594835 knowledge_engineer-0.2.0/setup.cfg
```

### Comparing `knowledge_engineer-0.1.9/LICENSE` & `knowledge_engineer-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `knowledge_engineer-0.1.9/PKG-INFO` & `knowledge_engineer-0.2.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,27 @@
 Metadata-Version: 2.1
 Name: knowledge_engineer
-Version: 0.1.9
+Version: 0.2.0
 Summary: Engineer GPT Knowledge within a process
 Home-page: https://github.com/JerryWestrick/Knowledge_Engineer
 Author: Jerry Westrick
-Author-email: jerry@westrick.com
+Author-email: Jerry Westrick <jerry@westrick.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: rich
+Requires-Dist: openai
+Requires-Dist: mistralai
+Requires-Dist: python-dotenv
+Requires-Dist: lark
+Requires-Dist: databases
+Requires-Dist: knowledge_engineer
 
 # Knowledge Engineer
 
 ***Command Line Program allowing for the Engineering of Knowledge for LLM's.***
```

### Comparing `knowledge_engineer-0.1.9/README.md` & `knowledge_engineer-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `knowledge_engineer-0.1.9/knowledge_engineer/AI_API_Costs.py` & `knowledge_engineer-0.2.0/knowledge_engineer/AI_API_Costs.py`

 * *Files identical despite different names*

### Comparing `knowledge_engineer-0.1.9/knowledge_engineer/ai.py` & `knowledge_engineer-0.2.0/knowledge_engineer/ai.py`

 * *Files 5% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 os_descriptor = platform.platform()
 
 
 class AI:
     log = Logger(namespace='AI', debug=True)
     log_a = Logger(namespace="Assistant", debug=True)
     memory = DB()
-    client = None
 
     def __init__(self, llm_name: str, model: str = "gpt-3.5-turbo-1106",
                  temperature: float = 0, max_tokens: int = 4000,
                  mode: str = 'complete', response_format=None):
         self.tools = None
         self.answer: str = ''
         self.llm_name: str = llm_name
@@ -49,17 +48,18 @@
             'total_tokens': 0.0,
             'sp_cost': 0.0,
             'sc_cost': 0.0,
             's_total': 0.0,
             'elapsed_time': 0.0,
         }
         self.db: Database | None = None
+        self.client = None
 
     def function_role(self) -> str:
-        if self.llm_name.lower() == 'Mistral':
+        if self.llm_name.lower() == 'mistral':
             return 'tool'
         return 'function'
 
     async def query_db_ai(self, sql: str, process_name: str):
 
         if self.db is None:
             self.db = Database(os.getenv('KE_PROC_DB_URL'))
@@ -206,22 +206,22 @@
         raise ValueError(f"Unknown LLM: {self.llm_name}")
 
     async def generate(self, step, user_messages: list[dict[str, str]], process_name: str):
 
         self.answer = f'Log of Step: {step.name} : {step.prompt_name}\n'
         pricing = AI_API_Costs[self.model]
 
-        if AI.client is None:
-            if self.llm_name == 'OpenAI':
-                AI.client = AsyncOpenAI()
-                AI.client.api_key = os.getenv('OPENAI_API_KEY')
+        if self.client is None:
+            if self.llm_name.lower() == 'openai':
+                self.client = AsyncOpenAI()
+                self.client.api_key = os.getenv('OPENAI_API_KEY')
 
-            elif self.llm_name == 'Mistral':
+            elif self.llm_name.lower() == 'mistral':
                 api_key = os.getenv('MISTRAL_API_KEY')
-                AI.client = MistralAsyncClient(api_key=api_key)
+                self.client = MistralAsyncClient(api_key=api_key)
 
             else:
                 raise ValueError(f"Unknown LLM: {self.llm_name}")
 
         box_open = False
 
         while user_messages:
@@ -273,15 +273,15 @@
             raise ValueError(f"Unknown LLM: {self.llm_name}")
 
         # self.log.info(f"Calling {self.model} chat with messages: ")
         # self.log.info(messages)
 
     async def chat_openai(self, messages: list[dict[str, str]], step, process_name):
         try:
-            response = await AI.client.chat.completions.create(
+            response = await self.client.chat.completions.create(
                 messages=messages,
                 model=self.model,
                 temperature=self.temperature,
                 functions=self.functions,
                 function_call="auto",
                 response_format=self.response_format)
         except Exception as err:
@@ -326,62 +326,64 @@
             self.e_stats['completion_tokens'] + response.usage.completion_tokens
 
         return repeat
 
     async def chat_mistral(self, messages: list[dict[str, str]], step, process_name):
         if self.tools is None:
             self.tools = [{"type": "function", "function": x} for x in self.functions]
-        try:
-            response = await AI.client.chat(
-                model=self.model,
-                messages=messages,
-                tools=self.tools,
-                tool_choice="auto",
-                response_format=self.response_format,
-            )
-        except Exception as err:
-            err_msg = f"Call to Mistral returned error: {err} ai.py line: {err.__traceback__.tb_lineno}"
-            self.log.error(err_msg)
-            response = {'role': 'system', 'error': err_msg}
-            # raise
-        response_message = response.choices[0].message
-        repeat = False
-        function_name = None
-        function_args = None
-        if response.choices[0].finish_reason == 'tool_calls':
-            function_call = response.choices[0].message.tool_calls[0].function
-            function_name = function_call.name
-            function_args = json.loads(function_call.arguments)
-            response_message = response.choices[0].message
-        else:
-            self.answer = f"{self.answer}\n\n - {response_message.content}"
+        repeat = True
+        while repeat:
+            repeat = False
+            # Call Mistral
+            try:
+                response = await self.client.chat(
+                    model=self.model,
+                    messages=messages,
+                    tools=self.tools,
+                    tool_choice="auto",
+                    response_format=self.response_format,
+                )
+            except Exception as err:
+                err_msg = f"Call to Mistral returned error: {err} ai.py line: {err.__traceback__.tb_lineno}"
+                self.log.error(err_msg)
+                response = {'role': 'system', 'error': err_msg}
+                raise Exception(err_msg)
 
-        self.messages.append(response_message)
-        self.log.ai_msg(step, response_message)  # Display with last message
-        if function_name:
-            new_msg = await self.available_functions[function_name](self, **function_args,
-                                                                    process_name=process_name)
-            self.messages.append(self.make_msg(new_msg))
-            self.log.ret_msg(step, new_msg)
-            repeat = True
-        else:
-            if response_message.content and response_message.content.lower().endswith("if you want to proceed?"):
+            response_message = response.choices[0].message
+            self.messages.append(response_message)
+            function_name = None
+            function_args = None
+            if response.choices[0].finish_reason == 'tool_calls':
+                for tool_call in response_message.tool_calls:
+                    function_call = tool_call.function
+                    function_name = function_call.name
+                    function_args = json.loads(function_call.arguments)
+                    self.log.ai_tool_call(step, tool_call)
+                    rtn = self.available_functions[function_name]
+                    new_msg = await rtn(self, **function_args, process_name=process_name)
+                    self.messages.append(ChatMessage(**new_msg))
+                    self.log.ret_msg(step, new_msg)
                 repeat = True
-                msg = {'role': 'user', 'content': 'Proceed.'}
-                self.messages.append(self.make_msg(msg))
-                self.log.umsg(step, msg)
+            else:
+                self.log.ai_msg(step, response_message)
+                self.answer = f"{self.answer}\n\n - {response_message.content}"
+                if response_message.content and response_message.content.lower().endswith("if you want to proceed?"):
+                    repeat = True
+                    msg = {'role': 'user', 'content': 'Proceed.'}
+                    self.messages.append(ChatMessage(**msg))
+                    self.log.umsg(step, msg)
 
-        # Gather Answer
-        self.e_stats['prompt_tokens'] = \
-            self.e_stats['prompt_tokens'] + response.usage.prompt_tokens
-        self.e_stats['completion_tokens'] = \
-            self.e_stats['completion_tokens'] + response.usage.completion_tokens
+            # Gather Answer
+            self.e_stats['prompt_tokens'] = \
+                self.e_stats['prompt_tokens'] + response.usage.prompt_tokens
+            self.e_stats['completion_tokens'] = \
+                self.e_stats['completion_tokens'] + response.usage.completion_tokens
+
+        return False
 
-        # AI.log.info(f"{self.model} chat Response")
-        return repeat
 
     def to_json(self) -> dict:
         return {
             'model': self.model,
             'temperature': self.temperature,
             'max_tokens': self.max_tokens,
             'mode': self.mode,
```

### Comparing `knowledge_engineer-0.1.9/knowledge_engineer/create_new_process.py` & `knowledge_engineer-0.2.0/knowledge_engineer/create_new_process.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
  - list all the rules to be implemented
  - implement all the requirements in the prompts
 Write the prompt to 'Planning/Gen_Code_Prompt.md' using function 'write_file'.
 .exec
 """,
 
     # ==========================================
-    '2- Make Snake Game.kepf':
+    '2- Make Mines Game.kepf':
         """.llm "llm_name": "OpenAI", "model": "gpt-4-0125-preview", "max_tokens": 50000
 
 .system
 You are an IT Engineer, programming a Python 3 Application
 Do not explain yourself.
 Do not apologize.
 Check all code for completeness, correctness, and make sure it is executable.
```

### Comparing `knowledge_engineer-0.1.9/knowledge_engineer/db.py` & `knowledge_engineer-0.2.0/knowledge_engineer/db.py`

 * *Files identical despite different names*

### Comparing `knowledge_engineer-0.1.9/knowledge_engineer/ke.py` & `knowledge_engineer-0.2.0/knowledge_engineer/ke.py`

 * *Files identical despite different names*

### Comparing `knowledge_engineer-0.1.9/knowledge_engineer/line_statement.py` & `knowledge_engineer-0.2.0/knowledge_engineer/line_statement.py`

 * *Files identical despite different names*

### Comparing `knowledge_engineer-0.1.9/knowledge_engineer/logger.py` & `knowledge_engineer-0.2.0/knowledge_engineer/logger.py`

 * *Files 16% similar despite different names*

```diff
@@ -101,14 +101,39 @@
                 self.p(f"{self.ts()}{head}{fn} ({lines[0]}, ...)[green]{lines[:2]}[/]")
             else:
                 self.p(f"{self.ts()}{head}{fn} ({args['name']}, ...)[green]{[arg_str]}[/]")
 
         else:
             self.p(f"{self.ts()}{head}[deep_sky_blue1]{'AI message':>14}[/] [green]{content}[/]")
 
+    def ai_tool_call(self, step, tool):
+
+        head = f"[green]{self.namespace:>10}::[/][white]│ [/][green]│ [/]"
+
+        func_name = tool.function.name
+        arg_str = tool.function.arguments
+
+        args = json.loads(arg_str)
+        fn = f"[deep_sky_blue1]{func_name:>14}[/]"
+
+        func_name_actions = {
+            'read_file': lambda: self.p(f"{self.ts()}{head}{fn} ({args['name']})"),
+            'write_file': lambda: self.p(f"{self.ts()}{head}{fn} ({args['name']}, ...)[green]{[arg_str]}[/]"),
+            'replace': lambda: self.p(f"{self.ts()}{head}{fn} ({args['name']}, ...)[green]{[arg_str]}[/]"),
+            'patch': lambda: [self.p(f"{self.ts()}{head}{fn} ({line}, ...)[green]{line[:2]}[/]") for line in
+                              args['patch_commands'].split('\n')],
+            'exec': lambda: [self.p(f"{self.ts()}{head}{fn} ({line}, ...)[green]{line[:2]}[/]") for line in
+                             args['command'].split('\n')],
+            'query_db': lambda: [self.p(f"{self.ts()}{head}{fn} ({line}, ...)[green]{line[:2]}[/]") for line in
+                                 args['sql'].split('\n')]
+        }
+
+        func_name_actions.get(func_name,
+                              lambda: self.p(f"{self.ts()}{head}{fn} ({args['name']}, ...)[green]{[arg_str]}[/]"))()
+
     def ret_msg(self, step, msg: dict):
         hcolor = 'green'
         role = msg['role']
         hrole = f"({role:9})"
         content = [f"{msg['content']}"]
 
         head = f"[green]{self.namespace:>10}::[/][white]│ [/][green]│ [/]"
```

### Comparing `knowledge_engineer-0.1.9/knowledge_engineer/step.py` & `knowledge_engineer-0.2.0/knowledge_engineer/step.py`

 * *Files identical despite different names*

### Comparing `knowledge_engineer-0.1.9/knowledge_engineer.egg-info/PKG-INFO` & `knowledge_engineer-0.2.0/knowledge_engineer.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,20 +1,27 @@
 Metadata-Version: 2.1
 Name: knowledge_engineer
-Version: 0.1.9
+Version: 0.2.0
 Summary: Engineer GPT Knowledge within a process
 Home-page: https://github.com/JerryWestrick/Knowledge_Engineer
 Author: Jerry Westrick
-Author-email: jerry@westrick.com
+Author-email: Jerry Westrick <jerry@westrick.com>
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: rich
+Requires-Dist: openai
+Requires-Dist: mistralai
+Requires-Dist: python-dotenv
+Requires-Dist: lark
+Requires-Dist: databases
+Requires-Dist: knowledge_engineer
 
 # Knowledge Engineer
 
 ***Command Line Program allowing for the Engineering of Knowledge for LLM's.***
```

### Comparing `knowledge_engineer-0.1.9/knowledge_engineer.egg-info/SOURCES.txt` & `knowledge_engineer-0.2.0/knowledge_engineer.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -12,8 +12,9 @@
 knowledge_engineer/logger.py
 knowledge_engineer/step.py
 knowledge_engineer/version.py
 knowledge_engineer.egg-info/PKG-INFO
 knowledge_engineer.egg-info/SOURCES.txt
 knowledge_engineer.egg-info/dependency_links.txt
 knowledge_engineer.egg-info/entry_points.txt
+knowledge_engineer.egg-info/requires.txt
 knowledge_engineer.egg-info/top_level.txt
```

### Comparing `knowledge_engineer-0.1.9/setup.cfg` & `knowledge_engineer-0.2.0/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 [metadata]
 name = knowledge_engineer
-version = 0.1.9
+version = 0.2.0
 author = Jerry Westrick
 author_email = jerry@westrick.com
 description = Engineer GPT Knowledge within a process
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/JerryWestrick/Knowledge_Engineer
 classifiers = 
 	Programming Language :: Python :: 3
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 
 [options]
-packages = find:
 python_requires = >=3.10
-include_package_data = False
+include_package_data = True
 
 [options.entry_points]
 console_scripts = 
 	knowledge-engineer = knowledge_engineer.ke:main
 
 [egg_info]
 tag_build =
```

