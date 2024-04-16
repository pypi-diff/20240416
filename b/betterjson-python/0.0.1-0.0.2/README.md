# Comparing `tmp/betterjson-python-0.0.1.tar.gz` & `tmp/betterjson-python-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "betterjson-python-0.0.1.tar", last modified: Tue Apr 16 16:01:42 2024, max compression
+gzip compressed data, was "BetterJSOn-0.0.2.tar", last modified: Tue Apr 16 16:23:49 2024, max compression
```

## Comparing `betterjson-python-0.0.1.tar` & `betterjson-python-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,13 @@
-drwxrwxrwx   0        0        0        0 2024-04-16 16:01:42.000573 betterjson-python-0.0.1/
--rw-rw-rw-   0        0        0      222 2024-04-16 16:01:41.999577 betterjson-python-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      605 2024-04-16 15:04:17.000000 betterjson-python-0.0.1/__version__.py
--rw-rw-rw-   0        0        0     3095 2024-04-16 15:47:51.000000 betterjson-python-0.0.1/betterjson.py
-drwxrwxrwx   0        0        0        0 2024-04-16 16:01:41.998579 betterjson-python-0.0.1/betterjson_python.egg-info/
--rw-rw-rw-   0        0        0      222 2024-04-16 16:01:41.000000 betterjson-python-0.0.1/betterjson_python.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      253 2024-04-16 16:01:41.000000 betterjson-python-0.0.1/betterjson_python.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-16 16:01:41.000000 betterjson-python-0.0.1/betterjson_python.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-16 16:01:41.000000 betterjson-python-0.0.1/betterjson_python.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2024-04-16 16:01:41.997582 betterjson-python-0.0.1/modules/
--rw-rw-rw-   0        0        0      923 2024-04-16 14:21:41.000000 betterjson-python-0.0.1/modules/files.py
--rw-rw-rw-   0        0        0     1732 2024-04-16 14:38:57.000000 betterjson-python-0.0.1/modules/format.py
--rw-rw-rw-   0        0        0     5002 2024-04-16 14:13:13.000000 betterjson-python-0.0.1/modules/parse.py
--rw-rw-rw-   0        0        0       42 2024-04-16 16:01:42.000573 betterjson-python-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      405 2024-04-16 16:01:31.000000 betterjson-python-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-16 16:23:49.120845 BetterJSOn-0.0.2/
+drwxrwxrwx   0        0        0        0 2024-04-16 16:23:49.118851 BetterJSOn-0.0.2/BetterJSOn.egg-info/
+-rw-rw-rw-   0        0        0     2119 2024-04-16 16:23:49.000000 BetterJSOn-0.0.2/BetterJSOn.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      196 2024-04-16 16:23:49.000000 BetterJSOn-0.0.2/BetterJSOn.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-16 16:23:49.000000 BetterJSOn-0.0.2/BetterJSOn.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-16 16:23:49.000000 BetterJSOn-0.0.2/BetterJSOn.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2119 2024-04-16 16:23:49.119848 BetterJSOn-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-16 16:23:49.117854 BetterJSOn-0.0.2/modules/
+-rw-rw-rw-   0        0        0      923 2024-04-16 14:21:41.000000 BetterJSOn-0.0.2/modules/files.py
+-rw-rw-rw-   0        0        0     1732 2024-04-16 14:38:57.000000 BetterJSOn-0.0.2/modules/format.py
+-rw-rw-rw-   0        0        0     5002 2024-04-16 14:13:13.000000 BetterJSOn-0.0.2/modules/parse.py
+-rw-rw-rw-   0        0        0       42 2024-04-16 16:23:49.120845 BetterJSOn-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      534 2024-04-16 16:23:40.000000 BetterJSOn-0.0.2/setup.py
```

### Comparing `betterjson-python-0.0.1/modules/files.py` & `BetterJSOn-0.0.2/modules/files.py`

 * *Files identical despite different names*

### Comparing `betterjson-python-0.0.1/modules/format.py` & `BetterJSOn-0.0.2/modules/format.py`

 * *Files identical despite different names*

### Comparing `betterjson-python-0.0.1/modules/parse.py` & `BetterJSOn-0.0.2/modules/parse.py`

 * *Files identical despite different names*

