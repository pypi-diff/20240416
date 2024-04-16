# Comparing `tmp/research_roc_utils-0.0.1.tar.gz` & `tmp/research_roc_utils-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "research_roc_utils-0.0.1.tar", last modified: Tue Apr 16 08:46:22 2024, max compression
+gzip compressed data, was "research_roc_utils-0.0.2.tar", last modified: Tue Apr 16 09:08:40 2024, max compression
```

## Comparing `research_roc_utils-0.0.1.tar` & `research_roc_utils-0.0.2.tar`

### file list

```diff
@@ -1,12 +1,18 @@
-drwxr-xr-x   0 jean-philippbruehwiler   (501) staff       (20)        0 2024-04-16 08:46:22.368394 research_roc_utils-0.0.1/
--rw-r--r--   0 jean-philippbruehwiler   (501) staff       (20)     1080 2024-04-12 08:42:51.000000 research_roc_utils-0.0.1/LICENSE
--rw-r--r--   0 jean-philippbruehwiler   (501) staff       (20)      543 2024-04-16 08:46:22.368117 research_roc_utils-0.0.1/PKG-INFO
--rw-r--r--   0 jean-philippbruehwiler   (501) staff       (20)        0 2024-04-10 14:34:49.000000 research_roc_utils-0.0.1/README.md
-drwxr-xr-x   0 jean-philippbruehwiler   (501) staff       (20)        0 2024-04-16 08:46:22.367884 research_roc_utils-0.0.1/research_roc_utils.egg-info/
--rw-r--r--   0 jean-philippbruehwiler   (501) staff       (20)      543 2024-04-16 08:46:22.000000 research_roc_utils-0.0.1/research_roc_utils.egg-info/PKG-INFO
--rw-r--r--   0 jean-philippbruehwiler   (501) staff       (20)      235 2024-04-16 08:46:22.000000 research_roc_utils-0.0.1/research_roc_utils.egg-info/SOURCES.txt
--rw-r--r--   0 jean-philippbruehwiler   (501) staff       (20)        1 2024-04-16 08:46:22.000000 research_roc_utils-0.0.1/research_roc_utils.egg-info/dependency_links.txt
--rw-r--r--   0 jean-philippbruehwiler   (501) staff       (20)      125 2024-04-16 08:46:22.000000 research_roc_utils-0.0.1/research_roc_utils.egg-info/requires.txt
--rw-r--r--   0 jean-philippbruehwiler   (501) staff       (20)        1 2024-04-16 08:46:22.000000 research_roc_utils-0.0.1/research_roc_utils.egg-info/top_level.txt
--rw-r--r--   0 jean-philippbruehwiler   (501) staff       (20)       38 2024-04-16 08:46:22.368449 research_roc_utils-0.0.1/setup.cfg
--rw-r--r--   0 jean-philippbruehwiler   (501) staff       (20)     1173 2024-04-16 08:42:19.000000 research_roc_utils-0.0.1/setup.py
+drwxr-xr-x   0 jean-philippbruehwiler   (501) staff       (20)        0 2024-04-16 09:08:40.958701 research_roc_utils-0.0.2/
+-rw-r--r--   0 jean-philippbruehwiler   (501) staff       (20)     1080 2024-04-12 08:42:51.000000 research_roc_utils-0.0.2/LICENSE
+-rw-r--r--   0 jean-philippbruehwiler   (501) staff       (20)      543 2024-04-16 09:08:40.958477 research_roc_utils-0.0.2/PKG-INFO
+-rw-r--r--   0 jean-philippbruehwiler   (501) staff       (20)        0 2024-04-10 14:34:49.000000 research_roc_utils-0.0.2/README.md
+drwxr-xr-x   0 jean-philippbruehwiler   (501) staff       (20)        0 2024-04-16 09:08:40.957211 research_roc_utils-0.0.2/research_roc_utils/
+-rw-r--r--   0 jean-philippbruehwiler   (501) staff       (20)        0 2024-04-16 07:47:53.000000 research_roc_utils-0.0.2/research_roc_utils/__init__.py
+-rw-r--r--   0 jean-philippbruehwiler   (501) staff       (20)     1365 2024-04-13 19:47:20.000000 research_roc_utils-0.0.2/research_roc_utils/bootstrap_p_val.py
+-rw-r--r--   0 jean-philippbruehwiler   (501) staff       (20)     5025 2024-04-14 08:25:59.000000 research_roc_utils-0.0.2/research_roc_utils/corr_coeff_table.py
+-rw-r--r--   0 jean-philippbruehwiler   (501) staff       (20)     3155 2024-04-14 13:54:13.000000 research_roc_utils-0.0.2/research_roc_utils/helpers.py
+-rw-r--r--   0 jean-philippbruehwiler   (501) staff       (20)     8394 2024-04-14 14:33:26.000000 research_roc_utils-0.0.2/research_roc_utils/roc_utils.py
+drwxr-xr-x   0 jean-philippbruehwiler   (501) staff       (20)        0 2024-04-16 09:08:40.958266 research_roc_utils-0.0.2/research_roc_utils.egg-info/
+-rw-r--r--   0 jean-philippbruehwiler   (501) staff       (20)      543 2024-04-16 09:08:40.000000 research_roc_utils-0.0.2/research_roc_utils.egg-info/PKG-INFO
+-rw-r--r--   0 jean-philippbruehwiler   (501) staff       (20)      405 2024-04-16 09:08:40.000000 research_roc_utils-0.0.2/research_roc_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 jean-philippbruehwiler   (501) staff       (20)        1 2024-04-16 09:08:40.000000 research_roc_utils-0.0.2/research_roc_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 jean-philippbruehwiler   (501) staff       (20)      125 2024-04-16 09:08:40.000000 research_roc_utils-0.0.2/research_roc_utils.egg-info/requires.txt
+-rw-r--r--   0 jean-philippbruehwiler   (501) staff       (20)       19 2024-04-16 09:08:40.000000 research_roc_utils-0.0.2/research_roc_utils.egg-info/top_level.txt
+-rw-r--r--   0 jean-philippbruehwiler   (501) staff       (20)       38 2024-04-16 09:08:40.958749 research_roc_utils-0.0.2/setup.cfg
+-rw-r--r--   0 jean-philippbruehwiler   (501) staff       (20)     1173 2024-04-16 09:08:18.000000 research_roc_utils-0.0.2/setup.py
```

### Comparing `research_roc_utils-0.0.1/LICENSE` & `research_roc_utils-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `research_roc_utils-0.0.1/PKG-INFO` & `research_roc_utils-0.0.2/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: research_roc_utils
-Version: 0.0.1
+Version: 0.0.2
 Summary: Utility functions to assist in the computation of ROC curve comparisons based on academic research.
 Home-page: https://github.com/jpbruehw/research-roc-utils
 Author: JP Bruehwiler
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>=1.26.4
 Requires-Dist: pandas>=2.2.2
```

### Comparing `research_roc_utils-0.0.1/research_roc_utils.egg-info/PKG-INFO` & `research_roc_utils-0.0.2/research_roc_utils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: research-roc-utils
-Version: 0.0.1
+Version: 0.0.2
 Summary: Utility functions to assist in the computation of ROC curve comparisons based on academic research.
 Home-page: https://github.com/jpbruehw/research-roc-utils
 Author: JP Bruehwiler
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: numpy>=1.26.4
 Requires-Dist: pandas>=2.2.2
```

### Comparing `research_roc_utils-0.0.1/setup.py` & `research_roc_utils-0.0.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Python setup.py for project_name package"""
 import io
 import os
 from setuptools import find_packages, setup
 
 def read(*paths, **kwargs):
     """Read the contents of a text file safely.
-    >>> read("research_roc_utils", "0.0.1")
-    '0.0.1'
+    >>> read("research_roc_utils", "0.0.2")
+    '0.0.2'
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
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 
 setup(
     name="research_roc_utils",
     version=VERSION,
     description="Utility functions to assist in the computation of ROC curve comparisons based on academic research.",
     url="https://github.com/jpbruehw/research-roc-utils",
     long_description=read("README.md"),
```

