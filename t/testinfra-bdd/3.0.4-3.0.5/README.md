# Comparing `tmp/testinfra-bdd-3.0.4.tar.gz` & `tmp/testinfra_bdd-3.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testinfra-bdd-3.0.4.tar", last modified: Sun Mar 10 10:43:58 2024, max compression
+gzip compressed data, was "testinfra_bdd-3.0.5.tar", last modified: Tue Apr 16 18:56:37 2024, max compression
```

## Comparing `testinfra-bdd-3.0.4.tar` & `testinfra_bdd-3.0.5.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 10:43:58.080907 testinfra-bdd-3.0.4/
--rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-03-10 10:43:40.000000 testinfra-bdd-3.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)    15179 2024-03-10 10:43:58.080907 testinfra-bdd-3.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    14497 2024-03-10 10:43:40.000000 testinfra-bdd-3.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-03-10 10:43:40.000000 testinfra-bdd-3.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      431 2024-03-10 10:43:58.080907 testinfra-bdd-3.0.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-03-10 10:43:40.000000 testinfra-bdd-3.0.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 10:43:58.080907 testinfra-bdd-3.0.4/testinfra_bdd/
--rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-03-10 10:43:40.000000 testinfra-bdd-3.0.4/testinfra_bdd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3150 2024-03-10 10:43:40.000000 testinfra-bdd-3.0.4/testinfra_bdd/address.py
--rw-r--r--   0 runner    (1001) docker     (127)     6447 2024-03-10 10:43:40.000000 testinfra-bdd-3.0.4/testinfra_bdd/command.py
--rw-r--r--   0 runner    (1001) docker     (127)      695 2024-03-10 10:43:40.000000 testinfra-bdd-3.0.4/testinfra_bdd/exception_message.py
--rw-r--r--   0 runner    (1001) docker     (127)     4879 2024-03-10 10:43:40.000000 testinfra-bdd-3.0.4/testinfra_bdd/file.py
--rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-03-10 10:43:40.000000 testinfra-bdd-3.0.4/testinfra_bdd/file_helpers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5095 2024-03-10 10:43:40.000000 testinfra-bdd-3.0.4/testinfra_bdd/fixture.py
--rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-03-10 10:43:40.000000 testinfra-bdd-3.0.4/testinfra_bdd/given.py
--rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-03-10 10:43:40.000000 testinfra-bdd-3.0.4/testinfra_bdd/group.py
--rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-03-10 10:43:40.000000 testinfra-bdd-3.0.4/testinfra_bdd/package.py
--rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-03-10 10:43:40.000000 testinfra-bdd-3.0.4/testinfra_bdd/parsers.py
--rw-r--r--   0 runner    (1001) docker     (127)     5026 2024-03-10 10:43:40.000000 testinfra-bdd-3.0.4/testinfra_bdd/pip.py
--rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-03-10 10:43:40.000000 testinfra-bdd-3.0.4/testinfra_bdd/process.py
--rw-r--r--   0 runner    (1001) docker     (127)     2657 2024-03-10 10:43:40.000000 testinfra-bdd-3.0.4/testinfra_bdd/service.py
--rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-03-10 10:43:40.000000 testinfra-bdd-3.0.4/testinfra_bdd/socket.py
--rw-r--r--   0 runner    (1001) docker     (127)     3281 2024-03-10 10:43:40.000000 testinfra-bdd-3.0.4/testinfra_bdd/user.py
--rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-03-10 10:43:40.000000 testinfra-bdd-3.0.4/testinfra_bdd/when.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 10:43:58.080907 testinfra-bdd-3.0.4/testinfra_bdd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    15179 2024-03-10 10:43:58.000000 testinfra-bdd-3.0.4/testinfra_bdd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-03-10 10:43:58.000000 testinfra-bdd-3.0.4/testinfra_bdd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-10 10:43:58.000000 testinfra-bdd-3.0.4/testinfra_bdd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-03-10 10:43:58.000000 testinfra-bdd-3.0.4/testinfra_bdd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-10 10:43:58.000000 testinfra-bdd-3.0.4/testinfra_bdd.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-10 10:43:58.080907 testinfra-bdd-3.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     3723 2024-03-10 10:43:40.000000 testinfra-bdd-3.0.4/tests/test_exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:56:37.851718 testinfra_bdd-3.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1530 2024-04-16 18:56:20.000000 testinfra_bdd-3.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)    15179 2024-04-16 18:56:37.851718 testinfra_bdd-3.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    14497 2024-04-16 18:56:20.000000 testinfra_bdd-3.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-16 18:56:20.000000 testinfra_bdd-3.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      442 2024-04-16 18:56:37.851718 testinfra_bdd-3.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1389 2024-04-16 18:56:20.000000 testinfra_bdd-3.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:56:37.847718 testinfra_bdd-3.0.5/testinfra_bdd/
+-rw-r--r--   0 runner    (1001) docker     (127)     1710 2024-04-16 18:56:20.000000 testinfra_bdd-3.0.5/testinfra_bdd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3150 2024-04-16 18:56:20.000000 testinfra_bdd-3.0.5/testinfra_bdd/address.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6447 2024-04-16 18:56:20.000000 testinfra_bdd-3.0.5/testinfra_bdd/command.py
+-rw-r--r--   0 runner    (1001) docker     (127)      695 2024-04-16 18:56:20.000000 testinfra_bdd-3.0.5/testinfra_bdd/exception_message.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4879 2024-04-16 18:56:20.000000 testinfra_bdd-3.0.5/testinfra_bdd/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2520 2024-04-16 18:56:20.000000 testinfra_bdd-3.0.5/testinfra_bdd/file_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5095 2024-04-16 18:56:20.000000 testinfra_bdd-3.0.5/testinfra_bdd/fixture.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1709 2024-04-16 18:56:20.000000 testinfra_bdd-3.0.5/testinfra_bdd/given.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2940 2024-04-16 18:56:20.000000 testinfra_bdd-3.0.5/testinfra_bdd/group.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1713 2024-04-16 18:56:20.000000 testinfra_bdd-3.0.5/testinfra_bdd/package.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1606 2024-04-16 18:56:20.000000 testinfra_bdd-3.0.5/testinfra_bdd/parsers.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5026 2024-04-16 18:56:20.000000 testinfra_bdd-3.0.5/testinfra_bdd/pip.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1855 2024-04-16 18:56:20.000000 testinfra_bdd-3.0.5/testinfra_bdd/process.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2657 2024-04-16 18:56:20.000000 testinfra_bdd-3.0.5/testinfra_bdd/service.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1373 2024-04-16 18:56:20.000000 testinfra_bdd-3.0.5/testinfra_bdd/socket.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3281 2024-04-16 18:56:20.000000 testinfra_bdd-3.0.5/testinfra_bdd/user.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1402 2024-04-16 18:56:20.000000 testinfra_bdd-3.0.5/testinfra_bdd/when.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:56:37.851718 testinfra_bdd-3.0.5/testinfra_bdd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    15179 2024-04-16 18:56:37.000000 testinfra_bdd-3.0.5/testinfra_bdd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-16 18:56:37.000000 testinfra_bdd-3.0.5/testinfra_bdd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 18:56:37.000000 testinfra_bdd-3.0.5/testinfra_bdd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-16 18:56:37.000000 testinfra_bdd-3.0.5/testinfra_bdd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-16 18:56:37.000000 testinfra_bdd-3.0.5/testinfra_bdd.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:56:37.851718 testinfra_bdd-3.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     3723 2024-04-16 18:56:20.000000 testinfra_bdd-3.0.5/tests/test_exceptions.py
```

### Comparing `testinfra-bdd-3.0.4/LICENSE` & `testinfra_bdd-3.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `testinfra-bdd-3.0.4/PKG-INFO` & `testinfra_bdd-3.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testinfra-bdd
-Version: 3.0.4
+Version: 3.0.5
 Summary: An interface between pytest-bdd and pytest-testinfra.
 Home-page: https://github.com/cbdq-io/testinfra-bdd
 Author: Cloud Based DQ Ltd.
 Author-email: info@cbdq.io
 Project-URL: Bug Tracker, https://github.com/cbdq-io/testinfra-bdd/issues
 Keywords: testinfra,bdd
 Classifier: Programming Language :: Python :: 3
```

### Comparing `testinfra-bdd-3.0.4/README.md` & `testinfra_bdd-3.0.5/README.md`

 * *Files identical despite different names*

### Comparing `testinfra-bdd-3.0.4/setup.py` & `testinfra_bdd-3.0.5/setup.py`

 * *Files identical despite different names*

### Comparing `testinfra-bdd-3.0.4/testinfra_bdd/__init__.py` & `testinfra_bdd-3.0.5/testinfra_bdd/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 ]
 
 """The version of the module.
 
 This is used by setuptools and by gitchangelog to identify the name of the name
 of the release.
 """
-__version__ = '3.0.4'
+__version__ = '3.0.5'
 
 
 def get_host_fixture(hostspec, timeout=0):
     """
     Return a host that is confirmed as ready.
 
     hostspec : str
```

### Comparing `testinfra-bdd-3.0.4/testinfra_bdd/address.py` & `testinfra_bdd-3.0.5/testinfra_bdd/address.py`

 * *Files identical despite different names*

### Comparing `testinfra-bdd-3.0.4/testinfra_bdd/command.py` & `testinfra_bdd-3.0.5/testinfra_bdd/command.py`

 * *Files identical despite different names*

### Comparing `testinfra-bdd-3.0.4/testinfra_bdd/exception_message.py` & `testinfra_bdd-3.0.5/testinfra_bdd/exception_message.py`

 * *Files identical despite different names*

### Comparing `testinfra-bdd-3.0.4/testinfra_bdd/file.py` & `testinfra_bdd-3.0.5/testinfra_bdd/file.py`

 * *Files identical despite different names*

### Comparing `testinfra-bdd-3.0.4/testinfra_bdd/file_helpers.py` & `testinfra_bdd-3.0.5/testinfra_bdd/file_helpers.py`

 * *Files identical despite different names*

### Comparing `testinfra-bdd-3.0.4/testinfra_bdd/fixture.py` & `testinfra_bdd-3.0.5/testinfra_bdd/fixture.py`

 * *Files identical despite different names*

### Comparing `testinfra-bdd-3.0.4/testinfra_bdd/given.py` & `testinfra_bdd-3.0.5/testinfra_bdd/given.py`

 * *Files identical despite different names*

### Comparing `testinfra-bdd-3.0.4/testinfra_bdd/group.py` & `testinfra_bdd-3.0.5/testinfra_bdd/group.py`

 * *Files identical despite different names*

### Comparing `testinfra-bdd-3.0.4/testinfra_bdd/package.py` & `testinfra_bdd-3.0.5/testinfra_bdd/package.py`

 * *Files identical despite different names*

### Comparing `testinfra-bdd-3.0.4/testinfra_bdd/parsers.py` & `testinfra_bdd-3.0.5/testinfra_bdd/parsers.py`

 * *Files identical despite different names*

### Comparing `testinfra-bdd-3.0.4/testinfra_bdd/pip.py` & `testinfra_bdd-3.0.5/testinfra_bdd/pip.py`

 * *Files identical despite different names*

### Comparing `testinfra-bdd-3.0.4/testinfra_bdd/process.py` & `testinfra_bdd-3.0.5/testinfra_bdd/process.py`

 * *Files identical despite different names*

### Comparing `testinfra-bdd-3.0.4/testinfra_bdd/service.py` & `testinfra_bdd-3.0.5/testinfra_bdd/service.py`

 * *Files identical despite different names*

### Comparing `testinfra-bdd-3.0.4/testinfra_bdd/socket.py` & `testinfra_bdd-3.0.5/testinfra_bdd/socket.py`

 * *Files identical despite different names*

### Comparing `testinfra-bdd-3.0.4/testinfra_bdd/user.py` & `testinfra_bdd-3.0.5/testinfra_bdd/user.py`

 * *Files identical despite different names*

### Comparing `testinfra-bdd-3.0.4/testinfra_bdd/when.py` & `testinfra_bdd-3.0.5/testinfra_bdd/when.py`

 * *Files identical despite different names*

### Comparing `testinfra-bdd-3.0.4/testinfra_bdd.egg-info/PKG-INFO` & `testinfra_bdd-3.0.5/testinfra_bdd.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testinfra-bdd
-Version: 3.0.4
+Version: 3.0.5
 Summary: An interface between pytest-bdd and pytest-testinfra.
 Home-page: https://github.com/cbdq-io/testinfra-bdd
 Author: Cloud Based DQ Ltd.
 Author-email: info@cbdq.io
 Project-URL: Bug Tracker, https://github.com/cbdq-io/testinfra-bdd/issues
 Keywords: testinfra,bdd
 Classifier: Programming Language :: Python :: 3
```

### Comparing `testinfra-bdd-3.0.4/testinfra_bdd.egg-info/SOURCES.txt` & `testinfra_bdd-3.0.5/testinfra_bdd.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `testinfra-bdd-3.0.4/tests/test_exceptions.py` & `testinfra_bdd-3.0.5/tests/test_exceptions.py`

 * *Files identical despite different names*

