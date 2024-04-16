# Comparing `tmp/convcom-0.0.0.tar.gz` & `tmp/convcom-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "convcom-0.0.0.tar", last modified: Tue Apr 16 13:06:00 2024, max compression
+gzip compressed data, was "convcom-0.1.1.tar", last modified: Tue Apr 16 13:13:42 2024, max compression
```

## Comparing `convcom-0.0.0.tar` & `convcom-0.1.1.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:06:00.541374 convcom-0.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-16 13:05:56.000000 convcom-0.0.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:06:00.537373 convcom-0.0.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:06:00.537373 convcom-0.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     3173 2024-04-16 13:05:56.000000 convcom-0.0.0/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-16 13:05:56.000000 convcom-0.0.0/.github/workflows/run-pytest.yml
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-16 13:05:56.000000 convcom-0.0.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-16 13:05:56.000000 convcom-0.0.0/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)    13852 2024-04-16 13:06:00.541374 convcom-0.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3945 2024-04-16 13:05:56.000000 convcom-0.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1052 2024-04-16 13:05:56.000000 convcom-0.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 13:06:00.541374 convcom-0.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:06:00.537373 convcom-0.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:06:00.541374 convcom-0.0.0/src/convcom/
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-16 13:05:56.000000 convcom-0.0.0/src/convcom/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:06:00.541374 convcom-0.0.0/src/convcom/v1/
--rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-16 13:05:56.000000 convcom-0.0.0/src/convcom/v1/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-16 13:05:56.000000 convcom-0.0.0/src/convcom/v1/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (127)     7693 2024-04-16 13:05:56.000000 convcom-0.0.0/src/convcom/v1/parse.py
--rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-04-16 13:05:56.000000 convcom-0.0.0/src/convcom/v1/types.py
--rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-04-16 13:05:56.000000 convcom-0.0.0/src/convcom/v1/unparse.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:06:00.541374 convcom-0.0.0/src/convcom.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    13852 2024-04-16 13:06:00.000000 convcom-0.0.0/src/convcom.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-16 13:06:00.000000 convcom-0.0.0/src/convcom.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 13:06:00.000000 convcom-0.0.0/src/convcom.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-16 13:06:00.000000 convcom-0.0.0/src/convcom.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-16 13:06:00.000000 convcom-0.0.0/src/convcom.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:06:00.541374 convcom-0.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)    16510 2024-04-16 13:05:56.000000 convcom-0.0.0/tests/test_parse.py
--rw-r--r--   0 runner    (1001) docker     (127)     5735 2024-04-16 13:05:56.000000 convcom-0.0.0/tests/test_unparse.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:13:42.742503 convcom-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-16 13:13:37.000000 convcom-0.1.1/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:13:42.738503 convcom-0.1.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:13:42.738503 convcom-0.1.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     3173 2024-04-16 13:13:37.000000 convcom-0.1.1/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-16 13:13:37.000000 convcom-0.1.1/.github/workflows/run-pytest.yml
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-16 13:13:37.000000 convcom-0.1.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)    11357 2024-04-16 13:13:37.000000 convcom-0.1.1/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)    13852 2024-04-16 13:13:42.742503 convcom-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3945 2024-04-16 13:13:37.000000 convcom-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1125 2024-04-16 13:13:37.000000 convcom-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 13:13:42.742503 convcom-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:13:42.738503 convcom-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:13:42.738503 convcom-0.1.1/src/convcom/
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-16 13:13:37.000000 convcom-0.1.1/src/convcom/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:13:42.742503 convcom-0.1.1/src/convcom/v1/
+-rw-r--r--   0 runner    (1001) docker     (127)      580 2024-04-16 13:13:37.000000 convcom-0.1.1/src/convcom/v1/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1063 2024-04-16 13:13:37.000000 convcom-0.1.1/src/convcom/v1/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7693 2024-04-16 13:13:37.000000 convcom-0.1.1/src/convcom/v1/parse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1329 2024-04-16 13:13:37.000000 convcom-0.1.1/src/convcom/v1/types.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1927 2024-04-16 13:13:37.000000 convcom-0.1.1/src/convcom/v1/unparse.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:13:42.742503 convcom-0.1.1/src/convcom.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    13852 2024-04-16 13:13:42.000000 convcom-0.1.1/src/convcom.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      502 2024-04-16 13:13:42.000000 convcom-0.1.1/src/convcom.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 13:13:42.000000 convcom-0.1.1/src/convcom.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       68 2024-04-16 13:13:42.000000 convcom-0.1.1/src/convcom.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-16 13:13:42.000000 convcom-0.1.1/src/convcom.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 13:13:42.742503 convcom-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    16510 2024-04-16 13:13:37.000000 convcom-0.1.1/tests/test_parse.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5735 2024-04-16 13:13:37.000000 convcom-0.1.1/tests/test_unparse.py
```

### Comparing `convcom-0.0.0/.github/workflows/publish-to-pypi.yml` & `convcom-0.1.1/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `convcom-0.0.0/.github/workflows/run-pytest.yml` & `convcom-0.1.1/.github/workflows/run-pytest.yml`

 * *Files identical despite different names*

### Comparing `convcom-0.0.0/LICENSE.md` & `convcom-0.1.1/LICENSE.md`

 * *Files identical despite different names*

### Comparing `convcom-0.0.0/PKG-INFO` & `convcom-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: convcom
-Version: 0.0.0
+Version: 0.1.1
 Summary: A simple pure-Python module for parsing conventional commits.
 Author-email: Alex Weatherhead <22604743+Alex-Weatherhead@users.noreply.github.com>
 Maintainer-email: Alex Weatherhead <22604743+Alex-Weatherhead@users.noreply.github.com>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `convcom-0.0.0/README.md` & `convcom-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `convcom-0.0.0/pyproject.toml` & `convcom-0.1.1/pyproject.toml`

 * *Files 21% similar despite different names*

```diff
@@ -33,7 +33,10 @@
 Repository = "https://github.com/Alex-Weatherhead/convcom"
 Issues = "https://github.com/Alex-Weatherhead/convcom/issues"
 
 [tool.pytest.ini_options]
 addopts = [
     "--import-mode=importlib",
 ]
+
+[tool.setuptools_scm]
+# This table is required to enable setuptools_scm
```

### Comparing `convcom-0.0.0/src/convcom/__init__.py` & `convcom-0.1.1/src/convcom/__init__.py`

 * *Files identical despite different names*

### Comparing `convcom-0.0.0/src/convcom/v1/__init__.py` & `convcom-0.1.1/src/convcom/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `convcom-0.0.0/src/convcom/v1/exceptions.py` & `convcom-0.1.1/src/convcom/v1/exceptions.py`

 * *Files identical despite different names*

### Comparing `convcom-0.0.0/src/convcom/v1/parse.py` & `convcom-0.1.1/src/convcom/v1/parse.py`

 * *Files identical despite different names*

### Comparing `convcom-0.0.0/src/convcom/v1/types.py` & `convcom-0.1.1/src/convcom/v1/types.py`

 * *Files identical despite different names*

### Comparing `convcom-0.0.0/src/convcom/v1/unparse.py` & `convcom-0.1.1/src/convcom/v1/unparse.py`

 * *Files identical despite different names*

### Comparing `convcom-0.0.0/src/convcom.egg-info/PKG-INFO` & `convcom-0.1.1/src/convcom.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: convcom
-Version: 0.0.0
+Version: 0.1.1
 Summary: A simple pure-Python module for parsing conventional commits.
 Author-email: Alex Weatherhead <22604743+Alex-Weatherhead@users.noreply.github.com>
 Maintainer-email: Alex Weatherhead <22604743+Alex-Weatherhead@users.noreply.github.com>
 License: 
                                          Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `convcom-0.0.0/tests/test_parse.py` & `convcom-0.1.1/tests/test_parse.py`

 * *Files identical despite different names*

### Comparing `convcom-0.0.0/tests/test_unparse.py` & `convcom-0.1.1/tests/test_unparse.py`

 * *Files identical despite different names*

