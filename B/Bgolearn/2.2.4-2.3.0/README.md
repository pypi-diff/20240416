# Comparing `tmp/Bgolearn-2.2.4.tar.gz` & `tmp/Bgolearn-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Bgolearn-2.2.4.tar", last modified: Sat Jan  6 15:19:58 2024, max compression
+gzip compressed data, was "Bgolearn-2.3.0.tar", last modified: Tue Apr 16 09:00:12 2024, max compression
```

## Comparing `Bgolearn-2.2.4.tar` & `Bgolearn-2.3.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 jacob      (501) staff       (20)        0 2024-01-06 15:19:58.803787 Bgolearn-2.2.4/
-drwxr-xr-x   0 jacob      (501) staff       (20)        0 2024-01-06 15:19:58.802045 Bgolearn-2.2.4/Bgolearn/
--rwxr-xr-x   0 jacob      (501) staff       (20)    29234 2024-01-06 15:13:48.000000 Bgolearn-2.2.4/Bgolearn/BGOsampling.py
-drwxr-xr-x   0 jacob      (501) staff       (20)        0 2024-01-06 15:19:58.803308 Bgolearn-2.2.4/Bgolearn/BgolearnFuns/
--rwxr-xr-x   0 jacob      (501) staff       (20)    24366 2023-12-28 13:22:41.000000 Bgolearn-2.2.4/Bgolearn/BgolearnFuns/BGO_eval.py
--rwxr-xr-x   0 jacob      (501) staff       (20)     4108 2023-12-27 07:44:45.000000 Bgolearn-2.2.4/Bgolearn/BgolearnFuns/BGOclf.py
--rwxr-xr-x   0 jacob      (501) staff       (20)    23232 2024-01-01 07:13:11.000000 Bgolearn-2.2.4/Bgolearn/BgolearnFuns/BGOmax.py
--rwxr-xr-x   0 jacob      (501) staff       (20)    23213 2024-01-01 07:13:14.000000 Bgolearn-2.2.4/Bgolearn/BgolearnFuns/BGOmin.py
--rw-r--r--   0 jacob      (501) staff       (20)     1001 2023-12-28 08:48:24.000000 Bgolearn-2.2.4/Bgolearn/BgolearnFuns/Untitled.ipynb
--rwxr-xr-x   0 jacob      (501) staff       (20)      651 2024-01-06 15:14:37.000000 Bgolearn-2.2.4/Bgolearn/__init__.py
-drwxr-xr-x   0 jacob      (501) staff       (20)        0 2024-01-06 15:19:58.802653 Bgolearn-2.2.4/Bgolearn.egg-info/
--rw-r--r--   0 jacob      (501) staff       (20)     2643 2024-01-06 15:19:58.000000 Bgolearn-2.2.4/Bgolearn.egg-info/PKG-INFO
--rw-r--r--   0 jacob      (501) staff       (20)      389 2024-01-06 15:19:58.000000 Bgolearn-2.2.4/Bgolearn.egg-info/SOURCES.txt
--rw-r--r--   0 jacob      (501) staff       (20)        1 2024-01-06 15:19:58.000000 Bgolearn-2.2.4/Bgolearn.egg-info/dependency_links.txt
--rw-r--r--   0 jacob      (501) staff       (20)       60 2024-01-06 15:19:58.000000 Bgolearn-2.2.4/Bgolearn.egg-info/requires.txt
--rw-r--r--   0 jacob      (501) staff       (20)        9 2024-01-06 15:19:58.000000 Bgolearn-2.2.4/Bgolearn.egg-info/top_level.txt
--rw-r--r--   0 jacob      (501) staff       (20)     2643 2024-01-06 15:19:58.803579 Bgolearn-2.2.4/PKG-INFO
--rw-r--r--   0 jacob      (501) staff       (20)     1917 2022-11-06 12:06:03.000000 Bgolearn-2.2.4/README.md
--rw-r--r--   0 jacob      (501) staff       (20)       38 2024-01-06 15:19:58.803828 Bgolearn-2.2.4/setup.cfg
--rw-r--r--   0 jacob      (501) staff       (20)     1147 2024-01-06 15:19:24.000000 Bgolearn-2.2.4/setup.py
+drwxr-xr-x   0 jacob      (501) staff       (20)        0 2024-04-16 09:00:12.641839 Bgolearn-2.3.0/
+drwxr-xr-x   0 jacob      (501) staff       (20)        0 2024-04-16 09:00:12.640129 Bgolearn-2.3.0/Bgolearn/
+-rwxr-xr-x   0 jacob      (501) staff       (20)    29136 2024-04-16 08:59:13.000000 Bgolearn-2.3.0/Bgolearn/BGOsampling.py
+drwxr-xr-x   0 jacob      (501) staff       (20)        0 2024-04-16 09:00:12.641386 Bgolearn-2.3.0/Bgolearn/BgolearnFuns/
+-rwxr-xr-x   0 jacob      (501) staff       (20)    24366 2023-12-28 13:22:41.000000 Bgolearn-2.3.0/Bgolearn/BgolearnFuns/BGO_eval.py
+-rwxr-xr-x   0 jacob      (501) staff       (20)     4108 2023-12-27 07:44:45.000000 Bgolearn-2.3.0/Bgolearn/BgolearnFuns/BGOclf.py
+-rwxr-xr-x   0 jacob      (501) staff       (20)    23232 2024-01-01 07:13:11.000000 Bgolearn-2.3.0/Bgolearn/BgolearnFuns/BGOmax.py
+-rwxr-xr-x   0 jacob      (501) staff       (20)    23213 2024-01-01 07:13:14.000000 Bgolearn-2.3.0/Bgolearn/BgolearnFuns/BGOmin.py
+-rw-r--r--   0 jacob      (501) staff       (20)     1001 2023-12-28 08:48:24.000000 Bgolearn-2.3.0/Bgolearn/BgolearnFuns/Untitled.ipynb
+-rwxr-xr-x   0 jacob      (501) staff       (20)      651 2024-01-06 15:14:37.000000 Bgolearn-2.3.0/Bgolearn/__init__.py
+drwxr-xr-x   0 jacob      (501) staff       (20)        0 2024-04-16 09:00:12.640739 Bgolearn-2.3.0/Bgolearn.egg-info/
+-rw-r--r--   0 jacob      (501) staff       (20)     2643 2024-04-16 09:00:12.000000 Bgolearn-2.3.0/Bgolearn.egg-info/PKG-INFO
+-rw-r--r--   0 jacob      (501) staff       (20)      389 2024-04-16 09:00:12.000000 Bgolearn-2.3.0/Bgolearn.egg-info/SOURCES.txt
+-rw-r--r--   0 jacob      (501) staff       (20)        1 2024-04-16 09:00:12.000000 Bgolearn-2.3.0/Bgolearn.egg-info/dependency_links.txt
+-rw-r--r--   0 jacob      (501) staff       (20)       60 2024-04-16 09:00:12.000000 Bgolearn-2.3.0/Bgolearn.egg-info/requires.txt
+-rw-r--r--   0 jacob      (501) staff       (20)        9 2024-04-16 09:00:12.000000 Bgolearn-2.3.0/Bgolearn.egg-info/top_level.txt
+-rw-r--r--   0 jacob      (501) staff       (20)     2643 2024-04-16 09:00:12.641636 Bgolearn-2.3.0/PKG-INFO
+-rw-r--r--   0 jacob      (501) staff       (20)     1917 2022-11-06 12:06:03.000000 Bgolearn-2.3.0/README.md
+-rw-r--r--   0 jacob      (501) staff       (20)       38 2024-04-16 09:00:12.641880 Bgolearn-2.3.0/setup.cfg
+-rw-r--r--   0 jacob      (501) staff       (20)     1147 2024-04-16 08:59:39.000000 Bgolearn-2.3.0/setup.py
```

### Comparing `Bgolearn-2.2.4/Bgolearn/BGOsampling.py` & `Bgolearn-2.3.0/Bgolearn/BGOsampling.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,20 +28,19 @@
 class Bgolearn(object):
     def __init__(self) -> None:
         os.makedirs('Bgolearn', exist_ok=True)
         
         now = datetime.datetime.now()
         formatted_date_time = now.strftime('%Y-%m-%d %H:%M:%S')
         print(text2art("Bgolearn"))
-        print('Package Name : Bgolearn')
-        print('Author : Bin CAO, HKUST(GZ)')
-        print('Intro : https://bgolearn.netlify.app/')
-        print('URL : https://github.com/Bin-Cao/Bgolearn')
-        print("Citation Format Suggestion:")
-        print('[Bin CAO et al]. "Active learning accelerates the discovery of high strength and high ductility lead-free solder alloys", [2023], [DOI : http://dx.doi.org/10.2139/ssrn.4686075].')
+        print(' Bgolearn, Bin CAO, HKUST(GZ)' )
+        print('URL : https://github.com/Bin-Cao/Bgolearn and https://bgolearn.netlify.app/')
+        print("Citation: ")
+        print('Materials & Design : https://doi.org/10.1016/j.matdes.2024.112921')
+        print('NPJ Computational Materials : https://doi.org/10.1038/s41524-024-01243-4')
         print('Executed on :',formatted_date_time, ' | Have a great day.')  
         print('='*80)
 
 
     def fit(self,data_matrix, Measured_response, virtual_samples, Mission ='Regression', Classifier = 'GaussianProcess',noise_std = None, Kriging_model = None, opt_num = 1 ,min_search = True, CV_test = False, Dynamic_W = False,seed=42):
         
         """
```

### Comparing `Bgolearn-2.2.4/Bgolearn/BgolearnFuns/BGO_eval.py` & `Bgolearn-2.3.0/Bgolearn/BgolearnFuns/BGO_eval.py`

 * *Files identical despite different names*

### Comparing `Bgolearn-2.2.4/Bgolearn/BgolearnFuns/BGOclf.py` & `Bgolearn-2.3.0/Bgolearn/BgolearnFuns/BGOclf.py`

 * *Files identical despite different names*

### Comparing `Bgolearn-2.2.4/Bgolearn/BgolearnFuns/BGOmax.py` & `Bgolearn-2.3.0/Bgolearn/BgolearnFuns/BGOmax.py`

 * *Files identical despite different names*

### Comparing `Bgolearn-2.2.4/Bgolearn/BgolearnFuns/BGOmin.py` & `Bgolearn-2.3.0/Bgolearn/BgolearnFuns/BGOmin.py`

 * *Files identical despite different names*

### Comparing `Bgolearn-2.2.4/Bgolearn/BgolearnFuns/Untitled.ipynb` & `Bgolearn-2.3.0/Bgolearn/BgolearnFuns/Untitled.ipynb`

 * *Files identical despite different names*

### Comparing `Bgolearn-2.2.4/Bgolearn/__init__.py` & `Bgolearn-2.3.0/Bgolearn/__init__.py`

 * *Files identical despite different names*

### Comparing `Bgolearn-2.2.4/Bgolearn.egg-info/PKG-INFO` & `Bgolearn-2.3.0/Bgolearn.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Bgolearn
-Version: 2.2.4
+Version: 2.3.0
 Summary: A Bayesian global optimization package for material design
 Home-page: https://github.com/Bin-Cao/Bgolearn
 Author: CaoBin
 Author-email: bcao@shu.edu.com
 Maintainer: CaoBin
 Maintainer-email: binjacobcao@gmail.com
 License: MIT License
```

### Comparing `Bgolearn-2.2.4/PKG-INFO` & `Bgolearn-2.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Bgolearn
-Version: 2.2.4
+Version: 2.3.0
 Summary: A Bayesian global optimization package for material design
 Home-page: https://github.com/Bin-Cao/Bgolearn
 Author: CaoBin
 Author-email: bcao@shu.edu.com
 Maintainer: CaoBin
 Maintainer-email: binjacobcao@gmail.com
 License: MIT License
```

### Comparing `Bgolearn-2.2.4/README.md` & `Bgolearn-2.3.0/README.md`

 * *Files identical despite different names*

### Comparing `Bgolearn-2.2.4/setup.py` & `Bgolearn-2.3.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='Bgolearn',
-    version='2.2.4',
+    version='2.3.0',
     description="A Bayesian global optimization package for material design",
     long_description=open('README.md', encoding='utf-8').read(),
     include_package_data=True,
     author='CaoBin',
     author_email='bcao@shu.edu.com',
     maintainer='CaoBin',
     maintainer_email='binjacobcao@gmail.com',
```

