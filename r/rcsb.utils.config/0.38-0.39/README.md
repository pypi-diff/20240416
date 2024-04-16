# Comparing `tmp/rcsb.utils.config-0.38.tar.gz` & `tmp/rcsb_utils_config-0.39.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rcsb.utils.config-0.38.tar", last modified: Tue Jan 10 15:32:39 2023, max compression
+gzip compressed data, was "rcsb_utils_config-0.39.tar", last modified: Tue Apr 16 11:01:02 2024, max compression
```

## Comparing `rcsb.utils.config-0.38.tar` & `rcsb_utils_config-0.39.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-10 15:32:39.943317 rcsb.utils.config-0.38/
--rw-r--r--   0 vsts      (1001) docker     (122)     2286 2023-01-10 15:31:44.000000 rcsb.utils.config-0.38/HISTORY.txt
--rw-r--r--   0 vsts      (1001) docker     (122)      552 2023-01-10 15:31:44.000000 rcsb.utils.config-0.38/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (122)      106 2023-01-10 15:31:44.000000 rcsb.utils.config-0.38/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (122)     1699 2023-01-10 15:32:39.943317 rcsb.utils.config-0.38/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)     1021 2023-01-10 15:31:44.000000 rcsb.utils.config-0.38/README.md
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-10 15:32:39.943317 rcsb.utils.config-0.38/rcsb/
--rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-01-10 15:31:44.000000 rcsb.utils.config-0.38/rcsb/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-10 15:32:39.943317 rcsb.utils.config-0.38/rcsb/utils/
--rw-r--r--   0 vsts      (1001) docker     (122)       65 2023-01-10 15:31:44.000000 rcsb.utils.config-0.38/rcsb/utils/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-10 15:32:39.943317 rcsb.utils.config-0.38/rcsb/utils/config/
--rw-r--r--   0 vsts      (1001) docker     (122)    29277 2023-01-10 15:31:44.000000 rcsb.utils.config-0.38/rcsb/utils/config/ConfigUtil.py
--rw-r--r--   0 vsts      (1001) docker     (122)      121 2023-01-10 15:31:44.000000 rcsb.utils.config-0.38/rcsb/utils/config/ExampleHelper.py
--rw-r--r--   0 vsts      (1001) docker     (122)      154 2023-01-10 15:31:44.000000 rcsb.utils.config-0.38/rcsb/utils/config/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (122)        0 2023-01-10 15:32:39.943317 rcsb.utils.config-0.38/rcsb.utils.config.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (122)     1699 2023-01-10 15:32:39.000000 rcsb.utils.config-0.38/rcsb.utils.config.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (122)      458 2023-01-10 15:32:39.000000 rcsb.utils.config-0.38/rcsb.utils.config.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-01-10 15:32:39.000000 rcsb.utils.config-0.38/rcsb.utils.config.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        1 2023-01-10 15:32:24.000000 rcsb.utils.config-0.38/rcsb.utils.config.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (122)      132 2023-01-10 15:32:39.000000 rcsb.utils.config-0.38/rcsb.utils.config.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (122)        5 2023-01-10 15:32:39.000000 rcsb.utils.config-0.38/rcsb.utils.config.egg-info/top_level.txt
--rw-r--r--   0 vsts      (1001) docker     (122)       95 2023-01-10 15:31:44.000000 rcsb.utils.config-0.38/requirements.txt
--rwxr-xr-x   0 vsts      (1001) docker     (122)      108 2023-01-10 15:32:39.943317 rcsb.utils.config-0.38/setup.cfg
--rwxr-xr-x   0 vsts      (1001) docker     (122)     2427 2023-01-10 15:31:44.000000 rcsb.utils.config-0.38/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-16 11:01:02.096746 rcsb_utils_config-0.39/
+-rw-r--r--   0 vsts      (1001) docker     (127)     2332 2024-04-16 10:59:55.000000 rcsb_utils_config-0.39/HISTORY.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)      552 2024-04-16 10:59:55.000000 rcsb_utils_config-0.39/LICENSE
+-rw-r--r--   0 vsts      (1001) docker     (127)      106 2024-04-16 10:59:55.000000 rcsb_utils_config-0.39/MANIFEST.in
+-rw-r--r--   0 vsts      (1001) docker     (127)     1951 2024-04-16 11:01:02.096746 rcsb_utils_config-0.39/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)     1021 2024-04-16 10:59:55.000000 rcsb_utils_config-0.39/README.md
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-16 11:01:02.096746 rcsb_utils_config-0.39/rcsb/
+-rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-04-16 10:59:55.000000 rcsb_utils_config-0.39/rcsb/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-16 11:01:02.096746 rcsb_utils_config-0.39/rcsb/utils/
+-rw-r--r--   0 vsts      (1001) docker     (127)       65 2024-04-16 10:59:55.000000 rcsb_utils_config-0.39/rcsb/utils/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-16 11:01:02.096746 rcsb_utils_config-0.39/rcsb/utils/config/
+-rw-r--r--   0 vsts      (1001) docker     (127)    29277 2024-04-16 10:59:55.000000 rcsb_utils_config-0.39/rcsb/utils/config/ConfigUtil.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      121 2024-04-16 10:59:55.000000 rcsb_utils_config-0.39/rcsb/utils/config/ExampleHelper.py
+-rw-r--r--   0 vsts      (1001) docker     (127)      154 2024-04-16 10:59:55.000000 rcsb_utils_config-0.39/rcsb/utils/config/__init__.py
+drwxr-xr-x   0 vsts      (1001) docker     (127)        0 2024-04-16 11:01:02.096746 rcsb_utils_config-0.39/rcsb.utils.config.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (127)     1951 2024-04-16 11:01:02.000000 rcsb_utils_config-0.39/rcsb.utils.config.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (127)      458 2024-04-16 11:01:02.000000 rcsb_utils_config-0.39/rcsb.utils.config.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-16 11:01:02.000000 rcsb_utils_config-0.39/rcsb.utils.config.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        1 2024-04-16 11:00:45.000000 rcsb_utils_config-0.39/rcsb.utils.config.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (127)      132 2024-04-16 11:01:02.000000 rcsb_utils_config-0.39/rcsb.utils.config.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)        5 2024-04-16 11:01:02.000000 rcsb_utils_config-0.39/rcsb.utils.config.egg-info/top_level.txt
+-rw-r--r--   0 vsts      (1001) docker     (127)       95 2024-04-16 10:59:55.000000 rcsb_utils_config-0.39/requirements.txt
+-rwxr-xr-x   0 vsts      (1001) docker     (127)      108 2024-04-16 11:01:02.096746 rcsb_utils_config-0.39/setup.cfg
+-rwxr-xr-x   0 vsts      (1001) docker     (127)     2427 2024-04-16 10:59:55.000000 rcsb_utils_config-0.39/setup.py
```

### Comparing `rcsb.utils.config-0.38/HISTORY.txt` & `rcsb_utils_config-0.39/HISTORY.txt`

 * *Files 9% similar despite different names*

```diff
@@ -26,8 +26,9 @@
  3-Feb-2020  - V0.31 Add a reserved option to support one level of automatically incorporated configuration.
  3-Feb-2020  - V0.32 Use a generic temporary directory of incorporated configs if cache is not explicitly pathed.
  3-Feb-2020  - V0.33 Change defaults for cache behavior.
 13-May-2020  - V0.34 Update dependencies
 13-May-2020  - V0.35 Update dependencies
 22-Aug-2021  - V0.36 Update install script and fix linting issues
  3-Mar-2022  - V0.37 Clean-up logging messages
- 9-Jan-2023  - V0.38 Configuration changes to support tox 4 and testing python 3.9
+ 9-Jan-2023  - V0.38 Configuration changes to support tox 4 and testing python 3.9
+16-Apr-2024  - V0.39 Update setuptools config
```

### Comparing `rcsb.utils.config-0.38/LICENSE` & `rcsb_utils_config-0.39/LICENSE`

 * *Files identical despite different names*

### Comparing `rcsb.utils.config-0.38/PKG-INFO` & `rcsb_utils_config-0.39/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,26 +1,33 @@
 Metadata-Version: 2.1
 Name: rcsb.utils.config
-Version: 0.38
+Version: 0.39
 Summary: RCSB Python Configuration Utilities
 Home-page: https://github.com/rcsb/py-rcsb_utils_config
 Author: John Westbrook
 Author-email: john.westbrook@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: future
+Requires-Dist: configparser; python_version < "3.0"
+Requires-Dist: ruamel.yaml
+Requires-Dist: PyNaCl>=1.3.0
+Requires-Dist: rcsb.utils.io>=0.63
 Provides-Extra: dev
+Requires-Dist: check-manifest; extra == "dev"
 Provides-Extra: test
-License-File: LICENSE
+Requires-Dist: coverage; extra == "test"
 
 # RCSB Python Configuration Utilities
 
 [![Build Status](https://dev.azure.com/rcsb/RCSB%20PDB%20Python%20Projects/_apis/build/status/rcsb.py-rcsb_utils_config?branchName=master)](https://dev.azure.com/rcsb/RCSB%20PDB%20Python%20Projects/_build/latest?definitionId=8&branchName=master)
 
 ## Introduction
```

### Comparing `rcsb.utils.config-0.38/README.md` & `rcsb_utils_config-0.39/README.md`

 * *Files identical despite different names*

### Comparing `rcsb.utils.config-0.38/rcsb/utils/config/ConfigUtil.py` & `rcsb_utils_config-0.39/rcsb/utils/config/ConfigUtil.py`

 * *Files identical despite different names*

### Comparing `rcsb.utils.config-0.38/rcsb.utils.config.egg-info/PKG-INFO` & `rcsb_utils_config-0.39/rcsb.utils.config.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,26 +1,33 @@
 Metadata-Version: 2.1
 Name: rcsb.utils.config
-Version: 0.38
+Version: 0.39
 Summary: RCSB Python Configuration Utilities
 Home-page: https://github.com/rcsb/py-rcsb_utils_config
 Author: John Westbrook
 Author-email: john.westbrook@rcsb.org
 License: Apache 2.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Description-Content-Type: text/markdown
+License-File: LICENSE
+Requires-Dist: future
+Requires-Dist: configparser; python_version < "3.0"
+Requires-Dist: ruamel.yaml
+Requires-Dist: PyNaCl>=1.3.0
+Requires-Dist: rcsb.utils.io>=0.63
 Provides-Extra: dev
+Requires-Dist: check-manifest; extra == "dev"
 Provides-Extra: test
-License-File: LICENSE
+Requires-Dist: coverage; extra == "test"
 
 # RCSB Python Configuration Utilities
 
 [![Build Status](https://dev.azure.com/rcsb/RCSB%20PDB%20Python%20Projects/_apis/build/status/rcsb.py-rcsb_utils_config?branchName=master)](https://dev.azure.com/rcsb/RCSB%20PDB%20Python%20Projects/_build/latest?definitionId=8&branchName=master)
 
 ## Introduction
```

### Comparing `rcsb.utils.config-0.38/setup.py` & `rcsb_utils_config-0.39/setup.py`

 * *Files identical despite different names*

