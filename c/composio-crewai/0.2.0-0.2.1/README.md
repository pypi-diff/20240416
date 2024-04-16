# Comparing `tmp/composio_crewai-0.2.0.tar.gz` & `tmp/composio_crewai-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "composio_crewai-0.2.0.tar", last modified: Mon Apr 15 09:07:52 2024, max compression
+gzip compressed data, was "composio_crewai-0.2.1.tar", last modified: Mon Apr 15 17:20:44 2024, max compression
```

## Comparing `composio_crewai-0.2.0.tar` & `composio_crewai-0.2.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-15 09:07:52.789043 composio_crewai-0.2.0/
--rw-r--r--   0 karanvaidya   (501) staff       (20)     3076 2024-04-15 09:07:52.788837 composio_crewai-0.2.0/PKG-INFO
--rw-r--r--   0 karanvaidya   (501) staff       (20)     2576 2024-04-15 07:39:40.000000 composio_crewai-0.2.0/README.md
-drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-15 09:07:52.787441 composio_crewai-0.2.0/composio_crewai/
--rw-r--r--   0 karanvaidya   (501) staff       (20)      110 2024-04-15 07:39:40.000000 composio_crewai-0.2.0/composio_crewai/__init__.py
-drwxr-xr-x   0 karanvaidya   (501) staff       (20)        0 2024-04-15 09:07:52.788616 composio_crewai-0.2.0/composio_crewai.egg-info/
--rw-r--r--   0 karanvaidya   (501) staff       (20)     3076 2024-04-15 09:07:52.000000 composio_crewai-0.2.0/composio_crewai.egg-info/PKG-INFO
--rw-r--r--   0 karanvaidya   (501) staff       (20)      255 2024-04-15 09:07:52.000000 composio_crewai-0.2.0/composio_crewai.egg-info/SOURCES.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)        1 2024-04-15 09:07:52.000000 composio_crewai-0.2.0/composio_crewai.egg-info/dependency_links.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)       27 2024-04-15 09:07:52.000000 composio_crewai-0.2.0/composio_crewai.egg-info/requires.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)       16 2024-04-15 09:07:52.000000 composio_crewai-0.2.0/composio_crewai.egg-info/top_level.txt
--rw-r--r--   0 karanvaidya   (501) staff       (20)      275 2024-04-15 09:07:06.000000 composio_crewai-0.2.0/pyproject.toml
--rw-r--r--   0 karanvaidya   (501) staff       (20)       38 2024-04-15 09:07:52.789081 composio_crewai-0.2.0/setup.cfg
--rw-r--r--   0 karanvaidya   (501) staff       (20)      838 2024-04-15 09:07:06.000000 composio_crewai-0.2.0/setup.py
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-15 17:20:44.503247 composio_crewai-0.2.1/
+-rw-r--r--   0 utkarsh    (501) staff       (20)     3076 2024-04-15 17:20:44.503057 composio_crewai-0.2.1/PKG-INFO
+-rw-r--r--   0 utkarsh    (501) staff       (20)     2576 2024-04-02 16:50:40.000000 composio_crewai-0.2.1/README.md
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-15 17:20:44.502032 composio_crewai-0.2.1/composio_crewai/
+-rw-r--r--   0 utkarsh    (501) staff       (20)      110 2024-04-12 09:34:46.000000 composio_crewai-0.2.1/composio_crewai/__init__.py
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-15 17:20:44.502896 composio_crewai-0.2.1/composio_crewai.egg-info/
+-rw-r--r--   0 utkarsh    (501) staff       (20)     3076 2024-04-15 17:20:44.000000 composio_crewai-0.2.1/composio_crewai.egg-info/PKG-INFO
+-rw-r--r--   0 utkarsh    (501) staff       (20)      255 2024-04-15 17:20:44.000000 composio_crewai-0.2.1/composio_crewai.egg-info/SOURCES.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)        1 2024-04-15 17:20:44.000000 composio_crewai-0.2.1/composio_crewai.egg-info/dependency_links.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)       27 2024-04-15 17:20:44.000000 composio_crewai-0.2.1/composio_crewai.egg-info/requires.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)       16 2024-04-15 17:20:44.000000 composio_crewai-0.2.1/composio_crewai.egg-info/top_level.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)      275 2024-04-15 12:25:07.000000 composio_crewai-0.2.1/pyproject.toml
+-rw-r--r--   0 utkarsh    (501) staff       (20)       38 2024-04-15 17:20:44.503288 composio_crewai-0.2.1/setup.cfg
+-rw-r--r--   0 utkarsh    (501) staff       (20)      838 2024-04-15 12:25:07.000000 composio_crewai-0.2.1/setup.py
```

### Comparing `composio_crewai-0.2.0/PKG-INFO` & `composio_crewai-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: composio_crewai
-Version: 0.2.0
+Version: 0.2.1
 Summary: Use Composio to get an array of tools with your CrewAI agent.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Himanshu
 Author-email: himanshu@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Requires-Dist: composio_langchain===0.2.0
+Requires-Dist: composio_langchain===0.2.1
 
 # Composio <> CrewAI
 
 ![CrewAI Logo](https://i.imgur.com/jXeNUda.png)
 
 **Composio** enables **CrewAI agents** to connect with numerous tools, making it easy for these agents to interact with external applications seamlessly.
```

### Comparing `composio_crewai-0.2.0/README.md` & `composio_crewai-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `composio_crewai-0.2.0/composio_crewai.egg-info/PKG-INFO` & `composio_crewai-0.2.1/composio_crewai.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: composio_crewai
-Version: 0.2.0
+Version: 0.2.1
 Summary: Use Composio to get an array of tools with your CrewAI agent.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Himanshu
 Author-email: himanshu@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Requires-Dist: composio_langchain===0.2.0
+Requires-Dist: composio_langchain===0.2.1
 
 # Composio <> CrewAI
 
 ![CrewAI Logo](https://i.imgur.com/jXeNUda.png)
 
 **Composio** enables **CrewAI agents** to connect with numerous tools, making it easy for these agents to interact with external applications seamlessly.
```

### Comparing `composio_crewai-0.2.0/setup.py` & `composio_crewai-0.2.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     return os.path.join(*paths)
 
 
 readme_path = resolve_paths(get_current_dir(), "README.md")
 
 setup(
     name="composio_crewai",
-    version="0.2.0",
+    version="0.2.1",
     author="Himanshu",
     author_email="himanshu@composio.dev",
     description="Use Composio to get an array of tools with your CrewAI agent.",
     long_description=open(readme_path).read(),
     long_description_content_type="text/markdown",
     url="https://github.com/SamparkAI/composio_sdk",
     classifiers=[
```

