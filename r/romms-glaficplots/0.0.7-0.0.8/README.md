# Comparing `tmp/romms_glaficplots-0.0.7.tar.gz` & `tmp/romms_glaficplots-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "romms_glaficplots-0.0.7.tar", last modified: Mon Mar 11 08:18:21 2024, max compression
+gzip compressed data, was "romms_glaficplots-0.0.8.tar", last modified: Tue Apr 16 19:14:03 2024, max compression
```

## Comparing `romms_glaficplots-0.0.7.tar` & `romms_glaficplots-0.0.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 ainsleylewis   (501) staff       (20)        0 2024-03-11 08:18:21.817729 romms_glaficplots-0.0.7/
--rw-r--r--   0 ainsleylewis   (501) staff       (20)     1074 2024-03-10 06:10:18.000000 romms_glaficplots-0.0.7/LICENSE.md
--rw-r--r--   0 ainsleylewis   (501) staff       (20)      918 2024-03-11 08:18:21.817499 romms_glaficplots-0.0.7/PKG-INFO
--rw-r--r--   0 ainsleylewis   (501) staff       (20)      630 2024-03-10 06:40:42.000000 romms_glaficplots-0.0.7/README.md
-drwxr-xr-x   0 ainsleylewis   (501) staff       (20)        0 2024-03-11 08:18:21.815871 romms_glaficplots-0.0.7/romms_glaficplots/
--rw-r--r--   0 ainsleylewis   (501) staff       (20)       64 2024-03-10 07:57:51.000000 romms_glaficplots-0.0.7/romms_glaficplots/__init__.py
--rw-r--r--   0 ainsleylewis   (501) staff       (20)     5020 2024-03-11 08:16:07.000000 romms_glaficplots-0.0.7/romms_glaficplots/plots.py
-drwxr-xr-x   0 ainsleylewis   (501) staff       (20)        0 2024-03-11 08:18:21.817174 romms_glaficplots-0.0.7/romms_glaficplots.egg-info/
--rw-r--r--   0 ainsleylewis   (501) staff       (20)      918 2024-03-11 08:18:21.000000 romms_glaficplots-0.0.7/romms_glaficplots.egg-info/PKG-INFO
--rw-r--r--   0 ainsleylewis   (501) staff       (20)      290 2024-03-11 08:18:21.000000 romms_glaficplots-0.0.7/romms_glaficplots.egg-info/SOURCES.txt
--rw-r--r--   0 ainsleylewis   (501) staff       (20)        1 2024-03-11 08:18:21.000000 romms_glaficplots-0.0.7/romms_glaficplots.egg-info/dependency_links.txt
--rw-r--r--   0 ainsleylewis   (501) staff       (20)       32 2024-03-11 08:18:21.000000 romms_glaficplots-0.0.7/romms_glaficplots.egg-info/requires.txt
--rw-r--r--   0 ainsleylewis   (501) staff       (20)       18 2024-03-11 08:18:21.000000 romms_glaficplots-0.0.7/romms_glaficplots.egg-info/top_level.txt
--rw-r--r--   0 ainsleylewis   (501) staff       (20)       38 2024-03-11 08:18:21.817778 romms_glaficplots-0.0.7/setup.cfg
--rw-r--r--   0 ainsleylewis   (501) staff       (20)     1121 2024-03-11 08:18:08.000000 romms_glaficplots-0.0.7/setup.py
+drwxr-xr-x   0 ainsleylewis   (501) staff       (20)        0 2024-04-16 19:14:03.442904 romms_glaficplots-0.0.8/
+-rw-r--r--   0 ainsleylewis   (501) staff       (20)     1074 2024-03-10 06:10:18.000000 romms_glaficplots-0.0.8/LICENSE.md
+-rw-r--r--   0 ainsleylewis   (501) staff       (20)      918 2024-04-16 19:14:03.442679 romms_glaficplots-0.0.8/PKG-INFO
+-rw-r--r--   0 ainsleylewis   (501) staff       (20)      708 2024-04-16 19:12:58.000000 romms_glaficplots-0.0.8/README.md
+drwxr-xr-x   0 ainsleylewis   (501) staff       (20)        0 2024-04-16 19:14:03.441400 romms_glaficplots-0.0.8/romms_glaficplots/
+-rw-r--r--   0 ainsleylewis   (501) staff       (20)       64 2024-03-10 07:57:51.000000 romms_glaficplots-0.0.8/romms_glaficplots/__init__.py
+-rw-r--r--   0 ainsleylewis   (501) staff       (20)     6170 2024-04-16 19:13:04.000000 romms_glaficplots-0.0.8/romms_glaficplots/plots.py
+drwxr-xr-x   0 ainsleylewis   (501) staff       (20)        0 2024-04-16 19:14:03.442454 romms_glaficplots-0.0.8/romms_glaficplots.egg-info/
+-rw-r--r--   0 ainsleylewis   (501) staff       (20)      918 2024-04-16 19:14:03.000000 romms_glaficplots-0.0.8/romms_glaficplots.egg-info/PKG-INFO
+-rw-r--r--   0 ainsleylewis   (501) staff       (20)      290 2024-04-16 19:14:03.000000 romms_glaficplots-0.0.8/romms_glaficplots.egg-info/SOURCES.txt
+-rw-r--r--   0 ainsleylewis   (501) staff       (20)        1 2024-04-16 19:14:03.000000 romms_glaficplots-0.0.8/romms_glaficplots.egg-info/dependency_links.txt
+-rw-r--r--   0 ainsleylewis   (501) staff       (20)       32 2024-04-16 19:14:03.000000 romms_glaficplots-0.0.8/romms_glaficplots.egg-info/requires.txt
+-rw-r--r--   0 ainsleylewis   (501) staff       (20)       18 2024-04-16 19:14:03.000000 romms_glaficplots-0.0.8/romms_glaficplots.egg-info/top_level.txt
+-rw-r--r--   0 ainsleylewis   (501) staff       (20)       38 2024-04-16 19:14:03.442952 romms_glaficplots-0.0.8/setup.cfg
+-rw-r--r--   0 ainsleylewis   (501) staff       (20)     1121 2024-04-16 19:14:00.000000 romms_glaficplots-0.0.8/setup.py
```

### Comparing `romms_glaficplots-0.0.7/LICENSE.md` & `romms_glaficplots-0.0.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `romms_glaficplots-0.0.7/PKG-INFO` & `romms_glaficplots-0.0.8/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: romms_glaficplots
-Version: 0.0.7
+Version: 0.0.8
 Summary: A python package to make basic plots (errors and critical curves) for glafic
 Home-page: https://github.com/romms921/romms_glaficplots.git
 Author: Rommulus Lewis
 Author-email: rommuluslewis@gmail.com
 License: BSD 2-clause
 Keywords: astronomy,astrophysics,gravitationallensing,lensing,glafic
 Classifier: Development Status :: 1 - Planning
```

### Comparing `romms_glaficplots-0.0.7/README.md` & `romms_glaficplots-0.0.8/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -26,13 +26,14 @@
 
 ```python
 import romms_glaficplots
 
 filename_1 = 'obs_point.dat'
 filename_2 = 'out_point.dat'
 filename_3 = 'out_crit.dat'
+plot_name = 'SIE (POS)' # Example Lens Name
 
-obs_data, pred_data = error_plot(filename_1, filename_2)
+obs_data, pred_data = error_plot(filename_1, filename_2, plot_name)
 
-obs_data, pred_data = critcurve_plot(filename_1, filename_3)
+obs_data, pred_data = critcurve_plot(filename_1, filename_2, filename_3, plot_name)
 ```
```

### Comparing `romms_glaficplots-0.0.7/romms_glaficplots.egg-info/PKG-INFO` & `romms_glaficplots-0.0.8/romms_glaficplots.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: romms-glaficplots
-Version: 0.0.7
+Version: 0.0.8
 Summary: A python package to make basic plots (errors and critical curves) for glafic
 Home-page: https://github.com/romms921/romms_glaficplots.git
 Author: Rommulus Lewis
 Author-email: rommuluslewis@gmail.com
 License: BSD 2-clause
 Keywords: astronomy,astrophysics,gravitationallensing,lensing,glafic
 Classifier: Development Status :: 1 - Planning
```

### Comparing `romms_glaficplots-0.0.7/setup.py` & `romms_glaficplots-0.0.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='romms_glaficplots',
-    version='0.0.7',    
+    version='0.0.8',    
     description='A python package to make basic plots (errors and critical curves) for glafic',
     url='https://github.com/romms921/romms_glaficplots.git',
     author='Rommulus Lewis',
     author_email='rommuluslewis@gmail.com',
     license='BSD 2-clause',
     keywords=['astronomy','astrophysics','gravitationallensing', 'lensing', 'glafic'], 
     packages=['romms_glaficplots'],
```

