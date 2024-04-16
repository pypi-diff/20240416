# Comparing `tmp/galmoss-20240216.4.tar.gz` & `tmp/galmoss-20240216.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/galmoss-20240216.4.tar", last modified: Fri Feb 16 04:21:47 2024, max compression
+gzip compressed data, was "dist/galmoss-20240216.5.tar", last modified: Fri Feb 16 04:23:54 2024, max compression
```

## Comparing `galmoss-20240216.4.tar` & `galmoss-20240216.5.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 cmloveczy   (501) staff       (20)        0 2024-02-16 04:21:47.000000 galmoss-20240216.4/
--rw-rw-rw-   0 cmloveczy   (501) staff       (20)    35148 2022-03-08 07:22:55.000000 galmoss-20240216.4/LICENSE
--rw-r--r--   0 cmloveczy   (501) staff       (20)     6759 2024-02-16 04:21:47.000000 galmoss-20240216.4/PKG-INFO
--rw-r--r--   0 cmloveczy   (501) staff       (20)     6054 2024-02-12 17:33:27.000000 galmoss-20240216.4/README.rst
-drwxr-xr-x   0 cmloveczy   (501) staff       (20)        0 2024-02-16 04:21:47.000000 galmoss-20240216.4/galmoss/
-drwxr-xr-x   0 cmloveczy   (501) staff       (20)        0 2024-02-16 04:21:47.000000 galmoss-20240216.4/galmoss/Parameter/
--rw-r--r--   0 cmloveczy   (501) staff       (20)        0 2024-02-15 19:16:32.000000 galmoss-20240216.4/galmoss/Parameter/__init__.py
--rw-r--r--   0 cmloveczy   (501) staff       (20)    17490 2024-02-15 19:16:34.000000 galmoss-20240216.4/galmoss/Parameter/basic.py
--rw-r--r--   0 cmloveczy   (501) staff       (20)    13560 2024-02-15 19:16:34.000000 galmoss-20240216.4/galmoss/Parameter/decorater.py
--rw-r--r--   0 cmloveczy   (501) staff       (20)      215 2024-02-16 04:18:42.000000 galmoss-20240216.4/galmoss/__init__.py
--rw-r--r--   0 cmloveczy   (501) staff       (20)    12219 2024-02-15 19:16:32.000000 galmoss-20240216.4/galmoss/data.py
--rw-r--r--   0 cmloveczy   (501) staff       (20)    26615 2024-02-15 19:16:32.000000 galmoss-20240216.4/galmoss/fitting.py
-drwxr-xr-x   0 cmloveczy   (501) staff       (20)        0 2024-02-16 04:21:47.000000 galmoss-20240216.4/galmoss/profile/
--rw-r--r--   0 cmloveczy   (501) staff       (20)        0 2024-02-15 19:16:32.000000 galmoss-20240216.4/galmoss/profile/__init__.py
--rw-r--r--   0 cmloveczy   (501) staff       (20)     8562 2024-02-15 19:16:34.000000 galmoss-20240216.4/galmoss/profile/basic.py
--rw-r--r--   0 cmloveczy   (501) staff       (20)    14977 2024-02-15 19:16:34.000000 galmoss-20240216.4/galmoss/profile/light_profile.py
--rw-r--r--   0 cmloveczy   (501) staff       (20)    16705 2024-02-15 19:16:32.000000 galmoss-20240216.4/galmoss/uncertainty.py
-drwxr-xr-x   0 cmloveczy   (501) staff       (20)        0 2024-02-16 04:21:47.000000 galmoss-20240216.4/galmoss.egg-info/
--rw-r--r--   0 cmloveczy   (501) staff       (20)     6759 2024-02-16 04:21:47.000000 galmoss-20240216.4/galmoss.egg-info/PKG-INFO
--rw-r--r--   0 cmloveczy   (501) staff       (20)      403 2024-02-16 04:21:47.000000 galmoss-20240216.4/galmoss.egg-info/SOURCES.txt
--rw-r--r--   0 cmloveczy   (501) staff       (20)        1 2024-02-16 04:21:47.000000 galmoss-20240216.4/galmoss.egg-info/dependency_links.txt
--rw-r--r--   0 cmloveczy   (501) staff       (20)        8 2024-02-16 04:21:47.000000 galmoss-20240216.4/galmoss.egg-info/top_level.txt
--rw-r--r--   0 cmloveczy   (501) staff       (20)       38 2024-02-16 04:21:47.000000 galmoss-20240216.4/setup.cfg
--rw-rw-rw-   0 cmloveczy   (501) staff       (20)      957 2024-02-16 04:21:24.000000 galmoss-20240216.4/setup.py
+drwxr-xr-x   0 cmloveczy   (501) staff       (20)        0 2024-02-16 04:23:54.000000 galmoss-20240216.5/
+-rw-rw-rw-   0 cmloveczy   (501) staff       (20)    35148 2022-03-08 07:22:55.000000 galmoss-20240216.5/LICENSE
+-rw-r--r--   0 cmloveczy   (501) staff       (20)     6749 2024-02-16 04:23:54.000000 galmoss-20240216.5/PKG-INFO
+-rw-r--r--   0 cmloveczy   (501) staff       (20)     6044 2024-02-16 04:23:25.000000 galmoss-20240216.5/README.rst
+drwxr-xr-x   0 cmloveczy   (501) staff       (20)        0 2024-02-16 04:23:54.000000 galmoss-20240216.5/galmoss/
+drwxr-xr-x   0 cmloveczy   (501) staff       (20)        0 2024-02-16 04:23:54.000000 galmoss-20240216.5/galmoss/Parameter/
+-rw-r--r--   0 cmloveczy   (501) staff       (20)        0 2024-02-15 19:16:32.000000 galmoss-20240216.5/galmoss/Parameter/__init__.py
+-rw-r--r--   0 cmloveczy   (501) staff       (20)    17490 2024-02-15 19:16:34.000000 galmoss-20240216.5/galmoss/Parameter/basic.py
+-rw-r--r--   0 cmloveczy   (501) staff       (20)    13560 2024-02-15 19:16:34.000000 galmoss-20240216.5/galmoss/Parameter/decorater.py
+-rw-r--r--   0 cmloveczy   (501) staff       (20)      215 2024-02-16 04:18:42.000000 galmoss-20240216.5/galmoss/__init__.py
+-rw-r--r--   0 cmloveczy   (501) staff       (20)    12219 2024-02-15 19:16:32.000000 galmoss-20240216.5/galmoss/data.py
+-rw-r--r--   0 cmloveczy   (501) staff       (20)    26615 2024-02-15 19:16:32.000000 galmoss-20240216.5/galmoss/fitting.py
+drwxr-xr-x   0 cmloveczy   (501) staff       (20)        0 2024-02-16 04:23:54.000000 galmoss-20240216.5/galmoss/profile/
+-rw-r--r--   0 cmloveczy   (501) staff       (20)        0 2024-02-15 19:16:32.000000 galmoss-20240216.5/galmoss/profile/__init__.py
+-rw-r--r--   0 cmloveczy   (501) staff       (20)     8562 2024-02-15 19:16:34.000000 galmoss-20240216.5/galmoss/profile/basic.py
+-rw-r--r--   0 cmloveczy   (501) staff       (20)    14977 2024-02-15 19:16:34.000000 galmoss-20240216.5/galmoss/profile/light_profile.py
+-rw-r--r--   0 cmloveczy   (501) staff       (20)    16705 2024-02-15 19:16:32.000000 galmoss-20240216.5/galmoss/uncertainty.py
+drwxr-xr-x   0 cmloveczy   (501) staff       (20)        0 2024-02-16 04:23:54.000000 galmoss-20240216.5/galmoss.egg-info/
+-rw-r--r--   0 cmloveczy   (501) staff       (20)     6749 2024-02-16 04:23:54.000000 galmoss-20240216.5/galmoss.egg-info/PKG-INFO
+-rw-r--r--   0 cmloveczy   (501) staff       (20)      403 2024-02-16 04:23:54.000000 galmoss-20240216.5/galmoss.egg-info/SOURCES.txt
+-rw-r--r--   0 cmloveczy   (501) staff       (20)        1 2024-02-16 04:23:54.000000 galmoss-20240216.5/galmoss.egg-info/dependency_links.txt
+-rw-r--r--   0 cmloveczy   (501) staff       (20)        8 2024-02-16 04:23:54.000000 galmoss-20240216.5/galmoss.egg-info/top_level.txt
+-rw-r--r--   0 cmloveczy   (501) staff       (20)       38 2024-02-16 04:23:54.000000 galmoss-20240216.5/setup.cfg
+-rw-rw-rw-   0 cmloveczy   (501) staff       (20)      957 2024-02-16 04:23:33.000000 galmoss-20240216.5/setup.py
```

### Comparing `galmoss-20240216.4/LICENSE` & `galmoss-20240216.5/LICENSE`

 * *Files identical despite different names*

### Comparing `galmoss-20240216.4/PKG-INFO` & `galmoss-20240216.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galmoss
-Version: 20240216.4
+Version: 20240216.5
 Summary: A Python-based, Torch-powered tool for two-dimensional fitting of galaxy profiles. By seamlessly enabling GPU parallelization, GalMOSS meets the high computational demands of large-scale galaxy surveys.
 Home-page: https://github.com/Chenmi0619/GALMoss
 Author: Chen Mi
 Author-email: chenmiastro@gmail.com
 Keywords: Astronomy data analysis,Astronomy toolbox,Galaxy profile fitting
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
@@ -13,30 +13,31 @@
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 
 .. image:: repo/logo.jpg
    :alt: 
 
-Why you choose GalMOSS?  
+Why use GalMOSS?  
 ===================================
-**8000 galaxies fitting, in only 10 mins!**
+
+**Fit 8,000 galaxies in just 10 minutes!**
 
 **GalMOSS** a Python-based, Torch-powered tool for two-dimensional fitting of galaxy profiles. By seamlessly enabling GPU parallelization, **GalMOSS** meets the high computational demands of large-scale galaxy surveys, placing galaxy profile fitting in the LSST-era. It incorporates widely used profiles such as the Sérsic, Exponential disk, Ferrer, King, Gaussian, and Moffat profiles, and allows for the easy integration of more complex models. 
 
 How to install 
 ===============
 We provide two kinds of methods to download and install **GalMOSS**, pip and git.
 
 Install via pip
 ---------------
 
 .. code-block:: python
 
-    pip install autogalaxy
+    pip install galmoss
 
 
 Install via git
 ---------------
 
 .. code-block:: python
```

### Comparing `galmoss-20240216.4/README.rst` & `galmoss-20240216.5/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 
 .. image:: repo/logo.jpg
    :alt: 
 
-Why you choose GalMOSS?  
+Why use GalMOSS?  
 ===================================
-**8000 galaxies fitting, in only 10 mins!**
+
+**Fit 8,000 galaxies in just 10 minutes!**
 
 **GalMOSS** a Python-based, Torch-powered tool for two-dimensional fitting of galaxy profiles. By seamlessly enabling GPU parallelization, **GalMOSS** meets the high computational demands of large-scale galaxy surveys, placing galaxy profile fitting in the LSST-era. It incorporates widely used profiles such as the Sérsic, Exponential disk, Ferrer, King, Gaussian, and Moffat profiles, and allows for the easy integration of more complex models. 
 
 How to install 
 ===============
 We provide two kinds of methods to download and install **GalMOSS**, pip and git.
 
 Install via pip
 ---------------
 
 .. code-block:: python
 
-    pip install autogalaxy
+    pip install galmoss
 
 
 Install via git
 ---------------
 
 .. code-block:: python
```

### Comparing `galmoss-20240216.4/galmoss/Parameter/basic.py` & `galmoss-20240216.5/galmoss/Parameter/basic.py`

 * *Files identical despite different names*

### Comparing `galmoss-20240216.4/galmoss/Parameter/decorater.py` & `galmoss-20240216.5/galmoss/Parameter/decorater.py`

 * *Files identical despite different names*

### Comparing `galmoss-20240216.4/galmoss/data.py` & `galmoss-20240216.5/galmoss/data.py`

 * *Files identical despite different names*

### Comparing `galmoss-20240216.4/galmoss/fitting.py` & `galmoss-20240216.5/galmoss/fitting.py`

 * *Files identical despite different names*

### Comparing `galmoss-20240216.4/galmoss/profile/basic.py` & `galmoss-20240216.5/galmoss/profile/basic.py`

 * *Files identical despite different names*

### Comparing `galmoss-20240216.4/galmoss/profile/light_profile.py` & `galmoss-20240216.5/galmoss/profile/light_profile.py`

 * *Files identical despite different names*

### Comparing `galmoss-20240216.4/galmoss/uncertainty.py` & `galmoss-20240216.5/galmoss/uncertainty.py`

 * *Files identical despite different names*

### Comparing `galmoss-20240216.4/galmoss.egg-info/PKG-INFO` & `galmoss-20240216.5/galmoss.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: galmoss
-Version: 20240216.4
+Version: 20240216.5
 Summary: A Python-based, Torch-powered tool for two-dimensional fitting of galaxy profiles. By seamlessly enabling GPU parallelization, GalMOSS meets the high computational demands of large-scale galaxy surveys.
 Home-page: https://github.com/Chenmi0619/GALMoss
 Author: Chen Mi
 Author-email: chenmiastro@gmail.com
 Keywords: Astronomy data analysis,Astronomy toolbox,Galaxy profile fitting
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
@@ -13,30 +13,31 @@
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 
 .. image:: repo/logo.jpg
    :alt: 
 
-Why you choose GalMOSS?  
+Why use GalMOSS?  
 ===================================
-**8000 galaxies fitting, in only 10 mins!**
+
+**Fit 8,000 galaxies in just 10 minutes!**
 
 **GalMOSS** a Python-based, Torch-powered tool for two-dimensional fitting of galaxy profiles. By seamlessly enabling GPU parallelization, **GalMOSS** meets the high computational demands of large-scale galaxy surveys, placing galaxy profile fitting in the LSST-era. It incorporates widely used profiles such as the Sérsic, Exponential disk, Ferrer, King, Gaussian, and Moffat profiles, and allows for the easy integration of more complex models. 
 
 How to install 
 ===============
 We provide two kinds of methods to download and install **GalMOSS**, pip and git.
 
 Install via pip
 ---------------
 
 .. code-block:: python
 
-    pip install autogalaxy
+    pip install galmoss
 
 
 Install via git
 ---------------
 
 .. code-block:: python
```

### Comparing `galmoss-20240216.4/setup.py` & `galmoss-20240216.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open('README.rst', 'r',encoding='utf-8') as fp:
     long_description = fp.read()
 
 setup(
     name='galmoss',
-    version='20240216.4',
+    version='20240216.5',
     description='A Python-based, Torch-powered tool for two-dimensional fitting of galaxy profiles. By seamlessly enabling GPU parallelization, GalMOSS meets the high computational demands of large-scale galaxy surveys.',
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url='https://github.com/Chenmi0619/GALMoss',
     keywords=['Astronomy data analysis', 'Astronomy toolbox', 'Galaxy profile fitting'],
     author='Chen Mi',
     author_email='chenmiastro@gmail.com',
```

