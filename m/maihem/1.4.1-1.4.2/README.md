# Comparing `tmp/maihem-1.4.1.tar.gz` & `tmp/maihem-1.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "maihem-1.4.1.tar", last modified: Tue Apr  2 17:09:30 2024, max compression
+gzip compressed data, was "maihem-1.4.2.tar", last modified: Tue Apr 16 07:49:17 2024, max compression
```

## Comparing `maihem-1.4.1.tar` & `maihem-1.4.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 eduardocandela   (501) staff       (20)        0 2024-04-02 17:09:30.194836 maihem-1.4.1/
--rw-r--r--   0 eduardocandela   (501) staff       (20)     1063 2023-12-12 19:12:18.000000 maihem-1.4.1/LICENSE
--rw-r--r--   0 eduardocandela   (501) staff       (20)        0 2023-12-14 20:19:47.000000 maihem-1.4.1/MANIFEST.in
--rw-r--r--   0 eduardocandela   (501) staff       (20)     3530 2024-04-02 17:09:30.194755 maihem-1.4.1/PKG-INFO
--rw-r--r--   0 eduardocandela   (501) staff       (20)     1754 2024-03-07 01:27:56.000000 maihem-1.4.1/README.md
--rw-r--r--   0 eduardocandela   (501) staff       (20)      685 2024-04-02 17:07:07.000000 maihem-1.4.1/pyproject.toml
--rw-r--r--   0 eduardocandela   (501) staff       (20)       38 2024-04-02 17:09:30.195041 maihem-1.4.1/setup.cfg
-drwxr-xr-x   0 eduardocandela   (501) staff       (20)        0 2024-04-02 17:09:30.192082 maihem-1.4.1/src/
-drwxr-xr-x   0 eduardocandela   (501) staff       (20)        0 2024-04-02 17:09:30.193182 maihem-1.4.1/src/maihem/
--rw-r--r--   0 eduardocandela   (501) staff       (20)       82 2024-03-06 21:21:19.000000 maihem-1.4.1/src/maihem/__init__.py
--rw-r--r--   0 eduardocandela   (501) staff       (20)     8747 2024-04-02 17:04:57.000000 maihem-1.4.1/src/maihem/functions.py
-drwxr-xr-x   0 eduardocandela   (501) staff       (20)        0 2024-04-02 17:09:30.194498 maihem-1.4.1/src/maihem.egg-info/
--rw-r--r--   0 eduardocandela   (501) staff       (20)     3530 2024-04-02 17:09:30.000000 maihem-1.4.1/src/maihem.egg-info/PKG-INFO
--rw-r--r--   0 eduardocandela   (501) staff       (20)      270 2024-04-02 17:09:30.000000 maihem-1.4.1/src/maihem.egg-info/SOURCES.txt
--rw-r--r--   0 eduardocandela   (501) staff       (20)        1 2024-04-02 17:09:30.000000 maihem-1.4.1/src/maihem.egg-info/dependency_links.txt
--rw-r--r--   0 eduardocandela   (501) staff       (20)       16 2024-04-02 17:09:30.000000 maihem-1.4.1/src/maihem.egg-info/requires.txt
--rw-r--r--   0 eduardocandela   (501) staff       (20)        7 2024-04-02 17:09:30.000000 maihem-1.4.1/src/maihem.egg-info/top_level.txt
+drwxr-xr-x   0 eduardocandela   (501) staff       (20)        0 2024-04-16 07:49:17.252378 maihem-1.4.2/
+-rw-r--r--   0 eduardocandela   (501) staff       (20)     1063 2023-12-12 19:12:18.000000 maihem-1.4.2/LICENSE
+-rw-r--r--   0 eduardocandela   (501) staff       (20)        0 2023-12-14 20:19:47.000000 maihem-1.4.2/MANIFEST.in
+-rw-r--r--   0 eduardocandela   (501) staff       (20)     3530 2024-04-16 07:49:17.252319 maihem-1.4.2/PKG-INFO
+-rw-r--r--   0 eduardocandela   (501) staff       (20)     1754 2024-03-07 01:27:56.000000 maihem-1.4.2/README.md
+-rw-r--r--   0 eduardocandela   (501) staff       (20)      685 2024-04-16 07:46:38.000000 maihem-1.4.2/pyproject.toml
+-rw-r--r--   0 eduardocandela   (501) staff       (20)       38 2024-04-16 07:49:17.252563 maihem-1.4.2/setup.cfg
+drwxr-xr-x   0 eduardocandela   (501) staff       (20)        0 2024-04-16 07:49:17.250302 maihem-1.4.2/src/
+drwxr-xr-x   0 eduardocandela   (501) staff       (20)        0 2024-04-16 07:49:17.251170 maihem-1.4.2/src/maihem/
+-rw-r--r--   0 eduardocandela   (501) staff       (20)       82 2024-03-06 21:21:19.000000 maihem-1.4.2/src/maihem/__init__.py
+-rw-r--r--   0 eduardocandela   (501) staff       (20)     8800 2024-04-16 07:47:55.000000 maihem-1.4.2/src/maihem/functions.py
+drwxr-xr-x   0 eduardocandela   (501) staff       (20)        0 2024-04-16 07:49:17.252128 maihem-1.4.2/src/maihem.egg-info/
+-rw-r--r--   0 eduardocandela   (501) staff       (20)     3530 2024-04-16 07:49:17.000000 maihem-1.4.2/src/maihem.egg-info/PKG-INFO
+-rw-r--r--   0 eduardocandela   (501) staff       (20)      270 2024-04-16 07:49:17.000000 maihem-1.4.2/src/maihem.egg-info/SOURCES.txt
+-rw-r--r--   0 eduardocandela   (501) staff       (20)        1 2024-04-16 07:49:17.000000 maihem-1.4.2/src/maihem.egg-info/dependency_links.txt
+-rw-r--r--   0 eduardocandela   (501) staff       (20)       16 2024-04-16 07:49:17.000000 maihem-1.4.2/src/maihem.egg-info/requires.txt
+-rw-r--r--   0 eduardocandela   (501) staff       (20)        7 2024-04-16 07:49:17.000000 maihem-1.4.2/src/maihem.egg-info/top_level.txt
```

### Comparing `maihem-1.4.1/LICENSE` & `maihem-1.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `maihem-1.4.1/PKG-INFO` & `maihem-1.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maihem
-Version: 1.4.1
+Version: 1.4.2
 Summary: LLM evaluations and synthetic data generation with the MAIHEM models
 Author: MAIHEM
 License: MIT License
         
         Copyright (c) 2023 MAIHEM
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `maihem-1.4.1/README.md` & `maihem-1.4.2/README.md`

 * *Files identical despite different names*

### Comparing `maihem-1.4.1/pyproject.toml` & `maihem-1.4.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "maihem"
-version = "1.4.1"
+version = "1.4.2"
 description = "LLM evaluations and synthetic data generation with the MAIHEM models"
 readme = "README.md"
 authors = [{ name = "MAIHEM"}]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `maihem-1.4.1/src/maihem/functions.py` & `maihem-1.4.2/src/maihem/functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
         if "info" in json_response:
             print(json_response['info'])    
             return json_response
         else:
             raise ExceptionAPI(json_response['detail'])
 
 
-def create_test(test_name: str, chatbot_role: str, industry: str, n: int, topic: str=None, language: str=None):
+def create_test(test_name: str, chatbot_role: str, industry: str, n: int, topic: str=None, intents: List[str]=None, language: str=None):
     """
     Create a test with a set of AI personas
 
     No return value
 
     Parameters
     ----------
@@ -98,14 +98,15 @@
 
     payload = {
         "test_name": test_name,
         "chatbot_role": chatbot_role,
         "industry": industry,
         "n": n,
         "topic": topic,
+        "intents": intents,
         "language": language
     }
     response = api._call_api(payload, "/create_test_simulated")
     print(response['response']) 
     
 
 def chat_with_persona(test_name: str, test_run_name: str, persona_id: int, message: str, num_turns_max=None) -> str:
```

### Comparing `maihem-1.4.1/src/maihem.egg-info/PKG-INFO` & `maihem-1.4.2/src/maihem.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maihem
-Version: 1.4.1
+Version: 1.4.2
 Summary: LLM evaluations and synthetic data generation with the MAIHEM models
 Author: MAIHEM
 License: MIT License
         
         Copyright (c) 2023 MAIHEM
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

