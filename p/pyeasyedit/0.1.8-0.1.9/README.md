# Comparing `tmp/pyeasyedit-0.1.8.tar.gz` & `tmp/pyeasyedit-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyeasyedit-0.1.8.tar", last modified: Tue Feb 27 21:14:06 2024, max compression
+gzip compressed data, was "pyeasyedit-0.1.9.tar", last modified: Tue Feb 27 21:25:02 2024, max compression
```

## Comparing `pyeasyedit-0.1.8.tar` & `pyeasyedit-0.1.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-02-27 21:14:06.027283 pyeasyedit-0.1.8/
--rw-rw-rw-   0        0        0       32 2024-02-26 17:56:52.000000 pyeasyedit-0.1.8/MANIFEST.in
--rw-rw-rw-   0        0        0     3710 2024-02-27 21:14:06.026369 pyeasyedit-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0     3176 2024-02-27 20:45:42.000000 pyeasyedit-0.1.8/README.md
-drwxrwxrwx   0        0        0        0 2024-02-27 21:14:06.003282 pyeasyedit-0.1.8/pyeasyedit/
--rw-rw-rw-   0        0        0     6250 2024-02-26 16:25:41.000000 pyeasyedit-0.1.8/pyeasyedit/LexersCustom.py
--rw-rw-rw-   0        0        0        0 2024-02-26 16:01:01.000000 pyeasyedit-0.1.8/pyeasyedit/__init__.py
--rw-rw-rw-   0        0        0    31683 2024-02-27 21:10:31.000000 pyeasyedit-0.1.8/pyeasyedit/__main__.py
-drwxrwxrwx   0        0        0        0 2024-02-27 21:14:06.023282 pyeasyedit-0.1.8/pyeasyedit/images/
--rw-rw-rw-   0        0        0  1957042 2024-02-26 16:13:56.000000 pyeasyedit-0.1.8/pyeasyedit/images/easyedit.png
--rw-rw-rw-   0        0        0   296016 2024-02-26 18:13:45.000000 pyeasyedit-0.1.8/pyeasyedit/images/icon.png
-drwxrwxrwx   0        0        0        0 2024-02-27 21:14:06.017282 pyeasyedit-0.1.8/pyeasyedit.egg-info/
--rw-rw-rw-   0        0        0     3710 2024-02-27 21:14:05.000000 pyeasyedit-0.1.8/pyeasyedit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      367 2024-02-27 21:14:05.000000 pyeasyedit-0.1.8/pyeasyedit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-02-27 21:14:05.000000 pyeasyedit-0.1.8/pyeasyedit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       57 2024-02-27 21:14:05.000000 pyeasyedit-0.1.8/pyeasyedit.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       73 2024-02-27 21:14:05.000000 pyeasyedit-0.1.8/pyeasyedit.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-02-27 21:14:05.000000 pyeasyedit-0.1.8/pyeasyedit.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-02-27 21:14:06.028388 pyeasyedit-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0     1008 2024-02-27 21:14:02.000000 pyeasyedit-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-02-27 21:25:02.172475 pyeasyedit-0.1.9/
+-rw-rw-rw-   0        0        0       32 2024-02-26 17:56:52.000000 pyeasyedit-0.1.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     3710 2024-02-27 21:25:02.172475 pyeasyedit-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0     3176 2024-02-27 20:45:42.000000 pyeasyedit-0.1.9/README.md
+drwxrwxrwx   0        0        0        0 2024-02-27 21:25:02.152457 pyeasyedit-0.1.9/pyeasyedit/
+-rw-rw-rw-   0        0        0     6250 2024-02-26 16:25:41.000000 pyeasyedit-0.1.9/pyeasyedit/LexersCustom.py
+-rw-rw-rw-   0        0        0        0 2024-02-26 16:01:01.000000 pyeasyedit-0.1.9/pyeasyedit/__init__.py
+-rw-rw-rw-   0        0        0    31683 2024-02-27 21:10:31.000000 pyeasyedit-0.1.9/pyeasyedit/__main__.py
+drwxrwxrwx   0        0        0        0 2024-02-27 21:25:02.169492 pyeasyedit-0.1.9/pyeasyedit/images/
+-rw-rw-rw-   0        0        0  1957042 2024-02-26 16:13:56.000000 pyeasyedit-0.1.9/pyeasyedit/images/easyedit.png
+-rw-rw-rw-   0        0        0   296016 2024-02-26 18:13:45.000000 pyeasyedit-0.1.9/pyeasyedit/images/icon.png
+drwxrwxrwx   0        0        0        0 2024-02-27 21:25:02.163474 pyeasyedit-0.1.9/pyeasyedit.egg-info/
+-rw-rw-rw-   0        0        0     3710 2024-02-27 21:25:02.000000 pyeasyedit-0.1.9/pyeasyedit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      367 2024-02-27 21:25:02.000000 pyeasyedit-0.1.9/pyeasyedit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-02-27 21:25:02.000000 pyeasyedit-0.1.9/pyeasyedit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       57 2024-02-27 21:25:02.000000 pyeasyedit-0.1.9/pyeasyedit.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       86 2024-02-27 21:25:02.000000 pyeasyedit-0.1.9/pyeasyedit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-02-27 21:25:02.000000 pyeasyedit-0.1.9/pyeasyedit.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-02-27 21:25:02.173457 pyeasyedit-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1033 2024-02-27 21:24:50.000000 pyeasyedit-0.1.9/setup.py
```

### Comparing `pyeasyedit-0.1.8/PKG-INFO` & `pyeasyedit-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyeasyedit
-Version: 0.1.8
+Version: 0.1.9
 Summary: A PyQt6 multi-tabbed editor based on QScintilla, includes limited IDE functions via Jedi
 Home-page: https://github.com/scottpeterman/pyeasyedit
 Author: Scott Peterman
 Author-email: scottpeterman@gmail.com
 License: GPLv3
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `pyeasyedit-0.1.8/README.md` & `pyeasyedit-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `pyeasyedit-0.1.8/pyeasyedit/LexersCustom.py` & `pyeasyedit-0.1.9/pyeasyedit/LexersCustom.py`

 * *Files identical despite different names*

### Comparing `pyeasyedit-0.1.8/pyeasyedit/__main__.py` & `pyeasyedit-0.1.9/pyeasyedit/__main__.py`

 * *Files identical despite different names*

### Comparing `pyeasyedit-0.1.8/pyeasyedit/images/easyedit.png` & `pyeasyedit-0.1.9/pyeasyedit/images/easyedit.png`

 * *Files identical despite different names*

### Comparing `pyeasyedit-0.1.8/pyeasyedit/images/icon.png` & `pyeasyedit-0.1.9/pyeasyedit/images/icon.png`

 * *Files identical despite different names*

### Comparing `pyeasyedit-0.1.8/pyeasyedit.egg-info/PKG-INFO` & `pyeasyedit-0.1.9/pyeasyedit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyeasyedit
-Version: 0.1.8
+Version: 0.1.9
 Summary: A PyQt6 multi-tabbed editor based on QScintilla, includes limited IDE functions via Jedi
 Home-page: https://github.com/scottpeterman/pyeasyedit
 Author: Scott Peterman
 Author-email: scottpeterman@gmail.com
 License: GPLv3
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `pyeasyedit-0.1.8/setup.py` & `pyeasyedit-0.1.9/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="pyeasyedit",
-    version="0.1.8",
+    version="0.1.9",
     description="A PyQt6 multi-tabbed editor based on QScintilla, includes limited IDE functions via Jedi",
     long_description=open('README.md').read(),
     long_description_content_type="text/markdown",
     author="Scott Peterman",
     author_email="scottpeterman@gmail.com",
     url="https://github.com/scottpeterman/pyeasyedit",
     license="GPLv3",
@@ -18,14 +18,15 @@
     packages=find_packages(),
     include_package_data=True,
     install_requires=[
         "PyQt6>=6.6.1",
         "PyQt6-Qt6>=6.6.2",
         "PyQt6-sip>=13.6.0",
         "PyQt6-QScintilla>=2.14.1",
+        "jedi>=0.19.1",
 
     ],
     entry_points={
         "console_scripts": [
             "pyeasyedit = pyeasyedit.__main__:main"
         ],
     },
```

