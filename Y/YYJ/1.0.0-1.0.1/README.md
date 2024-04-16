# Comparing `tmp/YYJ-1.0.0.tar.gz` & `tmp/YYJ-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\YYJ-1.0.0.tar", last modified: Tue Apr 16 11:14:23 2024, max compression
+gzip compressed data, was "dist\YYJ-1.0.1.tar", last modified: Tue Apr 16 11:45:56 2024, max compression
```

## Comparing `YYJ-1.0.0.tar` & `YYJ-1.0.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-16 11:14:23.451361 YYJ-1.0.0/
--rw-rw-rw-   0        0        0     1010 2024-04-16 11:14:23.451361 YYJ-1.0.0/PKG-INFO
--rw-rw-rw-   0        0        0       78 2024-04-16 10:40:13.000000 YYJ-1.0.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-16 11:14:23.447154 YYJ-1.0.0/YYJ/
--rw-rw-rw-   0        0        0     1006 2024-04-16 10:21:45.000000 YYJ-1.0.0/YYJ/__core.py
--rw-rw-rw-   0        0        0       24 2024-04-16 10:26:15.000000 YYJ-1.0.0/YYJ/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-16 11:14:23.451361 YYJ-1.0.0/YYJ.egg-info/
--rw-rw-rw-   0        0        0     1010 2024-04-16 11:14:23.000000 YYJ-1.0.0/YYJ.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      156 2024-04-16 11:14:23.000000 YYJ-1.0.0/YYJ.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-16 11:14:23.000000 YYJ-1.0.0/YYJ.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2024-04-16 11:14:23.000000 YYJ-1.0.0/YYJ.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-16 11:14:23.451361 YYJ-1.0.0/setup.cfg
--rw-rw-rw-   0        0        0     1244 2024-04-16 11:14:18.000000 YYJ-1.0.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-16 11:45:56.274067 YYJ-1.0.1/
+-rw-rw-rw-   0        0        0     1010 2024-04-16 11:45:56.274067 YYJ-1.0.1/PKG-INFO
+-rw-rw-rw-   0        0        0       78 2024-04-16 10:40:13.000000 YYJ-1.0.1/README.md
+drwxrwxrwx   0        0        0        0 2024-04-16 11:45:56.266932 YYJ-1.0.1/YYJ/
+-rw-rw-rw-   0        0        0     1006 2024-04-16 10:21:45.000000 YYJ-1.0.1/YYJ/__core.py
+-rw-rw-rw-   0        0        0       25 2024-04-16 11:33:26.000000 YYJ-1.0.1/YYJ/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-16 11:45:56.272070 YYJ-1.0.1/YYJ.egg-info/
+-rw-rw-rw-   0        0        0     1010 2024-04-16 11:45:56.000000 YYJ-1.0.1/YYJ.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      156 2024-04-16 11:45:56.000000 YYJ-1.0.1/YYJ.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-16 11:45:56.000000 YYJ-1.0.1/YYJ.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2024-04-16 11:45:56.000000 YYJ-1.0.1/YYJ.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-16 11:45:56.274067 YYJ-1.0.1/setup.cfg
+-rw-rw-rw-   0        0        0     1244 2024-04-16 11:45:47.000000 YYJ-1.0.1/setup.py
```

### Comparing `YYJ-1.0.0/PKG-INFO` & `YYJ-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: YYJ
-Version: 1.0.0
+Version: 1.0.1
 Summary: 瓦达西瓦YYJ得思，俺是一个来自D7 415的梗小鬼，俺打球像坤坤，俺打王者只会压力己方MVP，天天被狙击仔克制
 Home-page: https://pornhub.com
 Author: marf
 Author-email: chenmarf460@gmail.com
 License: Apache 2.0
 Description: 到这就说明宿舍仔你成功一部分了，还是那句话：欢迎狙击
 Keywords: yyj,pornhub
```

### Comparing `YYJ-1.0.0/YYJ/__core.py` & `YYJ-1.0.1/YYJ/__core.py`

 * *Files identical despite different names*

### Comparing `YYJ-1.0.0/YYJ.egg-info/PKG-INFO` & `YYJ-1.0.1/YYJ.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: YYJ
-Version: 1.0.0
+Version: 1.0.1
 Summary: 瓦达西瓦YYJ得思，俺是一个来自D7 415的梗小鬼，俺打球像坤坤，俺打王者只会压力己方MVP，天天被狙击仔克制
 Home-page: https://pornhub.com
 Author: marf
 Author-email: chenmarf460@gmail.com
 License: Apache 2.0
 Description: 到这就说明宿舍仔你成功一部分了，还是那句话：欢迎狙击
 Keywords: yyj,pornhub
```

### Comparing `YYJ-1.0.0/setup.py` & `YYJ-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import pathlib
 
 here = pathlib.Path(__file__).parent.resolve()
 long_description = (here / "README.md").read_text(encoding="utf-8")
 
 setuptools.setup(
     name="YYJ",
-    version="1.0.0",
+    version="1.0.1",
     author="marf",
     author_email="chenmarf460@gmail.com",
     description="瓦达西瓦YYJ得思，俺是一个来自D7 415的梗小鬼，俺打球像坤坤，俺打王者只会压力己方MVP，天天被狙击仔克制",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://pornhub.com",
     packages=setuptools.find_packages(),
```

