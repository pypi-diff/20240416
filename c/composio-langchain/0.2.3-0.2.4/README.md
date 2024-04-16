# Comparing `tmp/composio_langchain-0.2.3.tar.gz` & `tmp/composio_langchain-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "composio_langchain-0.2.3.tar", last modified: Tue Apr 16 12:47:33 2024, max compression
+gzip compressed data, was "composio_langchain-0.2.4.tar", last modified: Tue Apr 16 12:53:23 2024, max compression
```

## Comparing `composio_langchain-0.2.3.tar` & `composio_langchain-0.2.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-16 12:47:33.453178 composio_langchain-0.2.3/
--rw-r--r--   0 utkarsh    (501) staff       (20)        0 2024-03-16 10:20:25.000000 composio_langchain-0.2.3/MANIFEST.in
--rw-r--r--   0 utkarsh    (501) staff       (20)     3332 2024-04-16 12:47:33.452947 composio_langchain-0.2.3/PKG-INFO
--rw-r--r--   0 utkarsh    (501) staff       (20)     2591 2024-04-02 17:07:00.000000 composio_langchain-0.2.3/README.md
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-16 12:47:33.451946 composio_langchain-0.2.3/composio_langchain/
--rw-r--r--   0 utkarsh    (501) staff       (20)      101 2024-04-12 09:34:14.000000 composio_langchain-0.2.3/composio_langchain/__init__.py
--rw-r--r--   0 utkarsh    (501) staff       (20)     5332 2024-04-16 12:03:22.000000 composio_langchain-0.2.3/composio_langchain/composio_tool_spec.py
--rw-r--r--   0 utkarsh    (501) staff       (20)     2804 2024-03-18 18:14:40.000000 composio_langchain-0.2.3/composio_langchain/pydantic_utils.py
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-16 12:47:33.452713 composio_langchain-0.2.3/composio_langchain.egg-info/
--rw-r--r--   0 utkarsh    (501) staff       (20)     3332 2024-04-16 12:47:33.000000 composio_langchain-0.2.3/composio_langchain.egg-info/PKG-INFO
--rw-r--r--   0 utkarsh    (501) staff       (20)      363 2024-04-16 12:47:33.000000 composio_langchain-0.2.3/composio_langchain.egg-info/SOURCES.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)        1 2024-04-16 12:47:33.000000 composio_langchain-0.2.3/composio_langchain.egg-info/dependency_links.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)      148 2024-04-16 12:47:33.000000 composio_langchain-0.2.3/composio_langchain.egg-info/requires.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)       19 2024-04-16 12:47:33.000000 composio_langchain-0.2.3/composio_langchain.egg-info/top_level.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)      454 2024-04-16 12:46:58.000000 composio_langchain-0.2.3/pyproject.toml
--rw-r--r--   0 utkarsh    (501) staff       (20)       38 2024-04-16 12:47:33.453222 composio_langchain-0.2.3/setup.cfg
--rw-r--r--   0 utkarsh    (501) staff       (20)      838 2024-04-16 12:47:01.000000 composio_langchain-0.2.3/setup.py
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-16 12:53:23.715141 composio_langchain-0.2.4/
+-rw-r--r--   0 utkarsh    (501) staff       (20)        0 2024-03-16 10:20:25.000000 composio_langchain-0.2.4/MANIFEST.in
+-rw-r--r--   0 utkarsh    (501) staff       (20)     3332 2024-04-16 12:53:23.714907 composio_langchain-0.2.4/PKG-INFO
+-rw-r--r--   0 utkarsh    (501) staff       (20)     2591 2024-04-02 17:07:00.000000 composio_langchain-0.2.4/README.md
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-16 12:53:23.713746 composio_langchain-0.2.4/composio_langchain/
+-rw-r--r--   0 utkarsh    (501) staff       (20)      101 2024-04-12 09:34:14.000000 composio_langchain-0.2.4/composio_langchain/__init__.py
+-rw-r--r--   0 utkarsh    (501) staff       (20)     5332 2024-04-16 12:03:22.000000 composio_langchain-0.2.4/composio_langchain/composio_tool_spec.py
+-rw-r--r--   0 utkarsh    (501) staff       (20)     2804 2024-03-18 18:14:40.000000 composio_langchain-0.2.4/composio_langchain/pydantic_utils.py
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-16 12:53:23.714641 composio_langchain-0.2.4/composio_langchain.egg-info/
+-rw-r--r--   0 utkarsh    (501) staff       (20)     3332 2024-04-16 12:53:23.000000 composio_langchain-0.2.4/composio_langchain.egg-info/PKG-INFO
+-rw-r--r--   0 utkarsh    (501) staff       (20)      363 2024-04-16 12:53:23.000000 composio_langchain-0.2.4/composio_langchain.egg-info/SOURCES.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)        1 2024-04-16 12:53:23.000000 composio_langchain-0.2.4/composio_langchain.egg-info/dependency_links.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)      148 2024-04-16 12:53:23.000000 composio_langchain-0.2.4/composio_langchain.egg-info/requires.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)       19 2024-04-16 12:53:23.000000 composio_langchain-0.2.4/composio_langchain.egg-info/top_level.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)      454 2024-04-16 12:52:49.000000 composio_langchain-0.2.4/pyproject.toml
+-rw-r--r--   0 utkarsh    (501) staff       (20)       38 2024-04-16 12:53:23.715183 composio_langchain-0.2.4/setup.cfg
+-rw-r--r--   0 utkarsh    (501) staff       (20)      838 2024-04-16 12:52:49.000000 composio_langchain-0.2.4/setup.py
```

### Comparing `composio_langchain-0.2.3/PKG-INFO` & `composio_langchain-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: composio_langchain
-Version: 0.2.3
+Version: 0.2.4
 Summary: Use Composio to get an array of tools with your LangChain agent.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Karan
 Author-email: karan@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -14,15 +14,15 @@
 Requires-Dist: jsonschema
 Requires-Dist: argparse
 Requires-Dist: nest_asyncio
 Requires-Dist: langchain>=0.1.0
 Requires-Dist: langchain-openai>=0.0.2.post1
 Requires-Dist: langchainhub>=0.1.15
 Requires-Dist: pydantic>=2.6.4
-Requires-Dist: composio_core===0.2.3
+Requires-Dist: composio_core===0.2.4
 
 ## 🦜🔗 Using Composio With LangChain
 
 Integrate Composio with LangChain agents to allow them to interact seamlessly with external apps, enhancing their functionality and reach.
 
 ### Goal
```

### Comparing `composio_langchain-0.2.3/README.md` & `composio_langchain-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `composio_langchain-0.2.3/composio_langchain/composio_tool_spec.py` & `composio_langchain-0.2.4/composio_langchain/composio_tool_spec.py`

 * *Files identical despite different names*

### Comparing `composio_langchain-0.2.3/composio_langchain/pydantic_utils.py` & `composio_langchain-0.2.4/composio_langchain/pydantic_utils.py`

 * *Files identical despite different names*

### Comparing `composio_langchain-0.2.3/composio_langchain.egg-info/PKG-INFO` & `composio_langchain-0.2.4/composio_langchain.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: composio_langchain
-Version: 0.2.3
+Version: 0.2.4
 Summary: Use Composio to get an array of tools with your LangChain agent.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Karan
 Author-email: karan@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
@@ -14,15 +14,15 @@
 Requires-Dist: jsonschema
 Requires-Dist: argparse
 Requires-Dist: nest_asyncio
 Requires-Dist: langchain>=0.1.0
 Requires-Dist: langchain-openai>=0.0.2.post1
 Requires-Dist: langchainhub>=0.1.15
 Requires-Dist: pydantic>=2.6.4
-Requires-Dist: composio_core===0.2.3
+Requires-Dist: composio_core===0.2.4
 
 ## 🦜🔗 Using Composio With LangChain
 
 Integrate Composio with LangChain agents to allow them to interact seamlessly with external apps, enhancing their functionality and reach.
 
 ### Goal
```

### Comparing `composio_langchain-0.2.3/setup.py` & `composio_langchain-0.2.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     return os.path.join(*paths)
 
 
 readme_path = resolve_paths(get_current_dir(), "README.md")
 
 setup(
     name="composio_langchain",
-    version="0.2.3",
+    version="0.2.4",
     author="Karan",
     author_email="karan@composio.dev",
     description="Use Composio to get an array of tools with your LangChain agent.",
     long_description=open(readme_path).read(),
     long_description_content_type="text/markdown",
     url="https://github.com/SamparkAI/composio_sdk",
     classifiers=[
```

