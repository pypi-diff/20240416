# Comparing `tmp/qase-python-commons-2.0.8.tar.gz` & `tmp/qase-python-commons-2.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qase-python-commons-2.0.8.tar", last modified: Mon Mar 11 13:41:47 2024, max compression
+gzip compressed data, was "qase-python-commons-2.0.9.tar", last modified: Mon Mar 11 14:10:20 2024, max compression
```

## Comparing `qase-python-commons-2.0.8.tar` & `qase-python-commons-2.0.9.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 13:41:46.998896 qase-python-commons-2.0.8/
--rw-r--r--   0 runner    (1001) docker     (127)       76 2024-03-11 13:41:40.000000 qase-python-commons-2.0.8/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-03-11 13:41:46.998896 qase-python-commons-2.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      353 2024-03-11 13:41:40.000000 qase-python-commons-2.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-03-11 13:41:40.000000 qase-python-commons-2.0.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-11 13:41:46.998896 qase-python-commons-2.0.8/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 13:41:46.990896 qase-python-commons-2.0.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 13:41:46.998896 qase-python-commons-2.0.8/src/qase_python_commons.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-03-11 13:41:46.000000 qase-python-commons-2.0.8/src/qase_python_commons.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-03-11 13:41:46.000000 qase-python-commons-2.0.8/src/qase_python_commons.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-11 13:41:46.000000 qase-python-commons-2.0.8/src/qase_python_commons.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-03-11 13:41:46.000000 qase-python-commons-2.0.8/src/qase_python_commons.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-11 13:41:46.000000 qase-python-commons-2.0.8/src/qase_python_commons.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 13:41:46.994896 qase-python-commons-2.0.8/src/qaseio/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 13:41:46.994896 qase-python-commons-2.0.8/src/qaseio/commons/
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-03-11 13:41:40.000000 qase-python-commons-2.0.8/src/qaseio/commons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-03-11 13:41:40.000000 qase-python-commons-2.0.8/src/qaseio/commons/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     4268 2024-03-11 13:41:40.000000 qase-python-commons-2.0.8/src/qaseio/commons/interceptor.py
--rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-03-11 13:41:40.000000 qase-python-commons-2.0.8/src/qaseio/commons/loader.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 13:41:46.998896 qase-python-commons-2.0.8/src/qaseio/commons/models/
--rw-r--r--   0 runner    (1001) docker     (127)      436 2024-03-11 13:41:40.000000 qase-python-commons-2.0.8/src/qaseio/commons/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-03-11 13:41:40.000000 qase-python-commons-2.0.8/src/qaseio/commons/models/attachment.py
--rw-r--r--   0 runner    (1001) docker     (127)      278 2024-03-11 13:41:40.000000 qase-python-commons-2.0.8/src/qaseio/commons/models/relation.py
--rw-r--r--   0 runner    (1001) docker     (127)     4537 2024-03-11 13:41:40.000000 qase-python-commons-2.0.8/src/qaseio/commons/models/result.py
--rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-03-11 13:41:40.000000 qase-python-commons-2.0.8/src/qaseio/commons/models/run.py
--rw-r--r--   0 runner    (1001) docker     (127)      882 2024-03-11 13:41:40.000000 qase-python-commons-2.0.8/src/qaseio/commons/models/runtime.py
--rw-r--r--   0 runner    (1001) docker     (127)     4015 2024-03-11 13:41:40.000000 qase-python-commons-2.0.8/src/qaseio/commons/models/step.py
--rw-r--r--   0 runner    (1001) docker     (127)      307 2024-03-11 13:41:40.000000 qase-python-commons-2.0.8/src/qaseio/commons/models/suite.py
--rw-r--r--   0 runner    (1001) docker     (127)     4449 2024-03-11 13:41:40.000000 qase-python-commons-2.0.8/src/qaseio/commons/report.py
--rw-r--r--   0 runner    (1001) docker     (127)    14899 2024-03-11 13:41:40.000000 qase-python-commons-2.0.8/src/qaseio/commons/testops.py
--rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-03-11 13:41:40.000000 qase-python-commons-2.0.8/src/qaseio/commons/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 14:10:20.025025 qase-python-commons-2.0.9/
+-rw-r--r--   0 runner    (1001) docker     (127)       76 2024-03-11 14:10:09.000000 qase-python-commons-2.0.9/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-03-11 14:10:20.025025 qase-python-commons-2.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      353 2024-03-11 14:10:09.000000 qase-python-commons-2.0.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1941 2024-03-11 14:10:09.000000 qase-python-commons-2.0.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-11 14:10:20.025025 qase-python-commons-2.0.9/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 14:10:20.021024 qase-python-commons-2.0.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 14:10:20.025025 qase-python-commons-2.0.9/src/qase_python_commons.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1212 2024-03-11 14:10:20.000000 qase-python-commons-2.0.9/src/qase_python_commons.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-03-11 14:10:20.000000 qase-python-commons-2.0.9/src/qase_python_commons.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-11 14:10:20.000000 qase-python-commons-2.0.9/src/qase_python_commons.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-03-11 14:10:20.000000 qase-python-commons-2.0.9/src/qase_python_commons.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-03-11 14:10:20.000000 qase-python-commons-2.0.9/src/qase_python_commons.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 14:10:20.021024 qase-python-commons-2.0.9/src/qaseio/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 14:10:20.025025 qase-python-commons-2.0.9/src/qaseio/commons/
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-03-11 14:10:09.000000 qase-python-commons-2.0.9/src/qaseio/commons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1648 2024-03-11 14:10:09.000000 qase-python-commons-2.0.9/src/qaseio/commons/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4268 2024-03-11 14:10:09.000000 qase-python-commons-2.0.9/src/qaseio/commons/interceptor.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1046 2024-03-11 14:10:09.000000 qase-python-commons-2.0.9/src/qaseio/commons/loader.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-11 14:10:20.025025 qase-python-commons-2.0.9/src/qaseio/commons/models/
+-rw-r--r--   0 runner    (1001) docker     (127)      436 2024-03-11 14:10:09.000000 qase-python-commons-2.0.9/src/qaseio/commons/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1588 2024-03-11 14:10:09.000000 qase-python-commons-2.0.9/src/qaseio/commons/models/attachment.py
+-rw-r--r--   0 runner    (1001) docker     (127)      278 2024-03-11 14:10:09.000000 qase-python-commons-2.0.9/src/qaseio/commons/models/relation.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4537 2024-03-11 14:10:09.000000 qase-python-commons-2.0.9/src/qaseio/commons/models/result.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2541 2024-03-11 14:10:09.000000 qase-python-commons-2.0.9/src/qaseio/commons/models/run.py
+-rw-r--r--   0 runner    (1001) docker     (127)      882 2024-03-11 14:10:09.000000 qase-python-commons-2.0.9/src/qaseio/commons/models/runtime.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4015 2024-03-11 14:10:09.000000 qase-python-commons-2.0.9/src/qaseio/commons/models/step.py
+-rw-r--r--   0 runner    (1001) docker     (127)      307 2024-03-11 14:10:09.000000 qase-python-commons-2.0.9/src/qaseio/commons/models/suite.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4449 2024-03-11 14:10:09.000000 qase-python-commons-2.0.9/src/qaseio/commons/report.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14893 2024-03-11 14:10:09.000000 qase-python-commons-2.0.9/src/qaseio/commons/testops.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1593 2024-03-11 14:10:09.000000 qase-python-commons-2.0.9/src/qaseio/commons/utils.py
```

### Comparing `qase-python-commons-2.0.8/PKG-INFO` & `qase-python-commons-2.0.9/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qase-python-commons
-Version: 2.0.8
+Version: 2.0.9
 Summary: A library for Qase TestOps and Qase Report
 Author-email: Qase Team <support@qase.io>
 Project-URL: Homepage, https://github.com/qase-tms/qase-python/tree/master/qase-python-commons
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `qase-python-commons-2.0.8/pyproject.toml` & `qase-python-commons-2.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=69", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "qase-python-commons"
-version = "2.0.8"
+version = "2.0.9"
 description = "A library for Qase TestOps and Qase Report"
 readme = "README.md"
 authors = [{name = "Qase Team", email = "support@qase.io"}]
 license = {file = "LICENSE"}
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Programming Language :: Python",
```

### Comparing `qase-python-commons-2.0.8/src/qase_python_commons.egg-info/PKG-INFO` & `qase-python-commons-2.0.9/src/qase_python_commons.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qase-python-commons
-Version: 2.0.8
+Version: 2.0.9
 Summary: A library for Qase TestOps and Qase Report
 Author-email: Qase Team <support@qase.io>
 Project-URL: Homepage, https://github.com/qase-tms/qase-python/tree/master/qase-python-commons
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Programming Language :: Python
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `qase-python-commons-2.0.8/src/qase_python_commons.egg-info/SOURCES.txt` & `qase-python-commons-2.0.9/src/qase_python_commons.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `qase-python-commons-2.0.8/src/qaseio/commons/config.py` & `qase-python-commons-2.0.9/src/qaseio/commons/config.py`

 * *Files identical despite different names*

### Comparing `qase-python-commons-2.0.8/src/qaseio/commons/interceptor.py` & `qase-python-commons-2.0.9/src/qaseio/commons/interceptor.py`

 * *Files identical despite different names*

### Comparing `qase-python-commons-2.0.8/src/qaseio/commons/loader.py` & `qase-python-commons-2.0.9/src/qaseio/commons/loader.py`

 * *Files identical despite different names*

### Comparing `qase-python-commons-2.0.8/src/qaseio/commons/models/attachment.py` & `qase-python-commons-2.0.9/src/qaseio/commons/models/attachment.py`

 * *Files identical despite different names*

### Comparing `qase-python-commons-2.0.8/src/qaseio/commons/models/result.py` & `qase-python-commons-2.0.9/src/qaseio/commons/models/result.py`

 * *Files identical despite different names*

### Comparing `qase-python-commons-2.0.8/src/qaseio/commons/models/run.py` & `qase-python-commons-2.0.9/src/qaseio/commons/models/run.py`

 * *Files identical despite different names*

### Comparing `qase-python-commons-2.0.8/src/qaseio/commons/models/runtime.py` & `qase-python-commons-2.0.9/src/qaseio/commons/models/runtime.py`

 * *Files identical despite different names*

### Comparing `qase-python-commons-2.0.8/src/qaseio/commons/models/step.py` & `qase-python-commons-2.0.9/src/qaseio/commons/models/step.py`

 * *Files identical despite different names*

### Comparing `qase-python-commons-2.0.8/src/qaseio/commons/report.py` & `qase-python-commons-2.0.9/src/qaseio/commons/report.py`

 * *Files identical despite different names*

### Comparing `qase-python-commons-2.0.8/src/qaseio/commons/testops.py` & `qase-python-commons-2.0.9/src/qaseio/commons/testops.py`

 * *Files 1% similar despite different names*

```diff
@@ -87,16 +87,16 @@
     # Method loads environment by name and returns environment id
     def _get_environment(self, environment: str, project: str):
         if self.enabled:
             api_instance = EnvironmentsApi(self.client)
             response = api_instance.get_environments(code=project)
             if hasattr(response, 'result'):
                 for env in response.result.entities:
-                    if env["slug"] == environment:
-                        return env["id"]
+                    if env.slug == environment:
+                        return env.id
         return None
 
     def _send_bulk_results(self):
         if self.enabled and self.results:
             print()
             print(f"[Qase] Uploading attachments for Run ID: {self.run_id}...")
             results = []
```

### Comparing `qase-python-commons-2.0.8/src/qaseio/commons/utils.py` & `qase-python-commons-2.0.9/src/qaseio/commons/utils.py`

 * *Files identical despite different names*

