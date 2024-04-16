# Comparing `tmp/agave_pyclient-1.6.1.tar.gz` & `tmp/agave_pyclient-1.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "agave_pyclient-1.6.1.tar", last modified: Mon Apr 15 22:42:04 2024, max compression
+gzip compressed data, was "agave_pyclient-1.6.2.tar", last modified: Mon Apr 15 23:55:09 2024, max compression
```

## Comparing `agave_pyclient-1.6.1.tar` & `agave_pyclient-1.6.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:04.275708 agave_pyclient-1.6.1/
--rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-04-15 22:41:57.000000 agave_pyclient-1.6.1/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-04-15 22:41:57.000000 agave_pyclient-1.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-15 22:41:57.000000 agave_pyclient-1.6.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3204 2024-04-15 22:42:04.275708 agave_pyclient-1.6.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-04-15 22:41:57.000000 agave_pyclient-1.6.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:04.275708 agave_pyclient-1.6.1/agave_pyclient/
--rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-15 22:41:57.000000 agave_pyclient-1.6.1/agave_pyclient/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    30183 2024-04-15 22:41:57.000000 agave_pyclient-1.6.1/agave_pyclient/agave.py
--rw-r--r--   0 runner    (1001) docker     (127)     7785 2024-04-15 22:41:57.000000 agave_pyclient-1.6.1/agave_pyclient/commandbuffer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:04.275708 agave_pyclient-1.6.1/agave_pyclient.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3204 2024-04-15 22:42:04.000000 agave_pyclient-1.6.1/agave_pyclient.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-15 22:42:04.000000 agave_pyclient-1.6.1/agave_pyclient.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 22:42:04.000000 agave_pyclient-1.6.1/agave_pyclient.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 22:42:04.000000 agave_pyclient-1.6.1/agave_pyclient.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-15 22:42:04.000000 agave_pyclient-1.6.1/agave_pyclient.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-15 22:42:04.000000 agave_pyclient-1.6.1/agave_pyclient.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 22:42:04.275708 agave_pyclient-1.6.1/docs/
--rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-15 22:41:57.000000 agave_pyclient-1.6.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-15 22:41:57.000000 agave_pyclient-1.6.1/docs/agave_renderer.rst
--rwxr-xr-x   0 runner    (1001) docker     (127)     5379 2024-04-15 22:41:57.000000 agave_pyclient-1.6.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-15 22:41:57.000000 agave_pyclient-1.6.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-15 22:41:57.000000 agave_pyclient-1.6.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-15 22:42:04.279708 agave_pyclient-1.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-04-15 22:41:57.000000 agave_pyclient-1.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 23:55:09.532125 agave_pyclient-1.6.2/
+-rw-r--r--   0 runner    (1001) docker     (127)     1566 2024-04-15 23:55:02.000000 agave_pyclient-1.6.2/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1953 2024-04-15 23:55:02.000000 agave_pyclient-1.6.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      246 2024-04-15 23:55:02.000000 agave_pyclient-1.6.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3204 2024-04-15 23:55:09.532125 agave_pyclient-1.6.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1959 2024-04-15 23:55:02.000000 agave_pyclient-1.6.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 23:55:09.532125 agave_pyclient-1.6.2/agave_pyclient/
+-rw-r--r--   0 runner    (1001) docker     (127)      393 2024-04-15 23:55:02.000000 agave_pyclient-1.6.2/agave_pyclient/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    30183 2024-04-15 23:55:02.000000 agave_pyclient-1.6.2/agave_pyclient/agave.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7785 2024-04-15 23:55:02.000000 agave_pyclient-1.6.2/agave_pyclient/commandbuffer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 23:55:09.532125 agave_pyclient-1.6.2/agave_pyclient.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3204 2024-04-15 23:55:09.000000 agave_pyclient-1.6.2/agave_pyclient.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      453 2024-04-15 23:55:09.000000 agave_pyclient-1.6.2/agave_pyclient.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 23:55:09.000000 agave_pyclient-1.6.2/agave_pyclient.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 23:55:09.000000 agave_pyclient-1.6.2/agave_pyclient.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)      746 2024-04-15 23:55:09.000000 agave_pyclient-1.6.2/agave_pyclient.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       15 2024-04-15 23:55:09.000000 agave_pyclient-1.6.2/agave_pyclient.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 23:55:09.532125 agave_pyclient-1.6.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (127)      615 2024-04-15 23:55:02.000000 agave_pyclient-1.6.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (127)      119 2024-04-15 23:55:02.000000 agave_pyclient-1.6.2/docs/agave_renderer.rst
+-rwxr-xr-x   0 runner    (1001) docker     (127)     5379 2024-04-15 23:55:02.000000 agave_pyclient-1.6.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1122 2024-04-15 23:55:02.000000 agave_pyclient-1.6.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      776 2024-04-15 23:55:02.000000 agave_pyclient-1.6.2/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (127)      482 2024-04-15 23:55:09.536125 agave_pyclient-1.6.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     2619 2024-04-15 23:55:02.000000 agave_pyclient-1.6.2/setup.py
```

### Comparing `agave_pyclient-1.6.1/CONTRIBUTING.md` & `agave_pyclient-1.6.2/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `agave_pyclient-1.6.1/LICENSE` & `agave_pyclient-1.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `agave_pyclient-1.6.1/PKG-INFO` & `agave_pyclient-1.6.2/agave_pyclient.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: agave_pyclient
-Version: 1.6.1
+Name: agave-pyclient
+Version: 1.6.2
 Summary: A Python client for the Agave 3d volume renderer
 Home-page: https://github.com/allen-cell-animated/agave
 Author: Daniel Toloudis
 Author-email: danielt@alleninstitute.org
 License: Allen Institute Software License
 Keywords: agave_pyclient
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `agave_pyclient-1.6.1/README.md` & `agave_pyclient-1.6.2/README.md`

 * *Files identical despite different names*

### Comparing `agave_pyclient-1.6.1/agave_pyclient/agave.py` & `agave_pyclient-1.6.2/agave_pyclient/agave.py`

 * *Files identical despite different names*

### Comparing `agave_pyclient-1.6.1/agave_pyclient/commandbuffer.py` & `agave_pyclient-1.6.2/agave_pyclient/commandbuffer.py`

 * *Files identical despite different names*

### Comparing `agave_pyclient-1.6.1/agave_pyclient.egg-info/PKG-INFO` & `agave_pyclient-1.6.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: agave-pyclient
-Version: 1.6.1
+Name: agave_pyclient
+Version: 1.6.2
 Summary: A Python client for the Agave 3d volume renderer
 Home-page: https://github.com/allen-cell-animated/agave
 Author: Daniel Toloudis
 Author-email: danielt@alleninstitute.org
 License: Allen Institute Software License
 Keywords: agave_pyclient
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `agave_pyclient-1.6.1/agave_pyclient.egg-info/requires.txt` & `agave_pyclient-1.6.2/agave_pyclient.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `agave_pyclient-1.6.1/docs/Makefile` & `agave_pyclient-1.6.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `agave_pyclient-1.6.1/docs/conf.py` & `agave_pyclient-1.6.2/docs/conf.py`

 * *Files 2% similar despite different names*

```diff
@@ -74,15 +74,15 @@
 author = u"Daniel Toloudis"
 
 # The version info for the project you"re documenting, acts as replacement
 # for |version| and |release|, also used in various other places throughout
 # the built documents.
 #
 # The full version, including alpha/beta/rc tags
-release = "1.6.1"
+release = "1.6.2"
 
 # The language for content autogenerated by Sphinx. Refer to documentation
 # for a list of supported languages.
 #
 # This is also used if you do content translation via gettext catalogs.
 # Usually you set "language" from the command line for these cases.
 language = None
```

### Comparing `agave_pyclient-1.6.1/docs/index.rst` & `agave_pyclient-1.6.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `agave_pyclient-1.6.1/docs/make.bat` & `agave_pyclient-1.6.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `agave_pyclient-1.6.1/setup.py` & `agave_pyclient-1.6.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -79,10 +79,10 @@
     setup_requires=setup_requirements,
     test_suite="agave_pyclient/tests",
     tests_require=test_requirements,
     extras_require=extra_requirements,
     url="https://github.com/allen-cell-animated/agave",
     # Do not edit this string manually, always use bumpversion
     # Details in CONTRIBUTING.rst
-    version="1.6.1",
+    version="1.6.2",
     zip_safe=False,
 )
```

