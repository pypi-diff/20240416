# Comparing `tmp/search-engine-tool-0.1.0.tar.gz` & `tmp/search-engine-tool-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "search-engine-tool-0.1.0.tar", last modified: Tue Apr 16 09:43:11 2024, max compression
+gzip compressed data, was "search-engine-tool-0.2.0.tar", last modified: Tue Apr 16 11:29:56 2024, max compression
```

## Comparing `search-engine-tool-0.1.0.tar` & `search-engine-tool-0.2.0.tar`

### file list

```diff
@@ -1,12 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-16 09:43:11.403976 search-engine-tool-0.1.0/
--rw-rw-rw-   0        0        0     1086 2024-04-14 18:41:59.000000 search-engine-tool-0.1.0/LICENSE
--rw-rw-rw-   0        0        0      970 2024-04-16 09:43:11.402975 search-engine-tool-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      370 2024-04-16 09:37:18.000000 search-engine-tool-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2024-04-16 09:43:11.401910 search-engine-tool-0.1.0/search_engine_tool.egg-info/
--rw-rw-rw-   0        0        0      970 2024-04-16 09:43:11.000000 search-engine-tool-0.1.0/search_engine_tool.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      235 2024-04-16 09:43:11.000000 search-engine-tool-0.1.0/search_engine_tool.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-16 09:43:11.000000 search-engine-tool-0.1.0/search_engine_tool.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2024-04-16 09:43:11.000000 search-engine-tool-0.1.0/search_engine_tool.egg-info/requires.txt
--rw-rw-rw-   0        0        0        1 2024-04-16 09:43:11.000000 search-engine-tool-0.1.0/search_engine_tool.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-16 09:43:11.403976 search-engine-tool-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      813 2024-04-16 09:31:51.000000 search-engine-tool-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-16 11:29:56.707884 search-engine-tool-0.2.0/
+-rw-rw-rw-   0        0        0     1086 2024-04-14 18:41:59.000000 search-engine-tool-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0     1675 2024-04-16 11:29:56.707884 search-engine-tool-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1075 2024-04-16 11:11:36.000000 search-engine-tool-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2024-04-16 11:29:56.700432 search-engine-tool-0.2.0/search_engine_tool/
+-rw-rw-rw-   0        0        0       79 2024-04-16 11:05:59.000000 search-engine-tool-0.2.0/search_engine_tool/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-16 11:29:56.706187 search-engine-tool-0.2.0/search_engine_tool/engine/
+-rw-rw-rw-   0        0        0       35 2024-04-16 11:07:02.000000 search-engine-tool-0.2.0/search_engine_tool/engine/__init__.py
+-rw-rw-rw-   0        0        0     1668 2024-04-16 08:36:09.000000 search-engine-tool-0.2.0/search_engine_tool/engine/bing.py
+-rw-rw-rw-   0        0        0      223 2024-04-16 09:36:57.000000 search-engine-tool-0.2.0/search_engine_tool/search_engine_tool.py
+drwxrwxrwx   0        0        0        0 2024-04-16 11:29:56.705388 search-engine-tool-0.2.0/search_engine_tool.egg-info/
+-rw-rw-rw-   0        0        0     1675 2024-04-16 11:29:56.000000 search-engine-tool-0.2.0/search_engine_tool.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      379 2024-04-16 11:29:56.000000 search-engine-tool-0.2.0/search_engine_tool.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-16 11:29:56.000000 search-engine-tool-0.2.0/search_engine_tool.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2024-04-16 11:29:56.000000 search-engine-tool-0.2.0/search_engine_tool.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2024-04-16 11:29:56.000000 search-engine-tool-0.2.0/search_engine_tool.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-16 11:29:56.707884 search-engine-tool-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0      813 2024-04-16 11:29:34.000000 search-engine-tool-0.2.0/setup.py
```

### Comparing `search-engine-tool-0.1.0/LICENSE` & `search-engine-tool-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `search-engine-tool-0.1.0/setup.py` & `search-engine-tool-0.2.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="search-engine-tool",
-    version="0.1.0",
+    version="0.2.0",
     packages=find_packages(),
     install_requires=[
         "selenium"
     ],
 
     author="bluefrog",
     author_email="bluefrog.wu@gmail.com",
```

