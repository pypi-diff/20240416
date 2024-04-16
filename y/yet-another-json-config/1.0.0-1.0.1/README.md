# Comparing `tmp/yet-another-json-config-1.0.0.tar.gz` & `tmp/yet_another_json_config-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yet-another-json-config-1.0.0.tar", last modified: Sat Apr  6 18:04:41 2024, max compression
+gzip compressed data, was "yet_another_json_config-1.0.1.tar", last modified: Tue Apr 16 20:13:00 2024, max compression
```

## Comparing `yet-another-json-config-1.0.0.tar` & `yet_another_json_config-1.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:04:41.673148 yet-another-json-config-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-06 18:04:37.000000 yet-another-json-config-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4838 2024-04-06 18:04:41.673148 yet-another-json-config-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-04-06 18:04:37.000000 yet-another-json-config-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-06 18:04:37.000000 yet-another-json-config-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-06 18:04:41.673148 yet-another-json-config-1.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:04:41.669149 yet-another-json-config-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:04:41.669149 yet-another-json-config-1.0.0/src/yet_another_json_config/
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-06 18:04:37.000000 yet-another-json-config-1.0.0/src/yet_another_json_config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7312 2024-04-06 18:04:37.000000 yet-another-json-config-1.0.0/src/yet_another_json_config/yet_another_json_config.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:04:41.673148 yet-another-json-config-1.0.0/src/yet_another_json_config.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4838 2024-04-06 18:04:41.000000 yet-another-json-config-1.0.0/src/yet_another_json_config.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-06 18:04:41.000000 yet-another-json-config-1.0.0/src/yet_another_json_config.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 18:04:41.000000 yet-another-json-config-1.0.0/src/yet_another_json_config.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-06 18:04:41.000000 yet-another-json-config-1.0.0/src/yet_another_json_config.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 18:04:41.673148 yet-another-json-config-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     4814 2024-04-06 18:04:37.000000 yet-another-json-config-1.0.0/tests/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:13:00.299625 yet_another_json_config-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1066 2024-04-16 20:12:55.000000 yet_another_json_config-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4838 2024-04-16 20:13:00.299625 yet_another_json_config-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4237 2024-04-16 20:12:55.000000 yet_another_json_config-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      671 2024-04-16 20:12:55.000000 yet_another_json_config-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 20:13:00.299625 yet_another_json_config-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:13:00.295625 yet_another_json_config-1.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:13:00.299625 yet_another_json_config-1.0.1/src/yet_another_json_config/
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-16 20:12:55.000000 yet_another_json_config-1.0.1/src/yet_another_json_config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7318 2024-04-16 20:12:55.000000 yet_another_json_config-1.0.1/src/yet_another_json_config/yet_another_json_config.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:13:00.299625 yet_another_json_config-1.0.1/src/yet_another_json_config.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4838 2024-04-16 20:13:00.000000 yet_another_json_config-1.0.1/src/yet_another_json_config.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      352 2024-04-16 20:13:00.000000 yet_another_json_config-1.0.1/src/yet_another_json_config.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 20:13:00.000000 yet_another_json_config-1.0.1/src/yet_another_json_config.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-16 20:13:00.000000 yet_another_json_config-1.0.1/src/yet_another_json_config.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 20:13:00.299625 yet_another_json_config-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     4814 2024-04-16 20:12:55.000000 yet_another_json_config-1.0.1/tests/test_config.py
```

### Comparing `yet-another-json-config-1.0.0/LICENSE` & `yet_another_json_config-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `yet-another-json-config-1.0.0/PKG-INFO` & `yet_another_json_config-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yet-another-json-config
-Version: 1.0.0
+Version: 1.0.1
 Summary: Reads and write json files as a configuration file, supports nested json values.
 Author-email: engmtcdrm <gabif54409@rolenot.com>
 Project-URL: Homepage, https://github.com/engmtcdrm/yet-another-json-config
 Project-URL: Bug Tracker, https://github.com/engmtcdrm/yet-another-json-config/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `yet-another-json-config-1.0.0/README.md` & `yet_another_json_config-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `yet-another-json-config-1.0.0/pyproject.toml` & `yet_another_json_config-1.0.1/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ['setuptools>=42']
 build-backend = 'setuptools.build_meta'
 
 [project]
 name = "yet-another-json-config"
-version = "1.0.0"
+version = "1.0.1"
 authors = [
   { name="engmtcdrm", email="gabif54409@rolenot.com" },
 ]
 description = "Reads and write json files as a configuration file, supports nested json values."
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `yet-another-json-config-1.0.0/src/yet_another_json_config/yet_another_json_config.py` & `yet_another_json_config-1.0.1/src/yet_another_json_config/yet_another_json_config.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Reads and write json files as a configuration file, supports nested json values."""
 import json
 import os
-from typing import Union, Optional
+from typing import Union, Optional, List
 
 class Config():
     """
     Create an instance of a configuration file.
 
     :params config_file_path: The path to the configuration file.
     :params file_must_exist: (optional) Raises a FileNotFoundError exception if file does not exist. (default: ``False``)
@@ -58,15 +58,15 @@
             self._settings = settings
         else:
             raise FileNotFoundError(f'Config File {self._config_file_path} does not exist.')
 
     def _convert_keys_to_list(
         self,
         keys: Union[str, tuple, list]
-    ) -> list[str]:
+    ) -> List[str]:
         """
         Convert the keys to a list.
 
         :params keys: The keys to be converted.
         :return: The converted keys as a list.
         """
         if isinstance(keys[0], tuple):
```

### Comparing `yet-another-json-config-1.0.0/src/yet_another_json_config.egg-info/PKG-INFO` & `yet_another_json_config-1.0.1/src/yet_another_json_config.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yet-another-json-config
-Version: 1.0.0
+Version: 1.0.1
 Summary: Reads and write json files as a configuration file, supports nested json values.
 Author-email: engmtcdrm <gabif54409@rolenot.com>
 Project-URL: Homepage, https://github.com/engmtcdrm/yet-another-json-config
 Project-URL: Bug Tracker, https://github.com/engmtcdrm/yet-another-json-config/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `yet-another-json-config-1.0.0/tests/test_config.py` & `yet_another_json_config-1.0.1/tests/test_config.py`

 * *Files identical despite different names*

