# Comparing `tmp/composio_autogen-0.2.3.tar.gz` & `tmp/composio_autogen-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "composio_autogen-0.2.3.tar", last modified: Tue Apr 16 12:47:46 2024, max compression
+gzip compressed data, was "composio_autogen-0.2.4.tar", last modified: Tue Apr 16 12:53:38 2024, max compression
```

## Comparing `composio_autogen-0.2.3.tar` & `composio_autogen-0.2.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-16 12:47:46.546442 composio_autogen-0.2.3/
--rw-r--r--   0 utkarsh    (501) staff       (20)     3306 2024-04-16 12:47:46.546240 composio_autogen-0.2.3/PKG-INFO
--rw-r--r--   0 utkarsh    (501) staff       (20)     2776 2024-04-02 16:44:24.000000 composio_autogen-0.2.3/README.md
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-16 12:47:46.545153 composio_autogen-0.2.3/composio_autogen/
--rw-r--r--   0 utkarsh    (501) staff       (20)      100 2024-04-12 09:34:34.000000 composio_autogen-0.2.3/composio_autogen/__init__.py
--rw-r--r--   0 utkarsh    (501) staff       (20)     8535 2024-04-16 12:10:28.000000 composio_autogen-0.2.3/composio_autogen/autogen_toolspec.py
-drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-16 12:47:46.546061 composio_autogen-0.2.3/composio_autogen.egg-info/
--rw-r--r--   0 utkarsh    (501) staff       (20)     3306 2024-04-16 12:47:46.000000 composio_autogen-0.2.3/composio_autogen.egg-info/PKG-INFO
--rw-r--r--   0 utkarsh    (501) staff       (20)      298 2024-04-16 12:47:46.000000 composio_autogen-0.2.3/composio_autogen.egg-info/SOURCES.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)        1 2024-04-16 12:47:46.000000 composio_autogen-0.2.3/composio_autogen.egg-info/dependency_links.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)       40 2024-04-16 12:47:46.000000 composio_autogen-0.2.3/composio_autogen.egg-info/requires.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)       17 2024-04-16 12:47:46.000000 composio_autogen-0.2.3/composio_autogen.egg-info/top_level.txt
--rw-r--r--   0 utkarsh    (501) staff       (20)      297 2024-04-16 12:46:34.000000 composio_autogen-0.2.3/pyproject.toml
--rw-r--r--   0 utkarsh    (501) staff       (20)       38 2024-04-16 12:47:46.546481 composio_autogen-0.2.3/setup.cfg
--rw-r--r--   0 utkarsh    (501) staff       (20)      840 2024-04-16 12:46:41.000000 composio_autogen-0.2.3/setup.py
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-16 12:53:38.617483 composio_autogen-0.2.4/
+-rw-r--r--   0 utkarsh    (501) staff       (20)     3306 2024-04-16 12:53:38.617267 composio_autogen-0.2.4/PKG-INFO
+-rw-r--r--   0 utkarsh    (501) staff       (20)     2776 2024-04-02 16:44:24.000000 composio_autogen-0.2.4/README.md
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-16 12:53:38.616007 composio_autogen-0.2.4/composio_autogen/
+-rw-r--r--   0 utkarsh    (501) staff       (20)      100 2024-04-12 09:34:34.000000 composio_autogen-0.2.4/composio_autogen/__init__.py
+-rw-r--r--   0 utkarsh    (501) staff       (20)     8535 2024-04-16 12:10:28.000000 composio_autogen-0.2.4/composio_autogen/autogen_toolspec.py
+drwxr-xr-x   0 utkarsh    (501) staff       (20)        0 2024-04-16 12:53:38.617069 composio_autogen-0.2.4/composio_autogen.egg-info/
+-rw-r--r--   0 utkarsh    (501) staff       (20)     3306 2024-04-16 12:53:38.000000 composio_autogen-0.2.4/composio_autogen.egg-info/PKG-INFO
+-rw-r--r--   0 utkarsh    (501) staff       (20)      298 2024-04-16 12:53:38.000000 composio_autogen-0.2.4/composio_autogen.egg-info/SOURCES.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)        1 2024-04-16 12:53:38.000000 composio_autogen-0.2.4/composio_autogen.egg-info/dependency_links.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)       40 2024-04-16 12:53:38.000000 composio_autogen-0.2.4/composio_autogen.egg-info/requires.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)       17 2024-04-16 12:53:38.000000 composio_autogen-0.2.4/composio_autogen.egg-info/top_level.txt
+-rw-r--r--   0 utkarsh    (501) staff       (20)      297 2024-04-16 12:52:49.000000 composio_autogen-0.2.4/pyproject.toml
+-rw-r--r--   0 utkarsh    (501) staff       (20)       38 2024-04-16 12:53:38.617524 composio_autogen-0.2.4/setup.cfg
+-rw-r--r--   0 utkarsh    (501) staff       (20)      840 2024-04-16 12:52:49.000000 composio_autogen-0.2.4/setup.py
```

### Comparing `composio_autogen-0.2.3/PKG-INFO` & `composio_autogen-0.2.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: composio_autogen
-Version: 0.2.3
+Version: 0.2.4
 Summary: Use Composio to get an array of tools with your Autogen agent.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Sawradip
 Author-email: sawradip@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Requires-Dist: composio_core===0.2.3
+Requires-Dist: composio_core===0.2.4
 Requires-Dist: pyautogen>=0.2.29
 
 # Composio <> Autogen
 Use Composio to enhance your Autogen workflows with a suite of tools.
 
 ## Quick Start
```

### Comparing `composio_autogen-0.2.3/README.md` & `composio_autogen-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `composio_autogen-0.2.3/composio_autogen/autogen_toolspec.py` & `composio_autogen-0.2.4/composio_autogen/autogen_toolspec.py`

 * *Files identical despite different names*

### Comparing `composio_autogen-0.2.3/composio_autogen.egg-info/PKG-INFO` & `composio_autogen-0.2.4/composio_autogen.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 Metadata-Version: 2.1
 Name: composio_autogen
-Version: 0.2.3
+Version: 0.2.4
 Summary: Use Composio to get an array of tools with your Autogen agent.
 Home-page: https://github.com/SamparkAI/composio_sdk
 Author: Sawradip
 Author-email: sawradip@composio.dev
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
-Requires-Dist: composio_core===0.2.3
+Requires-Dist: composio_core===0.2.4
 Requires-Dist: pyautogen>=0.2.29
 
 # Composio <> Autogen
 Use Composio to enhance your Autogen workflows with a suite of tools.
 
 ## Quick Start
```

### Comparing `composio_autogen-0.2.3/setup.py` & `composio_autogen-0.2.4/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -10,15 +10,15 @@
     return os.path.join(*paths)
 
 
 readme_path = resolve_paths(get_current_dir(), "README.md")
 
 setup(
     name="composio_autogen",
-    version="0.2.3",
+    version="0.2.4",
     author="Sawradip",
     author_email="sawradip@composio.dev",
     description="Use Composio to get an array of tools with your Autogen agent.",
     long_description=open(readme_path).read(),
     long_description_content_type="text/markdown",
     url="https://github.com/SamparkAI/composio_sdk",
     classifiers=[
```

