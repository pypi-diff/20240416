# Comparing `tmp/mdod-0.1.0.tar.gz` & `tmp/mdod-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mdod-0.1.0.tar", last modified: Tue Apr 16 00:06:41 2024, max compression
+gzip compressed data, was "mdod-0.1.1.tar", last modified: Tue Apr 16 00:18:16 2024, max compression
```

## Comparing `mdod-0.1.0.tar` & `mdod-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-04-16 00:06:41.244759 mdod-0.1.0/
--rw-rw-rw-   0        0        0      455 2024-04-16 00:06:41.244759 mdod-0.1.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2024-04-16 00:06:41.230505 mdod-0.1.0/mdod/
--rw-rw-rw-   0        0        0     1492 2024-04-15 08:05:38.000000 mdod-0.1.0/mdod/LICENSE.txt
--rw-rw-rw-   0        0        0     1022 2024-04-16 00:03:59.000000 mdod-0.1.0/mdod/README.md
--rw-rw-rw-   0        0        0       71 2024-04-15 15:08:34.000000 mdod-0.1.0/mdod/__init__.py
--rw-rw-rw-   0        0        0     2400 2024-04-02 04:07:58.000000 mdod-0.1.0/mdod/mdod.py
-drwxrwxrwx   0        0        0        0 2024-04-16 00:06:41.243757 mdod-0.1.0/mdod.egg-info/
--rw-rw-rw-   0        0        0      455 2024-04-16 00:06:41.000000 mdod-0.1.0/mdod.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      182 2024-04-16 00:06:41.000000 mdod-0.1.0/mdod.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-16 00:06:41.000000 mdod-0.1.0/mdod.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-04-16 00:06:41.000000 mdod-0.1.0/mdod.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2024-04-16 00:06:41.245759 mdod-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      628 2024-04-15 15:09:23.000000 mdod-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-16 00:18:16.289812 mdod-0.1.1/
+-rw-rw-rw-   0        0        0      447 2024-04-16 00:18:16.289812 mdod-0.1.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2024-04-16 00:18:16.269211 mdod-0.1.1/mdod/
+-rw-rw-rw-   0        0        0     1492 2024-04-15 08:05:38.000000 mdod-0.1.1/mdod/LICENSE.txt
+-rw-rw-rw-   0        0        0     1022 2024-04-16 00:03:59.000000 mdod-0.1.1/mdod/README.md
+-rw-rw-rw-   0        0        0       71 2024-04-15 15:08:34.000000 mdod-0.1.1/mdod/__init__.py
+-rw-rw-rw-   0        0        0     2400 2024-04-02 04:07:58.000000 mdod-0.1.1/mdod/mdod.py
+drwxrwxrwx   0        0        0        0 2024-04-16 00:18:16.288801 mdod-0.1.1/mdod.egg-info/
+-rw-rw-rw-   0        0        0      447 2024-04-16 00:18:16.000000 mdod-0.1.1/mdod.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      182 2024-04-16 00:18:16.000000 mdod-0.1.1/mdod.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-16 00:18:16.000000 mdod-0.1.1/mdod.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-04-16 00:18:16.000000 mdod-0.1.1/mdod.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2024-04-16 00:18:16.290811 mdod-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      620 2024-04-16 00:16:20.000000 mdod-0.1.1/setup.py
```

### Comparing `mdod-0.1.0/mdod/LICENSE.txt` & `mdod-0.1.1/mdod/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `mdod-0.1.0/mdod/README.md` & `mdod-0.1.1/mdod/README.md`

 * *Files identical despite different names*

### Comparing `mdod-0.1.0/mdod/mdod.py` & `mdod-0.1.1/mdod/mdod.py`

 * *Files identical despite different names*

### Comparing `mdod-0.1.0/setup.py` & `mdod-0.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from setuptools import setup, find_packages
 
 setup(
     name="mdod",
-    version="0.1.0",
+    version="0.1.1",
     packages=find_packages(),
     package_data={"": ["*"]},  
     install_requires=[
         '',
     ],
     author="Z Shen",
     author_email="626456708@qq.com",
     description="MDOD, Multi-Dimensional data Outlier Detection",
     license="BSD 3-Clause License",
-    url="https://https://github.com/mddod/mdod",
+    url="https://github.com/mddod/mdod",
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
     ],
 )
```

