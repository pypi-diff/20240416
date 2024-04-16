# Comparing `tmp/corebridge-0.0.3.tar.gz` & `tmp/corebridge-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "corebridge-0.0.3.tar", last modified: Sat Oct 28 15:46:36 2023, max compression
+gzip compressed data, was "corebridge-0.0.5.tar", last modified: Tue Apr 16 10:11:52 2024, max compression
```

## Comparing `corebridge-0.0.3.tar` & `corebridge-0.0.5.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 fenke     (1000) users      (100)        0 2023-10-28 15:46:36.913644 corebridge-0.0.3/
--rw-rw-r--   0 fenke     (1000) users      (100)    11337 2023-04-27 10:12:58.000000 corebridge-0.0.3/LICENSE
--rw-rw-r--   0 fenke     (1000) users      (100)      111 2023-04-27 10:12:58.000000 corebridge-0.0.3/MANIFEST.in
--rw-r--r--   0 fenke     (1000) users      (100)     1055 2023-10-28 15:46:36.913644 corebridge-0.0.3/PKG-INFO
--rw-r--r--   0 fenke     (1000) users      (100)      290 2023-10-23 13:12:00.000000 corebridge-0.0.3/README.md
-drwxr-xr-x   0 fenke     (1000) users      (100)        0 2023-10-28 15:46:36.909644 corebridge-0.0.3/corebridge/
--rw-r--r--   0 fenke     (1000) users      (100)       22 2023-10-28 15:43:30.000000 corebridge-0.0.3/corebridge/__init__.py
--rw-r--r--   0 fenke     (1000) users      (100)      501 2023-10-28 15:43:30.000000 corebridge-0.0.3/corebridge/_modidx.py
--rw-r--r--   0 fenke     (1000) users      (100)      158 2023-10-28 15:43:30.000000 corebridge-0.0.3/corebridge/aicorebridge.py
--rw-r--r--   0 fenke     (1000) users      (100)      142 2023-10-23 13:11:48.000000 corebridge-0.0.3/corebridge/core.py
-drwxr-xr-x   0 fenke     (1000) users      (100)        0 2023-10-28 15:46:36.913644 corebridge-0.0.3/corebridge.egg-info/
--rw-r--r--   0 fenke     (1000) users      (100)     1055 2023-10-28 15:46:36.000000 corebridge-0.0.3/corebridge.egg-info/PKG-INFO
--rw-r--r--   0 fenke     (1000) users      (100)      381 2023-10-28 15:46:36.000000 corebridge-0.0.3/corebridge.egg-info/SOURCES.txt
--rw-r--r--   0 fenke     (1000) users      (100)        1 2023-10-28 15:46:36.000000 corebridge-0.0.3/corebridge.egg-info/dependency_links.txt
--rw-r--r--   0 fenke     (1000) users      (100)       42 2023-10-28 15:46:36.000000 corebridge-0.0.3/corebridge.egg-info/entry_points.txt
--rw-r--r--   0 fenke     (1000) users      (100)        1 2023-10-23 09:37:02.000000 corebridge-0.0.3/corebridge.egg-info/not-zip-safe
--rw-r--r--   0 fenke     (1000) users      (100)      207 2023-10-28 15:46:36.000000 corebridge-0.0.3/corebridge.egg-info/requires.txt
--rw-r--r--   0 fenke     (1000) users      (100)       11 2023-10-28 15:46:36.000000 corebridge-0.0.3/corebridge.egg-info/top_level.txt
--rw-r--r--   0 fenke     (1000) users      (100)     1125 2023-10-28 15:46:30.000000 corebridge-0.0.3/settings.ini
--rw-r--r--   0 fenke     (1000) users      (100)       38 2023-10-28 15:46:36.913644 corebridge-0.0.3/setup.cfg
--rw-rw-r--   0 fenke     (1000) users      (100)     2596 2023-04-27 10:12:58.000000 corebridge-0.0.3/setup.py
+drwxr-xr-x   0 fenke     (1000) users      (100)        0 2024-04-16 10:11:52.768525 corebridge-0.0.5/
+-rw-r--r--   0 fenke     (1000) users      (100)    11337 2024-01-31 12:54:47.000000 corebridge-0.0.5/LICENSE
+-rw-r--r--   0 fenke     (1000) users      (100)      111 2024-01-31 12:54:47.000000 corebridge-0.0.5/MANIFEST.in
+-rw-r--r--   0 fenke     (1000) users      (100)     1203 2024-04-16 10:11:52.768525 corebridge-0.0.5/PKG-INFO
+-rw-r--r--   0 fenke     (1000) users      (100)      435 2024-04-16 10:09:45.000000 corebridge-0.0.5/README.md
+drwxr-xr-x   0 fenke     (1000) users      (100)        0 2024-04-16 10:11:52.768525 corebridge-0.0.5/corebridge/
+-rw-r--r--   0 fenke     (1000) users      (100)       22 2024-04-16 10:09:53.000000 corebridge-0.0.5/corebridge/__init__.py
+-rw-r--r--   0 fenke     (1000) users      (100)     3024 2024-04-16 10:09:53.000000 corebridge-0.0.5/corebridge/_modidx.py
+-rw-r--r--   0 fenke     (1000) users      (100)     7767 2024-04-16 10:09:53.000000 corebridge-0.0.5/corebridge/aicorebridge.py
+-rw-r--r--   0 fenke     (1000) users      (100)     3766 2024-04-16 10:09:53.000000 corebridge-0.0.5/corebridge/core.py
+drwxr-xr-x   0 fenke     (1000) users      (100)        0 2024-04-16 10:11:52.768525 corebridge-0.0.5/corebridge.egg-info/
+-rw-r--r--   0 fenke     (1000) users      (100)     1203 2024-04-16 10:11:52.000000 corebridge-0.0.5/corebridge.egg-info/PKG-INFO
+-rw-r--r--   0 fenke     (1000) users      (100)      381 2024-04-16 10:11:52.000000 corebridge-0.0.5/corebridge.egg-info/SOURCES.txt
+-rw-r--r--   0 fenke     (1000) users      (100)        1 2024-04-16 10:11:52.000000 corebridge-0.0.5/corebridge.egg-info/dependency_links.txt
+-rw-r--r--   0 fenke     (1000) users      (100)       42 2024-04-16 10:11:52.000000 corebridge-0.0.5/corebridge.egg-info/entry_points.txt
+-rw-r--r--   0 fenke     (1000) users      (100)        1 2024-01-31 15:42:47.000000 corebridge-0.0.5/corebridge.egg-info/not-zip-safe
+-rw-r--r--   0 fenke     (1000) users      (100)      225 2024-04-16 10:11:52.000000 corebridge-0.0.5/corebridge.egg-info/requires.txt
+-rw-r--r--   0 fenke     (1000) users      (100)       11 2024-04-16 10:11:52.000000 corebridge-0.0.5/corebridge.egg-info/top_level.txt
+-rw-r--r--   0 fenke     (1000) users      (100)     1146 2024-01-31 15:48:02.000000 corebridge-0.0.5/settings.ini
+-rw-r--r--   0 fenke     (1000) users      (100)       38 2024-04-16 10:11:52.768525 corebridge-0.0.5/setup.cfg
+-rw-r--r--   0 fenke     (1000) users      (100)     2596 2024-01-31 12:54:47.000000 corebridge-0.0.5/setup.py
```

### Comparing `corebridge-0.0.3/LICENSE` & `corebridge-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `corebridge-0.0.3/PKG-INFO` & `corebridge-0.0.5/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: corebridge
-Version: 0.0.3
+Version: 0.0.5
 Summary: Bridge for Stactics AICore
 Home-page: https://github.com/fenke/corebridge
 Author: Fenke Meijer
-Author-email: nobody@example.com
+Author-email: fenkemeijer@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -18,14 +18,15 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # corebridge
 
+
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
 
 This file will become your README and also the index of your
 documentation.
 
 ## Install
 
@@ -38,7 +39,19 @@
 Fill me in please! Don’t forget code examples:
 
 ``` python
 1+1
 ```
 
     2
+
+## nbdev cycle
+
+- edit
+- nbdev_export
+- pip install -e ‘.\[dev\]’
+- nbdev_test
+- nbdev_clean
+- nbdev_readme
+- nbdev_prepare
+- git add .
+-
```

### Comparing `corebridge-0.0.3/corebridge.egg-info/PKG-INFO` & `corebridge-0.0.5/corebridge.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: corebridge
-Version: 0.0.3
+Version: 0.0.5
 Summary: Bridge for Stactics AICore
 Home-page: https://github.com/fenke/corebridge
 Author: Fenke Meijer
-Author-email: nobody@example.com
+Author-email: fenkemeijer@gmail.com
 License: Apache Software License 2.0
 Keywords: nbdev jupyter notebook python
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -18,14 +18,15 @@
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 License-File: LICENSE
 
 # corebridge
 
+
 <!-- WARNING: THIS FILE WAS AUTOGENERATED! DO NOT EDIT! -->
 
 This file will become your README and also the index of your
 documentation.
 
 ## Install
 
@@ -38,7 +39,19 @@
 Fill me in please! Don’t forget code examples:
 
 ``` python
 1+1
 ```
 
     2
+
+## nbdev cycle
+
+- edit
+- nbdev_export
+- pip install -e ‘.\[dev\]’
+- nbdev_test
+- nbdev_clean
+- nbdev_readme
+- nbdev_prepare
+- git add .
+-
```

### Comparing `corebridge-0.0.3/settings.ini` & `corebridge-0.0.5/settings.ini`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [DEFAULT]
 # All sections below are required unless otherwise specified.
 # See https://github.com/fastai/nbdev/blob/master/settings.ini for examples.
 
 ### Python library ###
 repo = corebridge
 lib_name = %(repo)s
-version = 0.0.3
+version = 0.0.5
 min_python = 3.7
 license = apache2
 black_formatting = False
 
 ### nbdev ###
 doc_path = _docs
 lib_path = corebridge
@@ -25,19 +25,19 @@
 doc_baseurl = /%(repo)s
 git_url = https://github.com/%(user)s/%(repo)s
 title = %(lib_name)s
 
 ### PyPI ###
 audience = Developers
 author = Fenke Meijer
-author_email = nobody@example.com
+author_email = fenkemeijer@gmail.com
 copyright = 2023 onwards, %(author)s
 description = Bridge for Stactics AICore
 keywords = nbdev jupyter notebook python
 language = English
 status = 3
 user = fenke
 
 ### Optional ###
-requirements = python-dateutil pytz numpy pandas scipy scikit-learn
-dev_requirements = python-dateutil pytz numpy pandas scipy scikit-learn jupyter ipywidgets jupyterlab>4 jupyter_contrib_nbextensions jupyterlab-git jupyterlab-quarto
+requirements = python-dateutil pytz numpy pandas scipy scikit-learn fastcore
+dev_requirements = python-dateutil pytz numpy pandas scipy scikit-learn fastcore jupyter ipywidgets jupyterlab>4 jupyter_contrib_nbextensions jupyterlab-git jupyterlab-quarto
 # console_scripts =
```

### Comparing `corebridge-0.0.3/setup.py` & `corebridge-0.0.5/setup.py`

 * *Files identical despite different names*

