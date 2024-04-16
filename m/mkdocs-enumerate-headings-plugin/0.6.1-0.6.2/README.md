# Comparing `tmp/mkdocs-enumerate-headings-plugin-0.6.1.tar.gz` & `tmp/mkdocs_enumerate_headings_plugin-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mkdocs-enumerate-headings-plugin-0.6.1.tar", last modified: Sat May 27 08:40:08 2023, max compression
+gzip compressed data, was "mkdocs_enumerate_headings_plugin-0.6.2.tar", last modified: Tue Apr 16 19:13:35 2024, max compression
```

## Comparing `mkdocs-enumerate-headings-plugin-0.6.1.tar` & `mkdocs_enumerate_headings_plugin-0.6.2.tar`

### file list

```diff
@@ -1,24 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 08:40:08.170551 mkdocs-enumerate-headings-plugin-0.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-05-27 08:39:45.000000 mkdocs-enumerate-headings-plugin-0.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7401 2023-05-27 08:40:08.170551 mkdocs-enumerate-headings-plugin-0.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6534 2023-05-27 08:39:45.000000 mkdocs-enumerate-headings-plugin-0.6.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 08:40:08.166551 mkdocs-enumerate-headings-plugin-0.6.1/mkdocs_enumerate_headings_plugin/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 08:39:45.000000 mkdocs-enumerate-headings-plugin-0.6.1/mkdocs_enumerate_headings_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2157 2023-05-27 08:39:45.000000 mkdocs-enumerate-headings-plugin-0.6.1/mkdocs_enumerate_headings_plugin/exclude.py
--rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-05-27 08:39:45.000000 mkdocs-enumerate-headings-plugin-0.6.1/mkdocs_enumerate_headings_plugin/heading.py
--rw-r--r--   0 runner    (1001) docker     (123)     3728 2023-05-27 08:39:45.000000 mkdocs-enumerate-headings-plugin-0.6.1/mkdocs_enumerate_headings_plugin/html_page.py
--rw-r--r--   0 runner    (1001) docker     (123)     7335 2023-05-27 08:39:45.000000 mkdocs-enumerate-headings-plugin-0.6.1/mkdocs_enumerate_headings_plugin/plugin.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 08:40:08.170551 mkdocs-enumerate-headings-plugin-0.6.1/mkdocs_enumerate_headings_plugin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7401 2023-05-27 08:40:08.000000 mkdocs-enumerate-headings-plugin-0.6.1/mkdocs_enumerate_headings_plugin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      671 2023-05-27 08:40:08.000000 mkdocs-enumerate-headings-plugin-0.6.1/mkdocs_enumerate_headings_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-27 08:40:08.000000 mkdocs-enumerate-headings-plugin-0.6.1/mkdocs_enumerate_headings_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-05-27 08:40:08.000000 mkdocs-enumerate-headings-plugin-0.6.1/mkdocs_enumerate_headings_plugin.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-27 08:40:08.000000 mkdocs-enumerate-headings-plugin-0.6.1/mkdocs_enumerate_headings_plugin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-27 08:40:08.000000 mkdocs-enumerate-headings-plugin-0.6.1/mkdocs_enumerate_headings_plugin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-27 08:40:08.170551 mkdocs-enumerate-headings-plugin-0.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-05-27 08:39:45.000000 mkdocs-enumerate-headings-plugin-0.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-27 08:40:08.170551 mkdocs-enumerate-headings-plugin-0.6.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-27 08:39:45.000000 mkdocs-enumerate-headings-plugin-0.6.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10924 2023-05-27 08:39:45.000000 mkdocs-enumerate-headings-plugin-0.6.1/tests/test_builds.py
--rw-r--r--   0 runner    (1001) docker     (123)     1904 2023-05-27 08:39:45.000000 mkdocs-enumerate-headings-plugin-0.6.1/tests/test_heading.py
--rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-05-27 08:39:45.000000 mkdocs-enumerate-headings-plugin-0.6.1/tests/test_html_page.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:13:35.868824 mkdocs_enumerate_headings_plugin-0.6.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-16 19:13:11.000000 mkdocs_enumerate_headings_plugin-0.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7468 2024-04-16 19:13:35.868824 mkdocs_enumerate_headings_plugin-0.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6534 2024-04-16 19:13:11.000000 mkdocs_enumerate_headings_plugin-0.6.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:13:35.864824 mkdocs_enumerate_headings_plugin-0.6.2/mkdocs_enumerate_headings_plugin/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 19:13:11.000000 mkdocs_enumerate_headings_plugin-0.6.2/mkdocs_enumerate_headings_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2157 2024-04-16 19:13:11.000000 mkdocs_enumerate_headings_plugin-0.6.2/mkdocs_enumerate_headings_plugin/exclude.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3237 2024-04-16 19:13:11.000000 mkdocs_enumerate_headings_plugin-0.6.2/mkdocs_enumerate_headings_plugin/heading.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3728 2024-04-16 19:13:11.000000 mkdocs_enumerate_headings_plugin-0.6.2/mkdocs_enumerate_headings_plugin/html_page.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7335 2024-04-16 19:13:11.000000 mkdocs_enumerate_headings_plugin-0.6.2/mkdocs_enumerate_headings_plugin/plugin.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:13:35.868824 mkdocs_enumerate_headings_plugin-0.6.2/mkdocs_enumerate_headings_plugin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7468 2024-04-16 19:13:35.000000 mkdocs_enumerate_headings_plugin-0.6.2/mkdocs_enumerate_headings_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      653 2024-04-16 19:13:35.000000 mkdocs_enumerate_headings_plugin-0.6.2/mkdocs_enumerate_headings_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 19:13:35.000000 mkdocs_enumerate_headings_plugin-0.6.2/mkdocs_enumerate_headings_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-16 19:13:35.000000 mkdocs_enumerate_headings_plugin-0.6.2/mkdocs_enumerate_headings_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-16 19:13:35.000000 mkdocs_enumerate_headings_plugin-0.6.2/mkdocs_enumerate_headings_plugin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       33 2024-04-16 19:13:35.000000 mkdocs_enumerate_headings_plugin-0.6.2/mkdocs_enumerate_headings_plugin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 19:13:35.868824 mkdocs_enumerate_headings_plugin-0.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1342 2024-04-16 19:13:11.000000 mkdocs_enumerate_headings_plugin-0.6.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:13:35.868824 mkdocs_enumerate_headings_plugin-0.6.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)    10924 2024-04-16 19:13:11.000000 mkdocs_enumerate_headings_plugin-0.6.2/tests/test_builds.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1904 2024-04-16 19:13:11.000000 mkdocs_enumerate_headings_plugin-0.6.2/tests/test_heading.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2323 2024-04-16 19:13:11.000000 mkdocs_enumerate_headings_plugin-0.6.2/tests/test_html_page.py
```

### Comparing `mkdocs-enumerate-headings-plugin-0.6.1/LICENSE` & `mkdocs_enumerate_headings_plugin-0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `mkdocs-enumerate-headings-plugin-0.6.1/PKG-INFO` & `mkdocs_enumerate_headings_plugin-0.6.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 Metadata-Version: 2.1
 Name: mkdocs-enumerate-headings-plugin
-Version: 0.6.1
+Version: 0.6.2
 Summary: MkDocs Plugin to enumerate the headings (h1-h6) across site pages
 Home-page: https://github.com/timvink/mkdocs-enumerate-headings-plugin.git
 Author: timvink
 Author-email: vinktim@gmail.com
 License: MIT
 Keywords: mkdocs enumerate headings plugin
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: mkdocs>=1.0.4
+Requires-Dist: beautifulsoup4>=4.9.0
 
 [![Actions Status](https://github.com/timvink/mkdocs-enumerate-headings-plugin/workflows/pytest/badge.svg)](https://github.com/timvink/mkdocs-enumerate-headings-plugin/actions)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mkdocs-enumerate-headings-plugin)
 ![PyPI](https://img.shields.io/pypi/v/mkdocs-enumerate-headings-plugin)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/mkdocs-enumerate-headings-plugin)
 [![codecov](https://codecov.io/gh/timvink/mkdocs-enumerate-headings-plugin/branch/master/graph/badge.svg)](https://codecov.io/gh/timvink/mkdocs-enumerate-headings-plugin)
 ![GitHub contributors](https://img.shields.io/github/contributors/timvink/mkdocs-enumerate-headings-plugin)
```

### Comparing `mkdocs-enumerate-headings-plugin-0.6.1/README.md` & `mkdocs_enumerate_headings_plugin-0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `mkdocs-enumerate-headings-plugin-0.6.1/mkdocs_enumerate_headings_plugin/exclude.py` & `mkdocs_enumerate_headings_plugin-0.6.2/mkdocs_enumerate_headings_plugin/exclude.py`

 * *Files identical despite different names*

### Comparing `mkdocs-enumerate-headings-plugin-0.6.1/mkdocs_enumerate_headings_plugin/heading.py` & `mkdocs_enumerate_headings_plugin-0.6.2/mkdocs_enumerate_headings_plugin/heading.py`

 * *Files identical despite different names*

### Comparing `mkdocs-enumerate-headings-plugin-0.6.1/mkdocs_enumerate_headings_plugin/html_page.py` & `mkdocs_enumerate_headings_plugin-0.6.2/mkdocs_enumerate_headings_plugin/html_page.py`

 * *Files identical despite different names*

### Comparing `mkdocs-enumerate-headings-plugin-0.6.1/mkdocs_enumerate_headings_plugin/plugin.py` & `mkdocs_enumerate_headings_plugin-0.6.2/mkdocs_enumerate_headings_plugin/plugin.py`

 * *Files identical despite different names*

### Comparing `mkdocs-enumerate-headings-plugin-0.6.1/mkdocs_enumerate_headings_plugin.egg-info/PKG-INFO` & `mkdocs_enumerate_headings_plugin-0.6.2/mkdocs_enumerate_headings_plugin.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,28 +1,30 @@
 Metadata-Version: 2.1
 Name: mkdocs-enumerate-headings-plugin
-Version: 0.6.1
+Version: 0.6.2
 Summary: MkDocs Plugin to enumerate the headings (h1-h6) across site pages
 Home-page: https://github.com/timvink/mkdocs-enumerate-headings-plugin.git
 Author: timvink
 Author-email: vinktim@gmail.com
 License: MIT
 Keywords: mkdocs enumerate headings plugin
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
+Requires-Dist: mkdocs>=1.0.4
+Requires-Dist: beautifulsoup4>=4.9.0
 
 [![Actions Status](https://github.com/timvink/mkdocs-enumerate-headings-plugin/workflows/pytest/badge.svg)](https://github.com/timvink/mkdocs-enumerate-headings-plugin/actions)
 ![PyPI - Python Version](https://img.shields.io/pypi/pyversions/mkdocs-enumerate-headings-plugin)
 ![PyPI](https://img.shields.io/pypi/v/mkdocs-enumerate-headings-plugin)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/mkdocs-enumerate-headings-plugin)
 [![codecov](https://codecov.io/gh/timvink/mkdocs-enumerate-headings-plugin/branch/master/graph/badge.svg)](https://codecov.io/gh/timvink/mkdocs-enumerate-headings-plugin)
 ![GitHub contributors](https://img.shields.io/github/contributors/timvink/mkdocs-enumerate-headings-plugin)
```

### Comparing `mkdocs-enumerate-headings-plugin-0.6.1/mkdocs_enumerate_headings_plugin.egg-info/SOURCES.txt` & `mkdocs_enumerate_headings_plugin-0.6.2/mkdocs_enumerate_headings_plugin.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -8,11 +8,10 @@
 mkdocs_enumerate_headings_plugin/plugin.py
 mkdocs_enumerate_headings_plugin.egg-info/PKG-INFO
 mkdocs_enumerate_headings_plugin.egg-info/SOURCES.txt
 mkdocs_enumerate_headings_plugin.egg-info/dependency_links.txt
 mkdocs_enumerate_headings_plugin.egg-info/entry_points.txt
 mkdocs_enumerate_headings_plugin.egg-info/requires.txt
 mkdocs_enumerate_headings_plugin.egg-info/top_level.txt
-tests/__init__.py
 tests/test_builds.py
 tests/test_heading.py
 tests/test_html_page.py
```

### Comparing `mkdocs-enumerate-headings-plugin-0.6.1/setup.py` & `mkdocs_enumerate_headings_plugin-0.6.2/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="mkdocs-enumerate-headings-plugin",
-    version="0.6.1",
+    version="0.6.2",
     description="MkDocs Plugin to enumerate the headings (h1-h6) across site pages",
     long_description=long_description,
     long_description_content_type="text/markdown",
     keywords="mkdocs enumerate headings plugin",
     url="https://github.com/timvink/mkdocs-enumerate-headings-plugin.git",
     author="timvink",
     author_email="vinktim@gmail.com",
@@ -18,19 +18,19 @@
     install_requires=["mkdocs>=1.0.4", "beautifulsoup4>=4.9.0"],
     classifiers=[
         "Intended Audience :: Developers",
         "Intended Audience :: Information Technology",
         "License :: OSI Approved :: MIT License",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3 :: Only",
-        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
     ],
-    packages=find_packages(),
+    packages=["mkdocs_enumerate_headings_plugin"],
     entry_points={
         "mkdocs.plugins": [
             "enumerate-headings=mkdocs_enumerate_headings_plugin.plugin:EnumerateHeadingsPlugin",
         ]
     },
 )
```

### Comparing `mkdocs-enumerate-headings-plugin-0.6.1/tests/test_builds.py` & `mkdocs_enumerate_headings_plugin-0.6.2/tests/test_builds.py`

 * *Files identical despite different names*

### Comparing `mkdocs-enumerate-headings-plugin-0.6.1/tests/test_heading.py` & `mkdocs_enumerate_headings_plugin-0.6.2/tests/test_heading.py`

 * *Files identical despite different names*

### Comparing `mkdocs-enumerate-headings-plugin-0.6.1/tests/test_html_page.py` & `mkdocs_enumerate_headings_plugin-0.6.2/tests/test_html_page.py`

 * *Files identical despite different names*

