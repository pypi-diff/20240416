# Comparing `tmp/find-similar-2.1.0.tar.gz` & `tmp/find_similar-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "find-similar-2.1.0.tar", last modified: Sun Nov 12 10:17:35 2023, max compression
+gzip compressed data, was "find_similar-2.2.0.tar", last modified: Tue Apr 16 14:28:12 2024, max compression
```

## Comparing `find-similar-2.1.0.tar` & `find_similar-2.2.0.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-12 10:17:35.615209 find-similar-2.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1068 2023-11-12 10:17:21.000000 find-similar-2.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     8041 2023-11-12 10:17:35.615209 find-similar-2.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6643 2023-11-12 10:17:21.000000 find-similar-2.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-12 10:17:35.611209 find-similar-2.1.0/find_similar/
--rw-r--r--   0 runner    (1001) docker     (127)      138 2023-11-12 10:17:21.000000 find-similar-2.1.0/find_similar/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3485 2023-11-12 10:17:21.000000 find-similar-2.1.0/find_similar/calc_functions.py
--rw-r--r--   0 runner    (1001) docker     (127)      396 2023-11-12 10:17:21.000000 find-similar-2.1.0/find_similar/calc_models.py
--rw-r--r--   0 runner    (1001) docker     (127)     1915 2023-11-12 10:17:21.000000 find-similar-2.1.0/find_similar/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-12 10:17:35.615209 find-similar-2.1.0/find_similar/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      121 2023-11-12 10:17:21.000000 find-similar-2.1.0/find_similar/examples/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      874 2023-11-12 10:17:21.000000 find-similar-2.1.0/find_similar/examples/analyze.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-12 10:17:35.615209 find-similar-2.1.0/find_similar/examples/data/
--rw-r--r--   0 runner    (1001) docker     (127)     2518 2023-11-12 10:17:21.000000 find-similar-2.1.0/find_similar/examples/data/films-demo-ru.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1715 2023-11-12 10:17:21.000000 find-similar-2.1.0/find_similar/examples/data/films-demo-tr.yml
--rw-r--r--   0 runner    (1001) docker     (127)     2440 2023-11-12 10:17:21.000000 find-similar-2.1.0/find_similar/examples/data/films-demo-ua.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1718 2023-11-12 10:17:21.000000 find-similar-2.1.0/find_similar/examples/data/films-demo.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1815 2023-11-12 10:17:21.000000 find-similar-2.1.0/find_similar/examples/data/films-description.yml
--rw-r--r--   0 runner    (1001) docker     (127)      109 2023-11-12 10:17:21.000000 find-similar-2.1.0/find_similar/examples/data/mock.yml
--rw-r--r--   0 runner    (1001) docker     (127)      985 2023-11-12 10:17:21.000000 find-similar-2.1.0/find_similar/examples/main.py
--rw-r--r--   0 runner    (1001) docker     (127)       81 2023-11-12 10:17:21.000000 find-similar-2.1.0/find_similar/package.py
--rw-r--r--   0 runner    (1001) docker     (127)     7264 2023-11-12 10:17:21.000000 find-similar-2.1.0/find_similar/tokenize.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2023-11-12 10:17:35.611209 find-similar-2.1.0/find_similar.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     8041 2023-11-12 10:17:35.000000 find-similar-2.1.0/find_similar.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      718 2023-11-12 10:17:35.000000 find-similar-2.1.0/find_similar.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2023-11-12 10:17:35.000000 find-similar-2.1.0/find_similar.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       54 2023-11-12 10:17:35.000000 find-similar-2.1.0/find_similar.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       13 2023-11-12 10:17:35.000000 find-similar-2.1.0/find_similar.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2023-11-12 10:17:35.615209 find-similar-2.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3644 2023-11-12 10:17:21.000000 find-similar-2.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:28:12.122543 find_similar-2.2.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1068 2024-04-16 14:28:08.000000 find_similar-2.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     7969 2024-04-16 14:28:12.122543 find_similar-2.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6553 2024-04-16 14:28:08.000000 find_similar-2.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:28:12.118543 find_similar-2.2.0/find_similar/
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-16 14:28:08.000000 find_similar-2.2.0/find_similar/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3485 2024-04-16 14:28:08.000000 find_similar-2.2.0/find_similar/calc_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)      396 2024-04-16 14:28:08.000000 find_similar-2.2.0/find_similar/calc_models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1915 2024-04-16 14:28:08.000000 find_similar-2.2.0/find_similar/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:28:12.118543 find_similar-2.2.0/find_similar/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      121 2024-04-16 14:28:08.000000 find_similar-2.2.0/find_similar/examples/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      874 2024-04-16 14:28:08.000000 find_similar-2.2.0/find_similar/examples/analyze.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:28:12.122543 find_similar-2.2.0/find_similar/examples/data/
+-rw-r--r--   0 runner    (1001) docker     (127)     2518 2024-04-16 14:28:08.000000 find_similar-2.2.0/find_similar/examples/data/films-demo-ru.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1715 2024-04-16 14:28:08.000000 find_similar-2.2.0/find_similar/examples/data/films-demo-tr.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     2440 2024-04-16 14:28:08.000000 find_similar-2.2.0/find_similar/examples/data/films-demo-ua.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1718 2024-04-16 14:28:08.000000 find_similar-2.2.0/find_similar/examples/data/films-demo.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1815 2024-04-16 14:28:08.000000 find_similar-2.2.0/find_similar/examples/data/films-description.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      109 2024-04-16 14:28:08.000000 find_similar-2.2.0/find_similar/examples/data/mock.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      985 2024-04-16 14:28:08.000000 find_similar-2.2.0/find_similar/examples/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)       94 2024-04-16 14:28:08.000000 find_similar-2.2.0/find_similar/package.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7264 2024-04-16 14:28:08.000000 find_similar-2.2.0/find_similar/tokenize.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 14:28:12.122543 find_similar-2.2.0/find_similar.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     7969 2024-04-16 14:28:12.000000 find_similar-2.2.0/find_similar.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      718 2024-04-16 14:28:12.000000 find_similar-2.2.0/find_similar.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 14:28:12.000000 find_similar-2.2.0/find_similar.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       54 2024-04-16 14:28:12.000000 find_similar-2.2.0/find_similar.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-16 14:28:12.000000 find_similar-2.2.0/find_similar.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 14:28:12.122543 find_similar-2.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3649 2024-04-16 14:28:08.000000 find_similar-2.2.0/setup.py
```

### Comparing `find-similar-2.1.0/LICENSE` & `find_similar-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `find-similar-2.1.0/PKG-INFO` & `find_similar-2.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: find-similar
-Version: 2.1.0
+Version: 2.2.0
 Summary: User-friendly library to find similar objects
 Home-page: https://github.com/findsimilar/find-similar
 Author: findsimilar
 Author-email: quill@craftsman.lol
 License: MIT
-Project-URL: Documentation, https://docs.findsimilar.org
+Project-URL: Documentation, https://findsimilar.craftsman.lol
 Project-URL: Source, https://github.com/findsimilar/find-similar
 Project-URL: Tracker, https://github.com/findsimilar/find-similar/issues
 Project-URL: Release notes, https://github.com/findsimilar/find-similar/releases
 Project-URL: Changelog, https://github.com/findsimilar/find-similar/releases
 Project-URL: Download, https://pypi.org/project/find-similar/
 Keywords: python,search,machine-learning,natural-language-processing,find,words,texts,similar
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Text Processing
@@ -32,16 +32,14 @@
 
 # FindSimilar
 
 User-friendly library to find similar objects
 
 You can find **Full Project Documentation** [here][documentation_path]
 
-First you can try our [DEMO WEBAPP](http://demo.findsimilar.org/) for a quick introduction to the `find-similar` 
-
 <hr>
 
 #### Workflows
 [![Tests](https://github.com/findsimilar/find-similar/actions/workflows/run-tests.yml/badge.svg?branch=main)](https://github.com/findsimilar/find-similar/actions/workflows/run-tests.yml)
 [![Pylint](https://github.com/findsimilar/find-similar/actions/workflows/lint.yml/badge.svg?branch=main)](https://github.com/findsimilar/find-similar/actions/workflows/lint.yml)
 
 #### PyPi
@@ -131,30 +129,30 @@
 - with or without stopwords
 - using dictionary (or not)
 - using keywords (or not)
 
 ## Requirements
 
 - nltk, pymorphy3
-- See more in [Full Documentation](https://docs.findsimilar.org/about.html#requirements)
+- See more in [Full Documentation](https://findsimilar.craftsman.lol/about.html#requirements)
 
 ## Development Status
 
 - Package already available on [PyPi](https://pypi.org/project/find-similar/)
-- See more in [Full Documentation](https://docs.findsimilar.org/about.html#development-status)
+- See more in [Full Documentation](https://findsimilar.craftsman.lol/about.html#development-status)
 
 ## Install
 
 ### with pip
 
 ```commandline
 pip install find-similar
 ```
 
-See more in [Full Documentation](https://docs.findsimilar.org/install.html)
+See more in [Full Documentation](https://findsimilar.craftsman.lol/install.html)
 
 ## Quickstart
 
 ```python
 from find_similar import find_similar
 
 texts = ['one two', 'two three', 'three four']
@@ -174,14 +172,14 @@
 ### See the demonstration and mini tutorial in the [Demo project](http://demo.findsimilar.org/)
 
 ## Contributing
 
 You are welcome! To easy start please check:
 - [Full Documentation][documentation_path]
 - [Contributing](CONTRIBUTING.md)
-- [Developer Documentation](https://docs.findsimilar.org/dev_documentation.html)
+- [Developer Documentation](https://findsimilar.craftsman.lol/dev_documentation.html)
 - [Code of Conduct](CODE_OF_CONDUCT.md)
 - [Security Policy](SECURITY.md)
 - [Governance](GOVERNANCE.md)
 - [Support](SUPPORT.md)
 
-[documentation_path]: https://docs.findsimilar.org
+[documentation_path]: https://findsimilar.craftsman.lol
```

### Comparing `find-similar-2.1.0/README.md` & `find_similar-2.2.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 # FindSimilar
 
 User-friendly library to find similar objects
 
 You can find **Full Project Documentation** [here][documentation_path]
 
-First you can try our [DEMO WEBAPP](http://demo.findsimilar.org/) for a quick introduction to the `find-similar` 
-
 <hr>
 
 #### Workflows
 [![Tests](https://github.com/findsimilar/find-similar/actions/workflows/run-tests.yml/badge.svg?branch=main)](https://github.com/findsimilar/find-similar/actions/workflows/run-tests.yml)
 [![Pylint](https://github.com/findsimilar/find-similar/actions/workflows/lint.yml/badge.svg?branch=main)](https://github.com/findsimilar/find-similar/actions/workflows/lint.yml)
 
 #### PyPi
@@ -99,30 +97,30 @@
 - with or without stopwords
 - using dictionary (or not)
 - using keywords (or not)
 
 ## Requirements
 
 - nltk, pymorphy3
-- See more in [Full Documentation](https://docs.findsimilar.org/about.html#requirements)
+- See more in [Full Documentation](https://findsimilar.craftsman.lol/about.html#requirements)
 
 ## Development Status
 
 - Package already available on [PyPi](https://pypi.org/project/find-similar/)
-- See more in [Full Documentation](https://docs.findsimilar.org/about.html#development-status)
+- See more in [Full Documentation](https://findsimilar.craftsman.lol/about.html#development-status)
 
 ## Install
 
 ### with pip
 
 ```commandline
 pip install find-similar
 ```
 
-See more in [Full Documentation](https://docs.findsimilar.org/install.html)
+See more in [Full Documentation](https://findsimilar.craftsman.lol/install.html)
 
 ## Quickstart
 
 ```python
 from find_similar import find_similar
 
 texts = ['one two', 'two three', 'three four']
@@ -142,14 +140,14 @@
 ### See the demonstration and mini tutorial in the [Demo project](http://demo.findsimilar.org/)
 
 ## Contributing
 
 You are welcome! To easy start please check:
 - [Full Documentation][documentation_path]
 - [Contributing](CONTRIBUTING.md)
-- [Developer Documentation](https://docs.findsimilar.org/dev_documentation.html)
+- [Developer Documentation](https://findsimilar.craftsman.lol/dev_documentation.html)
 - [Code of Conduct](CODE_OF_CONDUCT.md)
 - [Security Policy](SECURITY.md)
 - [Governance](GOVERNANCE.md)
 - [Support](SUPPORT.md)
 
-[documentation_path]: https://docs.findsimilar.org
+[documentation_path]: https://findsimilar.craftsman.lol
```

### Comparing `find-similar-2.1.0/find_similar/calc_functions.py` & `find_similar-2.2.0/find_similar/calc_functions.py`

 * *Files identical despite different names*

### Comparing `find-similar-2.1.0/find_similar/core.py` & `find_similar-2.2.0/find_similar/core.py`

 * *Files identical despite different names*

### Comparing `find-similar-2.1.0/find_similar/examples/analyze.py` & `find_similar-2.2.0/find_similar/examples/analyze.py`

 * *Files identical despite different names*

### Comparing `find-similar-2.1.0/find_similar/examples/data/films-demo-ru.yml` & `find_similar-2.2.0/find_similar/examples/data/films-demo-ru.yml`

 * *Files identical despite different names*

### Comparing `find-similar-2.1.0/find_similar/examples/data/films-demo-tr.yml` & `find_similar-2.2.0/find_similar/examples/data/films-demo-tr.yml`

 * *Files identical despite different names*

### Comparing `find-similar-2.1.0/find_similar/examples/data/films-demo-ua.yml` & `find_similar-2.2.0/find_similar/examples/data/films-demo-ua.yml`

 * *Files identical despite different names*

### Comparing `find-similar-2.1.0/find_similar/examples/data/films-demo.yml` & `find_similar-2.2.0/find_similar/examples/data/films-demo.yml`

 * *Files identical despite different names*

### Comparing `find-similar-2.1.0/find_similar/examples/data/films-description.yml` & `find_similar-2.2.0/find_similar/examples/data/films-description.yml`

 * *Files identical despite different names*

### Comparing `find-similar-2.1.0/find_similar/examples/main.py` & `find_similar-2.2.0/find_similar/examples/main.py`

 * *Files identical despite different names*

### Comparing `find-similar-2.1.0/find_similar/tokenize.py` & `find_similar-2.2.0/find_similar/tokenize.py`

 * *Files identical despite different names*

### Comparing `find-similar-2.1.0/find_similar.egg-info/PKG-INFO` & `find_similar-2.2.0/find_similar.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: find-similar
-Version: 2.1.0
+Version: 2.2.0
 Summary: User-friendly library to find similar objects
 Home-page: https://github.com/findsimilar/find-similar
 Author: findsimilar
 Author-email: quill@craftsman.lol
 License: MIT
-Project-URL: Documentation, https://docs.findsimilar.org
+Project-URL: Documentation, https://findsimilar.craftsman.lol
 Project-URL: Source, https://github.com/findsimilar/find-similar
 Project-URL: Tracker, https://github.com/findsimilar/find-similar/issues
 Project-URL: Release notes, https://github.com/findsimilar/find-similar/releases
 Project-URL: Changelog, https://github.com/findsimilar/find-similar/releases
 Project-URL: Download, https://pypi.org/project/find-similar/
 Keywords: python,search,machine-learning,natural-language-processing,find,words,texts,similar
-Classifier: Development Status :: 4 - Beta
+Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Text Processing
@@ -32,16 +32,14 @@
 
 # FindSimilar
 
 User-friendly library to find similar objects
 
 You can find **Full Project Documentation** [here][documentation_path]
 
-First you can try our [DEMO WEBAPP](http://demo.findsimilar.org/) for a quick introduction to the `find-similar` 
-
 <hr>
 
 #### Workflows
 [![Tests](https://github.com/findsimilar/find-similar/actions/workflows/run-tests.yml/badge.svg?branch=main)](https://github.com/findsimilar/find-similar/actions/workflows/run-tests.yml)
 [![Pylint](https://github.com/findsimilar/find-similar/actions/workflows/lint.yml/badge.svg?branch=main)](https://github.com/findsimilar/find-similar/actions/workflows/lint.yml)
 
 #### PyPi
@@ -131,30 +129,30 @@
 - with or without stopwords
 - using dictionary (or not)
 - using keywords (or not)
 
 ## Requirements
 
 - nltk, pymorphy3
-- See more in [Full Documentation](https://docs.findsimilar.org/about.html#requirements)
+- See more in [Full Documentation](https://findsimilar.craftsman.lol/about.html#requirements)
 
 ## Development Status
 
 - Package already available on [PyPi](https://pypi.org/project/find-similar/)
-- See more in [Full Documentation](https://docs.findsimilar.org/about.html#development-status)
+- See more in [Full Documentation](https://findsimilar.craftsman.lol/about.html#development-status)
 
 ## Install
 
 ### with pip
 
 ```commandline
 pip install find-similar
 ```
 
-See more in [Full Documentation](https://docs.findsimilar.org/install.html)
+See more in [Full Documentation](https://findsimilar.craftsman.lol/install.html)
 
 ## Quickstart
 
 ```python
 from find_similar import find_similar
 
 texts = ['one two', 'two three', 'three four']
@@ -174,14 +172,14 @@
 ### See the demonstration and mini tutorial in the [Demo project](http://demo.findsimilar.org/)
 
 ## Contributing
 
 You are welcome! To easy start please check:
 - [Full Documentation][documentation_path]
 - [Contributing](CONTRIBUTING.md)
-- [Developer Documentation](https://docs.findsimilar.org/dev_documentation.html)
+- [Developer Documentation](https://findsimilar.craftsman.lol/dev_documentation.html)
 - [Code of Conduct](CODE_OF_CONDUCT.md)
 - [Security Policy](SECURITY.md)
 - [Governance](GOVERNANCE.md)
 - [Support](SUPPORT.md)
 
-[documentation_path]: https://docs.findsimilar.org
+[documentation_path]: https://findsimilar.craftsman.lol
```

### Comparing `find-similar-2.1.0/find_similar.egg-info/SOURCES.txt` & `find_similar-2.2.0/find_similar.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `find-similar-2.1.0/setup.py` & `find_similar-2.2.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -59,15 +59,15 @@
         package_version = get_value_from_package_info(file_line, 'version', package_version)
         package_status = get_value_from_package_info(file_line, 'status', package_status)
 
     if not (package_pypi_name and package_version and package_status):
         raise RuntimeError("Unable to determine Package Info.")
 
 PROJECT_URLS = {
-    'Documentation': 'https://docs.findsimilar.org',
+    'Documentation': 'https://findsimilar.craftsman.lol',
     'Source': 'https://github.com/findsimilar/find-similar',
     'Tracker': 'https://github.com/findsimilar/find-similar/issues',
     'Release notes': 'https://github.com/findsimilar/find-similar/releases',
     'Changelog': 'https://github.com/findsimilar/find-similar/releases',
     'Download': 'https://pypi.org/project/find-similar/',
 }
```

