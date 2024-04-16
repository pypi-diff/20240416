# Comparing `tmp/backports.tarfile-1.0.0.tar.gz` & `tmp/backports_tarfile-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backports.tarfile-1.0.0.tar", last modified: Sat Apr  6 14:35:11 2024, max compression
+gzip compressed data, was "backports_tarfile-1.1.0.tar", last modified: Tue Apr 16 11:32:03 2024, max compression
```

## Comparing `backports.tarfile-1.0.0.tar` & `backports_tarfile-1.1.0.tar`

### file list

```diff
@@ -1,32 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:35:11.130358 backports.tarfile-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-06 14:34:55.000000 backports.tarfile-1.0.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-06 14:34:55.000000 backports.tarfile-1.0.0/.editorconfig
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:35:11.130358 backports.tarfile-1.0.0/.github/
--rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-06 14:34:55.000000 backports.tarfile-1.0.0/.github/dependabot.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:35:11.130358 backports.tarfile-1.0.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     2855 2024-04-06 14:34:55.000000 backports.tarfile-1.0.0/.github/workflows/main.yml
--rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-06 14:34:55.000000 backports.tarfile-1.0.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-06 14:34:55.000000 backports.tarfile-1.0.0/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-06 14:34:55.000000 backports.tarfile-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      135 2024-04-06 14:34:55.000000 backports.tarfile-1.0.0/NEWS.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-04-06 14:35:11.130358 backports.tarfile-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-06 14:34:55.000000 backports.tarfile-1.0.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:35:11.130358 backports.tarfile-1.0.0/backports/
--rwxr-xr-x   0 runner    (1001) docker     (127)   106920 2024-04-06 14:34:55.000000 backports.tarfile-1.0.0/backports/tarfile.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:35:11.130358 backports.tarfile-1.0.0/backports.tarfile.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1861 2024-04-06 14:35:11.000000 backports.tarfile-1.0.0/backports.tarfile.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      493 2024-04-06 14:35:11.000000 backports.tarfile-1.0.0/backports.tarfile.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-06 14:35:11.000000 backports.tarfile-1.0.0/backports.tarfile.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      157 2024-04-06 14:35:11.000000 backports.tarfile-1.0.0/backports.tarfile.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-06 14:35:11.000000 backports.tarfile-1.0.0/backports.tarfile.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-06 14:35:11.130358 backports.tarfile-1.0.0/docs/
--rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-04-06 14:34:55.000000 backports.tarfile-1.0.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-06 14:34:55.000000 backports.tarfile-1.0.0/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-06 14:34:55.000000 backports.tarfile-1.0.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-06 14:34:55.000000 backports.tarfile-1.0.0/mypy.ini
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-06 14:34:55.000000 backports.tarfile-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-06 14:34:55.000000 backports.tarfile-1.0.0/pytest.ini
--rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-06 14:34:55.000000 backports.tarfile-1.0.0/ruff.toml
--rw-r--r--   0 runner    (1001) docker     (127)      795 2024-04-06 14:35:11.134358 backports.tarfile-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-06 14:34:55.000000 backports.tarfile-1.0.0/towncrier.toml
--rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-04-06 14:34:55.000000 backports.tarfile-1.0.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:32:03.292290 backports_tarfile-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (127)      222 2024-04-16 11:31:46.000000 backports_tarfile-1.1.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-16 11:31:46.000000 backports_tarfile-1.1.0/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:32:03.284290 backports_tarfile-1.1.0/.github/
+-rw-r--r--   0 runner    (1001) docker     (127)      148 2024-04-16 11:31:46.000000 backports_tarfile-1.1.0/.github/dependabot.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:32:03.284290 backports_tarfile-1.1.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     2918 2024-04-16 11:31:46.000000 backports_tarfile-1.1.0/.github/workflows/main.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      116 2024-04-16 11:31:46.000000 backports_tarfile-1.1.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)      335 2024-04-16 11:31:46.000000 backports_tarfile-1.1.0/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1023 2024-04-16 11:31:46.000000 backports_tarfile-1.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      239 2024-04-16 11:31:46.000000 backports_tarfile-1.1.0/NEWS.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-04-16 11:32:03.292290 backports_tarfile-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      861 2024-04-16 11:31:46.000000 backports_tarfile-1.1.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:32:03.280290 backports_tarfile-1.1.0/backports/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:32:03.284290 backports_tarfile-1.1.0/backports/tarfile/
+-rwxr-xr-x   0 runner    (1001) docker     (127)   106960 2024-04-16 11:31:46.000000 backports_tarfile-1.1.0/backports/tarfile/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-16 11:31:46.000000 backports_tarfile-1.1.0/backports/tarfile/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:32:03.288290 backports_tarfile-1.1.0/backports/tarfile/compat/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 11:31:46.000000 backports_tarfile-1.1.0/backports/tarfile/compat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      568 2024-04-16 11:31:46.000000 backports_tarfile-1.1.0/backports/tarfile/compat/py38.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:32:03.292290 backports_tarfile-1.1.0/backports.tarfile.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1908 2024-04-16 11:32:03.000000 backports_tarfile-1.1.0/backports.tarfile.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      965 2024-04-16 11:32:03.000000 backports_tarfile-1.1.0/backports.tarfile.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 11:32:03.000000 backports_tarfile-1.1.0/backports.tarfile.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-16 11:32:03.000000 backports_tarfile-1.1.0/backports.tarfile.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-16 11:32:03.000000 backports_tarfile-1.1.0/backports.tarfile.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      770 2024-04-16 11:31:46.000000 backports_tarfile-1.1.0/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:32:03.288290 backports_tarfile-1.1.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1252 2024-04-16 11:31:46.000000 backports_tarfile-1.1.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-16 11:31:46.000000 backports_tarfile-1.1.0/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      341 2024-04-16 11:31:46.000000 backports_tarfile-1.1.0/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-16 11:31:46.000000 backports_tarfile-1.1.0/mypy.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-16 11:31:46.000000 backports_tarfile-1.1.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      584 2024-04-16 11:31:46.000000 backports_tarfile-1.1.0/pytest.ini
+-rw-r--r--   0 runner    (1001) docker     (127)      419 2024-04-16 11:31:46.000000 backports_tarfile-1.1.0/ruff.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      810 2024-04-16 11:32:03.292290 backports_tarfile-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:32:03.288290 backports_tarfile-1.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 11:31:46.000000 backports_tarfile-1.1.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:32:03.288290 backports_tarfile-1.1.0/tests/compat/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 11:31:46.000000 backports_tarfile-1.1.0/tests/compat/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6243 2024-04-16 11:31:46.000000 backports_tarfile-1.1.0/tests/compat/archiver_tests.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1169 2024-04-16 11:31:46.000000 backports_tarfile-1.1.0/tests/compat/py310.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1997 2024-04-16 11:31:46.000000 backports_tarfile-1.1.0/tests/compat/py38.py
+-rw-r--r--   0 runner    (1001) docker     (127)      753 2024-04-16 11:31:46.000000 backports_tarfile-1.1.0/tests/compat/py39.py
+-rw-r--r--   0 runner    (1001) docker     (127)      516 2024-04-16 11:31:46.000000 backports_tarfile-1.1.0/tests/recursion.tar
+-rw-r--r--   0 runner    (1001) docker     (127)   162773 2024-04-16 11:31:46.000000 backports_tarfile-1.1.0/tests/test_tarfile.py
+-rw-r--r--   0 runner    (1001) docker     (127)   435200 2024-04-16 11:31:46.000000 backports_tarfile-1.1.0/tests/testtar.tar
+-rw-r--r--   0 runner    (1001) docker     (127)      172 2024-04-16 11:31:46.000000 backports_tarfile-1.1.0/tests/testtar.tar.xz
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 11:32:03.292290 backports_tarfile-1.1.0/tests/tokenizedata/
+-rw-r--r--   0 runner    (1001) docker     (127)      302 2024-04-16 11:31:46.000000 backports_tarfile-1.1.0/tests/tokenizedata/tokenize_tests-no-coding-cookie-and-utf8-bom-sig-only.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     2717 2024-04-16 11:31:46.000000 backports_tarfile-1.1.0/tests/tokenizedata/tokenize_tests.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      374 2024-04-16 11:31:46.000000 backports_tarfile-1.1.0/tests/zipdir.zip
+-rw-r--r--   0 runner    (1001) docker     (127)       44 2024-04-16 11:31:46.000000 backports_tarfile-1.1.0/towncrier.toml
+-rw-r--r--   0 runner    (1001) docker     (127)     1364 2024-04-16 11:31:46.000000 backports_tarfile-1.1.0/tox.ini
```

### Comparing `backports.tarfile-1.0.0/.github/workflows/main.yml` & `backports_tarfile-1.1.0/.github/workflows/main.yml`

 * *Files 5% similar despite different names*

```diff
@@ -27,14 +27,15 @@
   TOX_OVERRIDE: >-
     testenv.pass_env+=GITHUB_*,FORCE_COLOR
 
 
 jobs:
   test:
     strategy:
+      # https://blog.jaraco.com/efficient-use-of-ci-resources/
       matrix:
         python:
         - "3.8"
         - "3.12"
         platform:
         - ubuntu-latest
         - macos-latest
```

### Comparing `backports.tarfile-1.0.0/LICENSE` & `backports_tarfile-1.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `backports.tarfile-1.0.0/PKG-INFO` & `backports_tarfile-1.1.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backports.tarfile
-Version: 1.0.0
+Version: 1.1.0
 Summary: Backport of CPython tarfile module
 Home-page: https://github.com/jaraco/backports.tarfile
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -13,14 +13,15 @@
 Requires-Python: >=3.8
 License-File: LICENSE
 Provides-Extra: testing
 Requires-Dist: pytest!=8.1.1,>=6; extra == "testing"
 Requires-Dist: pytest-checkdocs>=2.4; extra == "testing"
 Requires-Dist: pytest-cov; extra == "testing"
 Requires-Dist: pytest-enabler>=2.2; extra == "testing"
+Requires-Dist: jaraco.test; extra == "testing"
 Provides-Extra: docs
 Requires-Dist: sphinx>=3.5; extra == "docs"
 Requires-Dist: jaraco.packaging>=9.3; extra == "docs"
 Requires-Dist: rst.linker>=1.9; extra == "docs"
 Requires-Dist: furo; extra == "docs"
 Requires-Dist: sphinx-lint; extra == "docs"
```

### Comparing `backports.tarfile-1.0.0/README.rst` & `backports_tarfile-1.1.0/README.rst`

 * *Files identical despite different names*

### Comparing `backports.tarfile-1.0.0/backports/tarfile.py` & `backports_tarfile-1.1.0/backports/tarfile/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -44,14 +44,16 @@
 import stat
 import time
 import struct
 import copy
 import re
 import warnings
 
+from .compat.py38 import removesuffix
+
 try:
     import pwd
 except ImportError:
     pwd = None
 try:
     import grp
 except ImportError:
@@ -1361,15 +1363,15 @@
             next.name = nts(buf, tarfile.encoding, tarfile.errors)
         elif self.type == GNUTYPE_LONGLINK:
             next.linkname = nts(buf, tarfile.encoding, tarfile.errors)
 
         # Remove redundant slashes from directories. This is to be consistent
         # with frombuf().
         if next.isdir():
-            next.name = next.name.removesuffix("/")
+            next.name = removesuffix(next.name, "/")
 
         return next
 
     def _proc_sparse(self, tarfile):
         """Process a GNU sparse header plus extra headers.
         """
         # We already collected some sparse structures in frombuf().
```

### Comparing `backports.tarfile-1.0.0/backports.tarfile.egg-info/PKG-INFO` & `backports_tarfile-1.1.0/backports.tarfile.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backports.tarfile
-Version: 1.0.0
+Version: 1.1.0
 Summary: Backport of CPython tarfile module
 Home-page: https://github.com/jaraco/backports.tarfile
 Author: Jason R. Coombs
 Author-email: jaraco@jaraco.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
@@ -13,14 +13,15 @@
 Requires-Python: >=3.8
 License-File: LICENSE
 Provides-Extra: testing
 Requires-Dist: pytest!=8.1.1,>=6; extra == "testing"
 Requires-Dist: pytest-checkdocs>=2.4; extra == "testing"
 Requires-Dist: pytest-cov; extra == "testing"
 Requires-Dist: pytest-enabler>=2.2; extra == "testing"
+Requires-Dist: jaraco.test; extra == "testing"
 Provides-Extra: docs
 Requires-Dist: sphinx>=3.5; extra == "docs"
 Requires-Dist: jaraco.packaging>=9.3; extra == "docs"
 Requires-Dist: rst.linker>=1.9; extra == "docs"
 Requires-Dist: furo; extra == "docs"
 Requires-Dist: sphinx-lint; extra == "docs"
```

### Comparing `backports.tarfile-1.0.0/docs/conf.py` & `backports_tarfile-1.1.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `backports.tarfile-1.0.0/pytest.ini` & `backports_tarfile-1.1.0/pytest.ini`

 * *Files identical despite different names*

### Comparing `backports.tarfile-1.0.0/setup.cfg` & `backports_tarfile-1.1.0/setup.cfg`

 * *Files 22% similar despite different names*

```diff
@@ -19,14 +19,16 @@
 
 [options.extras_require]
 testing = 
 	pytest >= 6, != 8.1.1
 	pytest-checkdocs >= 2.4
 	pytest-cov
 	pytest-enabler >= 2.2
+	
+	jaraco.test
 docs = 
 	sphinx >= 3.5
 	jaraco.packaging >= 9.3
 	rst.linker >= 1.9
 	furo
 	sphinx-lint
```

### Comparing `backports.tarfile-1.0.0/tox.ini` & `backports_tarfile-1.1.0/tox.ini`

 * *Files identical despite different names*

