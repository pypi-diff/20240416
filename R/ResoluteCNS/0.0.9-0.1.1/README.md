# Comparing `tmp/resolutecns-0.0.9.tar.gz` & `tmp/resolutecns-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resolutecns-0.0.9.tar", last modified: Mon Apr 15 18:05:14 2024, max compression
+gzip compressed data, was "resolutecns-0.1.1.tar", last modified: Mon Apr 15 21:10:43 2024, max compression
```

## Comparing `resolutecns-0.0.9.tar` & `resolutecns-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,18 @@
-drwxrwxrwx   0        0        0        0 2024-04-15 18:05:13.997681 resolutecns-0.0.9/
--rw-rw-rw-   0        0        0      553 2024-04-15 18:05:13.991682 resolutecns-0.0.9/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-15 18:05:13.957683 resolutecns-0.0.9/ResoluteCNS/
--rw-rw-rw-   0        0        0     3460 2024-04-15 18:04:44.000000 resolutecns-0.0.9/ResoluteCNS/ResoluteCNS.py
--rw-rw-rw-   0        0        0       35 2024-04-15 16:59:56.000000 resolutecns-0.0.9/ResoluteCNS/__init__.py
-drwxrwxrwx   0        0        0        0 2024-04-15 18:05:13.985680 resolutecns-0.0.9/ResoluteCNS.egg-info/
--rw-rw-rw-   0        0        0      553 2024-04-15 18:05:13.000000 resolutecns-0.0.9/ResoluteCNS.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      233 2024-04-15 18:05:13.000000 resolutecns-0.0.9/ResoluteCNS.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-15 18:05:13.000000 resolutecns-0.0.9/ResoluteCNS.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       16 2024-04-15 18:05:13.000000 resolutecns-0.0.9/ResoluteCNS.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2024-04-15 18:05:13.000000 resolutecns-0.0.9/ResoluteCNS.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-15 18:05:13.998679 resolutecns-0.0.9/setup.cfg
--rw-rw-rw-   0        0        0     1052 2024-04-15 18:04:50.000000 resolutecns-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-15 21:10:43.451460 resolutecns-0.1.1/
+-rw-rw-rw-   0        0        0       31 2024-04-15 18:34:47.000000 resolutecns-0.1.1/MANIFEST.in
+-rw-rw-rw-   0        0        0      553 2024-04-15 21:10:43.445459 resolutecns-0.1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-15 21:10:43.385429 resolutecns-0.1.1/ResoluteCNS/
+-rw-rw-rw-   0        0        0     2042 2024-04-15 21:10:18.000000 resolutecns-0.1.1/ResoluteCNS/ResoluteCNS.py
+-rw-rw-rw-   0        0        0       35 2024-04-15 16:59:56.000000 resolutecns-0.1.1/ResoluteCNS/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-15 21:10:43.433507 resolutecns-0.1.1/ResoluteCNS/bankruptcies/
+-rw-rw-rw-   0        0        0       37 2024-04-15 20:45:24.000000 resolutecns-0.1.1/ResoluteCNS/bankruptcies/__init__.py
+-rw-rw-rw-   0        0        0     1819 2024-04-15 20:48:02.000000 resolutecns-0.1.1/ResoluteCNS/bankruptcies/bankruptcies.py
+-rw-rw-rw-   0        0        0  3834815 2024-02-29 20:00:53.000000 resolutecns-0.1.1/ResoluteCNS/uBlock0.xpi
+drwxrwxrwx   0        0        0        0 2024-04-15 21:10:43.440461 resolutecns-0.1.1/ResoluteCNS.egg-info/
+-rw-rw-rw-   0        0        0      553 2024-04-15 21:10:43.000000 resolutecns-0.1.1/ResoluteCNS.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      347 2024-04-15 21:10:43.000000 resolutecns-0.1.1/ResoluteCNS.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-15 21:10:43.000000 resolutecns-0.1.1/ResoluteCNS.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       16 2024-04-15 21:10:43.000000 resolutecns-0.1.1/ResoluteCNS.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2024-04-15 21:10:43.000000 resolutecns-0.1.1/ResoluteCNS.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-15 21:10:43.451460 resolutecns-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0     1146 2024-04-15 21:10:32.000000 resolutecns-0.1.1/setup.py
```

### Comparing `resolutecns-0.0.9/PKG-INFO` & `resolutecns-0.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ResoluteCNS
-Version: 0.0.9
+Version: 0.1.1
 Summary: CNS Scraping Package
 Author: Ryan Detlaff
 Author-email: rdetlaff@resolutecommercial.com
 Keywords: python,first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `resolutecns-0.0.9/ResoluteCNS.egg-info/PKG-INFO` & `resolutecns-0.1.1/ResoluteCNS.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ResoluteCNS
-Version: 0.0.9
+Version: 0.1.1
 Summary: CNS Scraping Package
 Author: Ryan Detlaff
 Author-email: rdetlaff@resolutecommercial.com
 Keywords: python,first package
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Education
 Classifier: Programming Language :: Python :: 2
```

### Comparing `resolutecns-0.0.9/setup.py` & `resolutecns-0.1.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,25 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.9' 
+VERSION = '0.1.1' 
 DESCRIPTION = 'CNS Scraping Package'
 LONG_DESCRIPTION = 'CNS Scraping Package'
 
 # Setting up
 setup(
        # the name must match the folder name 'verysimplemodule'
         name="ResoluteCNS", 
         version=VERSION,
         author="Ryan Detlaff",
         author_email="rdetlaff@resolutecommercial.com",
         description=DESCRIPTION,
         long_description=LONG_DESCRIPTION,
         packages=find_packages(),
+        package_data={"":["./ResoluteCNS/uBlock0.xpi"]},
+        include_package_data=True,
         install_requires=['selenium', 'pandas'], # add any additional packages that 
         # needs to be installed along with your package. Eg: 'caer'
         
         keywords=['python', 'first package'],
         classifiers= [
             "Development Status :: 3 - Alpha",
             "Intended Audience :: Education",
```

