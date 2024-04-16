# Comparing `tmp/MultiGATE-0.0.8.tar.gz` & `tmp/MultiGATE-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/MultiGATE-0.0.8.tar", last modified: Mon Apr  8 11:21:39 2024, max compression
+gzip compressed data, was "dist/MultiGATE-0.0.9.tar", last modified: Mon Apr  8 11:27:32 2024, max compression
```

## Comparing `MultiGATE-0.0.8.tar` & `MultiGATE-0.0.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwx---   0 s1155202250 (2030656) s1155202250 (2030656)        0 2024-04-08 11:21:39.000000 MultiGATE-0.0.8/
--rw-rw----   0 s1155202250 (2030656) s1155202250 (2030656)    11357 2024-04-07 14:52:50.000000 MultiGATE-0.0.8/LICENSE
-drwxrwx---   0 s1155202250 (2030656) s1155202250 (2030656)        0 2024-04-08 11:21:39.000000 MultiGATE-0.0.8/MultiGATE/
-drwxrwx---   0 s1155202250 (2030656) s1155202250 (2030656)        0 2024-04-08 11:21:39.000000 MultiGATE-0.0.8/MultiGATE/MultiGATE.egg-info/
--rw-rw----   0 s1155202250 (2030656) s1155202250 (2030656)      523 2024-04-08 11:21:39.000000 MultiGATE-0.0.8/MultiGATE/MultiGATE.egg-info/PKG-INFO
--rw-rw----   0 s1155202250 (2030656) s1155202250 (2030656)      240 2024-04-08 11:21:39.000000 MultiGATE-0.0.8/MultiGATE/MultiGATE.egg-info/SOURCES.txt
--rw-rw----   0 s1155202250 (2030656) s1155202250 (2030656)        1 2024-04-08 11:21:39.000000 MultiGATE-0.0.8/MultiGATE/MultiGATE.egg-info/dependency_links.txt
--rw-rw----   0 s1155202250 (2030656) s1155202250 (2030656)      305 2024-04-08 11:21:39.000000 MultiGATE-0.0.8/MultiGATE/MultiGATE.egg-info/requires.txt
--rw-rw----   0 s1155202250 (2030656) s1155202250 (2030656)        1 2024-04-08 11:21:39.000000 MultiGATE-0.0.8/MultiGATE/MultiGATE.egg-info/top_level.txt
--rw-rw----   0 s1155202250 (2030656) s1155202250 (2030656)      523 2024-04-08 11:21:39.000000 MultiGATE-0.0.8/PKG-INFO
--rw-rw----   0 s1155202250 (2030656) s1155202250 (2030656)       16 2024-04-07 14:52:50.000000 MultiGATE-0.0.8/README.md
--rw-rw----   0 s1155202250 (2030656) s1155202250 (2030656)       38 2024-04-08 11:21:39.000000 MultiGATE-0.0.8/setup.cfg
--rw-rw----   0 s1155202250 (2030656) s1155202250 (2030656)     1247 2024-04-08 11:21:36.000000 MultiGATE-0.0.8/setup.py
+drwxrwx---   0 s1155202250 (2030656) s1155202250 (2030656)        0 2024-04-08 11:27:32.000000 MultiGATE-0.0.9/
+-rw-rw----   0 s1155202250 (2030656) s1155202250 (2030656)    11357 2024-04-07 14:52:50.000000 MultiGATE-0.0.9/LICENSE
+drwxrwx---   0 s1155202250 (2030656) s1155202250 (2030656)        0 2024-04-08 11:27:32.000000 MultiGATE-0.0.9/MultiGATE/
+drwxrwx---   0 s1155202250 (2030656) s1155202250 (2030656)        0 2024-04-08 11:27:32.000000 MultiGATE-0.0.9/MultiGATE/MultiGATE.egg-info/
+-rw-rw----   0 s1155202250 (2030656) s1155202250 (2030656)      523 2024-04-08 11:27:32.000000 MultiGATE-0.0.9/MultiGATE/MultiGATE.egg-info/PKG-INFO
+-rw-rw----   0 s1155202250 (2030656) s1155202250 (2030656)      240 2024-04-08 11:27:32.000000 MultiGATE-0.0.9/MultiGATE/MultiGATE.egg-info/SOURCES.txt
+-rw-rw----   0 s1155202250 (2030656) s1155202250 (2030656)        1 2024-04-08 11:27:32.000000 MultiGATE-0.0.9/MultiGATE/MultiGATE.egg-info/dependency_links.txt
+-rw-rw----   0 s1155202250 (2030656) s1155202250 (2030656)      305 2024-04-08 11:27:32.000000 MultiGATE-0.0.9/MultiGATE/MultiGATE.egg-info/requires.txt
+-rw-rw----   0 s1155202250 (2030656) s1155202250 (2030656)        1 2024-04-08 11:27:32.000000 MultiGATE-0.0.9/MultiGATE/MultiGATE.egg-info/top_level.txt
+-rw-rw----   0 s1155202250 (2030656) s1155202250 (2030656)      523 2024-04-08 11:27:32.000000 MultiGATE-0.0.9/PKG-INFO
+-rw-rw----   0 s1155202250 (2030656) s1155202250 (2030656)       16 2024-04-07 14:52:50.000000 MultiGATE-0.0.9/README.md
+-rw-rw----   0 s1155202250 (2030656) s1155202250 (2030656)       38 2024-04-08 11:27:32.000000 MultiGATE-0.0.9/setup.cfg
+-rw-rw----   0 s1155202250 (2030656) s1155202250 (2030656)     1247 2024-04-08 11:27:29.000000 MultiGATE-0.0.9/setup.py
```

### Comparing `MultiGATE-0.0.8/LICENSE` & `MultiGATE-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `MultiGATE-0.0.8/MultiGATE/MultiGATE.egg-info/PKG-INFO` & `MultiGATE-0.0.9/MultiGATE/MultiGATE.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MultiGATE
-Version: 0.0.8
+Version: 0.0.9
 Summary: MultiGATE single cell
 Home-page: https://github.com/aqlkzf/MultiGATEtest1
 Author: Jinzhao LI & Jishuai MIAO
 Author-email: jishuaimiao@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `MultiGATE-0.0.8/PKG-INFO` & `MultiGATE-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MultiGATE
-Version: 0.0.8
+Version: 0.0.9
 Summary: MultiGATE single cell
 Home-page: https://github.com/aqlkzf/MultiGATEtest1
 Author: Jinzhao LI & Jishuai MIAO
 Author-email: jishuaimiao@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `MultiGATE-0.0.8/setup.py` & `MultiGATE-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="MultiGATE",
-    version="0.0.8",
+    version="0.0.9",
     description="MultiGATE single cell",
     package_dir={"": "MultiGATE"},
     packages=find_packages(where="MultiGATE"),
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/aqlkzf/MultiGATEtest1",
     author="Jinzhao LI & Jishuai MIAO",
```

