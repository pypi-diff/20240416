# Comparing `tmp/plone.releaser-2.2.1.tar.gz` & `tmp/plone.releaser-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone.releaser-2.2.1.tar", last modified: Thu Dec 14 10:10:48 2023, max compression
+gzip compressed data, was "plone.releaser-2.2.2.tar", last modified: Tue Apr 16 19:35:35 2024, max compression
```

## Comparing `plone.releaser-2.2.1.tar` & `plone.releaser-2.2.2.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-12-14 10:10:48.120859 plone.releaser-2.2.1/
--rw-r--r--   0 maurits    (501) staff       (20)     3287 2023-12-14 10:10:47.000000 plone.releaser-2.2.1/ADD-A-NEWS-ITEM.rst
--rw-r--r--   0 maurits    (501) staff       (20)     8133 2023-12-14 10:10:47.000000 plone.releaser-2.2.1/CHANGES.rst
--rw-r--r--   0 maurits    (501) staff       (20)       70 2023-12-14 10:10:47.000000 plone.releaser-2.2.1/CONTRIBUTING.rst
--rw-r--r--   0 maurits    (501) staff       (20)      142 2023-12-14 10:10:47.000000 plone.releaser-2.2.1/MANIFEST.in
--rw-r--r--   0 maurits    (501) staff       (20)     9862 2023-12-14 10:10:48.120437 plone.releaser-2.2.1/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)      713 2023-12-14 10:10:47.000000 plone.releaser-2.2.1/README.rst
--rw-r--r--   0 maurits    (501) staff       (20)      108 2023-12-14 10:10:47.000000 plone.releaser-2.2.1/buildout.cfg
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-12-14 10:10:48.107680 plone.releaser-2.2.1/plone/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2023-12-14 10:10:47.000000 plone.releaser-2.2.1/plone/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-12-14 10:10:48.113742 plone.releaser-2.2.1/plone/releaser/
--rw-r--r--   0 maurits    (501) staff       (20)      940 2023-12-14 10:10:47.000000 plone.releaser-2.2.1/plone/releaser/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     1276 2023-12-14 10:10:47.000000 plone.releaser-2.2.1/plone/releaser/base.py
--rw-r--r--   0 maurits    (501) staff       (20)    17801 2023-12-14 10:10:47.000000 plone.releaser-2.2.1/plone/releaser/buildout.py
--rw-r--r--   0 maurits    (501) staff       (20)    11798 2023-12-14 10:10:47.000000 plone.releaser-2.2.1/plone/releaser/changelog.py
--rw-r--r--   0 maurits    (501) staff       (20)      772 2023-12-14 10:10:47.000000 plone.releaser-2.2.1/plone/releaser/db.py
--rw-r--r--   0 maurits    (501) staff       (20)    11110 2023-12-14 10:10:47.000000 plone.releaser-2.2.1/plone/releaser/manage.py
--rw-r--r--   0 maurits    (501) staff       (20)    10899 2023-12-14 10:10:47.000000 plone.releaser-2.2.1/plone/releaser/package.py
--rw-r--r--   0 maurits    (501) staff       (20)    10721 2023-12-14 10:10:47.000000 plone.releaser-2.2.1/plone/releaser/pip.py
--rw-r--r--   0 maurits    (501) staff       (20)      701 2023-12-14 10:10:47.000000 plone.releaser-2.2.1/plone/releaser/pypi.py
--rw-r--r--   0 maurits    (501) staff       (20)    10440 2023-12-14 10:10:47.000000 plone.releaser-2.2.1/plone/releaser/release.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-12-14 10:10:48.115492 plone.releaser-2.2.1/plone/releaser/tests/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-12-14 10:10:47.000000 plone.releaser-2.2.1/plone/releaser/tests/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-12-14 10:10:48.119411 plone.releaser-2.2.1/plone/releaser/tests/input/
--rw-r--r--   0 maurits    (501) staff       (20)      465 2023-12-14 10:10:47.000000 plone.releaser-2.2.1/plone/releaser/tests/input/changes.md
--rw-r--r--   0 maurits    (501) staff       (20)      975 2023-12-14 10:10:47.000000 plone.releaser-2.2.1/plone/releaser/tests/input/changes.rst
--rw-r--r--   0 maurits    (501) staff       (20)      145 2023-12-14 10:10:47.000000 plone.releaser-2.2.1/plone/releaser/tests/input/checkouts.cfg
--rw-r--r--   0 maurits    (501) staff       (20)      313 2023-12-14 10:10:47.000000 plone.releaser-2.2.1/plone/releaser/tests/input/constraints.txt
--rw-r--r--   0 maurits    (501) staff       (20)       73 2023-12-14 10:10:47.000000 plone.releaser-2.2.1/plone/releaser/tests/input/constraints2.txt
--rw-r--r--   0 maurits    (501) staff       (20)       75 2023-12-14 10:10:47.000000 plone.releaser-2.2.1/plone/releaser/tests/input/constraints3.txt
--rw-r--r--   0 maurits    (501) staff       (20)       49 2023-12-14 10:10:47.000000 plone.releaser-2.2.1/plone/releaser/tests/input/constraints4.txt
--rw-r--r--   0 maurits    (501) staff       (20)      460 2023-12-14 10:10:47.000000 plone.releaser-2.2.1/plone/releaser/tests/input/mxdev.ini
--rw-r--r--   0 maurits    (501) staff       (20)      774 2023-12-14 10:10:47.000000 plone.releaser-2.2.1/plone/releaser/tests/input/sources.cfg
--rw-r--r--   0 maurits    (501) staff       (20)      408 2023-12-14 10:10:47.000000 plone.releaser-2.2.1/plone/releaser/tests/input/versions.cfg
--rw-r--r--   0 maurits    (501) staff       (20)      101 2023-12-14 10:10:47.000000 plone.releaser-2.2.1/plone/releaser/tests/input/versions2.cfg
--rw-r--r--   0 maurits    (501) staff       (20)      107 2023-12-14 10:10:47.000000 plone.releaser-2.2.1/plone/releaser/tests/input/versions3.cfg
--rw-r--r--   0 maurits    (501) staff       (20)       52 2023-12-14 10:10:47.000000 plone.releaser-2.2.1/plone/releaser/tests/input/versions4.cfg
--rw-r--r--   0 maurits    (501) staff       (20)    18352 2023-12-14 10:10:47.000000 plone.releaser-2.2.1/plone/releaser/tests/test_buildout.py
--rw-r--r--   0 maurits    (501) staff       (20)     1900 2023-12-14 10:10:47.000000 plone.releaser-2.2.1/plone/releaser/tests/test_changelog.py
--rw-r--r--   0 maurits    (501) staff       (20)    12777 2023-12-14 10:10:47.000000 plone.releaser-2.2.1/plone/releaser/tests/test_pip.py
--rw-r--r--   0 maurits    (501) staff       (20)     3008 2023-12-14 10:10:47.000000 plone.releaser-2.2.1/plone/releaser/tests/test_utils.py
--rw-r--r--   0 maurits    (501) staff       (20)     1137 2023-12-14 10:10:47.000000 plone.releaser-2.2.1/plone/releaser/tests/test_versions2constraints.py
--rw-r--r--   0 maurits    (501) staff       (20)     4812 2023-12-14 10:10:47.000000 plone.releaser-2.2.1/plone/releaser/utils.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-12-14 10:10:48.119871 plone.releaser-2.2.1/plone.releaser.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)     9862 2023-12-14 10:10:47.000000 plone.releaser-2.2.1/plone.releaser.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     1472 2023-12-14 10:10:48.000000 plone.releaser-2.2.1/plone.releaser.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-12-14 10:10:48.000000 plone.releaser-2.2.1/plone.releaser.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)      706 2023-12-14 10:10:48.000000 plone.releaser-2.2.1/plone.releaser.egg-info/entry_points.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2023-12-14 10:10:48.000000 plone.releaser-2.2.1/plone.releaser.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-12-14 10:10:47.000000 plone.releaser-2.2.1/plone.releaser.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)      143 2023-12-14 10:10:48.000000 plone.releaser-2.2.1/plone.releaser.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2023-12-14 10:10:48.000000 plone.releaser-2.2.1/plone.releaser.egg-info/top_level.txt
--rw-r--r--   0 maurits    (501) staff       (20)     4271 2023-12-14 10:10:47.000000 plone.releaser-2.2.1/pyproject.toml
--rw-r--r--   0 maurits    (501) staff       (20)       38 2023-12-14 10:10:48.120930 plone.releaser-2.2.1/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)     2573 2023-12-14 10:10:47.000000 plone.releaser-2.2.1/setup.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-16 19:35:35.333778 plone.releaser-2.2.2/
+-rw-r--r--   0 maurits    (501) staff       (20)     3287 2024-04-16 19:35:34.000000 plone.releaser-2.2.2/ADD-A-NEWS-ITEM.rst
+-rw-r--r--   0 maurits    (501) staff       (20)     8279 2024-04-16 19:35:34.000000 plone.releaser-2.2.2/CHANGES.rst
+-rw-r--r--   0 maurits    (501) staff       (20)       70 2024-04-16 19:35:34.000000 plone.releaser-2.2.2/CONTRIBUTING.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      142 2024-04-16 19:35:34.000000 plone.releaser-2.2.2/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)    10008 2024-04-16 19:35:35.333222 plone.releaser-2.2.2/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)      713 2024-04-16 19:35:34.000000 plone.releaser-2.2.2/README.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      108 2024-04-16 19:35:34.000000 plone.releaser-2.2.2/buildout.cfg
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-16 19:35:35.319175 plone.releaser-2.2.2/plone/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2024-04-16 19:35:34.000000 plone.releaser-2.2.2/plone/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-16 19:35:35.325382 plone.releaser-2.2.2/plone/releaser/
+-rw-r--r--   0 maurits    (501) staff       (20)      940 2024-04-16 19:35:34.000000 plone.releaser-2.2.2/plone/releaser/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1752 2024-04-16 19:35:34.000000 plone.releaser-2.2.2/plone/releaser/base.py
+-rw-r--r--   0 maurits    (501) staff       (20)    17582 2024-04-16 19:35:34.000000 plone.releaser-2.2.2/plone/releaser/buildout.py
+-rw-r--r--   0 maurits    (501) staff       (20)    11798 2024-04-16 19:35:34.000000 plone.releaser-2.2.2/plone/releaser/changelog.py
+-rw-r--r--   0 maurits    (501) staff       (20)      772 2024-04-16 19:35:34.000000 plone.releaser-2.2.2/plone/releaser/db.py
+-rw-r--r--   0 maurits    (501) staff       (20)    11110 2024-04-16 19:35:34.000000 plone.releaser-2.2.2/plone/releaser/manage.py
+-rw-r--r--   0 maurits    (501) staff       (20)    10899 2024-04-16 19:35:34.000000 plone.releaser-2.2.2/plone/releaser/package.py
+-rw-r--r--   0 maurits    (501) staff       (20)    10703 2024-04-16 19:35:34.000000 plone.releaser-2.2.2/plone/releaser/pip.py
+-rw-r--r--   0 maurits    (501) staff       (20)      701 2024-04-16 19:35:34.000000 plone.releaser-2.2.2/plone/releaser/pypi.py
+-rw-r--r--   0 maurits    (501) staff       (20)    10440 2024-04-16 19:35:34.000000 plone.releaser-2.2.2/plone/releaser/release.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-16 19:35:35.327498 plone.releaser-2.2.2/plone/releaser/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2024-04-16 19:35:34.000000 plone.releaser-2.2.2/plone/releaser/tests/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-16 19:35:35.332051 plone.releaser-2.2.2/plone/releaser/tests/input/
+-rw-r--r--   0 maurits    (501) staff       (20)      465 2024-04-16 19:35:34.000000 plone.releaser-2.2.2/plone/releaser/tests/input/changes.md
+-rw-r--r--   0 maurits    (501) staff       (20)      975 2024-04-16 19:35:34.000000 plone.releaser-2.2.2/plone/releaser/tests/input/changes.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      145 2024-04-16 19:35:34.000000 plone.releaser-2.2.2/plone/releaser/tests/input/checkouts.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)      313 2024-04-16 19:35:34.000000 plone.releaser-2.2.2/plone/releaser/tests/input/constraints.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       73 2024-04-16 19:35:34.000000 plone.releaser-2.2.2/plone/releaser/tests/input/constraints2.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       75 2024-04-16 19:35:34.000000 plone.releaser-2.2.2/plone/releaser/tests/input/constraints3.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       49 2024-04-16 19:35:34.000000 plone.releaser-2.2.2/plone/releaser/tests/input/constraints4.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      460 2024-04-16 19:35:34.000000 plone.releaser-2.2.2/plone/releaser/tests/input/mxdev.ini
+-rw-r--r--   0 maurits    (501) staff       (20)      774 2024-04-16 19:35:34.000000 plone.releaser-2.2.2/plone/releaser/tests/input/sources.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)      408 2024-04-16 19:35:34.000000 plone.releaser-2.2.2/plone/releaser/tests/input/versions.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)      101 2024-04-16 19:35:34.000000 plone.releaser-2.2.2/plone/releaser/tests/input/versions2.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)      107 2024-04-16 19:35:34.000000 plone.releaser-2.2.2/plone/releaser/tests/input/versions3.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)       52 2024-04-16 19:35:34.000000 plone.releaser-2.2.2/plone/releaser/tests/input/versions4.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)    18176 2024-04-16 19:35:34.000000 plone.releaser-2.2.2/plone/releaser/tests/test_buildout.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1900 2024-04-16 19:35:34.000000 plone.releaser-2.2.2/plone/releaser/tests/test_changelog.py
+-rw-r--r--   0 maurits    (501) staff       (20)    12684 2024-04-16 19:35:34.000000 plone.releaser-2.2.2/plone/releaser/tests/test_pip.py
+-rw-r--r--   0 maurits    (501) staff       (20)     3008 2024-04-16 19:35:34.000000 plone.releaser-2.2.2/plone/releaser/tests/test_utils.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1137 2024-04-16 19:35:34.000000 plone.releaser-2.2.2/plone/releaser/tests/test_versions2constraints.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4812 2024-04-16 19:35:34.000000 plone.releaser-2.2.2/plone/releaser/utils.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-16 19:35:35.332482 plone.releaser-2.2.2/plone.releaser.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)    10008 2024-04-16 19:35:35.000000 plone.releaser-2.2.2/plone.releaser.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     1472 2024-04-16 19:35:35.000000 plone.releaser-2.2.2/plone.releaser.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2024-04-16 19:35:35.000000 plone.releaser-2.2.2/plone.releaser.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)      706 2024-04-16 19:35:35.000000 plone.releaser-2.2.2/plone.releaser.egg-info/entry_points.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2024-04-16 19:35:35.000000 plone.releaser-2.2.2/plone.releaser.egg-info/namespace_packages.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2024-04-16 19:35:35.000000 plone.releaser-2.2.2/plone.releaser.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)      143 2024-04-16 19:35:35.000000 plone.releaser-2.2.2/plone.releaser.egg-info/requires.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2024-04-16 19:35:35.000000 plone.releaser-2.2.2/plone.releaser.egg-info/top_level.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     4271 2024-04-16 19:35:34.000000 plone.releaser-2.2.2/pyproject.toml
+-rw-r--r--   0 maurits    (501) staff       (20)       38 2024-04-16 19:35:35.333866 plone.releaser-2.2.2/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)     2573 2024-04-16 19:35:34.000000 plone.releaser-2.2.2/setup.py
```

### Comparing `plone.releaser-2.2.1/ADD-A-NEWS-ITEM.rst` & `plone.releaser-2.2.2/ADD-A-NEWS-ITEM.rst`

 * *Files identical despite different names*

### Comparing `plone.releaser-2.2.1/CHANGES.rst` & `plone.releaser-2.2.2/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,24 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+2.2.2 (2024-04-16)
+------------------
+
+Bug fixes:
+
+
+- Preserve the case of package names in versions2constraints and friends.
+  [maurits] (#65)
+
+
 2.2.1 (2023-12-14)
 ------------------
 
 Bug fixes:
 
 
 - Manage changelog: read markdown files as well.
```

### Comparing `plone.releaser-2.2.1/PKG-INFO` & `plone.releaser-2.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.releaser
-Version: 2.2.1
+Version: 2.2.2
 Summary: Plone release management utilities
 Home-page: https://github.com/plone/plone.releaser
 Author: Eric Steele
 Author-email: eric@esteele.net
 License: GPL
 Keywords: plone release
 Classifier: Development Status :: 5 - Production/Stable
@@ -79,14 +79,24 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+2.2.2 (2024-04-16)
+------------------
+
+Bug fixes:
+
+
+- Preserve the case of package names in versions2constraints and friends.
+  [maurits] (#65)
+
+
 2.2.1 (2023-12-14)
 ------------------
 
 Bug fixes:
 
 
 - Manage changelog: read markdown files as well.
```

### Comparing `plone.releaser-2.2.1/README.rst` & `plone.releaser-2.2.2/README.rst`

 * *Files identical despite different names*

### Comparing `plone.releaser-2.2.1/plone/releaser/__init__.py` & `plone.releaser-2.2.2/plone/releaser/__init__.py`

 * *Files identical despite different names*

### Comparing `plone.releaser-2.2.1/plone/releaser/base.py` & `plone.releaser-2.2.2/plone/releaser/base.py`

 * *Files 13% similar despite different names*

```diff
@@ -8,24 +8,35 @@
         self.file_location = file_location
         self.path = pathlib.Path(self.file_location).resolve()
 
     @property
     def data(self):
         raise NotImplementedError
 
+    @property
+    def lowerkeys(self):
+        # Map from lower case key to actual key in the data.
+        return {key.lower(): key for key in self.data}
+
     def __iter__(self):
         return self.data.__iter__()
 
     def __contains__(self, package_name):
-        return package_name.lower() in self.data
+        return package_name.lower() in self.lowerkeys
 
     def __getitem__(self, package_name):
-        if package_name in self:
-            return self.data.get(package_name.lower())
-        raise KeyError
+        # self.data may be a defaultdict, so we cannot use
+        # 'return self.data[package_name]'
+        if package_name not in self:
+            raise KeyError(package_name)
+        # The package_name is in the data, but the case might differ.
+        if package_name in self.data:
+            return self.data[package_name]
+        actual_key = self.lowerkeys[package_name.lower()]
+        return self.data[actual_key]
 
     def __setitem__(self, package_name, value):
         raise NotImplementedError
 
     def __delitem__(self, package_name):
         return self.__setitem__(package_name, False)
```

### Comparing `plone.releaser-2.2.1/plone/releaser/buildout.py` & `plone.releaser-2.2.2/plone/releaser/buildout.py`

 * *Files 5% similar despite different names*

```diff
@@ -78,18 +78,16 @@
         self.read_extends = read_extends
 
     @cached_property
     def config(self):
         # For versions.cfg we had strict=False, for the others not.
         # Let's use it always.
         config = ConfigParser(interpolation=ExtendedInterpolation(), strict=False)
-        # In SourcesFile we had this:
-        # config.optionxform = str
-        # This seems to make everything lowercase, and makes tests fail.
-        # TODO: we could use it if we choose.
+        # Preserve the case instead of the default lowercase transform:
+        config.optionxform = str
         with self.path.open() as f:
             config.read_file(f)
         # Especially in sources.cfg we may need to define a few extra variables
         # that are in a different buildout file that we do not parse here.
         # See this similar issue in mr.roboto:
         # https://github.com/plone/mr.roboto/issues/89
         if not config.has_section("buildout"):
@@ -99,15 +97,16 @@
         return config
 
     @cached_property
     def raw_config(self):
         # Read the same data, but without interpolation.
         # So keep a url like '${settings:plone}/package.git'
         config = ConfigParser(strict=False)
-        # config.optionxform = str
+        # Preserve the case instead of the default lowercase transform:
+        config.optionxform = str
         with self.path.open() as f:
             config.read_file(f)
         return config
 
     @property
     def extends(self):
         if self.config.has_section("buildout"):
@@ -157,15 +156,15 @@
                             versions[package][""] = version
                         else:
                             versions[package].update(version)
 
         for section in self.config.sections():
             if section == "versions":
                 for package, version in self.config[section].items():
-                    # Note: the package names are lower case.
+                    # Note: the package names used to be lower case, but not anymore.
                     versions[package][""] = version
             if not self.with_markers:
                 continue
             parts = section.split(":")
             if len(parts) != 2 or parts[0] != "versions":
                 continue
             marker = parts[1]
@@ -294,15 +293,15 @@
         There is just one thing to do: translate buildout-specific markers
         to ones that pip understands.
         Note that the other way around is no problem: Buildout can meanwhile
         understand the pip markers.
 
         An option would be to always do this for Buildout as well.
         Or have a command to normalize a buildout file, with this and other
-        small changes like making all package named lower case.
+        small changes.
         """
         new_data = {}
         for package, version in self.data.items():
             if isinstance(version, str):
                 new_data[package] = version
                 continue
             # version is a dict
@@ -349,24 +348,24 @@
 class SourcesFile(BaseBuildoutFile):
     @property
     def data(self):
         sources_dict = OrderedDict()
         # I don't think we need to support [sources:marker].
         for name, value in self.config["sources"].items():
             source = Source.create_from_string(value)
-            sources_dict[name.lower()] = source
+            sources_dict[name] = source
         return sources_dict
 
     @property
     def raw_data(self):
         sources_dict = OrderedDict()
         # I don't think we need to support [sources:marker].
         for name, value in self.raw_config["sources"].items():
             source = Source.create_from_string(value)
-            sources_dict[name.lower()] = source
+            sources_dict[name] = source
         return sources_dict
 
     def __setitem__(self, package_name, value):
         raise NotImplementedError
 
     def rewrite(self):
         """Rewrite the file based on the parsed data.
@@ -403,20 +402,21 @@
     def always_checkout(self):
         return self.config.get("buildout", "always-checkout")
 
     @property
     def data(self):
         # I don't think we need to support [buildout:marker].
         checkouts = self.config.get("buildout", "auto-checkout")
-        # Map from lower case to actual case, so we can find the package.
+        # In this case a set or list would be fine, but in all other
+        # cases the data is a dictionary, so let's use that.
         mapping = {}
         for package in checkouts.splitlines():
             if not package:
                 continue
-            mapping[package.lower()] = package
+            mapping[package] = True
         return mapping
 
     def __setitem__(self, package_name, enabled=True):
         contents = self.path.read_text()
         if not contents.endswith("\n"):
             # Make sure the file ends with a newline.
             contents += "\n"
@@ -444,19 +444,15 @@
 
         This will lose comments, and may change the order.
         """
         contents = ["[buildout]"]
         if self.always_checkout:
             contents.append(f"always-checkout = {self.always_checkout}"),
         contents.append("auto-checkout =")
-        # self.values has the original case.
-        # We could iterate over 'self' to get lowercase,
-        # which is what we get in most other places.
-        # But for now let's use the info we have.
-        for package in self.values():
+        for package in self:
             contents.append(f"    {package}")
         contents.append("")
         new_contents = "\n".join(contents)
         self.path.write_text(new_contents)
 
 
 class Buildout:
```

### Comparing `plone.releaser-2.2.1/plone/releaser/changelog.py` & `plone.releaser-2.2.2/plone/releaser/changelog.py`

 * *Files identical despite different names*

### Comparing `plone.releaser-2.2.1/plone/releaser/db.py` & `plone.releaser-2.2.2/plone/releaser/db.py`

 * *Files identical despite different names*

### Comparing `plone.releaser-2.2.1/plone/releaser/manage.py` & `plone.releaser-2.2.2/plone/releaser/manage.py`

 * *Files identical despite different names*

### Comparing `plone.releaser-2.2.1/plone/releaser/package.py` & `plone.releaser-2.2.2/plone/releaser/package.py`

 * *Files identical despite different names*

### Comparing `plone.releaser-2.2.1/plone/releaser/pip.py` & `plone.releaser-2.2.2/plone/releaser/pip.py`

 * *Files 2% similar despite different names*

```diff
@@ -56,15 +56,15 @@
                             constraints[package][""] = version
                         else:
                             constraints[package].update(version)
                 continue
             if "==" not in line:
                 # We might want to support e.g. '>=', but for now keep it simple.
                 continue
-            package = line.split("==")[0].strip().lower()
+            package = line.split("==")[0].strip()
             version = line.split("==", 1)[1].strip()
             # The line could also contain environment markers like this:
             # "; python_version >= '3.0'"
             # But currently I think we really only need the package name,
             # and not even the version.  Let's use the entire rest of the line.
             # Actually, for our purposes, we should ignore lines that have such
             # markers, just like we do in buildout.py:VersionsFile.
@@ -161,27 +161,30 @@
 
     @property
     def data(self):
         checkouts = {}
         for package in self.config.sections():
             use = to_bool(self.config[package].get("use", self.default_use))
             if use:
-                # Map from lower case to actual case, so we can find the package.
-                checkouts[package.lower()] = package
+                checkouts[package] = True
         return checkouts
 
     @property
     def sections(self):
         # If we want to use a package, we must first know that it exists.
         sections = {}
         for package in self.config.sections():
-            # Map from lower case to actual case, so we can find the package.
-            sections[package.lower()] = package
+            sections[package] = True
         return sections
 
+    @property
+    def lowerkeys_section(self):
+        # Map from lower case key to actual key in the sections.
+        return {key.lower(): key for key in self.sections}
+
     def __setitem__(self, package_name, enabled=True):
         """Enable or disable a checkout.
 
         Mostly this will be called to disable a checkout.
         Expected is that default-use is false.
         This means we can remove 'use = true' from the package.
 
@@ -189,15 +192,15 @@
         when default-use is true, we set 'use = false'.
 
         Note that in our Buildout setup, we have sources.cfg separately.
         In mxdev.ini the source definition and 'use = false/true' is combined.
         So if the package we want to enable is not defined, meaning it has no
         section, then we should fail loudly.
         """
-        stored_package_name = self.sections.get(package_name.lower())
+        stored_package_name = self.lowerkeys_section.get(package_name.lower())
         if not stored_package_name:
             raise KeyError(
                 f"{self.file_location}: There is no definition for {package_name}"
             )
         package_name = stored_package_name
         if package_name in self:
             use = to_bool(self.config[package_name].get("use", self.default_use))
@@ -263,15 +266,15 @@
         TODO Can we trust self.config? It won't get updated if we change any data
         after reading.
         """
         contents = ["[settings]"]
         for key, value in self.config["settings"].items():
             contents.append(f"{key} = {value}")
 
-        for package in self.sections.values():
+        for package in self.sections:
             contents.append("")
             contents.append(f"[{package}]")
             for key, value in self.config[package].items():
                 if self.config["settings"].get(key) != value:
                     contents.append(f"{key} = {value}")
 
         contents.append("")
```

### Comparing `plone.releaser-2.2.1/plone/releaser/pypi.py` & `plone.releaser-2.2.2/plone/releaser/pypi.py`

 * *Files identical despite different names*

### Comparing `plone.releaser-2.2.1/plone/releaser/release.py` & `plone.releaser-2.2.2/plone/releaser/release.py`

 * *Files identical despite different names*

### Comparing `plone.releaser-2.2.1/plone/releaser/tests/input/changes.rst` & `plone.releaser-2.2.2/plone/releaser/tests/input/changes.rst`

 * *Files identical despite different names*

### Comparing `plone.releaser-2.2.1/plone/releaser/tests/input/sources.cfg` & `plone.releaser-2.2.2/plone/releaser/tests/input/sources.cfg`

 * *Files identical despite different names*

### Comparing `plone.releaser-2.2.1/plone/releaser/tests/test_buildout.py` & `plone.releaser-2.2.2/plone/releaser/tests/test_buildout.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,18 +17,19 @@
 VERSIONS_FILE2 = INPUT_DIR / "versions2.cfg"
 VERSIONS_FILE3 = INPUT_DIR / "versions3.cfg"
 VERSIONS_FILE4 = INPUT_DIR / "versions4.cfg"
 
 
 def test_checkouts_file_data():
     cf = CheckoutsFile(CHECKOUTS_FILE)
-    # The data maps lower case to actual case.
+    # The data used to map lower case to actual case,
+    # but now actual case to True.
     assert cf.data == {
-        "camelcase": "CamelCase",
-        "package": "package",
+        "CamelCase": True,
+        "package": True,
     }
 
 
 def test_checkouts_file_contains():
     cf = CheckoutsFile(CHECKOUTS_FILE)
     assert "package" in cf
     assert "nope" not in cf
@@ -36,35 +37,34 @@
     assert "camelcase" in cf
     assert "CamelCase" in cf
     assert "CAMELCASE" in cf
 
 
 def test_checkouts_file_get():
     cf = CheckoutsFile(CHECKOUTS_FILE)
-    # The data maps lower case to actual case.
-    assert cf["package"] == "package"
-    assert cf.get("package") == "package"
-    assert cf["camelcase"] == "CamelCase"
-    assert cf["CAMELCASE"] == "CamelCase"
-    assert cf["CamelCase"] == "CamelCase"
+    assert cf["package"] is True
+    assert cf.get("package") is True
+    assert cf["camelcase"] is True
+    assert cf["CAMELCASE"] is True
+    assert cf["CamelCase"] is True
     with pytest.raises(KeyError):
         cf["nope"]
 
 
 def test_checkouts_file_add(tmp_path):
     # When we add or remove a checkout, the file changes, so we work on a copy.
     copy_path = tmp_path / "checkouts.cfg"
     shutil.copyfile(CHECKOUTS_FILE, copy_path)
     cf = CheckoutsFile(copy_path)
     assert "Extra" not in cf
     cf.add("Extra")
     # Let's read it fresh, for good measure.
     cf = CheckoutsFile(copy_path)
     assert "Extra" in cf
-    assert cf.get("extra") == "Extra"
+    assert cf.get("extra") is True
 
 
 def test_checkouts_file_remove(tmp_path):
     copy_path = tmp_path / "checkouts.cfg"
     shutil.copyfile(CHECKOUTS_FILE, copy_path)
     cf = CheckoutsFile(copy_path)
     assert "package" in cf
@@ -142,16 +142,15 @@
     assert src.branch == "6.0"
     assert src.egg is False
     assert src.path == "docs"
 
 
 def test_sources_file_data():
     sf = SourcesFile(SOURCES_FILE)
-    # Note that the keys are lowercase.
-    assert sorted(sf.data.keys()) == ["docs", "plone", "plone.alterego", "plone.base"]
+    assert sorted(sf.data.keys()) == ["Plone", "docs", "plone.alterego", "plone.base"]
 
 
 def test_sources_file_contains():
     sf = SourcesFile(SOURCES_FILE)
     assert "docs" in sf
     assert "plone.base" in sf
     assert "nope" not in sf
@@ -216,32 +215,31 @@
 
 [remotes]
 plone = https://github.com/plone
 plone_push = git@github.com:plone
 
 [sources]
 docs = git ${remotes:plone}/documentation.git branch=6.0 path=${buildout:docs-directory} egg=false
-plone = git ${remotes:plone}/Plone.git pushurl=${remotes:plone_push}/Plone.git branch=6.0.x
+Plone = git ${remotes:plone}/Plone.git pushurl=${remotes:plone_push}/Plone.git branch=6.0.x
 plone.alterego = git ${remotes:plone}/plone.alterego.git branch=master
 plone.base = git ${remotes:plone}/plone.base.git branch=main
 """
     )
 
 
 def test_versions_file_versions():
     vf = VersionsFile(VERSIONS_FILE)
-    # All versions are reported lowercased.
     assert vf.data == {
         "annotated": "1.0",
-        "camelcase": "1.0",
+        "CamelCase": "1.0",
         "duplicate": "1.0",
         "lowercase": "1.0",
         "package": "1.0",
         "pyspecific": "1.0",
-        "uppercase": "1.0",
+        "UPPERCASE": "1.0",
     }
 
 
 def test_versions_file_extends():
     vf = VersionsFile(VERSIONS_FILE)
     assert vf.extends == [
         "https://zopefoundation.github.io/Zope/releases/5.8.3/versions.cfg"
@@ -271,21 +269,21 @@
 
 
 def test_versions_file_versions_with_markers():
     vf = VersionsFile(VERSIONS_FILE, with_markers=True)
     # All versions are reported lowercased.
     assert vf.data == {
         "annotated": "1.0",
-        "camelcase": "1.0",
+        "CamelCase": "1.0",
         "duplicate": "1.0",
         "lowercase": "1.0",
         "onepython": {"python312": "2.1"},
         "package": "1.0",
         "pyspecific": {"": "1.0", "python312": "2.0"},
-        "uppercase": "1.0",
+        "UPPERCASE": "1.0",
     }
 
 
 def test_versions_file_contains():
     vf = VersionsFile(VERSIONS_FILE)
     assert "package" in vf
     assert "nope" not in vf
@@ -448,29 +446,28 @@
     assert vf.extends == vf2.extends
     assert vf.data == vf2.data
     # Check the entire text.
     # Note that there are differences with the original:
     # - the extends line is on a separate line
     # - all comments are removed
     # - the duplicate is removed
-    # - all package names are lowercased
     assert (
         copy_path.read_text()
         == """[buildout]
 extends =
     https://zopefoundation.github.io/Zope/releases/5.8.3/versions.cfg
 
 [versions]
 annotated = 1.0
-camelcase = 1.0
+CamelCase = 1.0
 duplicate = 1.0
 lowercase = 1.0
 package = 1.0
 pyspecific = 1.0
-uppercase = 1.0
+UPPERCASE = 1.0
 """
     )
 
 
 def test_versions_file_rewrite_2(tmp_path):
     copy_path = tmp_path / "versions2.cfg"
     shutil.copyfile(VERSIONS_FILE2, copy_path)
```

### Comparing `plone.releaser-2.2.1/plone/releaser/tests/test_changelog.py` & `plone.releaser-2.2.2/plone/releaser/tests/test_changelog.py`

 * *Files identical despite different names*

### Comparing `plone.releaser-2.2.1/plone/releaser/tests/test_pip.py` & `plone.releaser-2.2.2/plone/releaser/tests/test_pip.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,18 +13,19 @@
 CONSTRAINTS_FILE3 = INPUT_DIR / "constraints3.txt"
 CONSTRAINTS_FILE4 = INPUT_DIR / "constraints4.txt"
 MXDEV_FILE = INPUT_DIR / "mxdev.ini"
 
 
 def test_mxdev_file_data():
     mf = IniFile(MXDEV_FILE)
-    # The data maps lower case to actual case.
+    # The data used to map lower case to actual case,
+    # but now actual case to True.
     assert mf.data == {
-        "camelcase": "CamelCase",
-        "package": "package",
+        "CamelCase": True,
+        "package": True,
     }
 
 
 def test_mxdev_file_contains():
     mf = IniFile(MXDEV_FILE)
     assert "package" in mf
     assert "unused" not in mf
@@ -32,20 +33,19 @@
     assert "camelcase" in mf
     assert "CamelCase" in mf
     assert "CAMELCASE" in mf
 
 
 def test_mxdev_file_get():
     mf = IniFile(MXDEV_FILE)
-    # The data maps lower case to actual case.
-    assert mf["package"] == "package"
-    assert mf.get("package") == "package"
-    assert mf["camelcase"] == "CamelCase"
-    assert mf["CAMELCASE"] == "CamelCase"
-    assert mf["CamelCase"] == "CamelCase"
+    assert mf["package"] is True
+    assert mf.get("package") is True
+    assert mf["camelcase"] is True
+    assert mf["CAMELCASE"] is True
+    assert mf["CamelCase"] is True
     with pytest.raises(KeyError):
         mf["unused"]
     assert mf.get("unused") is None
 
 
 def test_mxdev_file_add_known(tmp_path):
     # When we add or remove a checkout, the file changes, so we work on a copy.
@@ -53,15 +53,15 @@
     shutil.copyfile(MXDEV_FILE, copy_path)
     mf = IniFile(copy_path)
     assert "unused" not in mf
     mf.add("unused")
     # Let's read it fresh, for good measure.
     mf = IniFile(copy_path)
     assert "unused" in mf
-    assert mf["unused"] == "unused"
+    assert mf["unused"] is True
 
 
 def test_mxdev_file_add_unknown(tmp_path):
     # We cannot edit mxdev.ini to use a package when it is not defined.
     copy_path = tmp_path / "mxdev.ini"
     shutil.copyfile(MXDEV_FILE, copy_path)
     mf = IniFile(copy_path)
@@ -133,20 +133,20 @@
 
 
 def test_constraints_file_constraints():
     cf = ConstraintsFile(CONSTRAINTS_FILE)
     # All constraints are reported lowercased.
     assert cf.data == {
         "annotated": "1.0",
-        "camelcase": "1.0",
+        "CamelCase": "1.0",
         "duplicate": "1.0",
         "lowercase": "1.0",
         "package": "1.0",
         "pyspecific": "1.0",
-        "uppercase": "1.0",
+        "UPPERCASE": "1.0",
     }
 
 
 def test_constraints_file_contains():
     cf = ConstraintsFile(CONSTRAINTS_FILE)
     assert "package" in cf
     assert "nope" not in cf
@@ -272,21 +272,21 @@
 
 
 def test_constraints_file_constraints_with_markers():
     cf = ConstraintsFile(CONSTRAINTS_FILE, with_markers=True)
     # All constraints are reported lowercased.
     assert cf.data == {
         "annotated": "1.0",
-        "camelcase": "1.0",
+        "CamelCase": "1.0",
         "duplicate": "1.0",
         "lowercase": "1.0",
         "onepython": {'python_version=="3.12"': "2.1"},
         "package": "1.0",
         "pyspecific": {"": "1.0", 'python_version=="3.12"': "2.0"},
-        "uppercase": "1.0",
+        "UPPERCASE": "1.0",
     }
 
 
 def test_constraints_file_rewrite(tmp_path):
     copy_path = tmp_path / "constraints.txt"
     shutil.copyfile(CONSTRAINTS_FILE, copy_path)
     cf = ConstraintsFile(copy_path)
@@ -296,25 +296,24 @@
     assert cf.extends == cf2.extends
     assert cf.data == cf2.data
     # Check the entire text.
     # Note that there are differences with the original:
     # - the extends line is on a separate line
     # - all comments are removed
     # - the duplicate is removed
-    # - all package names are lowercased
     assert (
         copy_path.read_text()
         == """-c https://zopefoundation.github.io/Zope/releases/5.8.3/constraints.txt
 annotated==1.0
-camelcase==1.0
+CamelCase==1.0
 duplicate==1.0
 lowercase==1.0
 package==1.0
 pyspecific==1.0
-uppercase==1.0
+UPPERCASE==1.0
 """
     )
 
 
 def test_constraints_file_rewrite_2(tmp_path):
     copy_path = tmp_path / "constraints2.txt"
     shutil.copyfile(CONSTRAINTS_FILE2, copy_path)
```

### Comparing `plone.releaser-2.2.1/plone/releaser/tests/test_utils.py` & `plone.releaser-2.2.2/plone/releaser/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `plone.releaser-2.2.1/plone/releaser/tests/test_versions2constraints.py` & `plone.releaser-2.2.2/plone/releaser/tests/test_versions2constraints.py`

 * *Files 10% similar despite different names*

```diff
@@ -24,17 +24,17 @@
     assert constraints_file.exists()
     cf = ConstraintsFile(constraints_file, with_markers=True)
     print(cf.data)
     assert (
         constraints_file.read_text()
         == """-c https://zopefoundation.github.io/Zope/releases/5.8.3/constraints.txt
 annotated==1.0
-camelcase==1.0
+CamelCase==1.0
 duplicate==1.0
 lowercase==1.0
 package==1.0
 pyspecific==1.0
 pyspecific==2.0; python_version == "3.12"
-uppercase==1.0
+UPPERCASE==1.0
 onepython==2.1; python_version == "3.12"
 """
     )
```

### Comparing `plone.releaser-2.2.1/plone/releaser/utils.py` & `plone.releaser-2.2.2/plone/releaser/utils.py`

 * *Files identical despite different names*

### Comparing `plone.releaser-2.2.1/plone.releaser.egg-info/PKG-INFO` & `plone.releaser-2.2.2/plone.releaser.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.releaser
-Version: 2.2.1
+Version: 2.2.2
 Summary: Plone release management utilities
 Home-page: https://github.com/plone/plone.releaser
 Author: Eric Steele
 Author-email: eric@esteele.net
 License: GPL
 Keywords: plone release
 Classifier: Development Status :: 5 - Production/Stable
@@ -79,14 +79,24 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+2.2.2 (2024-04-16)
+------------------
+
+Bug fixes:
+
+
+- Preserve the case of package names in versions2constraints and friends.
+  [maurits] (#65)
+
+
 2.2.1 (2023-12-14)
 ------------------
 
 Bug fixes:
 
 
 - Manage changelog: read markdown files as well.
```

### Comparing `plone.releaser-2.2.1/plone.releaser.egg-info/SOURCES.txt` & `plone.releaser-2.2.2/plone.releaser.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `plone.releaser-2.2.1/plone.releaser.egg-info/entry_points.txt` & `plone.releaser-2.2.2/plone.releaser.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `plone.releaser-2.2.1/pyproject.toml` & `plone.releaser-2.2.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `plone.releaser-2.2.1/setup.py` & `plone.releaser-2.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import find_packages
 from setuptools import setup
 
 
-version = "2.2.1"
+version = "2.2.2"
 
 long_description = "{}\n{}".format(
     open("README.rst").read(), open("CHANGES.rst").read()
 )
 
 setup(
     name="plone.releaser",
```

