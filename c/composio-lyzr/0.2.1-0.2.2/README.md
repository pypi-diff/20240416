# Comparing `tmp/composio_lyzr-0.2.1.tar.gz` & `tmp/composio_lyzr-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "composio_lyzr-0.2.1.tar", last modified: Mon Apr 15 17:20:58 2024, max compression
+gzip compressed data, was "composio_lyzr-0.2.2.tar", last modified: Tue Apr 16 12:27:33 2024, max compression
```

## Comparing `composio_lyzr-0.2.1.tar` & `composio_lyzr-0.2.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-15 17:20:58.732582 composio_lyzr-0.2.1/
--rw-r--r--   0 utkarsh    (501) staff       (20)        0 2024-04-12 15:05:13.000000 composio_lyzr-0.2.1/MANIFEST.in
--rw-r--r--   0 utkarsh    (501) staff       (20)     2715 2024-04-15 17:20:58.732389 composio_lyzr-0.2.1/PKG-INFO
--rw-r--r--   0 utkarsh    (501) staff       (20)     2122 2024-04-12 15:05:51.000000 composio_lyzr-0.2.1/README.md
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-15 17:20:58.731474 composio_lyzr-0.2.1/composio_lyzr/
--rw-r--r--   0 utkarsh    (501) staff       (20)      101 2024-04-12 15:03:16.000000 composio_lyzr-0.2.1/composio_lyzr/__init__.py
--rw-r--r--   0 utkarsh    (501) staff       (20)     5617 2024-04-15 12:16:34.000000 composio_lyzr-0.2.1/composio_lyzr/composio_tool_spec.py
--rw-r--r--   0 utkarsh    (501) staff       (20)     2804 2024-04-12 13:36:37.000000 composio_lyzr-0.2.1/composio_lyzr/pydantic_utils.py
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-15 17:20:58.732196 composio_lyzr-0.2.1/composio_lyzr.egg-info/
--rw-r--r--   0 utkarsh    (501) staff       (20)     2715 2024-04-15 17:20:58.000000 composio_lyzr-0.2.1/composio_lyzr.egg-info/PKG-INFO
--rw-r--r--   0 utkarsh    (501) staff       (20)      323 2024-04-15 17:20:58.000000 composio_lyzr-0.2.1/composio_lyzr.egg-info/SOURCES.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)        1 2024-04-15 17:20:58.000000 composio_lyzr-0.2.1/composio_lyzr.egg-info/dependency_links.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)       76 2024-04-15 17:20:58.000000 composio_lyzr-0.2.1/composio_lyzr.egg-info/requires.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)       14 2024-04-15 17:20:58.000000 composio_lyzr-0.2.1/composio_lyzr.egg-info/top_level.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)      342 2024-04-15 12:25:07.000000 composio_lyzr-0.2.1/pyproject.toml
--rw-r--r--   0 utkarsh    (501) staff       (20)       38 2024-04-15 17:20:58.732618 composio_lyzr-0.2.1/setup.cfg
--rw-r--r--   0 utkarsh    (501) staff       (20)      837 2024-04-15 12:25:07.000000 composio_lyzr-0.2.1/setup.py
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-16 12:27:33.439509 composio_lyzr-0.2.2/
+-rw-r--r--   0 utkarsh    (501) staff       (20)        0 2024-04-12 15:05:13.000000 composio_lyzr-0.2.2/MANIFEST.in
+-rw-r--r--   0 utkarsh    (501) staff       (20)     2715 2024-04-16 12:27:33.439327 composio_lyzr-0.2.2/PKG-INFO
+-rw-r--r--   0 utkarsh    (501) staff       (20)     2122 2024-04-12 15:05:51.000000 composio_lyzr-0.2.2/README.md
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-16 12:27:33.438293 composio_lyzr-0.2.2/composio_lyzr/
+-rw-r--r--   0 utkarsh    (501) staff       (20)      101 2024-04-12 15:03:16.000000 composio_lyzr-0.2.2/composio_lyzr/__init__.py
+-rw-r--r--   0 utkarsh    (501) staff       (20)     5622 2024-04-16 12:03:34.000000 composio_lyzr-0.2.2/composio_lyzr/composio_tool_spec.py
+-rw-r--r--   0 utkarsh    (501) staff       (20)     2804 2024-04-12 13:36:37.000000 composio_lyzr-0.2.2/composio_lyzr/pydantic_utils.py
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-16 12:27:33.439139 composio_lyzr-0.2.2/composio_lyzr.egg-info/
+-rw-r--r--   0 utkarsh    (501) staff       (20)     2715 2024-04-16 12:27:33.000000 composio_lyzr-0.2.2/composio_lyzr.egg-info/PKG-INFO
+-rw-r--r--   0 utkarsh    (501) staff       (20)      323 2024-04-16 12:27:33.000000 composio_lyzr-0.2.2/composio_lyzr.egg-info/SOURCES.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)        1 2024-04-16 12:27:33.000000 composio_lyzr-0.2.2/composio_lyzr.egg-info/dependency_links.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)       76 2024-04-16 12:27:33.000000 composio_lyzr-0.2.2/composio_lyzr.egg-info/requires.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)       14 2024-04-16 12:27:33.000000 composio_lyzr-0.2.2/composio_lyzr.egg-info/top_level.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)      342 2024-04-16 12:26:54.000000 composio_lyzr-0.2.2/pyproject.toml
+-rw-r--r--   0 utkarsh    (501) staff       (20)       38 2024-04-16 12:27:33.439549 composio_lyzr-0.2.2/setup.cfg
+-rw-r--r--   0 utkarsh    (501) staff       (20)      837 2024-04-16 12:26:54.000000 composio_lyzr-0.2.2/setup.py
```

### Comparing `composio_lyzr-0.2.1/PKG-INFO` & `composio_lyzr-0.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: composio_lyzr
-Version: 0.2.1
+Version: 0.2.2
 Summary: Use Composio to get an array of tools with your Lyzr workflow.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Sawradip
 Author-email: sawradip@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: lyzr-automata>=0.1.3
 Requires-Dist: pydantic>=2.6.4
-Requires-Dist: composio_core===0.2.1
+Requires-Dist: composio_core===0.2.2
 Requires-Dist: langchain>=0.1.0
 
 ## Using Composio With Lyzr
 
 Integrate Composio with Lyzr agents to allow them to interact seamlessly with external apps, enhancing their functionality and reach.
 
 ### Goal
```

### Comparing `composio_lyzr-0.2.1/README.md` & `composio_lyzr-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `composio_lyzr-0.2.1/composio_lyzr/composio_tool_spec.py` & `composio_lyzr-0.2.2/composio_lyzr/composio_tool_spec.py`

 * *Files 1% similar despite different names*

```diff
@@ -90,15 +90,15 @@
             optional_parameters.append(param)
     return required_parameters + optional_parameters
 
 client = ComposioCore(framework=FrameworkEnum.LYZR, api_key = os.environ.get("COMPOSIO_API_KEY", None))
 ComposioSDK = client.sdk
 
 class ComposioToolset:
-    def __init__(self, entity_id: str = None):
+    def __init__(self, entity_id: str = "default"):
         global client
         self.client = client
         self.entity_id = entity_id
 
     def get_lyzr_tool(self, action: Action):
         action_schema = self.client.sdk.get_list_of_actions(
                                             actions=[action])[0]
```

### Comparing `composio_lyzr-0.2.1/composio_lyzr/pydantic_utils.py` & `composio_lyzr-0.2.2/composio_lyzr/pydantic_utils.py`

 * *Files identical despite different names*

### Comparing `composio_lyzr-0.2.1/composio_lyzr.egg-info/PKG-INFO` & `composio_lyzr-0.2.2/composio_lyzr.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: composio_lyzr
-Version: 0.2.1
+Version: 0.2.2
 Summary: Use Composio to get an array of tools with your Lyzr workflow.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Sawradip
 Author-email: sawradip@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Requires-Dist: lyzr-automata>=0.1.3
 Requires-Dist: pydantic>=2.6.4
-Requires-Dist: composio_core===0.2.1
+Requires-Dist: composio_core===0.2.2
 Requires-Dist: langchain>=0.1.0
 
 ## Using Composio With Lyzr
 
 Integrate Composio with Lyzr agents to allow them to interact seamlessly with external apps, enhancing their functionality and reach.
 
 ### Goal
```

### Comparing `composio_lyzr-0.2.1/setup.py` & `composio_lyzr-0.2.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     return os.path.join(*paths)
 
 
 readme_path = resolve_paths(get_current_dir(), "README.md")
 
 setup(
     name="composio_lyzr",
-    version="0.2.1",
+    version="0.2.2",
     author="Sawradip",
     author_email="sawradip@composio.dev",
     description="Use Composio to get an array of tools with your Lyzr workflow.",
     long_description=open(readme_path).read(),
     long_description_content_type="text/markdown",
     url="https://github.com/SamparkAI/composio_sdk",
     classifiers=[
```

