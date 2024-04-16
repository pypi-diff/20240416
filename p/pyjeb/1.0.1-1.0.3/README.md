# Comparing `tmp/pyjeb-1.0.1.tar.gz` & `tmp/pyjeb-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyjeb-1.0.1.tar", last modified: Tue Mar  5 17:55:52 2024, max compression
+gzip compressed data, was "pyjeb-1.0.3.tar", last modified: Tue Apr 16 18:03:59 2024, max compression
```

## Comparing `pyjeb-1.0.1.tar` & `pyjeb-1.0.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 17:55:52.406572 pyjeb-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)     5536 2024-03-05 17:55:52.406572 pyjeb-1.0.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 17:55:52.406572 pyjeb-1.0.1/pyjeb/
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-03-05 17:55:46.000000 pyjeb-1.0.1/pyjeb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2900 2024-03-05 17:55:46.000000 pyjeb-1.0.1/pyjeb/controls.py
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-03-05 17:55:46.000000 pyjeb-1.0.1/pyjeb/exception.py
--rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-03-05 17:55:46.000000 pyjeb-1.0.1/pyjeb/expression.py
--rw-r--r--   0 runner    (1001) docker     (127)     6665 2024-03-05 17:55:46.000000 pyjeb-1.0.1/pyjeb/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-03-05 17:55:46.000000 pyjeb-1.0.1/pyjeb/variables.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-05 17:55:52.406572 pyjeb-1.0.1/pyjeb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5536 2024-03-05 17:55:52.000000 pyjeb-1.0.1/pyjeb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      232 2024-03-05 17:55:52.000000 pyjeb-1.0.1/pyjeb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-05 17:55:52.000000 pyjeb-1.0.1/pyjeb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        6 2024-03-05 17:55:52.000000 pyjeb-1.0.1/pyjeb.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-05 17:55:52.406572 pyjeb-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-03-05 17:55:46.000000 pyjeb-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:03:59.539910 pyjeb-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (127)     5536 2024-04-16 18:03:59.539910 pyjeb-1.0.3/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:03:59.539910 pyjeb-1.0.3/pyjeb/
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-16 18:03:54.000000 pyjeb-1.0.3/pyjeb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3088 2024-04-16 18:03:54.000000 pyjeb-1.0.3/pyjeb/controls.py
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-16 18:03:54.000000 pyjeb-1.0.3/pyjeb/exception.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2068 2024-04-16 18:03:54.000000 pyjeb-1.0.3/pyjeb/expression.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6665 2024-04-16 18:03:54.000000 pyjeb-1.0.3/pyjeb/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2183 2024-04-16 18:03:54.000000 pyjeb-1.0.3/pyjeb/variables.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 18:03:59.539910 pyjeb-1.0.3/pyjeb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5536 2024-04-16 18:03:59.000000 pyjeb-1.0.3/pyjeb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      232 2024-04-16 18:03:59.000000 pyjeb-1.0.3/pyjeb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 18:03:59.000000 pyjeb-1.0.3/pyjeb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        6 2024-04-16 18:03:59.000000 pyjeb-1.0.3/pyjeb.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 18:03:59.539910 pyjeb-1.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1078 2024-04-16 18:03:54.000000 pyjeb-1.0.3/setup.py
```

### Comparing `pyjeb-1.0.1/PKG-INFO` & `pyjeb-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyjeb
-Version: 1.0.1
+Version: 1.0.3
 Summary: A powerfull lightweight library to check and variabilize your configuration files
 Home-page: https://github.com/CSharplie/pyjeb/
 Download-URL: https://pypi.org/project/pyjeb/
 License: Apache License 2.0
 Project-URL: Bug Tracker, https://github.com/CSharplie/pyjeb/issues
 Project-URL: CI, https://github.com/CSharplie/pyjeb/actions
 Project-URL: Documentation, https://github.com/CSharplie/pyjeb
```

### Comparing `pyjeb-1.0.1/pyjeb/controls.py` & `pyjeb-1.0.3/pyjeb/controls.py`

 * *Files 4% similar despite different names*

```diff
@@ -49,15 +49,24 @@
     """Check if property is empty"""
 
     return not((value is None or str(value) == "")and not default_defined)
 
 def check_validset(value, validset):
     """Check if property is include in validset"""
 
-    return value in validset
+    if value in validset:
+        return True
+
+    for regex in validset:
+        try:
+            if re.match(regex, value):
+                return True
+        except re.error:
+            continue
+    return False
 
 def check_regex(value, expression):
     """Check if property match with regex"""
 
     return re.match(expression, value) is not None
 
 def check_type(value, value_type):
```

### Comparing `pyjeb-1.0.1/pyjeb/exception.py` & `pyjeb-1.0.3/pyjeb/exception.py`

 * *Files identical despite different names*

### Comparing `pyjeb-1.0.1/pyjeb/expression.py` & `pyjeb-1.0.3/pyjeb/expression.py`

 * *Files identical despite different names*

### Comparing `pyjeb-1.0.1/pyjeb/main.py` & `pyjeb-1.0.3/pyjeb/main.py`

 * *Files identical despite different names*

### Comparing `pyjeb-1.0.1/pyjeb/variables.py` & `pyjeb-1.0.3/pyjeb/variables.py`

 * *Files identical despite different names*

### Comparing `pyjeb-1.0.1/pyjeb.egg-info/PKG-INFO` & `pyjeb-1.0.3/pyjeb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyjeb
-Version: 1.0.1
+Version: 1.0.3
 Summary: A powerfull lightweight library to check and variabilize your configuration files
 Home-page: https://github.com/CSharplie/pyjeb/
 Download-URL: https://pypi.org/project/pyjeb/
 License: Apache License 2.0
 Project-URL: Bug Tracker, https://github.com/CSharplie/pyjeb/issues
 Project-URL: CI, https://github.com/CSharplie/pyjeb/actions
 Project-URL: Documentation, https://github.com/CSharplie/pyjeb
```

### Comparing `pyjeb-1.0.1/setup.py` & `pyjeb-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
     long_description = "".join(f.readlines())
 
 # replace relative link by absolute github link
 long_description = long_description.replace("(/", "(https://github.com/CSharplie/pyjeb/blob/main/")
 
 setup (
     name = "pyjeb",
-    version = "1.0.1",
+    version = "1.0.3",
     description="A powerfull lightweight library to check and variabilize your configuration files",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/CSharplie/pyjeb/",
     project_urls={
         "Bug Tracker": "https://github.com/CSharplie/pyjeb/issues",
         "CI": "https://github.com/CSharplie/pyjeb/actions",
```

