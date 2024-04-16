# Comparing `tmp/teachbooks-0.0.1.tar.gz` & `tmp/teachbooks-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "teachbooks-0.0.1.tar", last modified: Thu Apr  4 13:03:31 2024, max compression
+gzip compressed data, was "teachbooks-0.0.2.tar", last modified: Tue Apr 16 15:24:09 2024, max compression
```

## Comparing `teachbooks-0.0.1.tar` & `teachbooks-0.0.2.tar`

### file list

```diff
@@ -1,38 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:03:31.266230 teachbooks-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-04 13:03:31.266230 teachbooks-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-04 13:03:26.000000 teachbooks-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1198 2024-04-04 13:03:26.000000 teachbooks-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-04 13:03:31.266230 teachbooks-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:03:31.262230 teachbooks-0.0.1/teachbooks/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 13:03:26.000000 teachbooks-0.0.1/teachbooks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:03:31.262230 teachbooks-0.0.1/teachbooks/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 13:03:26.000000 teachbooks-0.0.1/teachbooks/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1488 2024-04-04 13:03:26.000000 teachbooks-0.0.1/teachbooks/cli/main.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:03:31.262230 teachbooks-0.0.1/teachbooks/plugins/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 13:03:26.000000 teachbooks-0.0.1/teachbooks/plugins/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:03:31.262230 teachbooks-0.0.1/teachbooks/plugins/pybtex/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 13:03:26.000000 teachbooks-0.0.1/teachbooks/plugins/pybtex/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:03:31.262230 teachbooks-0.0.1/teachbooks/plugins/pybtex/formatting/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 13:03:26.000000 teachbooks-0.0.1/teachbooks/plugins/pybtex/formatting/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    16205 2024-04-04 13:03:26.000000 teachbooks-0.0.1/teachbooks/plugins/pybtex/formatting/apa.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:03:31.262230 teachbooks-0.0.1/teachbooks/plugins/pybtex/labels/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 13:03:26.000000 teachbooks-0.0.1/teachbooks/plugins/pybtex/labels/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-04-04 13:03:26.000000 teachbooks-0.0.1/teachbooks/plugins/pybtex/labels/apa.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:03:31.262230 teachbooks-0.0.1/teachbooks/plugins/pybtex/names/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 13:03:26.000000 teachbooks-0.0.1/teachbooks/plugins/pybtex/names/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-04-04 13:03:26.000000 teachbooks-0.0.1/teachbooks/plugins/pybtex/names/firstlast.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:03:31.262230 teachbooks-0.0.1/teachbooks/plugins/sphinxcontrib_bibtex/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 13:03:26.000000 teachbooks-0.0.1/teachbooks/plugins/sphinxcontrib_bibtex/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:03:31.262230 teachbooks-0.0.1/teachbooks/plugins/sphinxcontrib_bibtex/style/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 13:03:26.000000 teachbooks-0.0.1/teachbooks/plugins/sphinxcontrib_bibtex/style/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:03:31.262230 teachbooks-0.0.1/teachbooks/plugins/sphinxcontrib_bibtex/style/referencing/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-04 13:03:26.000000 teachbooks-0.0.1/teachbooks/plugins/sphinxcontrib_bibtex/style/referencing/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-04 13:03:26.000000 teachbooks-0.0.1/teachbooks/plugins/sphinxcontrib_bibtex/style/referencing/author_year_apa.py
--rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-04 13:03:26.000000 teachbooks-0.0.1/teachbooks/publish.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-04 13:03:31.262230 teachbooks-0.0.1/teachbooks.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      705 2024-04-04 13:03:31.000000 teachbooks-0.0.1/teachbooks.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      918 2024-04-04 13:03:31.000000 teachbooks-0.0.1/teachbooks.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-04 13:03:31.000000 teachbooks-0.0.1/teachbooks.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-04 13:03:31.000000 teachbooks-0.0.1/teachbooks.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-04 13:03:31.000000 teachbooks-0.0.1/teachbooks.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-04 13:03:31.000000 teachbooks-0.0.1/teachbooks.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:24:09.256528 teachbooks-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-04-16 15:24:09.256528 teachbooks-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      197 2024-04-16 15:24:04.000000 teachbooks-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1290 2024-04-16 15:24:04.000000 teachbooks-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 15:24:09.256528 teachbooks-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:24:09.252528 teachbooks-0.0.2/teachbooks/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 15:24:04.000000 teachbooks-0.0.2/teachbooks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:24:09.252528 teachbooks-0.0.2/teachbooks/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 15:24:04.000000 teachbooks-0.0.2/teachbooks/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2212 2024-04-16 15:24:04.000000 teachbooks-0.0.2/teachbooks/cli/main.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:24:09.252528 teachbooks-0.0.2/teachbooks/plugins/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 15:24:04.000000 teachbooks-0.0.2/teachbooks/plugins/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:24:09.252528 teachbooks-0.0.2/teachbooks/plugins/pybtex/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 15:24:04.000000 teachbooks-0.0.2/teachbooks/plugins/pybtex/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:24:09.252528 teachbooks-0.0.2/teachbooks/plugins/pybtex/formatting/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 15:24:04.000000 teachbooks-0.0.2/teachbooks/plugins/pybtex/formatting/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16205 2024-04-16 15:24:04.000000 teachbooks-0.0.2/teachbooks/plugins/pybtex/formatting/apa.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:24:09.252528 teachbooks-0.0.2/teachbooks/plugins/pybtex/labels/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 15:24:04.000000 teachbooks-0.0.2/teachbooks/plugins/pybtex/labels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2151 2024-04-16 15:24:04.000000 teachbooks-0.0.2/teachbooks/plugins/pybtex/labels/apa.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:24:09.252528 teachbooks-0.0.2/teachbooks/plugins/pybtex/names/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 15:24:04.000000 teachbooks-0.0.2/teachbooks/plugins/pybtex/names/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1596 2024-04-16 15:24:04.000000 teachbooks-0.0.2/teachbooks/plugins/pybtex/names/firstlast.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:24:09.252528 teachbooks-0.0.2/teachbooks/plugins/sphinxcontrib_bibtex/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 15:24:04.000000 teachbooks-0.0.2/teachbooks/plugins/sphinxcontrib_bibtex/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:24:09.252528 teachbooks-0.0.2/teachbooks/plugins/sphinxcontrib_bibtex/style/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 15:24:04.000000 teachbooks-0.0.2/teachbooks/plugins/sphinxcontrib_bibtex/style/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:24:09.252528 teachbooks-0.0.2/teachbooks/plugins/sphinxcontrib_bibtex/style/referencing/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 15:24:04.000000 teachbooks-0.0.2/teachbooks/plugins/sphinxcontrib_bibtex/style/referencing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-16 15:24:04.000000 teachbooks-0.0.2/teachbooks/plugins/sphinxcontrib_bibtex/style/referencing/author_year_apa.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1051 2024-04-16 15:24:04.000000 teachbooks-0.0.2/teachbooks/publish.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4683 2024-04-16 15:24:04.000000 teachbooks-0.0.2/teachbooks/serve.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:24:09.252528 teachbooks-0.0.2/teachbooks.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      855 2024-04-16 15:24:09.000000 teachbooks-0.0.2/teachbooks.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      977 2024-04-16 15:24:09.000000 teachbooks-0.0.2/teachbooks.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 15:24:09.000000 teachbooks-0.0.2/teachbooks.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      466 2024-04-16 15:24:09.000000 teachbooks-0.0.2/teachbooks.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-16 15:24:09.000000 teachbooks-0.0.2/teachbooks.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-16 15:24:09.000000 teachbooks-0.0.2/teachbooks.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 15:24:09.252528 teachbooks-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 15:24:04.000000 teachbooks-0.0.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1763 2024-04-16 15:24:04.000000 teachbooks-0.0.2/tests/test_server.py
```

### Comparing `teachbooks-0.0.1/pyproject.toml` & `teachbooks-0.0.2/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,42 @@
 [build-system]
 requires = ["setuptools>=68.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "teachbooks"
-version = "0.0.1"
+version = "0.0.2"
 description = "TU Delft CiTG Jupyter Book Software Stack"
 readme = "README.md"
 requires-python = ">=3.10"
 authors = [
   {name = "Caspar Jungbacker", email = "c.a.a.jungbacker@tudelft.nl"}
 ]
 classifiers = [
   "Programming Language :: Python :: 3",
 ]
 dependencies = [
   "jupyter-book ~= 1.0",
+  "click",
+  "psutil",
   "numpy",
   "matplotlib",
   "scipy",
   "pandas"
 ]
 
 [project.scripts]
 teachbooks = "teachbooks.cli.main:main"
 
+[project.optional-dependencies]
+testing = [
+  "pytest",
+  "flaky"
+]
+
 [tool.setuptools.packages]
 find = {}
 
 [project.urls]
 "Homepage" = "https://gitlab.tudelft.nl/interactivetextbooks-citg/extensions/teachbooks-package"
 
 [project.entry-points."pybtex.style.formatting"]
```

### Comparing `teachbooks-0.0.1/teachbooks/plugins/pybtex/formatting/apa.py` & `teachbooks-0.0.2/teachbooks/plugins/pybtex/formatting/apa.py`

 * *Files identical despite different names*

### Comparing `teachbooks-0.0.1/teachbooks/plugins/pybtex/labels/apa.py` & `teachbooks-0.0.2/teachbooks/plugins/pybtex/labels/apa.py`

 * *Files identical despite different names*

### Comparing `teachbooks-0.0.1/teachbooks/plugins/pybtex/names/firstlast.py` & `teachbooks-0.0.2/teachbooks/plugins/pybtex/names/firstlast.py`

 * *Files identical despite different names*

### Comparing `teachbooks-0.0.1/teachbooks/plugins/sphinxcontrib_bibtex/style/referencing/author_year_apa.py` & `teachbooks-0.0.2/teachbooks/plugins/sphinxcontrib_bibtex/style/referencing/author_year_apa.py`

 * *Files identical despite different names*

### Comparing `teachbooks-0.0.1/teachbooks/publish.py` & `teachbooks-0.0.2/teachbooks/publish.py`

 * *Files identical despite different names*

### Comparing `teachbooks-0.0.1/teachbooks.egg-info/SOURCES.txt` & `teachbooks-0.0.2/teachbooks.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 README.md
 pyproject.toml
 teachbooks/__init__.py
 teachbooks/publish.py
+teachbooks/serve.py
 teachbooks.egg-info/PKG-INFO
 teachbooks.egg-info/SOURCES.txt
 teachbooks.egg-info/dependency_links.txt
 teachbooks.egg-info/entry_points.txt
 teachbooks.egg-info/requires.txt
 teachbooks.egg-info/top_level.txt
 teachbooks/cli/__init__.py
@@ -17,8 +18,10 @@
 teachbooks/plugins/pybtex/labels/__init__.py
 teachbooks/plugins/pybtex/labels/apa.py
 teachbooks/plugins/pybtex/names/__init__.py
 teachbooks/plugins/pybtex/names/firstlast.py
 teachbooks/plugins/sphinxcontrib_bibtex/__init__.py
 teachbooks/plugins/sphinxcontrib_bibtex/style/__init__.py
 teachbooks/plugins/sphinxcontrib_bibtex/style/referencing/__init__.py
-teachbooks/plugins/sphinxcontrib_bibtex/style/referencing/author_year_apa.py
+teachbooks/plugins/sphinxcontrib_bibtex/style/referencing/author_year_apa.py
+tests/__init__.py
+tests/test_server.py
```

