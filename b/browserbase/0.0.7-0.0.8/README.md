# Comparing `tmp/browserbase-0.0.7.tar.gz` & `tmp/browserbase-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "browserbase-0.0.7.tar", last modified: Mon Apr 15 14:23:31 2024, max compression
+gzip compressed data, was "browserbase-0.0.8.tar", last modified: Tue Apr 16 18:32:11 2024, max compression
```

## Comparing `browserbase-0.0.7.tar` & `browserbase-0.0.8.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 mish       (501) staff       (20)        0 2024-04-15 14:23:31.830652 browserbase-0.0.7/
--rw-r--r--   0 mish       (501) staff       (20)     1064 2024-04-09 17:45:47.000000 browserbase-0.0.7/LICENSE
--rw-r--r--   0 mish       (501) staff       (20)     1081 2024-04-15 14:23:31.830370 browserbase-0.0.7/PKG-INFO
--rw-r--r--   0 mish       (501) staff       (20)      544 2024-04-14 22:01:12.000000 browserbase-0.0.7/README.md
-drwxr-xr-x   0 mish       (501) staff       (20)        0 2024-04-15 14:23:31.828889 browserbase-0.0.7/browserbase/
--rw-r--r--   0 mish       (501) staff       (20)     3217 2024-04-15 14:21:43.000000 browserbase-0.0.7/browserbase/__init__.py
-drwxr-xr-x   0 mish       (501) staff       (20)        0 2024-04-15 14:23:31.829809 browserbase-0.0.7/browserbase/helpers/
--rw-r--r--   0 mish       (501) staff       (20)      503 2024-04-15 12:54:51.000000 browserbase-0.0.7/browserbase/helpers/gpt4.py
-drwxr-xr-x   0 mish       (501) staff       (20)        0 2024-04-15 14:23:31.830111 browserbase-0.0.7/browserbase.egg-info/
--rw-r--r--   0 mish       (501) staff       (20)     1081 2024-04-15 14:23:31.000000 browserbase-0.0.7/browserbase.egg-info/PKG-INFO
--rw-r--r--   0 mish       (501) staff       (20)      258 2024-04-15 14:23:31.000000 browserbase-0.0.7/browserbase.egg-info/SOURCES.txt
--rw-r--r--   0 mish       (501) staff       (20)        1 2024-04-15 14:23:31.000000 browserbase-0.0.7/browserbase.egg-info/dependency_links.txt
--rw-r--r--   0 mish       (501) staff       (20)       19 2024-04-15 14:23:31.000000 browserbase-0.0.7/browserbase.egg-info/requires.txt
--rw-r--r--   0 mish       (501) staff       (20)       12 2024-04-15 14:23:31.000000 browserbase-0.0.7/browserbase.egg-info/top_level.txt
--rw-r--r--   0 mish       (501) staff       (20)      618 2024-04-15 14:23:20.000000 browserbase-0.0.7/pyproject.toml
--rw-r--r--   0 mish       (501) staff       (20)       38 2024-04-15 14:23:31.830730 browserbase-0.0.7/setup.cfg
+drwxr-xr-x   0 mish       (501) staff       (20)        0 2024-04-16 18:32:11.311587 browserbase-0.0.8/
+-rw-r--r--   0 mish       (501) staff       (20)     1064 2024-04-09 17:45:47.000000 browserbase-0.0.8/LICENSE
+-rw-r--r--   0 mish       (501) staff       (20)     1081 2024-04-16 18:32:11.311361 browserbase-0.0.8/PKG-INFO
+-rw-r--r--   0 mish       (501) staff       (20)      544 2024-04-15 14:52:48.000000 browserbase-0.0.8/README.md
+drwxr-xr-x   0 mish       (501) staff       (20)        0 2024-04-16 18:32:11.309580 browserbase-0.0.8/browserbase/
+-rw-r--r--   0 mish       (501) staff       (20)     3217 2024-04-16 18:31:30.000000 browserbase-0.0.8/browserbase/__init__.py
+drwxr-xr-x   0 mish       (501) staff       (20)        0 2024-04-16 18:32:11.310579 browserbase-0.0.8/browserbase/helpers/
+-rw-r--r--   0 mish       (501) staff       (20)      301 2024-04-16 18:32:01.000000 browserbase-0.0.8/browserbase/helpers/anthropic.py
+-rw-r--r--   0 mish       (501) staff       (20)      503 2024-04-15 12:54:51.000000 browserbase-0.0.8/browserbase/helpers/gpt4.py
+drwxr-xr-x   0 mish       (501) staff       (20)        0 2024-04-16 18:32:11.311081 browserbase-0.0.8/browserbase.egg-info/
+-rw-r--r--   0 mish       (501) staff       (20)     1081 2024-04-16 18:32:11.000000 browserbase-0.0.8/browserbase.egg-info/PKG-INFO
+-rw-r--r--   0 mish       (501) staff       (20)      291 2024-04-16 18:32:11.000000 browserbase-0.0.8/browserbase.egg-info/SOURCES.txt
+-rw-r--r--   0 mish       (501) staff       (20)        1 2024-04-16 18:32:11.000000 browserbase-0.0.8/browserbase.egg-info/dependency_links.txt
+-rw-r--r--   0 mish       (501) staff       (20)       19 2024-04-16 18:32:11.000000 browserbase-0.0.8/browserbase.egg-info/requires.txt
+-rw-r--r--   0 mish       (501) staff       (20)       12 2024-04-16 18:32:11.000000 browserbase-0.0.8/browserbase.egg-info/top_level.txt
+-rw-r--r--   0 mish       (501) staff       (20)      618 2024-04-16 18:31:37.000000 browserbase-0.0.8/pyproject.toml
+-rw-r--r--   0 mish       (501) staff       (20)       38 2024-04-16 18:32:11.311638 browserbase-0.0.8/setup.cfg
```

### Comparing `browserbase-0.0.7/LICENSE` & `browserbase-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `browserbase-0.0.7/PKG-INFO` & `browserbase-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: browserbase
-Version: 0.0.7
+Version: 0.0.8
 Summary: Browserbase Python SDK
 Author-email: Browserbase <info@browserbase.com>
 Project-URL: Homepage, https://github.com/browserbase/python-sdk
 Project-URL: Issues, https://github.com/browserbase/python-sdk/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `browserbase-0.0.7/README.md` & `browserbase-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `browserbase-0.0.7/browserbase/__init__.py` & `browserbase-0.0.8/browserbase/__init__.py`

 * *Files identical despite different names*

### Comparing `browserbase-0.0.7/browserbase.egg-info/PKG-INFO` & `browserbase-0.0.8/browserbase.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: browserbase
-Version: 0.0.7
+Version: 0.0.8
 Summary: Browserbase Python SDK
 Author-email: Browserbase <info@browserbase.com>
 Project-URL: Homepage, https://github.com/browserbase/python-sdk
 Project-URL: Issues, https://github.com/browserbase/python-sdk/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `browserbase-0.0.7/pyproject.toml` & `browserbase-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "browserbase"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="Browserbase", email="info@browserbase.com" },
 ]
 description = "Browserbase Python SDK"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

