# Comparing `tmp/a9x_webstatistics_package-0.1.0.tar.gz` & `tmp/a9x_webstatistics_package-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "a9x_webstatistics_package-0.1.0.tar", last modified: Tue Apr  9 13:20:57 2024, max compression
+gzip compressed data, was "a9x_webstatistics_package-0.1.1.tar", last modified: Tue Apr 16 19:48:30 2024, max compression
```

## Comparing `a9x_webstatistics_package-0.1.0.tar` & `a9x_webstatistics_package-0.1.1.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:20:57.832666 a9x_webstatistics_package-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-09 13:20:44.000000 a9x_webstatistics_package-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-09 13:20:44.000000 a9x_webstatistics_package-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)    16832 2024-04-09 13:20:57.832666 a9x_webstatistics_package-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    15691 2024-04-09 13:20:44.000000 a9x_webstatistics_package-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-09 13:20:44.000000 a9x_webstatistics_package-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-09 13:20:57.832666 a9x_webstatistics_package-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1832 2024-04-09 13:20:44.000000 a9x_webstatistics_package-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:20:57.828665 a9x_webstatistics_package-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:20:57.828665 a9x_webstatistics_package-0.1.0/src/a9x_webstatistics/
--rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-09 13:20:44.000000 a9x_webstatistics_package-0.1.0/src/a9x_webstatistics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      603 2024-04-09 13:20:44.000000 a9x_webstatistics_package-0.1.0/src/a9x_webstatistics/main.py
--rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-09 13:20:44.000000 a9x_webstatistics_package-0.1.0/src/a9x_webstatistics/module1.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:20:57.832666 a9x_webstatistics_package-0.1.0/src/a9x_webstatistics_package.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)    16832 2024-04-09 13:20:57.000000 a9x_webstatistics_package-0.1.0/src/a9x_webstatistics_package.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-09 13:20:57.000000 a9x_webstatistics_package-0.1.0/src/a9x_webstatistics_package.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-09 13:20:57.000000 a9x_webstatistics_package-0.1.0/src/a9x_webstatistics_package.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-09 13:20:57.000000 a9x_webstatistics_package-0.1.0/src/a9x_webstatistics_package.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-09 13:20:57.000000 a9x_webstatistics_package-0.1.0/src/a9x_webstatistics_package.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-09 13:20:57.832666 a9x_webstatistics_package-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-09 13:20:44.000000 a9x_webstatistics_package-0.1.0/tests/test_module1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:48:30.047869 a9x_webstatistics_package-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1086 2024-04-16 19:48:15.000000 a9x_webstatistics_package-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       85 2024-04-16 19:48:15.000000 a9x_webstatistics_package-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)    16678 2024-04-16 19:48:30.047869 a9x_webstatistics_package-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    15637 2024-04-16 19:48:15.000000 a9x_webstatistics_package-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      170 2024-04-16 19:48:15.000000 a9x_webstatistics_package-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-16 19:48:30.051869 a9x_webstatistics_package-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1734 2024-04-16 19:48:15.000000 a9x_webstatistics_package-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:48:30.047869 a9x_webstatistics_package-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:48:30.047869 a9x_webstatistics_package-0.1.1/src/a9x_webstatistics/
+-rw-r--r--   0 runner    (1001) docker     (127)       46 2024-04-16 19:48:15.000000 a9x_webstatistics_package-0.1.1/src/a9x_webstatistics/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1509 2024-04-16 19:48:15.000000 a9x_webstatistics_package-0.1.1/src/a9x_webstatistics/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)      464 2024-04-16 19:48:15.000000 a9x_webstatistics_package-0.1.1/src/a9x_webstatistics/module1.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:48:30.047869 a9x_webstatistics_package-0.1.1/src/a9x_webstatistics_package.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)    16678 2024-04-16 19:48:29.000000 a9x_webstatistics_package-0.1.1/src/a9x_webstatistics_package.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-16 19:48:30.000000 a9x_webstatistics_package-0.1.1/src/a9x_webstatistics_package.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 19:48:29.000000 a9x_webstatistics_package-0.1.1/src/a9x_webstatistics_package.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-16 19:48:29.000000 a9x_webstatistics_package-0.1.1/src/a9x_webstatistics_package.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       18 2024-04-16 19:48:29.000000 a9x_webstatistics_package-0.1.1/src/a9x_webstatistics_package.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 19:48:30.047869 a9x_webstatistics_package-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)      235 2024-04-16 19:48:15.000000 a9x_webstatistics_package-0.1.1/tests/test_module1.py
```

### Comparing `a9x_webstatistics_package-0.1.0/LICENSE` & `a9x_webstatistics_package-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `a9x_webstatistics_package-0.1.0/PKG-INFO` & `a9x_webstatistics_package-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,47 +1,43 @@
 Metadata-Version: 2.1
 Name: a9x_webstatistics_package
-Version: 0.1.0
+Version: 0.1.1
 Summary: Web Statistics and Analytics Package
 Home-page: https://github.com/ava007/a9x-webstatistics
 Author: André von Arx
 Author-email: andrevonarx@bluewin.ch
 License: UNKNOWN
 Project-URL: Documentation, https://github.com/ava007/a9x-webstatistics
 Project-URL: Bug Reports, https://github.com/ava007/a9x-webstatistics/issues
 Project-URL: Source Code, https://github.com/ava007/a9x-webstatistics
 Keywords: webstats,statistics,analytics
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # Web Statistics and Analytics
 
 This package produces web statics and analytical output based on nginx access log files.
 
-[![PyPI package](https://img.shields.io/badge/pip%20install-a9x-webstatistics--pypi--package-brightgreen)](https://pypi.org/project/a9x-webstatistics/) [![version number](https://img.shields.io/pypi/v/example-pypi-package?color=green&label=version)](https://github.com/ava007/a9x-webstatistics/releases) [![Actions Status](https://github.com/ava007/a9x-webstatistics/workflows/Test/badge.svg)](https://github.com/ava007/a9x-webstatistics/actions) [![License](https://img.shields.io/github/license/ava007/a9x-webstatistics)](https://github.com/ava007/a9x-webstatistics/blob/main/LICENSE)
+[![PyPI package](https://img.shields.io/badge/pip%20install-example--pypi--package-brightgreen)](https://pypi.org/project/a9x-webstatistics-package/) [![version number](https://img.shields.io/pypi/v/example-pypi-package?color=green&label=version)](https://github.com/ava007/a9x-webstatistics/releases) [![Actions Status](https://github.com/ava007/a9x-webstatistics/workflows/Test/badge.svg)](https://github.com/ava007/a9x-webstatistics/actions) [![License](https://img.shields.io/github/license/ava007/a9x-webstatistics)](https://github.com/ava007/a9x-webstatistics/blob/main/LICENSE)
 
 
 
 ----------------
-
-
-# Example PyPI (Python Package Index) Package & Tutorial / Instruction / Workflow for 2021
+## old content from template starts here
 
 [![PyPI package](https://img.shields.io/badge/pip%20install-example--pypi--package-brightgreen)](https://pypi.org/project/example-pypi-package/) [![version number](https://img.shields.io/pypi/v/example-pypi-package?color=green&label=version)](https://github.com/tomchen/example_pypi_package/releases) [![Actions Status](https://github.com/tomchen/example_pypi_package/workflows/Test/badge.svg)](https://github.com/tomchen/example_pypi_package/actions) [![License](https://img.shields.io/github/license/tomchen/example_pypi_package)](https://github.com/tomchen/example_pypi_package/blob/main/LICENSE)
 
 This is an example [PyPI](https://pypi.org/) (Python Package Index) package set up with automated tests and package publishing workflow using GitHub Actions CI/CD. It is made primarily for GitHub + VS Code (Windows / Mac / Linux) users who are about to write and publish their first PyPI package. The package could serve as a starter / boilerplate / demo and the tutorial could give you a quick and concise explaination to solve some small but annoying problems you might encounter, such as package / module name confusion, and VS Code test configuration issues.
 
 <details><summary><strong>Differences from pypa/sampleproject (click to show/hide)</strong></summary>
```

### Comparing `a9x_webstatistics_package-0.1.0/README.md` & `a9x_webstatistics_package-0.1.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -1,19 +1,17 @@
 # Web Statistics and Analytics
 
 This package produces web statics and analytical output based on nginx access log files.
 
-[![PyPI package](https://img.shields.io/badge/pip%20install-a9x-webstatistics--pypi--package-brightgreen)](https://pypi.org/project/a9x-webstatistics/) [![version number](https://img.shields.io/pypi/v/example-pypi-package?color=green&label=version)](https://github.com/ava007/a9x-webstatistics/releases) [![Actions Status](https://github.com/ava007/a9x-webstatistics/workflows/Test/badge.svg)](https://github.com/ava007/a9x-webstatistics/actions) [![License](https://img.shields.io/github/license/ava007/a9x-webstatistics)](https://github.com/ava007/a9x-webstatistics/blob/main/LICENSE)
+[![PyPI package](https://img.shields.io/badge/pip%20install-example--pypi--package-brightgreen)](https://pypi.org/project/a9x-webstatistics-package/) [![version number](https://img.shields.io/pypi/v/example-pypi-package?color=green&label=version)](https://github.com/ava007/a9x-webstatistics/releases) [![Actions Status](https://github.com/ava007/a9x-webstatistics/workflows/Test/badge.svg)](https://github.com/ava007/a9x-webstatistics/actions) [![License](https://img.shields.io/github/license/ava007/a9x-webstatistics)](https://github.com/ava007/a9x-webstatistics/blob/main/LICENSE)
 
 
 
 ----------------
-
-
-# Example PyPI (Python Package Index) Package & Tutorial / Instruction / Workflow for 2021
+## old content from template starts here
 
 [![PyPI package](https://img.shields.io/badge/pip%20install-example--pypi--package-brightgreen)](https://pypi.org/project/example-pypi-package/) [![version number](https://img.shields.io/pypi/v/example-pypi-package?color=green&label=version)](https://github.com/tomchen/example_pypi_package/releases) [![Actions Status](https://github.com/tomchen/example_pypi_package/workflows/Test/badge.svg)](https://github.com/tomchen/example_pypi_package/actions) [![License](https://img.shields.io/github/license/tomchen/example_pypi_package)](https://github.com/tomchen/example_pypi_package/blob/main/LICENSE)
 
 This is an example [PyPI](https://pypi.org/) (Python Package Index) package set up with automated tests and package publishing workflow using GitHub Actions CI/CD. It is made primarily for GitHub + VS Code (Windows / Mac / Linux) users who are about to write and publish their first PyPI package. The package could serve as a starter / boilerplate / demo and the tutorial could give you a quick and concise explaination to solve some small but annoying problems you might encounter, such as package / module name confusion, and VS Code test configuration issues.
 
 <details><summary><strong>Differences from pypa/sampleproject (click to show/hide)</strong></summary>
```

### Comparing `a9x_webstatistics_package-0.1.0/setup.py` & `a9x_webstatistics_package-0.1.1/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -26,22 +26,20 @@
         # see https://pypi.org/classifiers/
         'Development Status :: 5 - Production/Stable',
 
         'Intended Audience :: Developers',
         'Topic :: Software Development :: Build Tools',
 
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3 :: Only',
         'License :: OSI Approved :: MIT License',
         'Operating System :: OS Independent',
     ],
-    python_requires='>=3.7',
+    python_requires='>=3.9',
     # install_requires=['Pillow'],
     extras_require={
         'dev': ['check-manifest'],
         # 'test': ['coverage'],
     },
     # entry_points={
     #     'console_scripts': [  # This can provide executable scripts
```

### Comparing `a9x_webstatistics_package-0.1.0/src/a9x_webstatistics_package.egg-info/PKG-INFO` & `a9x_webstatistics_package-0.1.1/src/a9x_webstatistics_package.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,47 +1,43 @@
 Metadata-Version: 2.1
 Name: a9x-webstatistics-package
-Version: 0.1.0
+Version: 0.1.1
 Summary: Web Statistics and Analytics Package
 Home-page: https://github.com/ava007/a9x-webstatistics
 Author: André von Arx
 Author-email: andrevonarx@bluewin.ch
 License: UNKNOWN
 Project-URL: Documentation, https://github.com/ava007/a9x-webstatistics
 Project-URL: Bug Reports, https://github.com/ava007/a9x-webstatistics/issues
 Project-URL: Source Code, https://github.com/ava007/a9x-webstatistics
 Keywords: webstats,statistics,analytics
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Software Development :: Build Tools
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # Web Statistics and Analytics
 
 This package produces web statics and analytical output based on nginx access log files.
 
-[![PyPI package](https://img.shields.io/badge/pip%20install-a9x-webstatistics--pypi--package-brightgreen)](https://pypi.org/project/a9x-webstatistics/) [![version number](https://img.shields.io/pypi/v/example-pypi-package?color=green&label=version)](https://github.com/ava007/a9x-webstatistics/releases) [![Actions Status](https://github.com/ava007/a9x-webstatistics/workflows/Test/badge.svg)](https://github.com/ava007/a9x-webstatistics/actions) [![License](https://img.shields.io/github/license/ava007/a9x-webstatistics)](https://github.com/ava007/a9x-webstatistics/blob/main/LICENSE)
+[![PyPI package](https://img.shields.io/badge/pip%20install-example--pypi--package-brightgreen)](https://pypi.org/project/a9x-webstatistics-package/) [![version number](https://img.shields.io/pypi/v/example-pypi-package?color=green&label=version)](https://github.com/ava007/a9x-webstatistics/releases) [![Actions Status](https://github.com/ava007/a9x-webstatistics/workflows/Test/badge.svg)](https://github.com/ava007/a9x-webstatistics/actions) [![License](https://img.shields.io/github/license/ava007/a9x-webstatistics)](https://github.com/ava007/a9x-webstatistics/blob/main/LICENSE)
 
 
 
 ----------------
-
-
-# Example PyPI (Python Package Index) Package & Tutorial / Instruction / Workflow for 2021
+## old content from template starts here
 
 [![PyPI package](https://img.shields.io/badge/pip%20install-example--pypi--package-brightgreen)](https://pypi.org/project/example-pypi-package/) [![version number](https://img.shields.io/pypi/v/example-pypi-package?color=green&label=version)](https://github.com/tomchen/example_pypi_package/releases) [![Actions Status](https://github.com/tomchen/example_pypi_package/workflows/Test/badge.svg)](https://github.com/tomchen/example_pypi_package/actions) [![License](https://img.shields.io/github/license/tomchen/example_pypi_package)](https://github.com/tomchen/example_pypi_package/blob/main/LICENSE)
 
 This is an example [PyPI](https://pypi.org/) (Python Package Index) package set up with automated tests and package publishing workflow using GitHub Actions CI/CD. It is made primarily for GitHub + VS Code (Windows / Mac / Linux) users who are about to write and publish their first PyPI package. The package could serve as a starter / boilerplate / demo and the tutorial could give you a quick and concise explaination to solve some small but annoying problems you might encounter, such as package / module name confusion, and VS Code test configuration issues.
 
 <details><summary><strong>Differences from pypa/sampleproject (click to show/hide)</strong></summary>
```

