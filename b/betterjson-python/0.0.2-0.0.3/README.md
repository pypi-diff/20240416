# Comparing `tmp/betterjson-python-0.0.2.tar.gz` & `tmp/betterjson-python-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BetterJSOn-0.0.2.tar", last modified: Tue Apr 16 16:23:49 2024, max compression
+gzip compressed data, was "betterjson_python-0.0.3.tar", last modified: Tue Apr 16 16:36:52 2024, max compression
```

## Comparing `betterjson-python-0.0.2.tar` & `betterjson-python-0.0.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-16 16:23:49.120845 BetterJSOn-0.0.2/
-drwxrwxrwx   0        0        0        0 2024-04-16 16:23:49.118851 BetterJSOn-0.0.2/BetterJSOn.egg-info/
--rw-rw-rw-   0        0        0     2119 2024-04-16 16:23:49.000000 BetterJSOn-0.0.2/BetterJSOn.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      196 2024-04-16 16:23:49.000000 BetterJSOn-0.0.2/BetterJSOn.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-16 16:23:49.000000 BetterJSOn-0.0.2/BetterJSOn.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-16 16:23:49.000000 BetterJSOn-0.0.2/BetterJSOn.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2119 2024-04-16 16:23:49.119848 BetterJSOn-0.0.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-16 16:23:49.117854 BetterJSOn-0.0.2/modules/
--rw-rw-rw-   0        0        0      923 2024-04-16 14:21:41.000000 BetterJSOn-0.0.2/modules/files.py
--rw-rw-rw-   0        0        0     1732 2024-04-16 14:38:57.000000 BetterJSOn-0.0.2/modules/format.py
--rw-rw-rw-   0        0        0     5002 2024-04-16 14:13:13.000000 BetterJSOn-0.0.2/modules/parse.py
--rw-rw-rw-   0        0        0       42 2024-04-16 16:23:49.120845 BetterJSOn-0.0.2/setup.cfg
--rw-rw-rw-   0        0        0      534 2024-04-16 16:23:40.000000 BetterJSOn-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-16 16:36:52.579617 betterjson_python-0.0.3/
+-rw-rw-rw-   0        0        0     2126 2024-04-16 16:36:52.578620 betterjson_python-0.0.3/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-16 16:36:52.577622 betterjson_python-0.0.3/betterjson_python.egg-info/
+-rw-rw-rw-   0        0        0     2126 2024-04-16 16:36:52.000000 betterjson_python-0.0.3/betterjson_python.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      224 2024-04-16 16:36:52.000000 betterjson_python-0.0.3/betterjson_python.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-16 16:36:52.000000 betterjson_python-0.0.3/betterjson_python.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-16 16:36:52.000000 betterjson_python-0.0.3/betterjson_python.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-16 16:36:52.576625 betterjson_python-0.0.3/modules/
+-rw-rw-rw-   0        0        0      923 2024-04-16 14:21:41.000000 betterjson_python-0.0.3/modules/files.py
+-rw-rw-rw-   0        0        0     1732 2024-04-16 14:38:57.000000 betterjson_python-0.0.3/modules/format.py
+-rw-rw-rw-   0        0        0     5002 2024-04-16 14:13:13.000000 betterjson_python-0.0.3/modules/parse.py
+-rw-rw-rw-   0        0        0       42 2024-04-16 16:36:52.579617 betterjson_python-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      570 2024-04-16 16:36:50.000000 betterjson_python-0.0.3/setup.py
```

### Comparing `BetterJSOn-0.0.2/BetterJSOn.egg-info/PKG-INFO` & `betterjson_python-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: BetterJSOn
-Version: 0.0.2
+Name: betterjson-python
+Version: 0.0.3
 Summary: BetterJSON is an enhanced version of the JSON data format
 Author: ruxixa
 License: MIT
 Project-URL: Source, https://github.com/ruxixa/BetterJSON/
 Description-Content-Type: text/markdown
 
 # betterjson-python
```

### Comparing `BetterJSOn-0.0.2/PKG-INFO` & `betterjson_python-0.0.3/betterjson_python.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: BetterJSOn
-Version: 0.0.2
+Name: betterjson-python
+Version: 0.0.3
 Summary: BetterJSON is an enhanced version of the JSON data format
 Author: ruxixa
 License: MIT
 Project-URL: Source, https://github.com/ruxixa/BetterJSON/
 Description-Content-Type: text/markdown
 
 # betterjson-python
```

### Comparing `BetterJSOn-0.0.2/modules/files.py` & `betterjson_python-0.0.3/modules/files.py`

 * *Files identical despite different names*

### Comparing `BetterJSOn-0.0.2/modules/format.py` & `betterjson_python-0.0.3/modules/format.py`

 * *Files identical despite different names*

### Comparing `BetterJSOn-0.0.2/modules/parse.py` & `betterjson_python-0.0.3/modules/parse.py`

 * *Files identical despite different names*

