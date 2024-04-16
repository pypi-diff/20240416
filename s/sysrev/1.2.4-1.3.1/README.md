# Comparing `tmp/sysrev-1.2.4.tar.gz` & `tmp/sysrev-1.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sysrev-1.2.4.tar", last modified: Mon Apr 15 13:49:10 2024, max compression
+gzip compressed data, was "sysrev-1.3.1.tar", last modified: Mon Apr 15 20:21:23 2024, max compression
```

## Comparing `sysrev-1.2.4.tar` & `sysrev-1.3.1.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:49:10.099267 sysrev-1.2.4/
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-15 13:49:10.099267 sysrev-1.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-15 13:49:04.000000 sysrev-1.2.4/README.md
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 13:49:10.099267 sysrev-1.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-15 13:49:04.000000 sysrev-1.2.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:49:10.095267 sysrev-1.2.4/sysrev/
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-15 13:49:04.000000 sysrev-1.2.4/sysrev/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     4863 2024-04-15 13:49:04.000000 sysrev-1.2.4/sysrev/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:49:10.099267 sysrev-1.2.4/sysrev.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-15 13:49:10.000000 sysrev-1.2.4/sysrev.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-15 13:49:10.000000 sysrev-1.2.4/sysrev.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 13:49:10.000000 sysrev-1.2.4/sysrev.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 13:49:09.000000 sysrev-1.2.4/sysrev.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-15 13:49:10.000000 sysrev-1.2.4/sysrev.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-15 13:49:10.000000 sysrev-1.2.4/sysrev.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 13:49:10.095267 sysrev-1.2.4/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-04-15 13:49:04.000000 sysrev-1.2.4/tests/test_client.py
--rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-15 13:49:04.000000 sysrev-1.2.4/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:21:23.443531 sysrev-1.3.1/
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-15 20:21:23.443531 sysrev-1.3.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      428 2024-04-15 20:21:17.000000 sysrev-1.3.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 20:21:23.443531 sysrev-1.3.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-15 20:21:17.000000 sysrev-1.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:21:23.443531 sysrev-1.3.1/sysrev/
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-15 20:21:17.000000 sysrev-1.3.1/sysrev/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8862 2024-04-15 20:21:17.000000 sysrev-1.3.1/sysrev/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:21:23.443531 sysrev-1.3.1/sysrev.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      726 2024-04-15 20:21:23.000000 sysrev-1.3.1/sysrev.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-15 20:21:23.000000 sysrev-1.3.1/sysrev.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 20:21:23.000000 sysrev-1.3.1/sysrev.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 20:21:23.000000 sysrev-1.3.1/sysrev.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-15 20:21:23.000000 sysrev-1.3.1/sysrev.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        7 2024-04-15 20:21:23.000000 sysrev-1.3.1/sysrev.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 20:21:23.443531 sysrev-1.3.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1933 2024-04-15 20:21:17.000000 sysrev-1.3.1/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1099 2024-04-15 20:21:17.000000 sysrev-1.3.1/tests/test_utils.py
```

### Comparing `sysrev-1.2.4/PKG-INFO` & `sysrev-1.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sysrev
-Version: 1.2.4
+Version: 1.3.1
 Summary: get sysrev project data and use the sysrev api
 Home-page: https://github.com/sysrev/PySysrev
 Author: Thomas Luechtefeld
 Author-email: tom@insilica.co
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: requests
```

### Comparing `sysrev-1.2.4/setup.py` & `sysrev-1.3.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Assuming your README file is in Markdown
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='sysrev',
-    version='1.2.4',
+    version='1.3.1',
     description='get sysrev project data and use the sysrev api',
     long_description=long_description,
     long_description_content_type='text/markdown',  # Specify the content type here
     url='https://github.com/sysrev/PySysrev',
     author='Thomas Luechtefeld',
     author_email='tom@insilica.co',
     packages=['sysrev'],
```

### Comparing `sysrev-1.2.4/sysrev.egg-info/PKG-INFO` & `sysrev-1.3.1/sysrev.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sysrev
-Version: 1.2.4
+Version: 1.3.1
 Summary: get sysrev project data and use the sysrev api
 Home-page: https://github.com/sysrev/PySysrev
 Author: Thomas Luechtefeld
 Author-email: tom@insilica.co
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Requires-Dist: requests
```

### Comparing `sysrev-1.2.4/tests/test_client.py` & `sysrev-1.3.1/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `sysrev-1.2.4/tests/test_utils.py` & `sysrev-1.3.1/tests/test_utils.py`

 * *Files identical despite different names*

