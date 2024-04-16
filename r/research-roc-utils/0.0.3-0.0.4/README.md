# Comparing `tmp/research_roc_utils-0.0.3.tar.gz` & `tmp/research_roc_utils-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "research_roc_utils-0.0.3.tar", last modified: Tue Apr 16 09:22:22 2024, max compression
+gzip compressed data, was "research_roc_utils-0.0.4.tar", last modified: Tue Apr 16 09:26:43 2024, max compression
```

## Comparing `research_roc_utils-0.0.3.tar` & `research_roc_utils-0.0.4.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 jean-philippbruehwiler   (501) staff       (20)        0 2024-04-16 09:22:22.501828 research_roc_utils-0.0.3/
--rw-r--r--   0 jean-philippbruehwiler   (501) staff       (20)     1080 2024-04-12 08:42:51.000000 research_roc_utils-0.0.3/LICENSE
--rw-r--r--   0 jean-philippbruehwiler   (501) staff       (20)      543 2024-04-16 09:22:22.501604 research_roc_utils-0.0.3/PKG-INFO
--rw-r--r--   0 jean-philippbruehwiler   (501) staff       (20)        0 2024-04-10 14:34:49.000000 research_roc_utils-0.0.3/README.md
-drwxr-xr-x   0 jean-philippbruehwiler   (501) staff       (20)        0 2024-04-16 09:22:22.499519 research_roc_utils-0.0.3/research_roc_utils.egg-info/
--rw-r--r--   0 jean-philippbruehwiler   (501) staff       (20)      543 2024-04-16 09:22:22.000000 research_roc_utils-0.0.3/research_roc_utils.egg-info/PKG-INFO
--rw-r--r--   0 jean-philippbruehwiler   (501) staff       (20)      235 2024-04-16 09:22:22.000000 research_roc_utils-0.0.3/research_roc_utils.egg-info/SOURCES.txt
--rw-r--r--   0 jean-philippbruehwiler   (501) staff       (20)        1 2024-04-16 09:22:22.000000 research_roc_utils-0.0.3/research_roc_utils.egg-info/dependency_links.txt
--rw-r--r--   0 jean-philippbruehwiler   (501) staff       (20)      125 2024-04-16 09:22:22.000000 research_roc_utils-0.0.3/research_roc_utils.egg-info/requires.txt
--rw-r--r--   0 jean-philippbruehwiler   (501) staff       (20)        1 2024-04-16 09:22:22.000000 research_roc_utils-0.0.3/research_roc_utils.egg-info/top_level.txt
--rw-r--r--   0 jean-philippbruehwiler   (501) staff       (20)       38 2024-04-16 09:22:22.501876 research_roc_utils-0.0.3/setup.cfg
--rw-r--r--   0 jean-philippbruehwiler   (501) staff       (20)     1173 2024-04-16 09:21:56.000000 research_roc_utils-0.0.3/setup.py
+drwxr-xr-x   0 jean-philippbruehwiler   (501) staff       (20)        0 2024-04-16 09:26:43.764231 research_roc_utils-0.0.4/
+-rw-r--r--   0 jean-philippbruehwiler   (501) staff       (20)     1080 2024-04-12 08:42:51.000000 research_roc_utils-0.0.4/LICENSE
+-rw-r--r--   0 jean-philippbruehwiler   (501) staff       (20)      543 2024-04-16 09:26:43.764015 research_roc_utils-0.0.4/PKG-INFO
+-rw-r--r--   0 jean-philippbruehwiler   (501) staff       (20)        0 2024-04-10 14:34:49.000000 research_roc_utils-0.0.4/README.md
+drwxr-xr-x   0 jean-philippbruehwiler   (501) staff       (20)        0 2024-04-16 09:26:43.763803 research_roc_utils-0.0.4/research_roc_utils.egg-info/
+-rw-r--r--   0 jean-philippbruehwiler   (501) staff       (20)      543 2024-04-16 09:26:43.000000 research_roc_utils-0.0.4/research_roc_utils.egg-info/PKG-INFO
+-rw-r--r--   0 jean-philippbruehwiler   (501) staff       (20)      235 2024-04-16 09:26:43.000000 research_roc_utils-0.0.4/research_roc_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 jean-philippbruehwiler   (501) staff       (20)        1 2024-04-16 09:26:43.000000 research_roc_utils-0.0.4/research_roc_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 jean-philippbruehwiler   (501) staff       (20)      125 2024-04-16 09:26:43.000000 research_roc_utils-0.0.4/research_roc_utils.egg-info/requires.txt
+-rw-r--r--   0 jean-philippbruehwiler   (501) staff       (20)        1 2024-04-16 09:26:43.000000 research_roc_utils-0.0.4/research_roc_utils.egg-info/top_level.txt
+-rw-r--r--   0 jean-philippbruehwiler   (501) staff       (20)       38 2024-04-16 09:26:43.764275 research_roc_utils-0.0.4/setup.cfg
+-rw-r--r--   0 jean-philippbruehwiler   (501) staff       (20)     1173 2024-04-16 09:26:36.000000 research_roc_utils-0.0.4/setup.py
```

### Comparing `research_roc_utils-0.0.3/LICENSE` & `research_roc_utils-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `research_roc_utils-0.0.3/PKG-INFO` & `research_roc_utils-0.0.4/PKG-INFO`

 * *Files 21% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: research_roc_utils
-Version: 0.0.3
+Version: 0.0.4
 Summary: Utility functions to assist in the computation of ROC curve comparisons based on academic research.
 Home-page: https://github.com/jpbruehw/research-roc-utils
 Author: JP Bruehwiler
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>=1.26.4
 Requires-Dist: pandas>=2.2.2
```

### Comparing `research_roc_utils-0.0.3/research_roc_utils.egg-info/PKG-INFO` & `research_roc_utils-0.0.4/research_roc_utils.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: research-roc-utils
-Version: 0.0.3
+Version: 0.0.4
 Summary: Utility functions to assist in the computation of ROC curve comparisons based on academic research.
 Home-page: https://github.com/jpbruehw/research-roc-utils
 Author: JP Bruehwiler
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>=1.26.4
 Requires-Dist: pandas>=2.2.2
```

### Comparing `research_roc_utils-0.0.3/setup.py` & `research_roc_utils-0.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Python setup.py for project_name package"""
 import io
 import os
 from setuptools import find_packages, setup
 
 def read(*paths, **kwargs):
     """Read the contents of a text file safely.
-    >>> read("research_roc_utils", "0.0.3")
-    '0.0.3'
+    >>> read("research_roc_utils", "0.0.4")
+    '0.0.4'
     >>> read("README.md")
     ...
     """
 
     content = ""
     with io.open(
         os.path.join(os.path.dirname(__file__), *paths),
@@ -22,15 +22,15 @@
 def read_requirements(path):
     return [
         line.strip()
         for line in read(path).split("\n")
         if not line.startswith(('"', "#", "-", "git+"))
     ]
 
-VERSION = '0.0.3'
+VERSION = '0.0.4'
 
 setup(
     name="research_roc_utils",
     version=VERSION,
     description="Utility functions to assist in the computation of ROC curve comparisons based on academic research.",
     url="https://github.com/jpbruehw/research-roc-utils",
     long_description=read("README.md"),
```

