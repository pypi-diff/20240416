# Comparing `tmp/example_package_mxgnxs-0.0.1.tar.gz` & `tmp/example_package_mxgnxs-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "example_package_mxgnxs-0.0.1.tar", last modified: Tue Apr 16 05:14:46 2024, max compression
+gzip compressed data, was "example_package_mxgnxs-0.0.2.tar", last modified: Tue Apr 16 05:21:47 2024, max compression
```

## Comparing `example_package_mxgnxs-0.0.1.tar` & `example_package_mxgnxs-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,12 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 05:14:46.280954 example_package_mxgnxs-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-04-16 05:14:42.000000 example_package_mxgnxs-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-16 05:14:46.280954 example_package_mxgnxs-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-16 05:14:42.000000 example_package_mxgnxs-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-16 05:14:42.000000 example_package_mxgnxs-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      564 2024-04-16 05:14:46.280954 example_package_mxgnxs-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 05:14:46.280954 example_package_mxgnxs-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 05:14:46.280954 example_package_mxgnxs-0.0.1/src/example-package-mxgnxs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 05:14:42.000000 example_package_mxgnxs-0.0.1/src/example-package-mxgnxs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       42 2024-04-16 05:14:42.000000 example_package_mxgnxs-0.0.1/src/example-package-mxgnxs/example.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 05:14:46.280954 example_package_mxgnxs-0.0.1/src/example_package_mxgnxs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-16 05:14:46.000000 example_package_mxgnxs-0.0.1/src/example_package_mxgnxs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      319 2024-04-16 05:14:46.000000 example_package_mxgnxs-0.0.1/src/example_package_mxgnxs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 05:14:46.000000 example_package_mxgnxs-0.0.1/src/example_package_mxgnxs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-16 05:14:46.000000 example_package_mxgnxs-0.0.1/src/example_package_mxgnxs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 05:21:47.004969 example_package_mxgnxs-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1054 2024-04-16 05:21:42.000000 example_package_mxgnxs-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-16 05:21:47.004969 example_package_mxgnxs-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-16 05:21:42.000000 example_package_mxgnxs-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      103 2024-04-16 05:21:42.000000 example_package_mxgnxs-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      527 2024-04-16 05:21:47.004969 example_package_mxgnxs-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 05:21:47.004969 example_package_mxgnxs-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 05:21:47.004969 example_package_mxgnxs-0.0.2/src/example_package_mxgnxs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-16 05:21:46.000000 example_package_mxgnxs-0.0.2/src/example_package_mxgnxs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      242 2024-04-16 05:21:47.000000 example_package_mxgnxs-0.0.2/src/example_package_mxgnxs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 05:21:46.000000 example_package_mxgnxs-0.0.2/src/example_package_mxgnxs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 05:21:46.000000 example_package_mxgnxs-0.0.2/src/example_package_mxgnxs.egg-info/top_level.txt
```

### Comparing `example_package_mxgnxs-0.0.1/LICENSE` & `example_package_mxgnxs-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `example_package_mxgnxs-0.0.1/PKG-INFO` & `example_package_mxgnxs-0.0.2/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: example_package_mxgnxs
-Version: 0.0.1
+Version: 0.0.2
 Summary: Simple test project
 Home-page: https://github.com/CMM02/python-publishing
 Author: Carl Magnus Meier
 Author-email: magnus.meier@outook.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `example_package_mxgnxs-0.0.1/setup.cfg` & `example_package_mxgnxs-0.0.2/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = example_package_mxgnxs
-version = 0.0.1
+version = 0.0.2
 author = Carl Magnus Meier
 author_email = magnus.meier@outook.de
 description = Simple test project
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/CMM02/python-publishing
 classifiers = 
@@ -14,14 +14,11 @@
 
 [options]
 package_dir = 
 	= src
 packages = find:
 python_requires = >=3.8
 
-[options.packages.find]
-where = src
-
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `example_package_mxgnxs-0.0.1/src/example_package_mxgnxs.egg-info/PKG-INFO` & `example_package_mxgnxs-0.0.2/src/example_package_mxgnxs.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: example_package_mxgnxs
-Version: 0.0.1
+Version: 0.0.2
 Summary: Simple test project
 Home-page: https://github.com/CMM02/python-publishing
 Author: Carl Magnus Meier
 Author-email: magnus.meier@outook.de
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

