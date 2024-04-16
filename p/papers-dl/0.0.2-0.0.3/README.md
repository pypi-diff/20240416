# Comparing `tmp/papers_dl-0.0.2.tar.gz` & `tmp/papers_dl-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "papers_dl-0.0.2.tar", last modified: Mon Apr 15 18:11:45 2024, max compression
+gzip compressed data, was "papers_dl-0.0.3.tar", last modified: Tue Apr 16 21:30:08 2024, max compression
```

## Comparing `papers_dl-0.0.2.tar` & `papers_dl-0.0.3.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2024-04-15 18:11:45.120850 papers_dl-0.0.2/
--rw-r--r--   0 ben        (501) staff       (20)     1070 2024-03-23 22:45:07.000000 papers_dl-0.0.2/LICENSE
--rw-r--r--   0 ben        (501) staff       (20)     1288 2024-04-15 18:11:45.120642 papers_dl-0.0.2/PKG-INFO
--rw-r--r--   0 ben        (501) staff       (20)      755 2024-04-14 23:03:56.000000 papers_dl-0.0.2/README.md
--rw-r--r--   0 ben        (501) staff       (20)      603 2024-04-15 18:11:14.000000 papers_dl-0.0.2/pyproject.toml
--rw-r--r--   0 ben        (501) staff       (20)       38 2024-04-15 18:11:45.120908 papers_dl-0.0.2/setup.cfg
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2024-04-15 18:11:45.119305 papers_dl-0.0.2/src/
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2024-04-15 18:11:45.120421 papers_dl-0.0.2/src/papers_dl.egg-info/
--rw-r--r--   0 ben        (501) staff       (20)     1288 2024-04-15 18:11:45.000000 papers_dl-0.0.2/src/papers_dl.egg-info/PKG-INFO
--rw-r--r--   0 ben        (501) staff       (20)      221 2024-04-15 18:11:45.000000 papers_dl-0.0.2/src/papers_dl.egg-info/SOURCES.txt
--rw-r--r--   0 ben        (501) staff       (20)        1 2024-04-15 18:11:45.000000 papers_dl-0.0.2/src/papers_dl.egg-info/dependency_links.txt
--rw-r--r--   0 ben        (501) staff       (20)       13 2024-04-15 18:11:45.000000 papers_dl-0.0.2/src/papers_dl.egg-info/top_level.txt
--rw-r--r--   0 ben        (501) staff       (20)      353 2024-04-15 17:55:03.000000 papers_dl-0.0.2/src/parse.py
--rw-r--r--   0 ben        (501) staff       (20)    10431 2024-04-14 01:36:31.000000 papers_dl-0.0.2/src/scihub.py
-drwxr-xr-x   0 ben        (501) staff       (20)        0 2024-04-15 18:11:45.120081 papers_dl-0.0.2/tests/
--rw-r--r--   0 ben        (501) staff       (20)     2130 2024-04-15 17:59:50.000000 papers_dl-0.0.2/tests/test.py
+drwxr-xr-x   0 ben        (501) staff       (20)        0 2024-04-16 21:30:08.009233 papers_dl-0.0.3/
+-rw-r--r--   0 ben        (501) staff       (20)     1070 2024-03-23 22:45:07.000000 papers_dl-0.0.3/LICENSE
+-rw-r--r--   0 ben        (501) staff       (20)     2264 2024-04-16 21:30:08.009002 papers_dl-0.0.3/PKG-INFO
+-rw-r--r--   0 ben        (501) staff       (20)     1131 2024-04-16 19:39:30.000000 papers_dl-0.0.3/README.md
+-rw-r--r--   0 ben        (501) staff       (20)      972 2024-04-16 21:30:05.000000 papers_dl-0.0.3/pyproject.toml
+-rw-r--r--   0 ben        (501) staff       (20)       38 2024-04-16 21:30:08.009284 papers_dl-0.0.3/setup.cfg
+drwxr-xr-x   0 ben        (501) staff       (20)        0 2024-04-16 21:30:08.006910 papers_dl-0.0.3/src/
+drwxr-xr-x   0 ben        (501) staff       (20)        0 2024-04-16 21:30:08.008713 papers_dl-0.0.3/src/papers_dl.egg-info/
+-rw-r--r--   0 ben        (501) staff       (20)     2264 2024-04-16 21:30:08.000000 papers_dl-0.0.3/src/papers_dl.egg-info/PKG-INFO
+-rw-r--r--   0 ben        (501) staff       (20)      257 2024-04-16 21:30:08.000000 papers_dl-0.0.3/src/papers_dl.egg-info/SOURCES.txt
+-rw-r--r--   0 ben        (501) staff       (20)        1 2024-04-16 21:30:08.000000 papers_dl-0.0.3/src/papers_dl.egg-info/dependency_links.txt
+-rw-r--r--   0 ben        (501) staff       (20)      225 2024-04-16 21:30:08.000000 papers_dl-0.0.3/src/papers_dl.egg-info/requires.txt
+-rw-r--r--   0 ben        (501) staff       (20)       13 2024-04-16 21:30:08.000000 papers_dl-0.0.3/src/papers_dl.egg-info/top_level.txt
+-rw-r--r--   0 ben        (501) staff       (20)      577 2024-04-16 19:15:05.000000 papers_dl-0.0.3/src/parse.py
+-rw-r--r--   0 ben        (501) staff       (20)    10448 2024-04-16 19:18:52.000000 papers_dl-0.0.3/src/scihub.py
+drwxr-xr-x   0 ben        (501) staff       (20)        0 2024-04-16 21:30:08.007872 papers_dl-0.0.3/tests/
+-rw-r--r--   0 ben        (501) staff       (20)     2130 2024-04-15 17:59:50.000000 papers_dl-0.0.3/tests/test.py
```

### Comparing `papers_dl-0.0.2/LICENSE` & `papers_dl-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `papers_dl-0.0.2/pyproject.toml` & `papers_dl-0.0.3/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,49 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "papers-dl"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Ben Muthalaly", email="benmuthalaly@gmail.com" },
 ]
 description = "A command line application for downloading scientific papers"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
+dependencies = [
+  "beautifulsoup4",
+  "bs4",
+  "certifi",
+  "cffi",
+  "charset-normalizer",
+  "cryptography",
+  "easygui",
+  "feedparser",
+  "google",
+  "idna",
+  "pdf2doi",
+  "pdfminer.six",
+  "pdftitle",
+  "pycparser",
+  "PyMuPDF",
+  "PyMuPDFb",
+  "PyPDF2",
+  "pyperclip",
+  "requests",
+  "retrying",
+  "sgmllib3k",
+  "six",
+  "soupsieve",
+  "urllib3",
+  "w3lib",
+]
 
 [project.urls]
 Homepage = "https://github.com/benmuth/papers-dl"
 Issues = "https://github.com/benmuth/papers-dl/issues"
```

### Comparing `papers_dl-0.0.2/src/scihub.py` & `papers_dl-0.0.3/src/scihub.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 [Search|Download] research papers from [scholar.google.com|sci-hub.io].
 
 @author zaytoun
 """
 
 from collections.abc import MutableMapping
 import re
-import argparse
 import hashlib
 import logging
 import os
 
 import requests
 import urllib3
 from bs4 import BeautifulSoup
@@ -162,15 +161,15 @@
 
                     if len(results["papers"]) >= limit:
                         return results
 
             start += 10
 
     @retry(wait_random_min=100, wait_random_max=1000, stop_max_attempt_number=10)
-    def download(self, identifier, destination="", path=None):
+    def download(self, identifier, destination="", path=None) -> dict[str, bytes | str] | None:
         """
         Downloads a paper from sci-hub given an indentifier (DOI, PMID, URL).
         Currently, this can potentially be blocked by a captcha if a certain
         limit has been reached.
         """
         data = self.fetch(identifier)
```

### Comparing `papers_dl-0.0.2/tests/test.py` & `papers_dl-0.0.3/tests/test.py`

 * *Files identical despite different names*

