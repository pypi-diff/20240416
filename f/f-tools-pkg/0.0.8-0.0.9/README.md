# Comparing `tmp/f_tools_pkg-0.0.8.tar.gz` & `tmp/f_tools_pkg-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\f_tools_pkg-0.0.8.tar", last modified: Mon Apr 15 11:08:41 2024, max compression
+gzip compressed data, was "dist\f_tools_pkg-0.0.9.tar", last modified: Tue Apr 16 07:39:06 2024, max compression
```

## Comparing `f_tools_pkg-0.0.8.tar` & `f_tools_pkg-0.0.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 11:08:41.000000 f_tools_pkg-0.0.8/
--rw-rw-rw-   0        0        0      625 2024-04-15 11:08:41.000000 f_tools_pkg-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      196 2024-04-15 11:08:01.000000 f_tools_pkg-0.0.8/README.md
-drwxrwxrwx   0        0        0        0 2024-04-15 11:08:41.000000 f_tools_pkg-0.0.8/f_tools_pkg/
--rw-rw-rw-   0        0        0      108 2022-07-20 05:57:19.000000 f_tools_pkg-0.0.8/f_tools_pkg/__init__.py
--rw-rw-rw-   0        0        0     5610 2022-07-20 05:56:17.000000 f_tools_pkg-0.0.8/f_tools_pkg/f_bmp.py
--rw-rw-rw-   0        0        0     5667 2024-04-10 12:46:32.000000 f_tools_pkg-0.0.8/f_tools_pkg/f_crypt.py
--rw-rw-rw-   0        0        0     3981 2024-04-15 11:07:02.000000 f_tools_pkg-0.0.8/f_tools_pkg/f_e.py
--rw-rw-rw-   0        0        0        0 2023-11-25 09:04:03.000000 f_tools_pkg-0.0.8/f_tools_pkg/f_ecc.py
--rw-rw-rw-   0        0        0     1621 2022-04-14 06:45:04.000000 f_tools_pkg-0.0.8/f_tools_pkg/f_excel.py
--rw-rw-rw-   0        0        0     1588 2022-03-11 02:30:39.000000 f_tools_pkg-0.0.8/f_tools_pkg/f_log.py
--rw-rw-rw-   0        0        0     2250 2022-07-20 03:22:56.000000 f_tools_pkg-0.0.8/f_tools_pkg/f_serial.py
-drwxrwxrwx   0        0        0        0 2024-04-15 11:08:41.000000 f_tools_pkg-0.0.8/f_tools_pkg.egg-info/
--rw-rw-rw-   0        0        0      625 2024-04-15 11:08:40.000000 f_tools_pkg-0.0.8/f_tools_pkg.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      368 2024-04-15 11:08:40.000000 f_tools_pkg-0.0.8/f_tools_pkg.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 11:08:40.000000 f_tools_pkg-0.0.8/f_tools_pkg.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       30 2024-04-15 11:08:40.000000 f_tools_pkg-0.0.8/f_tools_pkg.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-15 11:08:40.000000 f_tools_pkg-0.0.8/f_tools_pkg.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-15 11:08:41.000000 f_tools_pkg-0.0.8/setup.cfg
--rw-rw-rw-   0        0        0      724 2024-04-15 11:07:15.000000 f_tools_pkg-0.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-16 07:39:06.000000 f_tools_pkg-0.0.9/
+-rw-rw-rw-   0        0        0      653 2024-04-16 07:39:06.000000 f_tools_pkg-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0      224 2024-04-16 07:37:57.000000 f_tools_pkg-0.0.9/README.md
+drwxrwxrwx   0        0        0        0 2024-04-16 07:39:06.000000 f_tools_pkg-0.0.9/f_tools_pkg/
+-rw-rw-rw-   0        0        0      108 2022-07-20 05:57:19.000000 f_tools_pkg-0.0.9/f_tools_pkg/__init__.py
+-rw-rw-rw-   0        0        0     5610 2022-07-20 05:56:17.000000 f_tools_pkg-0.0.9/f_tools_pkg/f_bmp.py
+-rw-rw-rw-   0        0        0     5667 2024-04-10 12:46:32.000000 f_tools_pkg-0.0.9/f_tools_pkg/f_crypt.py
+-rw-rw-rw-   0        0        0     4756 2024-04-16 07:36:01.000000 f_tools_pkg-0.0.9/f_tools_pkg/f_e.py
+-rw-rw-rw-   0        0        0        0 2023-11-25 09:04:03.000000 f_tools_pkg-0.0.9/f_tools_pkg/f_ecc.py
+-rw-rw-rw-   0        0        0     1621 2022-04-14 06:45:04.000000 f_tools_pkg-0.0.9/f_tools_pkg/f_excel.py
+-rw-rw-rw-   0        0        0     1588 2022-03-11 02:30:39.000000 f_tools_pkg-0.0.9/f_tools_pkg/f_log.py
+-rw-rw-rw-   0        0        0     2250 2022-07-20 03:22:56.000000 f_tools_pkg-0.0.9/f_tools_pkg/f_serial.py
+drwxrwxrwx   0        0        0        0 2024-04-16 07:39:06.000000 f_tools_pkg-0.0.9/f_tools_pkg.egg-info/
+-rw-rw-rw-   0        0        0      653 2024-04-16 07:39:05.000000 f_tools_pkg-0.0.9/f_tools_pkg.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      368 2024-04-16 07:39:05.000000 f_tools_pkg-0.0.9/f_tools_pkg.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-16 07:39:05.000000 f_tools_pkg-0.0.9/f_tools_pkg.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       30 2024-04-16 07:39:05.000000 f_tools_pkg-0.0.9/f_tools_pkg.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-16 07:39:05.000000 f_tools_pkg-0.0.9/f_tools_pkg.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-16 07:39:06.000000 f_tools_pkg-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      724 2024-04-16 07:37:23.000000 f_tools_pkg-0.0.9/setup.py
```

### Comparing `f_tools_pkg-0.0.8/PKG-INFO` & `f_tools_pkg-0.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: f_tools_pkg
-Version: 0.0.8
+Version: 0.0.9
 Summary: some common tools(bmp/crypt/excel/log ...)
 Home-page: 
 Author: wushengyan
 Author-email: WUSY1991@163.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -17,8 +17,10 @@
 
 2024-3-27 V0.06  e bu add "type" parameter
 
 2024-4-10 v0.007 des3 key mast 24 Bytes, and 23:16 must not '0'
 
 2024-4-15 v0.008 command with timeout
 
+2024-4-15 v0.009 fix bug
+
```

### Comparing `f_tools_pkg-0.0.8/f_tools_pkg/f_bmp.py` & `f_tools_pkg-0.0.9/f_tools_pkg/f_bmp.py`

 * *Files identical despite different names*

### Comparing `f_tools_pkg-0.0.8/f_tools_pkg/f_crypt.py` & `f_tools_pkg-0.0.9/f_tools_pkg/f_crypt.py`

 * *Files identical despite different names*

### Comparing `f_tools_pkg-0.0.8/f_tools_pkg/f_excel.py` & `f_tools_pkg-0.0.9/f_tools_pkg/f_excel.py`

 * *Files identical despite different names*

### Comparing `f_tools_pkg-0.0.8/f_tools_pkg/f_log.py` & `f_tools_pkg-0.0.9/f_tools_pkg/f_log.py`

 * *Files identical despite different names*

### Comparing `f_tools_pkg-0.0.8/f_tools_pkg/f_serial.py` & `f_tools_pkg-0.0.9/f_tools_pkg/f_serial.py`

 * *Files identical despite different names*

### Comparing `f_tools_pkg-0.0.8/f_tools_pkg.egg-info/PKG-INFO` & `f_tools_pkg-0.0.9/f_tools_pkg.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: f-tools-pkg
-Version: 0.0.8
+Version: 0.0.9
 Summary: some common tools(bmp/crypt/excel/log ...)
 Home-page: 
 Author: wushengyan
 Author-email: WUSY1991@163.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
@@ -17,8 +17,10 @@
 
 2024-3-27 V0.06  e bu add "type" parameter
 
 2024-4-10 v0.007 des3 key mast 24 Bytes, and 23:16 must not '0'
 
 2024-4-15 v0.008 command with timeout
 
+2024-4-15 v0.009 fix bug
+
```

### Comparing `f_tools_pkg-0.0.8/setup.py` & `f_tools_pkg-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name='f_tools_pkg',
-    version='0.0.8',
+    version='0.0.9',
     packages=setuptools.find_packages(),
     url='',
     license='MIT',
     author='wushengyan',
     author_email='WUSY1991@163.com',
     description='some common tools(bmp/crypt/excel/log ...)',
     long_description=long_description,
```

