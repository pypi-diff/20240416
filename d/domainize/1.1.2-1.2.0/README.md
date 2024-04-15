# Comparing `tmp/domainize-1.1.2.tar.gz` & `tmp/domainize-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "domainize-1.1.2.tar", max compression
+gzip compressed data, was "domainize-1.2.0.tar", max compression
```

## Comparing `domainize-1.1.2.tar` & `domainize-1.2.0.tar`

### file list

```diff
@@ -1,4 +1,5 @@
--rw-r--r--   0        0        0      455 2023-10-11 15:32:14.957015 domainize-1.1.2/README.md
--rw-r--r--   0        0        0     1022 2023-10-11 15:32:14.958015 domainize-1.1.2/domainize/__init__.py
--rw-r--r--   0        0        0     1457 2023-10-11 15:32:14.958015 domainize-1.1.2/pyproject.toml
--rw-r--r--   0        0        0     1266 1970-01-01 00:00:00.000000 domainize-1.1.2/PKG-INFO
+-rw-r--r--   0        0        0      455 2024-04-15 23:01:03.698965 domainize-1.2.0/README.md
+-rw-r--r--   0        0        0     1071 2024-04-15 23:01:03.698965 domainize-1.2.0/domainize/__init__.py
+-rw-r--r--   0        0        0    85498 2024-04-15 23:01:03.698965 domainize-1.2.0/domainize/resources/public_suffix_list.dat.gz
+-rw-r--r--   0        0        0     1457 2024-04-15 23:01:03.698965 domainize-1.2.0/pyproject.toml
+-rw-r--r--   0        0        0     1317 1970-01-01 00:00:00.000000 domainize-1.2.0/PKG-INFO
```

### Comparing `domainize-1.1.2/pyproject.toml` & `domainize-1.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "domainize"
-version = "1.1.2"
+version = "1.2.0"
 description = "Library for extracting domains."
 authors = ["Data <data@camber.io>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://gitlab.com/rocket-boosters/pipper/domainize"
 repository = "https://gitlab.com/rocket-boosters/pipper/domainize"
 documentation = "https://gitlab.com/rocket-boosters/pipper/domainize"
```

### Comparing `domainize-1.1.2/PKG-INFO` & `domainize-1.2.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: domainize
-Version: 1.1.2
+Version: 1.2.0
 Summary: Library for extracting domains.
 Home-page: https://gitlab.com/rocket-boosters/pipper/domainize
 License: MIT
 Author: Data
 Author-email: data@camber.io
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Typing :: Typed
 Project-URL: Documentation, https://gitlab.com/rocket-boosters/pipper/domainize
 Project-URL: Repository, https://gitlab.com/rocket-boosters/pipper/domainize
 Description-Content-Type: text/markdown
 
 # Domainize
```

