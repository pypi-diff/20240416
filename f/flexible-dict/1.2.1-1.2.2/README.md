# Comparing `tmp/flexible_dict-1.2.1.tar.gz` & `tmp/flexible_dict-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flexible_dict-1.2.1.tar", last modified: Tue Aug 29 08:29:15 2023, max compression
+gzip compressed data, was "flexible_dict-1.2.2.tar", last modified: Tue Apr 16 06:48:49 2024, max compression
```

## Comparing `flexible_dict-1.2.1.tar` & `flexible_dict-1.2.2.tar`

### file list

```diff
@@ -1,22 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 08:29:15.632219 flexible_dict-1.2.1/
--rw-r--r--   0 runner    (1001) docker     (999)     2071 2023-08-29 08:29:15.632219 flexible_dict-1.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)     1791 2023-08-29 08:28:59.000000 flexible_dict-1.2.1/README.md
--rwxr-xr-x   0 runner    (1001) docker     (999)      117 2023-08-29 08:28:59.000000 flexible_dict-1.2.1/build.sh
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 08:29:15.632219 flexible_dict-1.2.1/flexible_dict/
--rw-r--r--   0 runner    (1001) docker     (999)      234 2023-08-29 08:28:59.000000 flexible_dict-1.2.1/flexible_dict/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)      532 2023-08-29 08:28:59.000000 flexible_dict-1.2.1/flexible_dict/__main__.py
--rw-r--r--   0 runner    (1001) docker     (999)      148 2023-08-29 08:29:15.000000 flexible_dict-1.2.1/flexible_dict/_dist_ver.py
--rw-r--r--   0 runner    (1001) docker     (999)     6299 2023-08-29 08:28:59.000000 flexible_dict-1.2.1/flexible_dict/adapter.py
--rw-r--r--   0 runner    (1001) docker     (999)    16994 2023-08-29 08:28:59.000000 flexible_dict-1.2.1/flexible_dict/json_object.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 08:29:15.632219 flexible_dict-1.2.1/flexible_dict/script/
--rw-r--r--   0 runner    (1001) docker     (999)       24 2023-08-29 08:28:59.000000 flexible_dict-1.2.1/flexible_dict/script/__init__.py
--rw-r--r--   0 runner    (1001) docker     (999)    12046 2023-08-29 08:28:59.000000 flexible_dict-1.2.1/flexible_dict/script/class_builder.py
--rw-r--r--   0 runner    (1001) docker     (999)      356 2023-08-29 08:28:59.000000 flexible_dict-1.2.1/flexible_dict/version.py
-drwxr-xr-x   0 runner    (1001) docker     (999)        0 2023-08-29 08:29:15.632219 flexible_dict-1.2.1/flexible_dict.egg-info/
--rw-r--r--   0 runner    (1001) docker     (999)     2071 2023-08-29 08:29:15.000000 flexible_dict-1.2.1/flexible_dict.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (999)      426 2023-08-29 08:29:15.000000 flexible_dict-1.2.1/flexible_dict.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (999)        1 2023-08-29 08:29:15.000000 flexible_dict-1.2.1/flexible_dict.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (999)       84 2023-08-29 08:29:15.000000 flexible_dict-1.2.1/flexible_dict.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (999)      828 2023-08-29 08:28:59.000000 flexible_dict-1.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (999)       55 2023-08-29 08:28:59.000000 flexible_dict-1.2.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (999)       38 2023-08-29 08:29:15.632219 flexible_dict-1.2.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 06:48:49.922201 flexible_dict-1.2.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     2179 2024-04-16 06:48:49.922201 flexible_dict-1.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1791 2024-04-16 06:48:44.000000 flexible_dict-1.2.2/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (127)      117 2024-04-16 06:48:44.000000 flexible_dict-1.2.2/build.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 06:48:49.918200 flexible_dict-1.2.2/flexible_dict/
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-16 06:48:44.000000 flexible_dict-1.2.2/flexible_dict/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      532 2024-04-16 06:48:44.000000 flexible_dict-1.2.2/flexible_dict/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-16 06:48:49.000000 flexible_dict-1.2.2/flexible_dict/_dist_ver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6299 2024-04-16 06:48:44.000000 flexible_dict-1.2.2/flexible_dict/adapter.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25777 2024-04-16 06:48:44.000000 flexible_dict-1.2.2/flexible_dict/json_object.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 06:48:49.922201 flexible_dict-1.2.2/flexible_dict/script/
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-16 06:48:44.000000 flexible_dict-1.2.2/flexible_dict/script/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12046 2024-04-16 06:48:44.000000 flexible_dict-1.2.2/flexible_dict/script/class_builder.py
+-rw-r--r--   0 runner    (1001) docker     (127)      356 2024-04-16 06:48:44.000000 flexible_dict-1.2.2/flexible_dict/version.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 06:48:49.922201 flexible_dict-1.2.2/flexible_dict.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2179 2024-04-16 06:48:49.000000 flexible_dict-1.2.2/flexible_dict.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-16 06:48:49.000000 flexible_dict-1.2.2/flexible_dict.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 06:48:49.000000 flexible_dict-1.2.2/flexible_dict.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       84 2024-04-16 06:48:49.000000 flexible_dict-1.2.2/flexible_dict.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      828 2024-04-16 06:48:44.000000 flexible_dict-1.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       55 2024-04-16 06:48:44.000000 flexible_dict-1.2.2/requirements.txt
+-rwxr-xr-x   0 runner    (1001) docker     (127)      359 2024-04-16 06:48:44.000000 flexible_dict-1.2.2/run_test.sh
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 06:48:49.922201 flexible_dict-1.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-16 06:48:44.000000 flexible_dict-1.2.2/tox.ini
```

### Comparing `flexible_dict-1.2.1/PKG-INFO` & `flexible_dict-1.2.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,7 @@
-Metadata-Version: 2.1
-Name: flexible_dict
-Version: 1.2.1
-Summary: A flexible way to access dict data instead of built-in dict.
-Author-email: darkpeath <darkpeath@gmail.com>
-Project-URL: Homepage, https://github.com/darkpeath/flexible_dict
-Description-Content-Type: text/markdown
-
 # Flexible Dict
 
 A flexible way to access dict data instead of built-in dict.
 
 ## Installation
 
 ```shell
```

### Comparing `flexible_dict-1.2.1/README.md` & `flexible_dict-1.2.2/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+Metadata-Version: 2.1
+Name: flexible_dict
+Version: 1.2.2
+Summary: A flexible way to access dict data instead of built-in dict.
+Author-email: darkpeath <darkpeath@gmail.com>
+Project-URL: Homepage, https://github.com/darkpeath/flexible_dict
+Description-Content-Type: text/markdown
+Requires-Dist: dataclasses; python_version < "3.7"
+Requires-Dist: typing_extensions; python_version < "3.8"
+
 # Flexible Dict
 
 A flexible way to access dict data instead of built-in dict.
 
 ## Installation
 
 ```shell
```

### Comparing `flexible_dict-1.2.1/flexible_dict/__main__.py` & `flexible_dict-1.2.2/flexible_dict/__main__.py`

 * *Files identical despite different names*

### Comparing `flexible_dict-1.2.1/flexible_dict/adapter.py` & `flexible_dict-1.2.2/flexible_dict/adapter.py`

 * *Files identical despite different names*

### Comparing `flexible_dict-1.2.1/flexible_dict/script/class_builder.py` & `flexible_dict-1.2.2/flexible_dict/script/class_builder.py`

 * *Files identical despite different names*

### Comparing `flexible_dict-1.2.1/flexible_dict.egg-info/PKG-INFO` & `flexible_dict-1.2.2/flexible_dict.egg-info/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
-Name: flexible-dict
-Version: 1.2.1
+Name: flexible_dict
+Version: 1.2.2
 Summary: A flexible way to access dict data instead of built-in dict.
 Author-email: darkpeath <darkpeath@gmail.com>
 Project-URL: Homepage, https://github.com/darkpeath/flexible_dict
 Description-Content-Type: text/markdown
+Requires-Dist: dataclasses; python_version < "3.7"
+Requires-Dist: typing_extensions; python_version < "3.8"
 
 # Flexible Dict
 
 A flexible way to access dict data instead of built-in dict.
 
 ## Installation
```

### Comparing `flexible_dict-1.2.1/pyproject.toml` & `flexible_dict-1.2.2/pyproject.toml`

 * *Files identical despite different names*

