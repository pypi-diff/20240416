# Comparing `tmp/PySideX-0.0.1.tar.gz` & `tmp/PySideX-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PySideX-0.0.1.tar", last modified: Wed Apr 10 03:35:42 2024, max compression
+gzip compressed data, was "PySideX-0.0.2.tar", last modified: Tue Apr 16 18:56:59 2024, max compression
```

## Comparing `PySideX-0.0.1.tar` & `PySideX-0.0.2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-10 03:35:42.123098 PySideX-0.0.1/
--rw-rw-rw-   0        0        0     1088 2024-04-06 01:02:53.000000 PySideX-0.0.1/LICENSE
--rw-rw-rw-   0        0        0     1791 2024-04-10 03:35:42.122108 PySideX-0.0.1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-10 03:35:42.097100 PySideX-0.0.1/PySideX/
--rw-rw-rw-   0        0        0      383 2024-04-09 12:57:37.000000 PySideX-0.0.1/PySideX/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-10 03:35:42.121105 PySideX-0.0.1/PySideX.egg-info/
--rw-rw-rw-   0        0        0     1791 2024-04-10 03:35:42.000000 PySideX-0.0.1/PySideX.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      200 2024-04-10 03:35:42.000000 PySideX-0.0.1/PySideX.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-10 03:35:42.000000 PySideX-0.0.1/PySideX.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        8 2024-04-10 03:35:42.000000 PySideX-0.0.1/PySideX.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2024-04-10 03:35:42.000000 PySideX-0.0.1/PySideX.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      288 2024-04-06 01:07:23.000000 PySideX-0.0.1/README.md
--rw-rw-rw-   0        0        0       42 2024-04-10 03:35:42.123098 PySideX-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      666 2024-04-10 03:34:23.000000 PySideX-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-16 18:56:59.460606 PySideX-0.0.2/
+-rw-rw-rw-   0        0        0     1088 2024-04-06 01:02:53.000000 PySideX-0.0.2/LICENSE
+-rw-rw-rw-   0        0        0     1791 2024-04-16 18:56:59.459567 PySideX-0.0.2/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-16 18:56:59.451557 PySideX-0.0.2/PySideX/
+-rw-rw-rw-   0        0        0      365 2024-04-16 18:49:37.000000 PySideX-0.0.2/PySideX/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-16 18:56:59.458559 PySideX-0.0.2/PySideX.egg-info/
+-rw-rw-rw-   0        0        0     1791 2024-04-16 18:56:58.000000 PySideX-0.0.2/PySideX.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      200 2024-04-16 18:56:58.000000 PySideX-0.0.2/PySideX.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-16 18:56:58.000000 PySideX-0.0.2/PySideX.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        8 2024-04-16 18:56:58.000000 PySideX-0.0.2/PySideX.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2024-04-16 18:56:58.000000 PySideX-0.0.2/PySideX.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      288 2024-04-06 01:07:23.000000 PySideX-0.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2024-04-16 18:56:59.460606 PySideX-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      666 2024-04-16 18:52:45.000000 PySideX-0.0.2/setup.py
```

### Comparing `PySideX-0.0.1/LICENSE` & `PySideX-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `PySideX-0.0.1/PKG-INFO` & `PySideX-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PySideX
-Version: 0.0.1
+Version: 0.0.2
 Summary: Unofficial PySide6 library, produced with the aim of facilitating the construction of more elegant and improved interfaces using PySide6 technology
 Author: Ryan Souza Anselmo
 Author-email: ryansouza.cwb@email.com
 License: MIT License
         
         Copyright (c) 2024 Ryan Souza
```

### Comparing `PySideX-0.0.1/PySideX.egg-info/PKG-INFO` & `PySideX-0.0.2/PySideX.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PySideX
-Version: 0.0.1
+Version: 0.0.2
 Summary: Unofficial PySide6 library, produced with the aim of facilitating the construction of more elegant and improved interfaces using PySide6 technology
 Author: Ryan Souza Anselmo
 Author-email: ryansouza.cwb@email.com
 License: MIT License
         
         Copyright (c) 2024 Ryan Souza
```

### Comparing `PySideX-0.0.1/setup.py` & `PySideX-0.0.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open("PySideX/README.md", "r") as arq:
         readme = arq.read()
 
 with open("PySideX/LICENSE", "r") as arq:
         licence = arq.read()
 
 setup(name='PySideX',
-    version='0.0.1',
+    version='0.0.2',
     license=licence,
     author='Ryan Souza Anselmo',
     long_description=readme,
     long_description_content_type="text/markdown",
     author_email='ryansouza.cwb@email.com',
     keywords='pysidex',
     description=u'Unofficial PySide6 library, produced with the aim of facilitating the construction of more elegant and improved interfaces using PySide6 technology',
```

