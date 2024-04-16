# Comparing `tmp/betterjson-python-0.0.3.tar.gz` & `tmp/betterjson_python-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "betterjson_python-0.0.3.tar", last modified: Tue Apr 16 16:36:52 2024, max compression
+gzip compressed data, was "betterjson_python-0.0.4.tar", last modified: Tue Apr 16 16:42:48 2024, max compression
```

## Comparing `betterjson-python-0.0.3.tar` & `betterjson_python-0.0.4.tar`

### file list

```diff
@@ -1,13 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-16 16:36:52.579617 betterjson_python-0.0.3/
--rw-rw-rw-   0        0        0     2126 2024-04-16 16:36:52.578620 betterjson_python-0.0.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-16 16:36:52.577622 betterjson_python-0.0.3/betterjson_python.egg-info/
--rw-rw-rw-   0        0        0     2126 2024-04-16 16:36:52.000000 betterjson_python-0.0.3/betterjson_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      224 2024-04-16 16:36:52.000000 betterjson_python-0.0.3/betterjson_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-16 16:36:52.000000 betterjson_python-0.0.3/betterjson_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-16 16:36:52.000000 betterjson_python-0.0.3/betterjson_python.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-16 16:36:52.576625 betterjson_python-0.0.3/modules/
--rw-rw-rw-   0        0        0      923 2024-04-16 14:21:41.000000 betterjson_python-0.0.3/modules/files.py
--rw-rw-rw-   0        0        0     1732 2024-04-16 14:38:57.000000 betterjson_python-0.0.3/modules/format.py
--rw-rw-rw-   0        0        0     5002 2024-04-16 14:13:13.000000 betterjson_python-0.0.3/modules/parse.py
--rw-rw-rw-   0        0        0       42 2024-04-16 16:36:52.579617 betterjson_python-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0      570 2024-04-16 16:36:50.000000 betterjson_python-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-16 16:42:48.881219 betterjson_python-0.0.4/
+-rw-rw-rw-   0        0        0     2126 2024-04-16 16:42:48.880221 betterjson_python-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1859 2024-04-16 16:42:30.000000 betterjson_python-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2024-04-16 16:42:48.879224 betterjson_python-0.0.4/betterjson_python.egg-info/
+-rw-rw-rw-   0        0        0     2126 2024-04-16 16:42:48.000000 betterjson_python-0.0.4/betterjson_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      234 2024-04-16 16:42:48.000000 betterjson_python-0.0.4/betterjson_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-16 16:42:48.000000 betterjson_python-0.0.4/betterjson_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-16 16:42:48.000000 betterjson_python-0.0.4/betterjson_python.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-16 16:42:48.878226 betterjson_python-0.0.4/modules/
+-rw-rw-rw-   0        0        0      923 2024-04-16 14:21:41.000000 betterjson_python-0.0.4/modules/files.py
+-rw-rw-rw-   0        0        0     1732 2024-04-16 14:38:57.000000 betterjson_python-0.0.4/modules/format.py
+-rw-rw-rw-   0        0        0     5002 2024-04-16 14:13:13.000000 betterjson_python-0.0.4/modules/parse.py
+-rw-rw-rw-   0        0        0       42 2024-04-16 16:42:48.881219 betterjson_python-0.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      544 2024-04-16 16:42:02.000000 betterjson_python-0.0.4/setup.py
```

### Comparing `betterjson_python-0.0.3/PKG-INFO` & `betterjson_python-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: betterjson-python
-Version: 0.0.3
+Version: 0.0.4
 Summary: BetterJSON is an enhanced version of the JSON data format
 Author: ruxixa
 License: MIT
 Project-URL: Source, https://github.com/ruxixa/BetterJSON/
 Description-Content-Type: text/markdown
 
 # betterjson-python
```

### Comparing `betterjson_python-0.0.3/betterjson_python.egg-info/PKG-INFO` & `betterjson_python-0.0.4/betterjson_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: betterjson-python
-Version: 0.0.3
+Version: 0.0.4
 Summary: BetterJSON is an enhanced version of the JSON data format
 Author: ruxixa
 License: MIT
 Project-URL: Source, https://github.com/ruxixa/BetterJSON/
 Description-Content-Type: text/markdown
 
 # betterjson-python
```

### Comparing `betterjson_python-0.0.3/modules/files.py` & `betterjson_python-0.0.4/modules/files.py`

 * *Files identical despite different names*

### Comparing `betterjson_python-0.0.3/modules/format.py` & `betterjson_python-0.0.4/modules/format.py`

 * *Files identical despite different names*

### Comparing `betterjson_python-0.0.3/modules/parse.py` & `betterjson_python-0.0.4/modules/parse.py`

 * *Files identical despite different names*

### Comparing `betterjson_python-0.0.3/setup.py` & `betterjson_python-0.0.4/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 from setuptools import setup
 
-with open("DESCRIPTION.md", "r", encoding="utf-8") as fh:
-    long_description = fh.read()
+with open('README.md', 'r') as f:
+    long_description = f.read()
 
 print(long_description)
 
 setup (
     name = 'betterjson-python' ,
-    version ='0.0.3',
+    version ='0.0.4',
     author = 'ruxixa',
     description ='BetterJSON is an enhanced version of the JSON data format',
-    long_description = long_description,
-    long_description_content_type="text/markdown",
     packages = ['modules'],
     install_requires = [],
     license = 'MIT',
     project_urls = {'Source': 'https://github.com/ruxixa/BetterJSON/'},
+    long_description= long_description,
+    long_description_content_type='text/markdown',
 )
```

