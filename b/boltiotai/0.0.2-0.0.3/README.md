# Comparing `tmp/boltiotai-0.0.2.tar.gz` & `tmp/boltiotai-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "boltiotai-0.0.2.tar", last modified: Tue Apr  9 11:27:54 2024, max compression
+gzip compressed data, was "boltiotai-0.0.3.tar", last modified: Tue Apr 16 07:25:42 2024, max compression
```

## Comparing `boltiotai-0.0.2.tar` & `boltiotai-0.0.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-09 11:27:54.456074 boltiotai-0.0.2/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1081 2024-04-08 19:19:48.000000 boltiotai-0.0.2/LICENSE
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      412 2024-04-09 11:27:54.456074 boltiotai-0.0.2/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-08 19:09:19.000000 boltiotai-0.0.2/README.md
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-09 11:27:54.452074 boltiotai-0.0.2/boltiotai/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       45 2024-04-09 11:09:34.000000 boltiotai-0.0.2/boltiotai/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1169 2024-04-09 11:17:16.000000 boltiotai-0.0.2/boltiotai/_client.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      711 2024-04-09 11:15:33.000000 boltiotai-0.0.2/boltiotai/_request.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-09 11:27:54.452074 boltiotai-0.0.2/boltiotai/resources/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       50 2024-04-08 12:56:31.000000 boltiotai-0.0.2/boltiotai/resources/__init__.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-09 11:27:54.452074 boltiotai-0.0.2/boltiotai/resources/chat/
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       23 2024-04-02 13:26:00.000000 boltiotai-0.0.2/boltiotai/resources/chat/__init__.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      121 2024-04-03 13:59:16.000000 boltiotai-0.0.2/boltiotai/resources/chat/chat.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      583 2024-04-09 11:16:19.000000 boltiotai-0.0.2/boltiotai/resources/chat/completions.py
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      845 2024-04-08 18:40:44.000000 boltiotai-0.0.2/boltiotai/resources/images.py
-drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-09 11:27:54.456074 boltiotai-0.0.2/boltiotai.egg-info/
--rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      412 2024-04-09 11:27:54.000000 boltiotai-0.0.2/boltiotai.egg-info/PKG-INFO
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      433 2024-04-09 11:27:54.000000 boltiotai-0.0.2/boltiotai.egg-info/SOURCES.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-04-09 11:27:54.000000 boltiotai-0.0.2/boltiotai.egg-info/dependency_links.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        9 2024-04-09 11:27:54.000000 boltiotai-0.0.2/boltiotai.egg-info/requires.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       10 2024-04-09 11:27:54.000000 boltiotai-0.0.2/boltiotai.egg-info/top_level.txt
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      629 2024-04-09 11:27:46.000000 boltiotai-0.0.2/pyproject.toml
--rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-04-09 11:27:54.456074 boltiotai-0.0.2/setup.cfg
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-16 07:25:42.992789 boltiotai-0.0.3/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1081 2024-04-08 19:19:48.000000 boltiotai-0.0.3/LICENSE
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      412 2024-04-16 07:25:42.992789 boltiotai-0.0.3/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-08 19:09:19.000000 boltiotai-0.0.3/README.md
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-16 07:25:42.988789 boltiotai-0.0.3/boltiotai/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       45 2024-04-09 11:09:34.000000 boltiotai-0.0.3/boltiotai/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     1329 2024-04-11 15:26:03.000000 boltiotai-0.0.3/boltiotai/_client.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      711 2024-04-09 11:15:33.000000 boltiotai-0.0.3/boltiotai/_request.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-16 07:25:42.988789 boltiotai-0.0.3/boltiotai/resources/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       50 2024-04-08 12:56:31.000000 boltiotai-0.0.3/boltiotai/resources/__init__.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-16 07:25:42.988789 boltiotai-0.0.3/boltiotai/resources/chat/
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       23 2024-04-02 13:26:00.000000 boltiotai-0.0.3/boltiotai/resources/chat/__init__.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      121 2024-04-03 13:59:16.000000 boltiotai-0.0.3/boltiotai/resources/chat/chat.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      584 2024-04-15 16:01:59.000000 boltiotai-0.0.3/boltiotai/resources/chat/completions.py
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)     2344 2024-04-16 06:47:56.000000 boltiotai-0.0.3/boltiotai/resources/images.py
+drwxrwxr-x   0 ubuntu    (1000) ubuntu    (1000)        0 2024-04-16 07:25:42.992789 boltiotai-0.0.3/boltiotai.egg-info/
+-rw-r--r--   0 ubuntu    (1000) ubuntu    (1000)      412 2024-04-16 07:25:42.000000 boltiotai-0.0.3/boltiotai.egg-info/PKG-INFO
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      433 2024-04-16 07:25:42.000000 boltiotai-0.0.3/boltiotai.egg-info/SOURCES.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        1 2024-04-16 07:25:42.000000 boltiotai-0.0.3/boltiotai.egg-info/dependency_links.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)        9 2024-04-16 07:25:42.000000 boltiotai-0.0.3/boltiotai.egg-info/requires.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       10 2024-04-16 07:25:42.000000 boltiotai-0.0.3/boltiotai.egg-info/top_level.txt
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)      629 2024-04-16 07:25:22.000000 boltiotai-0.0.3/pyproject.toml
+-rw-rw-r--   0 ubuntu    (1000) ubuntu    (1000)       38 2024-04-16 07:25:42.992789 boltiotai-0.0.3/setup.cfg
```

### Comparing `boltiotai-0.0.2/LICENSE` & `boltiotai-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `boltiotai-0.0.2/boltiotai/_client.py` & `boltiotai-0.0.3/boltiotai/_client.py`

 * *Files 13% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 chat = resources.Chat
 
 class OpenAI:
 
 
     chat = resources.Chat
     images = resources.Images
+    Images = resources.Images()
     request_api = RequestAPI()
     api_key = None
 
     def __init__(self, api_key=None, base_url=None):
         if api_key is None:
             api_key = os.environ.get("OPENAI_API_KEY")
 
@@ -38,8 +39,22 @@
     def api_key(self, value):
         self._api_key = value
         self.on_api_key_change(value)
 
     def on_api_key_change(self, api_key):
         self.request_api.update_api_key(api_key)
 
+
+class App:
+    def __init__():
+        pass
+
+    def add(name, resource):
+        pass
+
+    def query(query):
+        pass
+
 openai = OpenAI()
+
+
+
```

### Comparing `boltiotai-0.0.2/boltiotai/_request.py` & `boltiotai-0.0.3/boltiotai/_request.py`

 * *Files identical despite different names*

### Comparing `boltiotai-0.0.2/boltiotai/resources/chat/completions.py` & `boltiotai-0.0.3/boltiotai/resources/chat/completions.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 from ..._request import HttpMethod, RequestAPI
 
 
 class Completions:
 
+
     URL = 'https://trainings.boltiot.com/api/aitools/v1/chats/completions'
     request_api = RequestAPI()
     def __init__(self, api_key=None):
         self.api_key = api_key
 
     def create(self, model, messages):
         return self.call_openai_chat(model, messages)
```

### Comparing `boltiotai-0.0.2/pyproject.toml` & `boltiotai-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "boltiotai"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Pranav Kundaikar", email="support@boltiot.com" },
 ]
 description = "A package for managing API access to LLMs"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

