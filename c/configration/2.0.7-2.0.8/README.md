# Comparing `tmp/configration-2.0.7.tar.gz` & `tmp/configration-2.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "configration-2.0.7.tar", last modified: Sun Aug  6 15:31:21 2023, max compression
+gzip compressed data, was "configration-2.0.8.tar", last modified: Tue Apr 16 13:29:04 2024, max compression
```

## Comparing `configration-2.0.7.tar` & `configration-2.0.8.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-08-06 15:31:21.063592 configration-2.0.7/
--rwxrwxrwx   0 jeff      (1000) jeff      (1001)    33889 2018-03-05 16:24:54.000000 configration-2.0.7/LICENSE.txt
--rw-r--r--   0 jeff      (1000) jeff      (1001)     1311 2023-08-06 15:31:21.063592 configration-2.0.7/PKG-INFO
--rwxrwxrwx   0 jeff      (1000) jeff      (1001)      115 2023-05-10 10:08:06.000000 configration-2.0.7/README.md
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-08-06 15:31:21.053592 configration-2.0.7/configration/
--rw-r--r--   0 jeff      (1000) jeff      (1001)      175 2023-05-29 08:17:28.000000 configration-2.0.7/configration/__init__.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)       22 2023-08-06 13:47:54.000000 configration-2.0.7/configration/_version.py
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-08-06 15:31:21.060259 configration-2.0.7/configration/src/
--rw-r--r--   0 jeff      (1000) jeff      (1001)        0 2023-06-29 13:36:13.000000 configration-2.0.7/configration/src/__init__.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     2631 2023-06-29 13:36:13.000000 configration-2.0.7/configration/src/config.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)      397 2023-06-29 13:36:13.000000 configration-2.0.7/configration/src/constants.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     1509 2023-06-29 13:36:13.000000 configration-2.0.7/configration/src/json_config.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     2019 2023-08-06 15:04:48.000000 configration-2.0.7/configration/src/toml_config.py
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-08-06 15:31:21.063592 configration-2.0.7/configration/tests/
--rw-r--r--   0 jeff      (1000) jeff      (1001)        0 2023-06-29 13:36:13.000000 configration-2.0.7/configration/tests/__init__.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     2909 2023-06-29 13:36:13.000000 configration-2.0.7/configration/tests/test_config.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     1762 2023-06-29 13:36:13.000000 configration-2.0.7/configration/tests/test_json.py
--rw-r--r--   0 jeff      (1000) jeff      (1001)     2257 2023-08-06 15:30:15.000000 configration-2.0.7/configration/tests/test_toml.py
-drwxr-xr-x   0 jeff      (1000) jeff      (1001)        0 2023-08-06 15:31:21.056925 configration-2.0.7/configration.egg-info/
--rw-r--r--   0 jeff      (1000) jeff      (1001)     1311 2023-08-06 15:31:21.000000 configration-2.0.7/configration.egg-info/PKG-INFO
--rw-r--r--   0 jeff      (1000) jeff      (1001)      513 2023-08-06 15:31:21.000000 configration-2.0.7/configration.egg-info/SOURCES.txt
--rw-r--r--   0 jeff      (1000) jeff      (1001)        1 2023-08-06 15:31:21.000000 configration-2.0.7/configration.egg-info/dependency_links.txt
--rw-r--r--   0 jeff      (1000) jeff      (1001)       13 2023-08-06 15:31:21.000000 configration-2.0.7/configration.egg-info/top_level.txt
--rw-r--r--   0 jeff      (1000) jeff      (1001)       38 2023-08-06 15:31:21.063592 configration-2.0.7/setup.cfg
--rw-r--r--   0 jeff      (1000) jeff      (1001)     1180 2023-07-24 08:24:01.000000 configration-2.0.7/setup.py
+drwxr-xr-x   0 jeff      (1000) jeff      (1000)        0 2024-04-16 13:29:04.984440 configration-2.0.8/
+-rw-r--r--   0 jeff      (1000) jeff      (1000)    33889 2018-03-05 16:24:54.000000 configration-2.0.8/LICENSE.txt
+-rw-r--r--   0 jeff      (1000) jeff      (1000)     1321 2024-04-16 13:29:04.981106 configration-2.0.8/PKG-INFO
+-rw-r--r--   0 jeff      (1000) jeff      (1000)      115 2023-05-10 10:08:06.000000 configration-2.0.8/README.md
+drwxr-xr-x   0 jeff      (1000) jeff      (1000)        0 2024-04-16 13:29:04.981106 configration-2.0.8/configration/
+-rw-r--r--   0 jeff      (1000) jeff      (1000)      175 2023-05-29 08:17:28.000000 configration-2.0.8/configration/__init__.py
+-rw-r--r--   0 jeff      (1000) jeff      (1000)       22 2024-04-16 13:27:15.000000 configration-2.0.8/configration/_version.py
+drwxr-xr-x   0 jeff      (1000) jeff      (1000)        0 2024-04-16 13:29:04.981106 configration-2.0.8/configration/src/
+-rw-r--r--   0 jeff      (1000) jeff      (1000)        0 2023-06-29 13:36:12.000000 configration-2.0.8/configration/src/__init__.py
+-rw-r--r--   0 jeff      (1000) jeff      (1000)     2791 2024-04-16 13:26:52.000000 configration-2.0.8/configration/src/config.py
+-rw-r--r--   0 jeff      (1000) jeff      (1000)      397 2023-06-29 13:36:12.000000 configration-2.0.8/configration/src/constants.py
+-rw-r--r--   0 jeff      (1000) jeff      (1000)     1509 2023-06-29 13:36:12.000000 configration-2.0.8/configration/src/json_config.py
+-rw-r--r--   0 jeff      (1000) jeff      (1000)     2019 2023-08-06 15:04:48.000000 configration-2.0.8/configration/src/toml_config.py
+drwxr-xr-x   0 jeff      (1000) jeff      (1000)        0 2024-04-16 13:29:04.981106 configration-2.0.8/configration/tests/
+-rw-r--r--   0 jeff      (1000) jeff      (1000)        0 2023-06-29 13:36:12.000000 configration-2.0.8/configration/tests/__init__.py
+-rw-r--r--   0 jeff      (1000) jeff      (1000)     2909 2023-06-29 13:36:12.000000 configration-2.0.8/configration/tests/test_config.py
+-rw-r--r--   0 jeff      (1000) jeff      (1000)     1762 2023-06-29 13:36:12.000000 configration-2.0.8/configration/tests/test_json.py
+-rw-r--r--   0 jeff      (1000) jeff      (1000)     2257 2023-08-06 15:30:14.000000 configration-2.0.8/configration/tests/test_toml.py
+drwxr-xr-x   0 jeff      (1000) jeff      (1000)        0 2024-04-16 13:29:04.981106 configration-2.0.8/configration.egg-info/
+-rw-r--r--   0 jeff      (1000) jeff      (1000)     1321 2024-04-16 13:29:04.000000 configration-2.0.8/configration.egg-info/PKG-INFO
+-rw-r--r--   0 jeff      (1000) jeff      (1000)      513 2024-04-16 13:29:04.000000 configration-2.0.8/configration.egg-info/SOURCES.txt
+-rw-r--r--   0 jeff      (1000) jeff      (1000)        1 2024-04-16 13:29:04.000000 configration-2.0.8/configration.egg-info/dependency_links.txt
+-rw-r--r--   0 jeff      (1000) jeff      (1000)       13 2024-04-16 13:29:04.000000 configration-2.0.8/configration.egg-info/top_level.txt
+-rw-r--r--   0 jeff      (1000) jeff      (1000)       38 2024-04-16 13:29:04.984440 configration-2.0.8/setup.cfg
+-rw-r--r--   0 jeff      (1000) jeff      (1000)     1158 2023-12-03 12:32:36.000000 configration-2.0.8/setup.py
```

### Comparing `configration-2.0.7/LICENSE.txt` & `configration-2.0.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `configration-2.0.7/PKG-INFO` & `configration-2.0.8/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: configration
-Version: 2.0.7
-Summary: """A collection of modules that supports workbooks with openpyxl."""
+Version: 2.0.8
+Summary: """A utility for json or toml config files."""
 Home-page: https://psionman@bitbucket.org/psionman/bfgdealer.git
+Download-URL: https://pypi.org/project/bfgdealer/
 Author: jeff watkins
 Author-email: support@bidforgame.com
 License: MIT
-Download-URL: https://pypi.org/project/bfgdealer/
 Keywords: cli,input
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # configration
 
 A module to validate and load config files.
 
@@ -21,14 +20,20 @@
 ```bash
 pip install configration
 ```
 
 
 # Version History
 
+Version 2.0.8 16 Apr 2024
+
+1. Add defaults
+
+------
+
 Version 2.0.7 6 Aug 2023
 
 1. Status constant on  save toml_config
 
 ------
 
 Version 2.0.6 29 Jun 2023
@@ -85,9 +90,7 @@
 ------
 
 Version 0.0.0 10 May 2023
 
 1. Initial version
 
 ------
-
-
```

### Comparing `configration-2.0.7/configration/src/config.py` & `configration-2.0.8/configration/src/config.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,18 +29,23 @@
 
     create: bool
         Whether or not the config should be created if missing.
         Defaults to False.
         (The individual sub-classes implement the function.)
     """
 
-    def __init__(self, path: str,
-                 attrs: dict[str, list[type]] = {},
-                 create: bool = False):
+    def __init__(
+            self,
+            path: str,
+            defaults: dict[str, str] = {},
+            attrs: dict[str, list[type]] = {},
+            create: bool = False
+        ):
         self.path = path
+        self.defaults = defaults
         self.attrs = attrs
         self.create = create
         self.config = self._get_config()
         for key, item in self.config.items():
             self.__dict__[key] = item
 
     def __repr__(self):
@@ -56,14 +61,17 @@
         config = self._read_config()
 
         if config and not self.attrs:
             return config
 
         if config and self._validate_config(config):
             return config
+
+        if self.defaults:
+            return self.defaults
         return {}
 
     def _validate_config(self, config: dict[str, type]) -> bool:
         # Return True if structure and values in config are valid.
         for name, item_types in self.attrs.items():
             if name not in config:
                 cprint(f"{CORRUPT_FILE_MSG} {MISSING_ATTR_MSG} {name}", ERROR_COLOUR)
```

### Comparing `configration-2.0.7/configration/src/json_config.py` & `configration-2.0.8/configration/src/json_config.py`

 * *Files identical despite different names*

### Comparing `configration-2.0.7/configration/src/toml_config.py` & `configration-2.0.8/configration/src/toml_config.py`

 * *Files identical despite different names*

### Comparing `configration-2.0.7/configration/tests/test_config.py` & `configration-2.0.8/configration/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `configration-2.0.7/configration/tests/test_json.py` & `configration-2.0.8/configration/tests/test_json.py`

 * *Files identical despite different names*

### Comparing `configration-2.0.7/configration/tests/test_toml.py` & `configration-2.0.8/configration/tests/test_toml.py`

 * *Files identical despite different names*

### Comparing `configration-2.0.7/configration.egg-info/PKG-INFO` & `configration-2.0.8/configration.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 Metadata-Version: 2.1
 Name: configration
-Version: 2.0.7
-Summary: """A collection of modules that supports workbooks with openpyxl."""
+Version: 2.0.8
+Summary: """A utility for json or toml config files."""
 Home-page: https://psionman@bitbucket.org/psionman/bfgdealer.git
+Download-URL: https://pypi.org/project/bfgdealer/
 Author: jeff watkins
 Author-email: support@bidforgame.com
 License: MIT
-Download-URL: https://pypi.org/project/bfgdealer/
 Keywords: cli,input
-Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # configration
 
 A module to validate and load config files.
 
@@ -21,14 +20,20 @@
 ```bash
 pip install configration
 ```
 
 
 # Version History
 
+Version 2.0.8 16 Apr 2024
+
+1. Add defaults
+
+------
+
 Version 2.0.7 6 Aug 2023
 
 1. Status constant on  save toml_config
 
 ------
 
 Version 2.0.6 29 Jun 2023
@@ -85,9 +90,7 @@
 ------
 
 Version 0.0.0 10 May 2023
 
 1. Initial version
 
 ------
-
-
```

### Comparing `configration-2.0.7/configration.egg-info/SOURCES.txt` & `configration-2.0.8/configration.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `configration-2.0.7/setup.py` & `configration-2.0.8/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 else:
     raise RuntimeError(f'Unable to find version string in {VERSION_FILE}.')
 
 
 setup_args = dict(
     name='configration',
     version=version_string,
-    description='"""A collection of modules that supports workbooks with openpyxl."""',
+    description='"""A utility for json or toml config files."""',
     long_description_content_type="text/markdown",
     long_description=README + '\n\n' + HISTORY,
     license='MIT',
     packages=find_packages(),
     author='jeff watkins',
     author_email='support@bidforgame.com',
     keywords=['cli', 'input'],
```

