# Comparing `tmp/taskgen-ai-1.3.0.tar.gz` & `tmp/taskgen_ai-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "taskgen-ai-1.3.0.tar", last modified: Tue Mar 26 08:14:05 2024, max compression
+gzip compressed data, was "taskgen_ai-1.3.1.tar", last modified: Tue Apr 16 15:44:22 2024, max compression
```

## Comparing `taskgen-ai-1.3.0.tar` & `taskgen_ai-1.3.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 tanchongmin   (501) staff       (20)        0 2024-03-26 08:14:05.059642 taskgen-ai-1.3.0/
--rw-rw-r--   0 tanchongmin   (501) staff       (20)     1073 2024-02-26 00:45:10.000000 taskgen-ai-1.3.0/LICENSE
--rw-r--r--   0 tanchongmin   (501) staff       (20)    21014 2024-03-26 08:14:05.058795 taskgen-ai-1.3.0/PKG-INFO
--rw-rw-r--   0 tanchongmin   (501) staff       (20)    20432 2024-03-26 08:13:07.000000 taskgen-ai-1.3.0/README.md
--rw-rw-r--   0 tanchongmin   (501) staff       (20)      649 2024-03-26 08:13:17.000000 taskgen-ai-1.3.0/pyproject.toml
--rw-r--r--   0 tanchongmin   (501) staff       (20)       38 2024-03-26 08:14:05.059778 taskgen-ai-1.3.0/setup.cfg
--rw-rw-r--   0 tanchongmin   (501) staff       (20)      180 2024-03-26 08:13:15.000000 taskgen-ai-1.3.0/setup.py
-drwxr-xr-x   0 tanchongmin   (501) staff       (20)        0 2024-03-26 08:14:05.054320 taskgen-ai-1.3.0/taskgen/
--rw-rw-r--   0 tanchongmin   (501) staff       (20)      170 2024-03-14 09:43:26.000000 taskgen-ai-1.3.0/taskgen/__init__.py
--rw-r--r--   0 tanchongmin   (501) staff       (20)    33533 2024-03-26 07:25:08.000000 taskgen-ai-1.3.0/taskgen/agent.py
--rw-r--r--   0 tanchongmin   (501) staff       (20)    36496 2024-03-22 16:27:30.000000 taskgen-ai-1.3.0/taskgen/base.py
-drwxr-xr-x   0 tanchongmin   (501) staff       (20)        0 2024-03-26 08:14:05.057895 taskgen-ai-1.3.0/taskgen_ai.egg-info/
--rw-r--r--   0 tanchongmin   (501) staff       (20)    21014 2024-03-26 08:14:05.000000 taskgen-ai-1.3.0/taskgen_ai.egg-info/PKG-INFO
--rw-r--r--   0 tanchongmin   (501) staff       (20)      263 2024-03-26 08:14:05.000000 taskgen-ai-1.3.0/taskgen_ai.egg-info/SOURCES.txt
--rw-r--r--   0 tanchongmin   (501) staff       (20)        1 2024-03-26 08:14:05.000000 taskgen-ai-1.3.0/taskgen_ai.egg-info/dependency_links.txt
--rw-r--r--   0 tanchongmin   (501) staff       (20)       14 2024-03-26 08:14:05.000000 taskgen-ai-1.3.0/taskgen_ai.egg-info/requires.txt
--rw-r--r--   0 tanchongmin   (501) staff       (20)        8 2024-03-26 08:14:05.000000 taskgen-ai-1.3.0/taskgen_ai.egg-info/top_level.txt
+drwxr-xr-x   0 tanchongmin   (501) staff       (20)        0 2024-04-16 15:44:22.560490 taskgen_ai-1.3.1/
+-rw-rw-r--   0 tanchongmin   (501) staff       (20)     1073 2024-02-26 00:45:10.000000 taskgen_ai-1.3.1/LICENSE
+-rw-r--r--   0 tanchongmin   (501) staff       (20)    21085 2024-04-16 15:44:22.560018 taskgen_ai-1.3.1/PKG-INFO
+-rw-rw-r--   0 tanchongmin   (501) staff       (20)    20503 2024-04-16 15:00:00.000000 taskgen_ai-1.3.1/README.md
+-rw-rw-r--   0 tanchongmin   (501) staff       (20)      649 2024-04-16 15:43:59.000000 taskgen_ai-1.3.1/pyproject.toml
+-rw-r--r--   0 tanchongmin   (501) staff       (20)       38 2024-04-16 15:44:22.560575 taskgen_ai-1.3.1/setup.cfg
+-rw-rw-r--   0 tanchongmin   (501) staff       (20)      180 2024-04-16 15:00:11.000000 taskgen_ai-1.3.1/setup.py
+drwxr-xr-x   0 tanchongmin   (501) staff       (20)        0 2024-04-16 15:44:22.556525 taskgen_ai-1.3.1/taskgen/
+-rw-rw-r--   0 tanchongmin   (501) staff       (20)      170 2024-03-14 09:43:26.000000 taskgen_ai-1.3.1/taskgen/__init__.py
+-rw-r--r--   0 tanchongmin   (501) staff       (20)    33533 2024-04-05 09:43:06.000000 taskgen_ai-1.3.1/taskgen/agent.py
+-rw-r--r--   0 tanchongmin   (501) staff       (20)    36446 2024-04-05 09:43:08.000000 taskgen_ai-1.3.1/taskgen/base.py
+drwxr-xr-x   0 tanchongmin   (501) staff       (20)        0 2024-04-16 15:44:22.559506 taskgen_ai-1.3.1/taskgen_ai.egg-info/
+-rw-r--r--   0 tanchongmin   (501) staff       (20)    21085 2024-04-16 15:44:22.000000 taskgen_ai-1.3.1/taskgen_ai.egg-info/PKG-INFO
+-rw-r--r--   0 tanchongmin   (501) staff       (20)      263 2024-04-16 15:44:22.000000 taskgen_ai-1.3.1/taskgen_ai.egg-info/SOURCES.txt
+-rw-r--r--   0 tanchongmin   (501) staff       (20)        1 2024-04-16 15:44:22.000000 taskgen_ai-1.3.1/taskgen_ai.egg-info/dependency_links.txt
+-rw-r--r--   0 tanchongmin   (501) staff       (20)       14 2024-04-16 15:44:22.000000 taskgen_ai-1.3.1/taskgen_ai.egg-info/requires.txt
+-rw-r--r--   0 tanchongmin   (501) staff       (20)        8 2024-04-16 15:44:22.000000 taskgen_ai-1.3.1/taskgen_ai.egg-info/top_level.txt
```

### Comparing `taskgen-ai-1.3.0/LICENSE` & `taskgen_ai-1.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `taskgen-ai-1.3.0/PKG-INFO` & `taskgen_ai-1.3.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: taskgen-ai
-Version: 1.3.0
+Version: 1.3.1
 Summary: A Task-based agentic framework building on StrictJSON outputs by LLM agents
 Author-email: John Tan Chong Min <tanchongmin@gmail.com>
 Project-URL: Homepage, https://github.com/simbianai/taskgen
 Project-URL: Issues, https://github.com/simbianai/taskgen/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: openai==1.3.6
+Requires-Dist: openai>=1.3.6
 
-# TaskGen v1.3.0
+# TaskGen v1.3.1
 ### A Task-based agentic framework building on StrictJSON outputs by LLM agents
 - Related Repositories: StrictJSON (https://github.com/tanchongmin/strictjson)
-- Video: https://www.youtube.com/watch?v=O_XyTT7QGH4
+- Video (Part 1): https://www.youtube.com/watch?v=O_XyTT7QGH4
+- Video (Part 2): https://www.youtube.com/watch?v=OWk7moRfTPE
 
 ### Creator's Preamble
 Happy to share that the task-based agentic framework I have been working on - TaskGen - is largely complete! 
 
 Noteable features include:
 - Splitting of Tasks into subtasks for bite-sized solutions for each subtask
 - Single Agent with LLM Functions
```

### Comparing `taskgen-ai-1.3.0/README.md` & `taskgen_ai-1.3.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,12 @@
-# TaskGen v1.3.0
+# TaskGen v1.3.1
 ### A Task-based agentic framework building on StrictJSON outputs by LLM agents
 - Related Repositories: StrictJSON (https://github.com/tanchongmin/strictjson)
-- Video: https://www.youtube.com/watch?v=O_XyTT7QGH4
+- Video (Part 1): https://www.youtube.com/watch?v=O_XyTT7QGH4
+- Video (Part 2): https://www.youtube.com/watch?v=OWk7moRfTPE
 
 ### Creator's Preamble
 Happy to share that the task-based agentic framework I have been working on - TaskGen - is largely complete! 
 
 Noteable features include:
 - Splitting of Tasks into subtasks for bite-sized solutions for each subtask
 - Single Agent with LLM Functions
```

### Comparing `taskgen-ai-1.3.0/pyproject.toml` & `taskgen_ai-1.3.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "taskgen-ai"
-version = "1.3.0"
+version = "1.3.1"
 authors = [
   { name="John Tan Chong Min", email="tanchongmin@gmail.com" },
 ]
 description = "A Task-based agentic framework building on StrictJSON outputs by LLM agents"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
-dependencies = ["openai==1.3.6"]
+dependencies = ["openai>=1.3.6"]
 
 [project.urls]
 Homepage = "https://github.com/simbianai/taskgen"
 Issues = "https://github.com/simbianai/taskgen/issues"
```

### Comparing `taskgen-ai-1.3.0/taskgen/agent.py` & `taskgen_ai-1.3.1/taskgen/agent.py`

 * *Files identical despite different names*

### Comparing `taskgen-ai-1.3.0/taskgen/base.py` & `taskgen_ai-1.3.1/taskgen/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -469,15 +469,15 @@
         # start off with no error message
         error_msg = ''
 
         # wrap the values with angle brackets and wrap keys with delimiter to encourage LLM to modify it
         new_output_format = wrap_with_angle_brackets(output_format, delimiter, 1)
         
         output_format_prompt = f'''\nOutput in the following json string format: {new_output_format}
-Update text enclosed in <>. Be concise. Output only the json string without any explanation. You must output valid json with all keys present.'''
+Update text enclosed in <>. Be concise. Output only the json string without any explanation.'''
 
         for i in range(num_tries):
             my_system_prompt = str(system_prompt) + output_format_prompt + error_msg
             my_user_prompt = str(user_prompt) 
 
             # Use OpenAI to get a response
             res = chat(my_system_prompt, my_user_prompt, **kwargs)
```

### Comparing `taskgen-ai-1.3.0/taskgen_ai.egg-info/PKG-INFO` & `taskgen_ai-1.3.1/taskgen_ai.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 Metadata-Version: 2.1
 Name: taskgen-ai
-Version: 1.3.0
+Version: 1.3.1
 Summary: A Task-based agentic framework building on StrictJSON outputs by LLM agents
 Author-email: John Tan Chong Min <tanchongmin@gmail.com>
 Project-URL: Homepage, https://github.com/simbianai/taskgen
 Project-URL: Issues, https://github.com/simbianai/taskgen/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: openai==1.3.6
+Requires-Dist: openai>=1.3.6
 
-# TaskGen v1.3.0
+# TaskGen v1.3.1
 ### A Task-based agentic framework building on StrictJSON outputs by LLM agents
 - Related Repositories: StrictJSON (https://github.com/tanchongmin/strictjson)
-- Video: https://www.youtube.com/watch?v=O_XyTT7QGH4
+- Video (Part 1): https://www.youtube.com/watch?v=O_XyTT7QGH4
+- Video (Part 2): https://www.youtube.com/watch?v=OWk7moRfTPE
 
 ### Creator's Preamble
 Happy to share that the task-based agentic framework I have been working on - TaskGen - is largely complete! 
 
 Noteable features include:
 - Splitting of Tasks into subtasks for bite-sized solutions for each subtask
 - Single Agent with LLM Functions
```

