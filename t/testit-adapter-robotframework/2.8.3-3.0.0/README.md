# Comparing `tmp/testit-adapter-robotframework-2.8.3.tar.gz` & `tmp/testit_adapter_robotframework-3.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testit-adapter-robotframework-2.8.3.tar", last modified: Fri Mar 15 06:55:31 2024, max compression
+gzip compressed data, was "testit_adapter_robotframework-3.0.0.tar", last modified: Mon Apr 15 10:42:43 2024, max compression
```

## Comparing `testit-adapter-robotframework-2.8.3.tar` & `testit_adapter_robotframework-3.0.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 06:55:31.373275 testit-adapter-robotframework-2.8.3/
--rw-r--r--   0 runner    (1001) docker     (127)    14097 2024-03-15 06:55:31.373275 testit-adapter-robotframework-2.8.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    13296 2024-03-15 06:55:26.000000 testit-adapter-robotframework-2.8.3/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-15 06:55:31.373275 testit-adapter-robotframework-2.8.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-03-15 06:55:26.000000 testit-adapter-robotframework-2.8.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 06:55:31.369275 testit-adapter-robotframework-2.8.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 06:55:31.373275 testit-adapter-robotframework-2.8.3/src/testit_adapter_robotframework/
--rw-r--r--   0 runner    (1001) docker     (127)     4350 2024-03-15 06:55:26.000000 testit-adapter-robotframework-2.8.3/src/testit_adapter_robotframework/TMSLibrary.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-03-15 06:55:26.000000 testit-adapter-robotframework-2.8.3/src/testit_adapter_robotframework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4236 2024-03-15 06:55:26.000000 testit-adapter-robotframework-2.8.3/src/testit_adapter_robotframework/listeners.py
--rw-r--r--   0 runner    (1001) docker     (127)     9334 2024-03-15 06:55:26.000000 testit-adapter-robotframework-2.8.3/src/testit_adapter_robotframework/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-03-15 06:55:26.000000 testit-adapter-robotframework-2.8.3/src/testit_adapter_robotframework/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-15 06:55:31.373275 testit-adapter-robotframework-2.8.3/src/testit_adapter_robotframework.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    14097 2024-03-15 06:55:31.000000 testit-adapter-robotframework-2.8.3/src/testit_adapter_robotframework.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      530 2024-03-15 06:55:31.000000 testit-adapter-robotframework-2.8.3/src/testit_adapter_robotframework.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-15 06:55:31.000000 testit-adapter-robotframework-2.8.3/src/testit_adapter_robotframework.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       50 2024-03-15 06:55:31.000000 testit-adapter-robotframework-2.8.3/src/testit_adapter_robotframework.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       30 2024-03-15 06:55:31.000000 testit-adapter-robotframework-2.8.3/src/testit_adapter_robotframework.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:42:43.825276 testit_adapter_robotframework-3.0.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    14097 2024-04-15 10:42:43.825276 testit_adapter_robotframework-3.0.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    13296 2024-04-15 10:42:39.000000 testit_adapter_robotframework-3.0.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 10:42:43.825276 testit_adapter_robotframework-3.0.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-15 10:42:39.000000 testit_adapter_robotframework-3.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:42:43.821277 testit_adapter_robotframework-3.0.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:42:43.821277 testit_adapter_robotframework-3.0.0/src/testit_adapter_robotframework/
+-rw-r--r--   0 runner    (1001) docker     (127)     4350 2024-04-15 10:42:39.000000 testit_adapter_robotframework-3.0.0/src/testit_adapter_robotframework/TMSLibrary.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 10:42:39.000000 testit_adapter_robotframework-3.0.0/src/testit_adapter_robotframework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4218 2024-04-15 10:42:39.000000 testit_adapter_robotframework-3.0.0/src/testit_adapter_robotframework/listeners.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9316 2024-04-15 10:42:39.000000 testit_adapter_robotframework-3.0.0/src/testit_adapter_robotframework/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2761 2024-04-15 10:42:39.000000 testit_adapter_robotframework-3.0.0/src/testit_adapter_robotframework/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 10:42:43.825276 testit_adapter_robotframework-3.0.0/src/testit_adapter_robotframework.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    14097 2024-04-15 10:42:43.000000 testit_adapter_robotframework-3.0.0/src/testit_adapter_robotframework.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      530 2024-04-15 10:42:43.000000 testit_adapter_robotframework-3.0.0/src/testit_adapter_robotframework.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 10:42:43.000000 testit_adapter_robotframework-3.0.0/src/testit_adapter_robotframework.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       50 2024-04-15 10:42:43.000000 testit_adapter_robotframework-3.0.0/src/testit_adapter_robotframework.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       30 2024-04-15 10:42:43.000000 testit_adapter_robotframework-3.0.0/src/testit_adapter_robotframework.egg-info/top_level.txt
```

### Comparing `testit-adapter-robotframework-2.8.3/PKG-INFO` & `testit_adapter_robotframework-3.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testit-adapter-robotframework
-Version: 2.8.3
+Version: 3.0.0
 Summary: Robot Framework adapter for Test IT
 Home-page: https://github.com/testit-tms/adapters-python/
 Author: Integration team
 Author-email: integrations@testit.software
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 Requires-Dist: attrs
 Requires-Dist: robotframework
-Requires-Dist: testit-python-commons==2.8.3
+Requires-Dist: testit-python-commons==3.0.0
 
 # Test IT TMS adapter for Robot Framework
 ![Test IT](https://raw.githubusercontent.com/testit-tms/adapters-python/master/images/banner.png)
 
 [![Release
 Status](https://img.shields.io/pypi/v/testit-adapter-robotframework?style=plastic)](https://pypi.python.org/pypi/testit-adapter-robotframework)
 [![Downloads](https://img.shields.io/pypi/dm/testit-adapter-robotframework?style=plastic)](https://pypi.python.org/pypi/testit-adapter-robotframework)
```

### Comparing `testit-adapter-robotframework-2.8.3/README.md` & `testit_adapter_robotframework-3.0.0/README.md`

 * *Files identical despite different names*

### Comparing `testit-adapter-robotframework-2.8.3/setup.py` & `testit_adapter_robotframework-3.0.0/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages, setup
 
 setup(
     name='testit-adapter-robotframework',
-    version='2.8.3',
+    version='3.0.0',
     description='Robot Framework adapter for Test IT',
     long_description=open('README.md', "r").read(),
     long_description_content_type="text/markdown",
     url='https://github.com/testit-tms/adapters-python/',
     author='Integration team',
     author_email='integrations@testit.software',
     license='Apache-2.0',
@@ -19,9 +19,9 @@
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         'Programming Language :: Python :: 3.12',
     ],
     py_modules=['testit_adapter_robotframework'],
     packages=find_packages(where='src'),
     package_dir={'': 'src'},
-    install_requires=['attrs', 'robotframework', 'testit-python-commons==2.8.3']
+    install_requires=['attrs', 'robotframework', 'testit-python-commons==3.0.0']
 )
```

### Comparing `testit-adapter-robotframework-2.8.3/src/testit_adapter_robotframework/TMSLibrary.py` & `testit_adapter_robotframework-3.0.0/src/testit_adapter_robotframework/TMSLibrary.py`

 * *Files identical despite different names*

### Comparing `testit-adapter-robotframework-2.8.3/src/testit_adapter_robotframework/listeners.py` & `testit_adapter_robotframework-3.0.0/src/testit_adapter_robotframework/listeners.py`

 * *Files 1% similar despite different names*

```diff
@@ -94,15 +94,15 @@
             raise SystemExit
 
     def start_suite(self, suite):
         suite.tests = [t for t in suite.tests if self._is_included(t)]
 
     def _is_included(self, test):
         tags = test.tags
-        external_id = get_hash(test.longname.split('.', 1)[-1])
+        external_id = get_hash(test.longname)
         for tag in tags:
             if str(tag).lower().startswith('testit.externalid'):
                 external_id = tag.split(':', 1)[-1].strip()
         return external_id in self.tests
 
     def end_suite(self, suite):
         suite.suites = [s for s in suite.suites if s.test_count > 0]
```

### Comparing `testit-adapter-robotframework-2.8.3/src/testit_adapter_robotframework/models.py` & `testit_adapter_robotframework-3.0.0/src/testit_adapter_robotframework/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -143,15 +143,15 @@
                 elif attr == 'namespace':
                     self.namespace = str(value).replace("'", "").replace('"', '')
                 elif attr == 'classname':
                     self.classname = str(value).replace("'", "").replace('"', '')
                 else:
                     logger.error(f"[TestIt] Unknown attribute: {attr}")
         if not self.externalID:
-            self.externalID = get_hash(attrs['longname'].split('.', 1)[-1])
+            self.externalID = get_hash(attrs['longname'])
 
     def add_step(self, step_type, title, description, parameters):
         if len(self.step_depth) == 0:
             if step_type.lower() == 'setup':
                 self.setUp.append(Step(title, description))
                 self.step_depth.append(self.setUp[-1])
                 self.setUpResults.append(StepResult(title, description, parameters=parameters))
```

### Comparing `testit-adapter-robotframework-2.8.3/src/testit_adapter_robotframework/utils.py` & `testit_adapter_robotframework-3.0.0/src/testit_adapter_robotframework/utils.py`

 * *Files identical despite different names*

### Comparing `testit-adapter-robotframework-2.8.3/src/testit_adapter_robotframework.egg-info/PKG-INFO` & `testit_adapter_robotframework-3.0.0/src/testit_adapter_robotframework.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testit-adapter-robotframework
-Version: 2.8.3
+Version: 3.0.0
 Summary: Robot Framework adapter for Test IT
 Home-page: https://github.com/testit-tms/adapters-python/
 Author: Integration team
 Author-email: integrations@testit.software
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
@@ -13,15 +13,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Description-Content-Type: text/markdown
 Requires-Dist: attrs
 Requires-Dist: robotframework
-Requires-Dist: testit-python-commons==2.8.3
+Requires-Dist: testit-python-commons==3.0.0
 
 # Test IT TMS adapter for Robot Framework
 ![Test IT](https://raw.githubusercontent.com/testit-tms/adapters-python/master/images/banner.png)
 
 [![Release
 Status](https://img.shields.io/pypi/v/testit-adapter-robotframework?style=plastic)](https://pypi.python.org/pypi/testit-adapter-robotframework)
 [![Downloads](https://img.shields.io/pypi/dm/testit-adapter-robotframework?style=plastic)](https://pypi.python.org/pypi/testit-adapter-robotframework)
```

### Comparing `testit-adapter-robotframework-2.8.3/src/testit_adapter_robotframework.egg-info/SOURCES.txt` & `testit_adapter_robotframework-3.0.0/src/testit_adapter_robotframework.egg-info/SOURCES.txt`

 * *Files identical despite different names*

