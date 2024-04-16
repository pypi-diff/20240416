# Comparing `tmp/DataWeaver-0.3.3.tar.gz` & `tmp/dataweaver-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DataWeaver-0.3.3.tar", last modified: Thu Feb 29 09:46:58 2024, max compression
+gzip compressed data, was "dataweaver-0.3.4.tar", last modified: Tue Apr 16 16:21:28 2024, max compression
```

## Comparing `DataWeaver-0.3.3.tar` & `dataweaver-0.3.4.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 09:46:58.164842 DataWeaver-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-02-29 09:46:48.000000 DataWeaver-0.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     9227 2024-02-29 09:46:58.164842 DataWeaver-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     8514 2024-02-29 09:46:48.000000 DataWeaver-0.3.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      924 2024-02-29 09:46:48.000000 DataWeaver-0.3.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-02-29 09:46:58.164842 DataWeaver-0.3.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 09:46:58.160843 DataWeaver-0.3.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 09:46:58.164842 DataWeaver-0.3.3/src/DataWeaver.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     9227 2024-02-29 09:46:58.000000 DataWeaver-0.3.3/src/DataWeaver.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      298 2024-02-29 09:46:58.000000 DataWeaver-0.3.3/src/DataWeaver.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-02-29 09:46:58.000000 DataWeaver-0.3.3/src/DataWeaver.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-02-29 09:46:58.000000 DataWeaver-0.3.3/src/DataWeaver.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       12 2024-02-29 09:46:58.000000 DataWeaver-0.3.3/src/DataWeaver.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-02-29 09:46:58.164842 DataWeaver-0.3.3/src/data_weaver/
--rw-r--r--   0 runner    (1001) docker     (127)      165 2024-02-29 09:46:48.000000 DataWeaver-0.3.3/src/data_weaver/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     5397 2024-02-29 09:46:48.000000 DataWeaver-0.3.3/src/data_weaver/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-02-29 09:46:48.000000 DataWeaver-0.3.3/src/data_weaver/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:21:28.941903 dataweaver-0.3.4/
+-rw-r--r--   0 runner    (1001) docker     (127)     1072 2024-04-16 16:21:19.000000 dataweaver-0.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     9227 2024-04-16 16:21:28.941903 dataweaver-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     8514 2024-04-16 16:21:19.000000 dataweaver-0.3.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      924 2024-04-16 16:21:19.000000 dataweaver-0.3.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 16:21:28.941903 dataweaver-0.3.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:21:28.937903 dataweaver-0.3.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:21:28.941903 dataweaver-0.3.4/src/DataWeaver.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     9227 2024-04-16 16:21:28.000000 dataweaver-0.3.4/src/DataWeaver.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      328 2024-04-16 16:21:28.000000 dataweaver-0.3.4/src/DataWeaver.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 16:21:28.000000 dataweaver-0.3.4/src/DataWeaver.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-16 16:21:28.000000 dataweaver-0.3.4/src/DataWeaver.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       12 2024-04-16 16:21:28.000000 dataweaver-0.3.4/src/DataWeaver.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:21:28.941903 dataweaver-0.3.4/src/data_weaver/
+-rw-r--r--   0 runner    (1001) docker     (127)      165 2024-04-16 16:21:19.000000 dataweaver-0.3.4/src/data_weaver/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5760 2024-04-16 16:21:19.000000 dataweaver-0.3.4/src/data_weaver/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3549 2024-04-16 16:21:19.000000 dataweaver-0.3.4/src/data_weaver/transforms.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2367 2024-04-16 16:21:19.000000 dataweaver-0.3.4/src/data_weaver/utils.py
```

### Comparing `DataWeaver-0.3.3/LICENSE` & `dataweaver-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `DataWeaver-0.3.3/PKG-INFO` & `dataweaver-0.3.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DataWeaver
-Version: 0.3.3
+Version: 0.3.4
 Summary: DataWeaver is a Python library for mapping data and transform object to an other. It offers flexible field mapping through a simple configuration object, enabling easy data integration and transformation for analysis and processing.
 Author-email: RICHARD Quentin <richard.quentin88@gmail.com>
 License: MIT License
 Project-URL: homepage, https://github.com/RICHARD-Quentin/DataWeaver
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `DataWeaver-0.3.3/README.md` & `dataweaver-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `DataWeaver-0.3.3/pyproject.toml` & `dataweaver-0.3.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "DataWeaver"
-version = "0.3.3"
+version = "0.3.4"
 authors = [{name = "RICHARD Quentin", email = "richard.quentin88@gmail.com"}]
 description = "DataWeaver is a Python library for mapping data and transform object to an other. It offers flexible field mapping through a simple configuration object, enabling easy data integration and transformation for analysis and processing."
 readme = "README.md"
 license = {text = "MIT License"}  # Update the license as appropriate
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `DataWeaver-0.3.3/src/DataWeaver.egg-info/PKG-INFO` & `dataweaver-0.3.4/src/DataWeaver.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DataWeaver
-Version: 0.3.3
+Version: 0.3.4
 Summary: DataWeaver is a Python library for mapping data and transform object to an other. It offers flexible field mapping through a simple configuration object, enabling easy data integration and transformation for analysis and processing.
 Author-email: RICHARD Quentin <richard.quentin88@gmail.com>
 License: MIT License
 Project-URL: homepage, https://github.com/RICHARD-Quentin/DataWeaver
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `DataWeaver-0.3.3/src/data_weaver/main.py` & `dataweaver-0.3.4/src/data_weaver/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,22 +34,31 @@
     Args:
         data (dict): The input data dictionary.
         final_result (dict): The dictionary to store the mapped key-value pairs.
 
     Returns:
         None
     """
-    for full_key, value in data.items():
-        new_key = await get_new_key(full_key)
-        if isinstance(new_key, list):
-            for key in new_key:
-                final_result[key] = value
+    for key, source_key in config.get('mapping').items():
+        if isinstance(source_key, list):
+            value = { key: data[key] for key in source_key}
+        elif isinstance(source_key, dict):
+            value = [ data[key] for key in source_key]
+        else : 
+            value = data.get(source_key)
+        final_result[key] = value
 
-        if isinstance(new_key, str):
-            final_result[new_key] = value
+    # for full_key, value in data.items():
+    #     new_key = await get_new_key(full_key)
+    #     if isinstance(new_key, list):
+    #         for key in new_key:
+    #             final_result[key] = value
+
+    #     if isinstance(new_key, str):
+    #         final_result[new_key] = value
 
 async def parse_entry(object: dict, final_result, prefix: str = ''):
     """
     Parse the given object recursively and update the final_result dictionary with the extracted fields.
 
     Parameters:
         object (dict): The object to be parsed.
```

### Comparing `DataWeaver-0.3.3/src/data_weaver/utils.py` & `dataweaver-0.3.4/src/data_weaver/utils.py`

 * *Files identical despite different names*

