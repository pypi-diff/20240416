# Comparing `tmp/dotprompt-0.1.1.tar.gz` & `tmp/dotprompt-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dotprompt-0.1.1.tar", last modified: Mon Apr 15 10:54:13 2024, max compression
+gzip compressed data, was "dotprompt-0.1.6.tar", last modified: Tue Apr 16 16:02:38 2024, max compression
```

## Comparing `dotprompt-0.1.1.tar` & `dotprompt-0.1.6.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 10:54:13.946799 dotprompt-0.1.1/
--rw-rw-rw-   0        0        0    35823 2024-04-15 08:48:14.000000 dotprompt-0.1.1/LICENSE
--rw-rw-rw-   0        0        0    42080 2024-04-15 10:54:13.945800 dotprompt-0.1.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-15 10:54:13.921815 dotprompt-0.1.1/dotprompt/
--rw-rw-rw-   0        0        0     1078 2024-04-15 10:48:03.000000 dotprompt-0.1.1/dotprompt/__init__.py
--rw-rw-rw-   0        0        0      145 2024-04-15 08:36:08.000000 dotprompt-0.1.1/dotprompt/exceptions.py
--rw-rw-rw-   0        0        0     2765 2024-04-15 10:52:34.000000 dotprompt-0.1.1/dotprompt/prompt.py
-drwxrwxrwx   0        0        0        0 2024-04-15 10:54:13.942802 dotprompt-0.1.1/dotprompt.egg-info/
--rw-rw-rw-   0        0        0    42080 2024-04-15 10:54:13.000000 dotprompt-0.1.1/dotprompt.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      261 2024-04-15 10:54:13.000000 dotprompt-0.1.1/dotprompt.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 10:54:13.000000 dotprompt-0.1.1/dotprompt.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       44 2024-04-15 10:54:13.000000 dotprompt-0.1.1/dotprompt.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-04-15 10:54:13.000000 dotprompt-0.1.1/dotprompt.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1280 2024-04-15 10:53:57.000000 dotprompt-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-15 10:54:13.947799 dotprompt-0.1.1/setup.cfg
--rw-rw-rw-   0        0        0      221 2024-04-15 10:53:57.000000 dotprompt-0.1.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-16 16:02:38.396535 dotprompt-0.1.6/
+-rw-rw-rw-   0        0        0    35823 2024-04-15 08:48:14.000000 dotprompt-0.1.6/LICENSE
+-rw-rw-rw-   0        0        0    44844 2024-04-16 16:02:38.395536 dotprompt-0.1.6/PKG-INFO
+-rw-rw-rw-   0        0        0     2760 2024-04-15 08:36:09.000000 dotprompt-0.1.6/README.md
+drwxrwxrwx   0        0        0        0 2024-04-16 16:02:38.372551 dotprompt-0.1.6/dotprompt/
+-rw-rw-rw-   0        0        0     1600 2024-04-16 16:02:05.000000 dotprompt-0.1.6/dotprompt/__init__.py
+-rw-rw-rw-   0        0        0      145 2024-04-15 08:36:08.000000 dotprompt-0.1.6/dotprompt/exceptions.py
+-rw-rw-rw-   0        0        0     2765 2024-04-15 10:52:34.000000 dotprompt-0.1.6/dotprompt/prompt.py
+drwxrwxrwx   0        0        0        0 2024-04-16 16:02:38.392538 dotprompt-0.1.6/dotprompt.egg-info/
+-rw-rw-rw-   0        0        0    44844 2024-04-16 16:02:38.000000 dotprompt-0.1.6/dotprompt.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      271 2024-04-16 16:02:38.000000 dotprompt-0.1.6/dotprompt.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-16 16:02:38.000000 dotprompt-0.1.6/dotprompt.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       44 2024-04-16 16:02:38.000000 dotprompt-0.1.6/dotprompt.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-16 16:02:38.000000 dotprompt-0.1.6/dotprompt.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1280 2024-04-16 16:02:20.000000 dotprompt-0.1.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-16 16:02:38.396535 dotprompt-0.1.6/setup.cfg
+-rw-rw-rw-   0        0        0      221 2024-04-16 16:02:20.000000 dotprompt-0.1.6/setup.py
```

### Comparing `dotprompt-0.1.1/LICENSE` & `dotprompt-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `dotprompt-0.1.1/PKG-INFO` & `dotprompt-0.1.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dotprompt
-Version: 0.1.1
+Version: 0.1.6
 Summary: Module to incorporate .prompt file to your python code for GenAI
 Author-email: AKoscianski <arnaud.koscianski@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -690,7 +690,102 @@
 License-File: LICENSE
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: bumpver; extra == "dev"
 Requires-Dist: isort; extra == "dev"
 Requires-Dist: pip-tools; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
+
+# Dotprompt
+
+Dotprompt is a simple library allowing to store your GenAI prompts as .prompt files. 
+It is a simple way to keep your prompts organized and easily accessible alongside your python code.
+
+## How to use
+Store your prompts as .prompts or .jprompt files in a prompts folder in your at the root of your code directory.
+Exemple :
+```
+my_project/
+    my_code.py
+    prompts/
+        my_prompt.system.prompt
+        not_specific.prompt
+        my_other_prompt.jprompt
+```
+
+Then simply import dotprompt in your code and get your prompts as object of dotprompts
+
+```python
+import dotprompt
+
+...
+
+res = gen_ai_client.complete(dotprompt.my_prompt.system)
+```
+
+When getting a prompt, the library return it as a string and you can use variables to enrich it.
+```my_prompt.system.prompt
+/* A system prompt with variables {speciality} and {age} */
+You are an AI specialized in {speciality}. You are {age} years old.
+```
+```python
+import dotprompt
+
+res = genai_client.complete(
+    prompt = dotprompt.my_prompt.system.format(
+        speciality = "medicine",
+        age = 3
+    )
+)
+```
+
+When comments have been add to the prompt files, the dotprompt store it in the info attribute of the prompt object.
+```python
+import dotprompt
+
+print(dotprompt.my_prompt.info['system'])
+>>>"A system prompt with variables {speciality} and {age}"
+```
+
+
+## Files format
+### .prompt
+The .prompt file format is a simple text file containing the prompt as a string.
+
+It uses a second extension to specify the type of prompt in the file.
+
+Example:
+If you have a prompt with a system prompt and a user prompt, you'll make two files as follows:
+- my_prompt.system.prompt
+- my_prompt.user.prompt
+
+And you'll be able to access them as follows:
+```python
+import dotprompt
+
+res = gen_ai_client.complete(
+    prompt = {
+        "system": dotprompt.my_prompt.system, 
+        "user": dotprompt.my_prompt.user
+    })
+```
+
+If you don't provide a second extension in the prompt file name, the prompt will be considered as a "prompt".
+```python
+import dotprompt
+
+...
+res = gen_ai_client.complete(dotprompt.not_specific.prompt)
+```
+
+The .prompt files can contain comments at the beginning of the file, between /* and */ characters. 
+The comments will be stored in the info attribute of the prompt object and will not be displayed as part of the prompt.
+
+### .jprompt
+The .jprompt file format is a json file containing multiple prompts with the specified type.
+```json
+{
+    "system": "You are an AI specialized in {speciality}. You are {age} years old.",
+    "user": "Tells me about the studies to be come an expert in {speciality}."
+}
+```
+The jprompt can be commented the same way as the .prompt files.
```

### Comparing `dotprompt-0.1.1/dotprompt/__init__.py` & `dotprompt-0.1.6/dotprompt/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,19 +1,32 @@
 import logging
 import os
+import inspect
+import sys
 from .prompt import Prompt
 from .exceptions import PrompDirectoryNotFoundError, PromptError
 
 
 IGNORED_EXT = ['py']
 
 
 logging.info("Loading prompt files")
 __prompt_dir =os.path.join(os.getcwd(), 'prompts')
 if not os.path.isdir(__prompt_dir):
+    not_found = True
+    ROOT_DIR = os.path.abspath(os.curdir)
+    caller_path = os.path.dirname(sys.argv[0])
+    while not_found:
+        if "prompts" in os.listdir(caller_path):
+            __prompt_dir = os.path.join(caller_path, "prompts")
+            not_found = False
+        elif caller_path == ROOT_DIR:
+            raise PrompDirectoryNotFoundError(f"No prompt dir found in {ROOT_DIR}")
+        caller_path = os.path.dirname(caller_path)
+if not os.path.isdir(__prompt_dir):
     raise PrompDirectoryNotFoundError("Prompt directory \"prompts\" not found")
 for f in os.listdir(__prompt_dir):
     parts = f.split('.')
     if parts[-1] == "prompt":
         if parts[0] in globals():
             globals()[parts[0]].add_file(os.path.join(__prompt_dir, f))
         else:
```

### Comparing `dotprompt-0.1.1/dotprompt/prompt.py` & `dotprompt-0.1.6/dotprompt/prompt.py`

 * *Files identical despite different names*

### Comparing `dotprompt-0.1.1/dotprompt.egg-info/PKG-INFO` & `dotprompt-0.1.6/dotprompt.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dotprompt
-Version: 0.1.1
+Version: 0.1.6
 Summary: Module to incorporate .prompt file to your python code for GenAI
 Author-email: AKoscianski <arnaud.koscianski@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
@@ -690,7 +690,102 @@
 License-File: LICENSE
 Provides-Extra: dev
 Requires-Dist: black; extra == "dev"
 Requires-Dist: bumpver; extra == "dev"
 Requires-Dist: isort; extra == "dev"
 Requires-Dist: pip-tools; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
+
+# Dotprompt
+
+Dotprompt is a simple library allowing to store your GenAI prompts as .prompt files. 
+It is a simple way to keep your prompts organized and easily accessible alongside your python code.
+
+## How to use
+Store your prompts as .prompts or .jprompt files in a prompts folder in your at the root of your code directory.
+Exemple :
+```
+my_project/
+    my_code.py
+    prompts/
+        my_prompt.system.prompt
+        not_specific.prompt
+        my_other_prompt.jprompt
+```
+
+Then simply import dotprompt in your code and get your prompts as object of dotprompts
+
+```python
+import dotprompt
+
+...
+
+res = gen_ai_client.complete(dotprompt.my_prompt.system)
+```
+
+When getting a prompt, the library return it as a string and you can use variables to enrich it.
+```my_prompt.system.prompt
+/* A system prompt with variables {speciality} and {age} */
+You are an AI specialized in {speciality}. You are {age} years old.
+```
+```python
+import dotprompt
+
+res = genai_client.complete(
+    prompt = dotprompt.my_prompt.system.format(
+        speciality = "medicine",
+        age = 3
+    )
+)
+```
+
+When comments have been add to the prompt files, the dotprompt store it in the info attribute of the prompt object.
+```python
+import dotprompt
+
+print(dotprompt.my_prompt.info['system'])
+>>>"A system prompt with variables {speciality} and {age}"
+```
+
+
+## Files format
+### .prompt
+The .prompt file format is a simple text file containing the prompt as a string.
+
+It uses a second extension to specify the type of prompt in the file.
+
+Example:
+If you have a prompt with a system prompt and a user prompt, you'll make two files as follows:
+- my_prompt.system.prompt
+- my_prompt.user.prompt
+
+And you'll be able to access them as follows:
+```python
+import dotprompt
+
+res = gen_ai_client.complete(
+    prompt = {
+        "system": dotprompt.my_prompt.system, 
+        "user": dotprompt.my_prompt.user
+    })
+```
+
+If you don't provide a second extension in the prompt file name, the prompt will be considered as a "prompt".
+```python
+import dotprompt
+
+...
+res = gen_ai_client.complete(dotprompt.not_specific.prompt)
+```
+
+The .prompt files can contain comments at the beginning of the file, between /* and */ characters. 
+The comments will be stored in the info attribute of the prompt object and will not be displayed as part of the prompt.
+
+### .jprompt
+The .jprompt file format is a json file containing multiple prompts with the specified type.
+```json
+{
+    "system": "You are an AI specialized in {speciality}. You are {age} years old.",
+    "user": "Tells me about the studies to be come an expert in {speciality}."
+}
+```
+The jprompt can be commented the same way as the .prompt files.
```

### Comparing `dotprompt-0.1.1/pyproject.toml` & `dotprompt-0.1.6/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "dotprompt"
-version = "0.1.1"
+version = "0.1.6"
 description = "Module to incorporate .prompt file to your python code for GenAI"
 readme = "README.md"
 authors = [{ name = "AKoscianski", email = "arnaud.koscianski@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
@@ -25,15 +25,15 @@
 [project.urls]
 Homepage = "https://github.com/Akoscianski/dotprompt"
 
 [project.optional-dependencies]
 dev = ["black", "bumpver", "isort", "pip-tools", "pytest"]
 
 [tool.bumpver]
-current_version = "0.1.1"
+current_version = "0.1.6"
 version_pattern = "MAJOR.MINOR.PATCH"
 commit_message  = "Bump version {old_version} -> {new_version}"
 commit          = true
 tag             = true
 push            = false
 
 [tool.bumpver.file_patterns]
```

