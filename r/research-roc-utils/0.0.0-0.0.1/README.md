# Comparing `tmp/research_roc_utils-0.0.0.tar.gz` & `tmp/research_roc_utils-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "research_roc_utils-0.0.0.tar", last modified: Tue Apr 16 08:07:18 2024, max compression
+gzip compressed data, was "research_roc_utils-0.0.1.tar", last modified: Tue Apr 16 08:46:22 2024, max compression
```

## Comparing `research_roc_utils-0.0.0.tar` & `research_roc_utils-0.0.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxr-xr-x   0 jean-philippbruehwiler   (501) staff       (20)        0 2024-04-16 08:07:18.410791 research_roc_utils-0.0.0/
--rw-r--r--   0 jean-philippbruehwiler   (501) staff       (20)     1080 2024-04-12 08:42:51.000000 research_roc_utils-0.0.0/LICENSE
--rw-r--r--   0 jean-philippbruehwiler   (501) staff       (20)      883 2024-04-16 08:07:18.410609 research_roc_utils-0.0.0/PKG-INFO
--rw-r--r--   0 jean-philippbruehwiler   (501) staff       (20)        0 2024-04-10 14:34:49.000000 research_roc_utils-0.0.0/README.md
-drwxr-xr-x   0 jean-philippbruehwiler   (501) staff       (20)        0 2024-04-16 08:07:18.410388 research_roc_utils-0.0.0/research_roc_utils.egg-info/
--rw-r--r--   0 jean-philippbruehwiler   (501) staff       (20)      883 2024-04-16 08:07:18.000000 research_roc_utils-0.0.0/research_roc_utils.egg-info/PKG-INFO
--rw-r--r--   0 jean-philippbruehwiler   (501) staff       (20)      235 2024-04-16 08:07:18.000000 research_roc_utils-0.0.0/research_roc_utils.egg-info/SOURCES.txt
--rw-r--r--   0 jean-philippbruehwiler   (501) staff       (20)        1 2024-04-16 08:07:18.000000 research_roc_utils-0.0.0/research_roc_utils.egg-info/dependency_links.txt
--rw-r--r--   0 jean-philippbruehwiler   (501) staff       (20)      300 2024-04-16 08:07:18.000000 research_roc_utils-0.0.0/research_roc_utils.egg-info/requires.txt
--rw-r--r--   0 jean-philippbruehwiler   (501) staff       (20)        1 2024-04-16 08:07:18.000000 research_roc_utils-0.0.0/research_roc_utils.egg-info/top_level.txt
--rw-r--r--   0 jean-philippbruehwiler   (501) staff       (20)       38 2024-04-16 08:07:18.410833 research_roc_utils-0.0.0/setup.cfg
--rw-r--r--   0 jean-philippbruehwiler   (501) staff       (20)     1133 2024-04-16 08:04:35.000000 research_roc_utils-0.0.0/setup.py
+drwxr-xr-x   0 jean-philippbruehwiler   (501) staff       (20)        0 2024-04-16 08:46:22.368394 research_roc_utils-0.0.1/
+-rw-r--r--   0 jean-philippbruehwiler   (501) staff       (20)     1080 2024-04-12 08:42:51.000000 research_roc_utils-0.0.1/LICENSE
+-rw-r--r--   0 jean-philippbruehwiler   (501) staff       (20)      543 2024-04-16 08:46:22.368117 research_roc_utils-0.0.1/PKG-INFO
+-rw-r--r--   0 jean-philippbruehwiler   (501) staff       (20)        0 2024-04-10 14:34:49.000000 research_roc_utils-0.0.1/README.md
+drwxr-xr-x   0 jean-philippbruehwiler   (501) staff       (20)        0 2024-04-16 08:46:22.367884 research_roc_utils-0.0.1/research_roc_utils.egg-info/
+-rw-r--r--   0 jean-philippbruehwiler   (501) staff       (20)      543 2024-04-16 08:46:22.000000 research_roc_utils-0.0.1/research_roc_utils.egg-info/PKG-INFO
+-rw-r--r--   0 jean-philippbruehwiler   (501) staff       (20)      235 2024-04-16 08:46:22.000000 research_roc_utils-0.0.1/research_roc_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 jean-philippbruehwiler   (501) staff       (20)        1 2024-04-16 08:46:22.000000 research_roc_utils-0.0.1/research_roc_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 jean-philippbruehwiler   (501) staff       (20)      125 2024-04-16 08:46:22.000000 research_roc_utils-0.0.1/research_roc_utils.egg-info/requires.txt
+-rw-r--r--   0 jean-philippbruehwiler   (501) staff       (20)        1 2024-04-16 08:46:22.000000 research_roc_utils-0.0.1/research_roc_utils.egg-info/top_level.txt
+-rw-r--r--   0 jean-philippbruehwiler   (501) staff       (20)       38 2024-04-16 08:46:22.368449 research_roc_utils-0.0.1/setup.cfg
+-rw-r--r--   0 jean-philippbruehwiler   (501) staff       (20)     1173 2024-04-16 08:42:19.000000 research_roc_utils-0.0.1/setup.py
```

### Comparing `research_roc_utils-0.0.0/LICENSE` & `research_roc_utils-0.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `research_roc_utils-0.0.0/setup.py` & `research_roc_utils-0.0.1/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Python setup.py for project_name package"""
 import io
 import os
 from setuptools import find_packages, setup
 
 def read(*paths, **kwargs):
     """Read the contents of a text file safely.
-    >>> read("research_roc_utils", "1.0.0")
-    '1.0.0'
+    >>> read("research_roc_utils", "0.0.1")
+    '0.0.1'
     >>> read("README.md")
     ...
     """
 
     content = ""
     with io.open(
         os.path.join(os.path.dirname(__file__), *paths),
@@ -22,16 +22,19 @@
 def read_requirements(path):
     return [
         line.strip()
         for line in read(path).split("\n")
         if not line.startswith(('"', "#", "-", "git+"))
     ]
 
+VERSION = '0.0.1'
+
 setup(
     name="research_roc_utils",
+    version=VERSION,
     description="Utility functions to assist in the computation of ROC curve comparisons based on academic research.",
     url="https://github.com/jpbruehw/research-roc-utils",
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     author="JP Bruehwiler",
     packages=find_packages(exclude=["tests", ".github"]),
     install_requires=read_requirements("requirements.txt"),
```

