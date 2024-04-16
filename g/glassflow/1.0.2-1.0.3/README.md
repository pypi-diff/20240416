# Comparing `tmp/glassflow-1.0.2.tar.gz` & `tmp/glassflow-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "glassflow-1.0.2.tar", last modified: Mon Apr  8 10:00:36 2024, max compression
+gzip compressed data, was "glassflow-1.0.3.tar", last modified: Tue Apr 16 07:35:17 2024, max compression
```

## Comparing `glassflow-1.0.2.tar` & `glassflow-1.0.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 10:00:36.538823 glassflow-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-08 10:00:32.000000 glassflow-1.0.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     5805 2024-04-08 10:00:36.538823 glassflow-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4940 2024-04-08 10:00:32.000000 glassflow-1.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-08 10:00:32.000000 glassflow-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 10:00:36.538823 glassflow-1.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-08 10:00:32.000000 glassflow-1.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 10:00:36.534823 glassflow-1.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 10:00:36.534823 glassflow-1.0.2/src/glassflow/
--rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-08 10:00:32.000000 glassflow-1.0.2/src/glassflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1801 2024-04-08 10:00:32.000000 glassflow-1.0.2/src/glassflow/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-08 10:00:32.000000 glassflow-1.0.2/src/glassflow/config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 10:00:36.534823 glassflow-1.0.2/src/glassflow/models/
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-08 10:00:32.000000 glassflow-1.0.2/src/glassflow/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 10:00:36.538823 glassflow-1.0.2/src/glassflow/models/errors/
--rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-08 10:00:32.000000 glassflow-1.0.2/src/glassflow/models/errors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-08 10:00:32.000000 glassflow-1.0.2/src/glassflow/models/errors/clienterror.py
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-08 10:00:32.000000 glassflow-1.0.2/src/glassflow/models/errors/error.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 10:00:36.538823 glassflow-1.0.2/src/glassflow/models/operations/
--rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-08 10:00:32.000000 glassflow-1.0.2/src/glassflow/models/operations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-04-08 10:00:32.000000 glassflow-1.0.2/src/glassflow/models/operations/consumeevent.py
--rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-04-08 10:00:32.000000 glassflow-1.0.2/src/glassflow/models/operations/consumefailed.py
--rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-04-08 10:00:32.000000 glassflow-1.0.2/src/glassflow/models/operations/publishevent.py
--rw-r--r--   0 runner    (1001) docker     (127)    10930 2024-04-08 10:00:32.000000 glassflow-1.0.2/src/glassflow/pipelines.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 10:00:36.538823 glassflow-1.0.2/src/glassflow/utils/
--rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-08 10:00:32.000000 glassflow-1.0.2/src/glassflow/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    22663 2024-04-08 10:00:32.000000 glassflow-1.0.2/src/glassflow/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 10:00:36.538823 glassflow-1.0.2/src/glassflow.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5805 2024-04-08 10:00:36.000000 glassflow-1.0.2/src/glassflow.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      732 2024-04-08 10:00:36.000000 glassflow-1.0.2/src/glassflow.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 10:00:36.000000 glassflow-1.0.2/src/glassflow.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-08 10:00:36.000000 glassflow-1.0.2/src/glassflow.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-08 10:00:36.000000 glassflow-1.0.2/src/glassflow.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:35:17.113086 glassflow-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1071 2024-04-16 07:35:12.000000 glassflow-1.0.3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5805 2024-04-16 07:35:17.113086 glassflow-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4940 2024-04-16 07:35:12.000000 glassflow-1.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       86 2024-04-16 07:35:12.000000 glassflow-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 07:35:17.113086 glassflow-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1111 2024-04-16 07:35:12.000000 glassflow-1.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:35:17.109086 glassflow-1.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:35:17.113086 glassflow-1.0.3/src/glassflow/
+-rw-r--r--   0 runner    (1001) docker     (127)       73 2024-04-16 07:35:12.000000 glassflow-1.0.3/src/glassflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2078 2024-04-16 07:35:12.000000 glassflow-1.0.3/src/glassflow/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      595 2024-04-16 07:35:12.000000 glassflow-1.0.3/src/glassflow/config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:35:17.113086 glassflow-1.0.3/src/glassflow/models/
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-16 07:35:12.000000 glassflow-1.0.3/src/glassflow/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:35:17.113086 glassflow-1.0.3/src/glassflow/models/errors/
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-16 07:35:12.000000 glassflow-1.0.3/src/glassflow/models/errors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1253 2024-04-16 07:35:12.000000 glassflow-1.0.3/src/glassflow/models/errors/clienterror.py
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-16 07:35:12.000000 glassflow-1.0.3/src/glassflow/models/errors/error.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:35:17.113086 glassflow-1.0.3/src/glassflow/models/operations/
+-rw-r--r--   0 runner    (1001) docker     (127)      370 2024-04-16 07:35:12.000000 glassflow-1.0.3/src/glassflow/models/operations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2870 2024-04-16 07:35:12.000000 glassflow-1.0.3/src/glassflow/models/operations/consumeevent.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2873 2024-04-16 07:35:12.000000 glassflow-1.0.3/src/glassflow/models/operations/consumefailed.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2503 2024-04-16 07:35:12.000000 glassflow-1.0.3/src/glassflow/models/operations/publishevent.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10930 2024-04-16 07:35:12.000000 glassflow-1.0.3/src/glassflow/pipelines.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:35:17.113086 glassflow-1.0.3/src/glassflow/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)       21 2024-04-16 07:35:12.000000 glassflow-1.0.3/src/glassflow/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22663 2024-04-16 07:35:12.000000 glassflow-1.0.3/src/glassflow/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:35:17.113086 glassflow-1.0.3/src/glassflow.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5805 2024-04-16 07:35:17.000000 glassflow-1.0.3/src/glassflow.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      732 2024-04-16 07:35:17.000000 glassflow-1.0.3/src/glassflow.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 07:35:17.000000 glassflow-1.0.3/src/glassflow.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      299 2024-04-16 07:35:17.000000 glassflow-1.0.3/src/glassflow.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-16 07:35:17.000000 glassflow-1.0.3/src/glassflow.egg-info/top_level.txt
```

### Comparing `glassflow-1.0.2/LICENSE.md` & `glassflow-1.0.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `glassflow-1.0.2/PKG-INFO` & `glassflow-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glassflow
-Version: 1.0.2
+Version: 1.0.3
 Summary: GlassFlow Python Client SDK
 Home-page: https://learn.glassflow.dev/docs
 Author: glassflow
 Project-URL: Source, https://github.com/glassflow/glassflow-python-sdk
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: glassflow Version: 1.0.2 Summary: GlassFlow Python
+Metadata-Version: 2.1 Name: glassflow Version: 1.0.3 Summary: GlassFlow Python
 Client SDK Home-page: https://learn.glassflow.dev/docs Author: glassflow
 Project-URL: Source, https://github.com/glassflow/glassflow-python-sdk
 Requires-Python: >=3.8 Description-Content-Type: text/markdown License-File:
 LICENSE.md Requires-Dist: urllib3==1.26.15 Requires-Dist: certifi>=2023.7.22
 Requires-Dist: charset-normalizer>=3.2.0 Requires-Dist: dataclasses-json>=0.6.4
 Requires-Dist: idna>=3.4 Requires-Dist: jsonpath-python>=1.0.6 Requires-Dist:
 marshmallow>=3.19.0 Requires-Dist: mypy-extensions>=1.0.0 Requires-Dist:
```

### Comparing `glassflow-1.0.2/README.md` & `glassflow-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `glassflow-1.0.2/setup.py` & `glassflow-1.0.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     with open("README.md", "r") as fh:
         long_description = fh.read()
 except FileNotFoundError:
     long_description = ""
 
 setuptools.setup(
     name="glassflow",
-    version="1.0.2",
+    version="1.0.3",
     author="glassflow",
     description="GlassFlow Python Client SDK",
     url="https://learn.glassflow.dev/docs",
     project_urls={
         'Source': 'https://github.com/glassflow/glassflow-python-sdk',
     },
     long_description=long_description,
```

### Comparing `glassflow-1.0.2/src/glassflow/client.py` & `glassflow-1.0.3/src/glassflow/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -35,11 +35,18 @@
             space_id: The space id where the pipeline is located
             pipeline_id: The pipeline id to interact with
             pipeline_access_token: The access token to access the pipeline
 
         Returns:
             PipelineClient: Client object to publish and consume events from the given pipeline.
         """
+        if not pipeline_id:
+            raise ValueError(
+                "pipeline_id is required to create a PipelineClient")
+        if not pipeline_access_token:
+            raise ValueError(
+                "pipeline_access_token is required to create a PipelineClient")
+
         return PipelineClient(glassflow_client=self,
                               space_id=space_id,
                               pipeline_id=pipeline_id,
                               pipeline_access_token=pipeline_access_token)
```

### Comparing `glassflow-1.0.2/src/glassflow/config.py` & `glassflow-1.0.3/src/glassflow/config.py`

 * *Files identical despite different names*

### Comparing `glassflow-1.0.2/src/glassflow/models/errors/clienterror.py` & `glassflow-1.0.3/src/glassflow/models/errors/clienterror.py`

 * *Files identical despite different names*

### Comparing `glassflow-1.0.2/src/glassflow/models/errors/error.py` & `glassflow-1.0.3/src/glassflow/models/errors/error.py`

 * *Files identical despite different names*

### Comparing `glassflow-1.0.2/src/glassflow/models/operations/consumeevent.py` & `glassflow-1.0.3/src/glassflow/models/operations/consumeevent.py`

 * *Files identical despite different names*

### Comparing `glassflow-1.0.2/src/glassflow/models/operations/consumefailed.py` & `glassflow-1.0.3/src/glassflow/models/operations/consumefailed.py`

 * *Files identical despite different names*

### Comparing `glassflow-1.0.2/src/glassflow/models/operations/publishevent.py` & `glassflow-1.0.3/src/glassflow/models/operations/publishevent.py`

 * *Files identical despite different names*

### Comparing `glassflow-1.0.2/src/glassflow/pipelines.py` & `glassflow-1.0.3/src/glassflow/pipelines.py`

 * *Files identical despite different names*

### Comparing `glassflow-1.0.2/src/glassflow/utils/utils.py` & `glassflow-1.0.3/src/glassflow/utils/utils.py`

 * *Files identical despite different names*

### Comparing `glassflow-1.0.2/src/glassflow.egg-info/PKG-INFO` & `glassflow-1.0.3/src/glassflow.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: glassflow
-Version: 1.0.2
+Version: 1.0.3
 Summary: GlassFlow Python Client SDK
 Home-page: https://learn.glassflow.dev/docs
 Author: glassflow
 Project-URL: Source, https://github.com/glassflow/glassflow-python-sdk
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: glassflow Version: 1.0.2 Summary: GlassFlow Python
+Metadata-Version: 2.1 Name: glassflow Version: 1.0.3 Summary: GlassFlow Python
 Client SDK Home-page: https://learn.glassflow.dev/docs Author: glassflow
 Project-URL: Source, https://github.com/glassflow/glassflow-python-sdk
 Requires-Python: >=3.8 Description-Content-Type: text/markdown License-File:
 LICENSE.md Requires-Dist: urllib3==1.26.15 Requires-Dist: certifi>=2023.7.22
 Requires-Dist: charset-normalizer>=3.2.0 Requires-Dist: dataclasses-json>=0.6.4
 Requires-Dist: idna>=3.4 Requires-Dist: jsonpath-python>=1.0.6 Requires-Dist:
 marshmallow>=3.19.0 Requires-Dist: mypy-extensions>=1.0.0 Requires-Dist:
```

### Comparing `glassflow-1.0.2/src/glassflow.egg-info/SOURCES.txt` & `glassflow-1.0.3/src/glassflow.egg-info/SOURCES.txt`

 * *Files identical despite different names*

