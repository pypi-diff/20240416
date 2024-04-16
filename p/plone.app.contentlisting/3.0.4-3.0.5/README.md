# Comparing `tmp/plone.app.contentlisting-3.0.4.tar.gz` & `tmp/plone.app.contentlisting-3.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "plone.app.contentlisting-3.0.4.tar", last modified: Fri Oct  6 22:20:02 2023, max compression
+gzip compressed data, was "plone.app.contentlisting-3.0.5.tar", last modified: Tue Apr 16 19:32:08 2024, max compression
```

## Comparing `plone.app.contentlisting-3.0.4.tar` & `plone.app.contentlisting-3.0.5.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-10-06 22:20:02.183672 plone.app.contentlisting-3.0.4/
--rw-r--r--   0 maurits    (501) staff       (20)     1342 2023-10-06 22:20:01.000000 plone.app.contentlisting-3.0.4/.editorconfig
--rw-r--r--   0 maurits    (501) staff       (20)      540 2023-10-06 22:20:01.000000 plone.app.contentlisting-3.0.4/.flake8
--rw-r--r--   0 maurits    (501) staff       (20)      663 2023-10-06 22:20:01.000000 plone.app.contentlisting-3.0.4/.gitignore
--rw-r--r--   0 maurits    (501) staff       (20)      274 2023-10-06 22:20:01.000000 plone.app.contentlisting-3.0.4/.meta.toml
--rw-r--r--   0 maurits    (501) staff       (20)     1880 2023-10-06 22:20:01.000000 plone.app.contentlisting-3.0.4/.pre-commit-config.yaml
--rw-r--r--   0 maurits    (501) staff       (20)     7058 2023-10-06 22:20:01.000000 plone.app.contentlisting-3.0.4/CHANGES.rst
--rw-r--r--   0 maurits    (501) staff       (20)       70 2023-10-06 22:20:01.000000 plone.app.contentlisting-3.0.4/CONTRIBUTING.rst
--rw-r--r--   0 maurits    (501) staff       (20)      144 2023-10-06 22:20:01.000000 plone.app.contentlisting-3.0.4/MANIFEST.in
--rw-r--r--   0 maurits    (501) staff       (20)    18126 2023-10-06 22:20:02.182975 plone.app.contentlisting-3.0.4/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     9752 2023-10-06 22:20:01.000000 plone.app.contentlisting-3.0.4/README.rst
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-10-06 22:20:02.171571 plone.app.contentlisting-3.0.4/docs/
--rw-r--r--   0 maurits    (501) staff       (20)    15220 2023-10-06 22:20:01.000000 plone.app.contentlisting-3.0.4/docs/LICENSE.GPL
--rw-r--r--   0 maurits    (501) staff       (20)      686 2023-10-06 22:20:01.000000 plone.app.contentlisting-3.0.4/docs/LICENSE.txt
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-10-06 22:20:02.171998 plone.app.contentlisting-3.0.4/plone/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2023-10-06 22:20:01.000000 plone.app.contentlisting-3.0.4/plone/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-10-06 22:20:02.176124 plone.app.contentlisting-3.0.4/plone/app/
--rw-r--r--   0 maurits    (501) staff       (20)       56 2023-10-06 22:20:01.000000 plone.app.contentlisting-3.0.4/plone/app/__init__.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-10-06 22:20:02.179181 plone.app.contentlisting-3.0.4/plone/app/contentlisting/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-10-06 22:20:01.000000 plone.app.contentlisting-3.0.4/plone/app/contentlisting/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     1455 2023-10-06 22:20:01.000000 plone.app.contentlisting-3.0.4/plone/app/contentlisting/browser.py
--rw-r--r--   0 maurits    (501) staff       (20)     5990 2023-10-06 22:20:01.000000 plone.app.contentlisting-3.0.4/plone/app/contentlisting/catalog.py
--rw-r--r--   0 maurits    (501) staff       (20)     1677 2023-10-06 22:20:01.000000 plone.app.contentlisting-3.0.4/plone/app/contentlisting/configure.zcml
--rw-r--r--   0 maurits    (501) staff       (20)     5954 2023-10-06 22:20:01.000000 plone.app.contentlisting-3.0.4/plone/app/contentlisting/contentlisting.py
--rw-r--r--   0 maurits    (501) staff       (20)     2165 2023-10-06 22:20:01.000000 plone.app.contentlisting-3.0.4/plone/app/contentlisting/interfaces.py
--rw-r--r--   0 maurits    (501) staff       (20)     3769 2023-10-06 22:20:01.000000 plone.app.contentlisting-3.0.4/plone/app/contentlisting/realobject.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-10-06 22:20:02.181353 plone.app.contentlisting-3.0.4/plone/app/contentlisting/tests/
--rw-r--r--   0 maurits    (501) staff       (20)        0 2023-10-06 22:20:01.000000 plone.app.contentlisting-3.0.4/plone/app/contentlisting/tests/__init__.py
--rw-r--r--   0 maurits    (501) staff       (20)     1726 2023-10-06 22:20:01.000000 plone.app.contentlisting-3.0.4/plone/app/contentlisting/tests/base.py
--rw-r--r--   0 maurits    (501) staff       (20)     8027 2023-10-06 22:20:01.000000 plone.app.contentlisting-3.0.4/plone/app/contentlisting/tests/integration.rst
--rw-r--r--   0 maurits    (501) staff       (20)      591 2023-10-06 22:20:01.000000 plone.app.contentlisting-3.0.4/plone/app/contentlisting/tests/test_integration_doctest.py
--rw-r--r--   0 maurits    (501) staff       (20)    16709 2023-10-06 22:20:01.000000 plone.app.contentlisting-3.0.4/plone/app/contentlisting/tests/test_integration_unit.py
-drwxr-xr-x   0 maurits    (501) staff       (20)        0 2023-10-06 22:20:02.175671 plone.app.contentlisting-3.0.4/plone.app.contentlisting.egg-info/
--rw-r--r--   0 maurits    (501) staff       (20)    18126 2023-10-06 22:20:01.000000 plone.app.contentlisting-3.0.4/plone.app.contentlisting.egg-info/PKG-INFO
--rw-r--r--   0 maurits    (501) staff       (20)     1133 2023-10-06 22:20:02.000000 plone.app.contentlisting-3.0.4/plone.app.contentlisting.egg-info/SOURCES.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-10-06 22:20:01.000000 plone.app.contentlisting-3.0.4/plone.app.contentlisting.egg-info/dependency_links.txt
--rw-r--r--   0 maurits    (501) staff       (20)       40 2023-10-06 22:20:01.000000 plone.app.contentlisting-3.0.4/plone.app.contentlisting.egg-info/entry_points.txt
--rw-r--r--   0 maurits    (501) staff       (20)       16 2023-10-06 22:20:02.000000 plone.app.contentlisting-3.0.4/plone.app.contentlisting.egg-info/namespace_packages.txt
--rw-r--r--   0 maurits    (501) staff       (20)        1 2023-10-06 22:20:01.000000 plone.app.contentlisting-3.0.4/plone.app.contentlisting.egg-info/not-zip-safe
--rw-r--r--   0 maurits    (501) staff       (20)      201 2023-10-06 22:20:02.000000 plone.app.contentlisting-3.0.4/plone.app.contentlisting.egg-info/requires.txt
--rw-r--r--   0 maurits    (501) staff       (20)        6 2023-10-06 22:20:02.000000 plone.app.contentlisting-3.0.4/plone.app.contentlisting.egg-info/top_level.txt
--rw-r--r--   0 maurits    (501) staff       (20)     4244 2023-10-06 22:20:01.000000 plone.app.contentlisting-3.0.4/pyproject.toml
--rw-r--r--   0 maurits    (501) staff       (20)       38 2023-10-06 22:20:02.183788 plone.app.contentlisting-3.0.4/setup.cfg
--rw-r--r--   0 maurits    (501) staff       (20)     1866 2023-10-06 22:20:01.000000 plone.app.contentlisting-3.0.4/setup.py
--rw-r--r--   0 maurits    (501) staff       (20)     4629 2023-10-06 22:20:01.000000 plone.app.contentlisting-3.0.4/tox.ini
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-16 19:32:08.423272 plone.app.contentlisting-3.0.5/
+-rw-r--r--   0 maurits    (501) staff       (20)     1342 2024-04-16 19:32:07.000000 plone.app.contentlisting-3.0.5/.editorconfig
+-rw-r--r--   0 maurits    (501) staff       (20)      540 2024-04-16 19:32:07.000000 plone.app.contentlisting-3.0.5/.flake8
+-rw-r--r--   0 maurits    (501) staff       (20)      663 2024-04-16 19:32:07.000000 plone.app.contentlisting-3.0.5/.gitignore
+-rw-r--r--   0 maurits    (501) staff       (20)      274 2024-04-16 19:32:07.000000 plone.app.contentlisting-3.0.5/.meta.toml
+-rw-r--r--   0 maurits    (501) staff       (20)     1880 2024-04-16 19:32:07.000000 plone.app.contentlisting-3.0.5/.pre-commit-config.yaml
+-rw-r--r--   0 maurits    (501) staff       (20)     7181 2024-04-16 19:32:07.000000 plone.app.contentlisting-3.0.5/CHANGES.rst
+-rw-r--r--   0 maurits    (501) staff       (20)       70 2024-04-16 19:32:07.000000 plone.app.contentlisting-3.0.5/CONTRIBUTING.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      144 2024-04-16 19:32:07.000000 plone.app.contentlisting-3.0.5/MANIFEST.in
+-rw-r--r--   0 maurits    (501) staff       (20)    18297 2024-04-16 19:32:08.422442 plone.app.contentlisting-3.0.5/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     9752 2024-04-16 19:32:07.000000 plone.app.contentlisting-3.0.5/README.rst
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-16 19:32:08.412148 plone.app.contentlisting-3.0.5/docs/
+-rw-r--r--   0 maurits    (501) staff       (20)    15220 2024-04-16 19:32:07.000000 plone.app.contentlisting-3.0.5/docs/LICENSE.GPL
+-rw-r--r--   0 maurits    (501) staff       (20)      686 2024-04-16 19:32:07.000000 plone.app.contentlisting-3.0.5/docs/LICENSE.txt
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-16 19:32:08.412409 plone.app.contentlisting-3.0.5/plone/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2024-04-16 19:32:07.000000 plone.app.contentlisting-3.0.5/plone/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-16 19:32:08.416614 plone.app.contentlisting-3.0.5/plone/app/
+-rw-r--r--   0 maurits    (501) staff       (20)       56 2024-04-16 19:32:07.000000 plone.app.contentlisting-3.0.5/plone/app/__init__.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-16 19:32:08.419005 plone.app.contentlisting-3.0.5/plone/app/contentlisting/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2024-04-16 19:32:07.000000 plone.app.contentlisting-3.0.5/plone/app/contentlisting/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1455 2024-04-16 19:32:07.000000 plone.app.contentlisting-3.0.5/plone/app/contentlisting/browser.py
+-rw-r--r--   0 maurits    (501) staff       (20)     5990 2024-04-16 19:32:07.000000 plone.app.contentlisting-3.0.5/plone/app/contentlisting/catalog.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1677 2024-04-16 19:32:07.000000 plone.app.contentlisting-3.0.5/plone/app/contentlisting/configure.zcml
+-rw-r--r--   0 maurits    (501) staff       (20)     5954 2024-04-16 19:32:07.000000 plone.app.contentlisting-3.0.5/plone/app/contentlisting/contentlisting.py
+-rw-r--r--   0 maurits    (501) staff       (20)     2165 2024-04-16 19:32:07.000000 plone.app.contentlisting-3.0.5/plone/app/contentlisting/interfaces.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4001 2024-04-16 19:32:07.000000 plone.app.contentlisting-3.0.5/plone/app/contentlisting/realobject.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-16 19:32:08.420591 plone.app.contentlisting-3.0.5/plone/app/contentlisting/tests/
+-rw-r--r--   0 maurits    (501) staff       (20)        0 2024-04-16 19:32:07.000000 plone.app.contentlisting-3.0.5/plone/app/contentlisting/tests/__init__.py
+-rw-r--r--   0 maurits    (501) staff       (20)     1726 2024-04-16 19:32:07.000000 plone.app.contentlisting-3.0.5/plone/app/contentlisting/tests/base.py
+-rw-r--r--   0 maurits    (501) staff       (20)     8027 2024-04-16 19:32:07.000000 plone.app.contentlisting-3.0.5/plone/app/contentlisting/tests/integration.rst
+-rw-r--r--   0 maurits    (501) staff       (20)      591 2024-04-16 19:32:07.000000 plone.app.contentlisting-3.0.5/plone/app/contentlisting/tests/test_integration_doctest.py
+-rw-r--r--   0 maurits    (501) staff       (20)    17372 2024-04-16 19:32:07.000000 plone.app.contentlisting-3.0.5/plone/app/contentlisting/tests/test_integration_unit.py
+drwxr-xr-x   0 maurits    (501) staff       (20)        0 2024-04-16 19:32:08.421290 plone.app.contentlisting-3.0.5/plone.app.contentlisting.egg-info/
+-rw-r--r--   0 maurits    (501) staff       (20)    18297 2024-04-16 19:32:08.000000 plone.app.contentlisting-3.0.5/plone.app.contentlisting.egg-info/PKG-INFO
+-rw-r--r--   0 maurits    (501) staff       (20)     1133 2024-04-16 19:32:08.000000 plone.app.contentlisting-3.0.5/plone.app.contentlisting.egg-info/SOURCES.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2024-04-16 19:32:08.000000 plone.app.contentlisting-3.0.5/plone.app.contentlisting.egg-info/dependency_links.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       40 2024-04-16 19:32:08.000000 plone.app.contentlisting-3.0.5/plone.app.contentlisting.egg-info/entry_points.txt
+-rw-r--r--   0 maurits    (501) staff       (20)       16 2024-04-16 19:32:08.000000 plone.app.contentlisting-3.0.5/plone.app.contentlisting.egg-info/namespace_packages.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        1 2024-04-16 19:32:08.000000 plone.app.contentlisting-3.0.5/plone.app.contentlisting.egg-info/not-zip-safe
+-rw-r--r--   0 maurits    (501) staff       (20)      217 2024-04-16 19:32:08.000000 plone.app.contentlisting-3.0.5/plone.app.contentlisting.egg-info/requires.txt
+-rw-r--r--   0 maurits    (501) staff       (20)        6 2024-04-16 19:32:08.000000 plone.app.contentlisting-3.0.5/plone.app.contentlisting.egg-info/top_level.txt
+-rw-r--r--   0 maurits    (501) staff       (20)     4244 2024-04-16 19:32:07.000000 plone.app.contentlisting-3.0.5/pyproject.toml
+-rw-r--r--   0 maurits    (501) staff       (20)       38 2024-04-16 19:32:08.423451 plone.app.contentlisting-3.0.5/setup.cfg
+-rw-r--r--   0 maurits    (501) staff       (20)     1897 2024-04-16 19:32:07.000000 plone.app.contentlisting-3.0.5/setup.py
+-rw-r--r--   0 maurits    (501) staff       (20)     4629 2024-04-16 19:32:07.000000 plone.app.contentlisting-3.0.5/tox.ini
```

### Comparing `plone.app.contentlisting-3.0.4/.editorconfig` & `plone.app.contentlisting-3.0.5/.editorconfig`

 * *Files identical despite different names*

### Comparing `plone.app.contentlisting-3.0.4/.flake8` & `plone.app.contentlisting-3.0.5/.flake8`

 * *Files identical despite different names*

### Comparing `plone.app.contentlisting-3.0.4/.gitignore` & `plone.app.contentlisting-3.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `plone.app.contentlisting-3.0.4/.pre-commit-config.yaml` & `plone.app.contentlisting-3.0.5/.pre-commit-config.yaml`

 * *Files 5% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 # See the inline comments on how to expand/tweak this configuration file
 ci:
     autofix_prs: false
     autoupdate_schedule: monthly
 
 repos:
 -   repo: https://github.com/asottile/pyupgrade
-    rev: v3.14.0
+    rev: v3.15.2
     hooks:
     -   id: pyupgrade
         args: [--py38-plus]
 -   repo: https://github.com/pycqa/isort
-    rev: 5.12.0
+    rev: 5.13.2
     hooks:
     -   id: isort
 -   repo: https://github.com/psf/black
-    rev: 23.9.1
+    rev: 24.3.0
     hooks:
     -   id: black
 -   repo: https://github.com/collective/zpretty
     rev: 3.1.0
     hooks:
     -   id: zpretty
 
@@ -28,15 +28,15 @@
 # Add extra configuration options in .meta.toml:
 #  [pre_commit]
 #  zpretty_extra_lines = """
 #  _your own configuration lines_
 #  """
 ##
 -   repo: https://github.com/PyCQA/flake8
-    rev: 6.1.0
+    rev: 7.0.0
     hooks:
     -   id: flake8
 
 ##
 # Add extra configuration options in .meta.toml:
 #  [pre_commit]
 #  flake8_extra_lines = """
@@ -62,20 +62,20 @@
     hooks:
     -   id: check-manifest
 -   repo: https://github.com/regebro/pyroma
     rev: "4.2"
     hooks:
     -   id: pyroma
 -   repo: https://github.com/mgedmin/check-python-versions
-    rev: "0.21.2"
+    rev: "0.22.0"
     hooks:
     -   id: check-python-versions
         args: ['--only', 'setup.py,pyproject.toml']
 -   repo: https://github.com/collective/i18ndude
-    rev: "6.0.0"
+    rev: "6.1.0"
     hooks:
     -   id: i18ndude
 
 ##
 # Add extra configuration options in .meta.toml:
 #  [pre_commit]
 #  extra_lines = """
```

### Comparing `plone.app.contentlisting-3.0.4/CHANGES.rst` & `plone.app.contentlisting-3.0.5/CHANGES.rst`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,23 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+3.0.5 (2024-04-16)
+------------------
+
+Bug fixes:
+
+
+- Support image_scales in RealContentListingObject. @davisagli (#64)
+
+
 3.0.4 (2023-10-07)
 ------------------
 
 Internal:
 
 
 - Update configuration files.
```

### Comparing `plone.app.contentlisting-3.0.4/PKG-INFO` & `plone.app.contentlisting-3.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.app.contentlisting
-Version: 3.0.4
+Version: 3.0.5
 Summary: Listing of content for the Plone CMS
 Home-page: https://pypi.org/project/plone.app.contentlisting
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL version 2
 Keywords: content list Plone
 Classifier: Development Status :: 5 - Production/Stable
@@ -27,14 +27,15 @@
 Requires-Dist: plone.registry
 Requires-Dist: plone.rfc822
 Requires-Dist: plone.uuid
 Provides-Extra: test
 Requires-Dist: plone.app.contenttypes[test]; extra == "test"
 Requires-Dist: plone.app.testing; extra == "test"
 Requires-Dist: plone.batching; extra == "test"
+Requires-Dist: plone.namedfile; extra == "test"
 Requires-Dist: plone.testing; extra == "test"
 
 =============================================================================
 Listing and working with Plone content objects using plone.app.contentlisting
 =============================================================================
 
 This is valid for Plone 4.1 upwards.
@@ -295,14 +296,23 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+3.0.5 (2024-04-16)
+------------------
+
+Bug fixes:
+
+
+- Support image_scales in RealContentListingObject. @davisagli (#64)
+
+
 3.0.4 (2023-10-07)
 ------------------
 
 Internal:
 
 
 - Update configuration files.
```

### Comparing `plone.app.contentlisting-3.0.4/README.rst` & `plone.app.contentlisting-3.0.5/README.rst`

 * *Files identical despite different names*

### Comparing `plone.app.contentlisting-3.0.4/docs/LICENSE.GPL` & `plone.app.contentlisting-3.0.5/docs/LICENSE.GPL`

 * *Files identical despite different names*

### Comparing `plone.app.contentlisting-3.0.4/docs/LICENSE.txt` & `plone.app.contentlisting-3.0.5/docs/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `plone.app.contentlisting-3.0.4/plone/app/contentlisting/browser.py` & `plone.app.contentlisting-3.0.5/plone/app/contentlisting/browser.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentlisting-3.0.4/plone/app/contentlisting/catalog.py` & `plone.app.contentlisting-3.0.5/plone/app/contentlisting/catalog.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentlisting-3.0.4/plone/app/contentlisting/configure.zcml` & `plone.app.contentlisting-3.0.5/plone/app/contentlisting/configure.zcml`

 * *Files identical despite different names*

### Comparing `plone.app.contentlisting-3.0.4/plone/app/contentlisting/contentlisting.py` & `plone.app.contentlisting-3.0.5/plone/app/contentlisting/contentlisting.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentlisting-3.0.4/plone/app/contentlisting/interfaces.py` & `plone.app.contentlisting-3.0.5/plone/app/contentlisting/interfaces.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentlisting-3.0.4/plone/app/contentlisting/realobject.py` & `plone.app.contentlisting-3.0.5/plone/app/contentlisting/realobject.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 from Acquisition import aq_get
 from plone.app.contentlisting.contentlisting import BaseContentListingObject
 from plone.app.contentlisting.interfaces import IContentListingObject
+from plone.base.interfaces import IImageScalesAdapter
 from plone.base.utils import base_hasattr
 from plone.base.utils import human_readable_size
 from plone.rfc822.interfaces import IPrimaryFieldInfo
 from plone.uuid.interfaces import IUUID
 from Products.CMFCore.utils import getToolByName
+from zope.component import getMultiAdapter
 from zope.interface import implementer
 
 
 MARKER = object()
 
 
 @implementer(IContentListingObject)
@@ -101,7 +103,11 @@
     # Currently Type() returns different values depending on the data source being
     # a brain or a real object. Probably needed. Support for all the attributes
     # from the indexablemetadata wrappers.
 
     def PortalType(self):
         obj = self.getObject()
         return obj.portal_type
+
+    def image_scales(self):
+        obj = self.getObject()
+        return getMultiAdapter((obj, self.request), IImageScalesAdapter)()
```

### Comparing `plone.app.contentlisting-3.0.4/plone/app/contentlisting/tests/base.py` & `plone.app.contentlisting-3.0.5/plone/app/contentlisting/tests/base.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentlisting-3.0.4/plone/app/contentlisting/tests/integration.rst` & `plone.app.contentlisting-3.0.5/plone/app/contentlisting/tests/integration.rst`

 * *Files identical despite different names*

### Comparing `plone.app.contentlisting-3.0.4/plone/app/contentlisting/tests/test_integration_doctest.py` & `plone.app.contentlisting-3.0.5/plone/app/contentlisting/tests/test_integration_doctest.py`

 * *Files identical despite different names*

### Comparing `plone.app.contentlisting-3.0.4/plone/app/contentlisting/tests/test_integration_unit.py` & `plone.app.contentlisting-3.0.5/plone/app/contentlisting/tests/test_integration_unit.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,19 +1,26 @@
 from plone.app.contentlisting.interfaces import IContentListing
 from plone.app.contentlisting.interfaces import IContentListingObject
 from plone.app.contentlisting.tests.base import CONTENTLISTING_FUNCTIONAL_TESTING
 from plone.app.testing import setRoles
 from plone.app.testing import TEST_USER_ID
 from plone.batching.interfaces import IBatch
+from plone.namedfile.file import NamedBlobImage
 from Products.CMFCore.utils import getToolByName
 from zope.interface.verify import verifyObject
 
+import base64
 import unittest
 
 
+TEST_IMAGE_DATA = base64.b64decode(
+    "iVBORw0KGgoAAAANSUhEUgAAAAEAAAABCAQAAAC1HAwCAAAAC0lEQVR42mNk+A8AAQUBAScY42YAAAAASUVORK5CYII="
+)
+
+
 class TestSetup(unittest.TestCase):
     layer = CONTENTLISTING_FUNCTIONAL_TESTING
 
     def setUp(self):
         super().setUp()
         self.portal = self.layer["portal"]
         self.folder = self.portal["test-folder"]
@@ -261,14 +268,29 @@
             self.assertEqual(self.item.test_none, None)
         except AttributeError:
             self.fail(
                 "Accessing attributes which return ``None`` should not "
                 "result in an AttributeError."
             )
 
+    def test_item_image_scales(self):
+        self.folder.invokeFactory(
+            "Image",
+            "myimage",
+            title="My Image",
+        )
+        myimage = self.folder.myimage
+        myimage.image = NamedBlobImage(
+            data=TEST_IMAGE_DATA,
+            filename="test.png",
+        )
+        item = IContentListingObject(myimage)
+        image_scales = item.image_scales()
+        self.assertIn("download", image_scales["image"][0])
+
 
 class TestFolderContents(unittest.TestCase):
     """Testing that the folder contents browserview works and behaves
     as it should.
     """
 
     layer = CONTENTLISTING_FUNCTIONAL_TESTING
```

### Comparing `plone.app.contentlisting-3.0.4/plone.app.contentlisting.egg-info/PKG-INFO` & `plone.app.contentlisting-3.0.5/plone.app.contentlisting.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: plone.app.contentlisting
-Version: 3.0.4
+Version: 3.0.5
 Summary: Listing of content for the Plone CMS
 Home-page: https://pypi.org/project/plone.app.contentlisting
 Author: Plone Foundation
 Author-email: plone-developers@lists.sourceforge.net
 License: GPL version 2
 Keywords: content list Plone
 Classifier: Development Status :: 5 - Production/Stable
@@ -27,14 +27,15 @@
 Requires-Dist: plone.registry
 Requires-Dist: plone.rfc822
 Requires-Dist: plone.uuid
 Provides-Extra: test
 Requires-Dist: plone.app.contenttypes[test]; extra == "test"
 Requires-Dist: plone.app.testing; extra == "test"
 Requires-Dist: plone.batching; extra == "test"
+Requires-Dist: plone.namedfile; extra == "test"
 Requires-Dist: plone.testing; extra == "test"
 
 =============================================================================
 Listing and working with Plone content objects using plone.app.contentlisting
 =============================================================================
 
 This is valid for Plone 4.1 upwards.
@@ -295,14 +296,23 @@
 .. You should *NOT* be adding new change log entries to this file.
    You should create a file in the news directory instead.
    For helpful instructions, please see:
    https://github.com/plone/plone.releaser/blob/master/ADD-A-NEWS-ITEM.rst
 
 .. towncrier release notes start
 
+3.0.5 (2024-04-16)
+------------------
+
+Bug fixes:
+
+
+- Support image_scales in RealContentListingObject. @davisagli (#64)
+
+
 3.0.4 (2023-10-07)
 ------------------
 
 Internal:
 
 
 - Update configuration files.
```

### Comparing `plone.app.contentlisting-3.0.4/plone.app.contentlisting.egg-info/SOURCES.txt` & `plone.app.contentlisting-3.0.5/plone.app.contentlisting.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `plone.app.contentlisting-3.0.4/pyproject.toml` & `plone.app.contentlisting-3.0.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `plone.app.contentlisting-3.0.4/setup.py` & `plone.app.contentlisting-3.0.5/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from pathlib import Path
 from setuptools import find_packages
 from setuptools import setup
 
 
-version = "3.0.4"
+version = "3.0.5"
 
 long_description = (
     f"{Path('README.rst').read_text()}\n{Path('CHANGES.rst').read_text()}\n"
 )
 
 setup(
     name="plone.app.contentlisting",
@@ -50,14 +50,15 @@
         "plone.uuid",
     ],
     extras_require={
         "test": [
             "plone.app.contenttypes[test]",
             "plone.app.testing",
             "plone.batching",
+            "plone.namedfile",
             "plone.testing",
         ],
     },
     entry_points="""
     [z3c.autoinclude.plugin]
     target = plone
     """,
```

### Comparing `plone.app.contentlisting-3.0.4/tox.ini` & `plone.app.contentlisting-3.0.5/tox.ini`

 * *Files identical despite different names*

