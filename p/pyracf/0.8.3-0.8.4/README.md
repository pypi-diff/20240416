# Comparing `tmp/pyracf-0.8.3.tar.gz` & `tmp/pyracf-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyracf-0.8.3.tar", last modified: Mon Apr 15 18:27:33 2024, max compression
+gzip compressed data, was "pyracf-0.8.4.tar", last modified: Tue Apr 16 21:33:11 2024, max compression
```

## Comparing `pyracf-0.8.3.tar` & `pyracf-0.8.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxrwxr-x   0 henri     (1000) henri     (1000)        0 2024-04-15 18:27:33.583570 pyracf-0.8.3/
--rw-rw-r--   0 henri     (1000) henri     (1000)    11357 2023-05-01 20:17:28.000000 pyracf-0.8.3/LICENSE
--rw-rw-r--   0 henri     (1000) henri     (1000)      172 2022-04-04 21:07:37.000000 pyracf-0.8.3/MANIFEST.in
--rw-r--r--   0 henri     (1000) henri     (1000)    15118 2024-04-15 18:27:33.583570 pyracf-0.8.3/PKG-INFO
--rw-rw-r--   0 henri     (1000) henri     (1000)    14510 2024-04-15 10:15:48.000000 pyracf-0.8.3/README.md
--rw-rw-r--   0 henri     (1000) henri     (1000)       38 2024-04-15 18:27:33.583570 pyracf-0.8.3/setup.cfg
--rw-rw-r--   0 henri     (1000) henri     (1000)      956 2024-04-15 18:11:35.000000 pyracf-0.8.3/setup.py
-drwxrwxr-x   0 henri     (1000) henri     (1000)        0 2024-04-15 18:27:33.583570 pyracf-0.8.3/src/
-drwxrwxr-x   0 henri     (1000) henri     (1000)        0 2024-04-15 18:27:33.583570 pyracf-0.8.3/src/pyracf/
--rw-rw-r--   0 henri     (1000) henri     (1000)    56953 2024-04-15 18:26:41.000000 pyracf-0.8.3/src/pyracf/__init__.py
--rw-rw-r--   0 henri     (1000) henri     (1000)     1829 2024-04-15 10:15:48.000000 pyracf-0.8.3/src/pyracf/getOffsets.py
--rw-rw-r--   0 henri     (1000) henri     (1000)   253950 2024-04-15 10:15:48.000000 pyracf-0.8.3/src/pyracf/offsets.json
-drwxrwxr-x   0 henri     (1000) henri     (1000)        0 2024-04-15 18:27:33.583570 pyracf-0.8.3/src/pyracf.egg-info/
--rw-r--r--   0 henri     (1000) henri     (1000)    15118 2024-04-15 18:27:33.000000 pyracf-0.8.3/src/pyracf.egg-info/PKG-INFO
--rw-rw-r--   0 henri     (1000) henri     (1000)      279 2024-04-15 18:27:33.000000 pyracf-0.8.3/src/pyracf.egg-info/SOURCES.txt
--rw-rw-r--   0 henri     (1000) henri     (1000)        1 2024-04-15 18:27:33.000000 pyracf-0.8.3/src/pyracf.egg-info/dependency_links.txt
--rw-rw-r--   0 henri     (1000) henri     (1000)       38 2024-04-15 18:27:33.000000 pyracf-0.8.3/src/pyracf.egg-info/requires.txt
--rw-rw-r--   0 henri     (1000) henri     (1000)        7 2024-04-15 18:27:33.000000 pyracf-0.8.3/src/pyracf.egg-info/top_level.txt
+drwxrwxr-x   0 henri     (1000) henri     (1000)        0 2024-04-16 21:33:11.184994 pyracf-0.8.4/
+-rw-rw-r--   0 henri     (1000) henri     (1000)    11357 2023-05-01 20:17:28.000000 pyracf-0.8.4/LICENSE
+-rw-rw-r--   0 henri     (1000) henri     (1000)      172 2022-04-04 21:07:37.000000 pyracf-0.8.4/MANIFEST.in
+-rw-r--r--   0 henri     (1000) henri     (1000)    15118 2024-04-16 21:33:11.184994 pyracf-0.8.4/PKG-INFO
+-rw-rw-r--   0 henri     (1000) henri     (1000)    14510 2024-04-16 21:31:02.000000 pyracf-0.8.4/README.md
+-rw-rw-r--   0 henri     (1000) henri     (1000)       38 2024-04-16 21:33:11.184994 pyracf-0.8.4/setup.cfg
+-rw-rw-r--   0 henri     (1000) henri     (1000)      956 2024-04-16 21:32:36.000000 pyracf-0.8.4/setup.py
+drwxrwxr-x   0 henri     (1000) henri     (1000)        0 2024-04-16 21:33:11.184994 pyracf-0.8.4/src/
+drwxrwxr-x   0 henri     (1000) henri     (1000)        0 2024-04-16 21:33:11.184994 pyracf-0.8.4/src/pyracf/
+-rw-rw-r--   0 henri     (1000) henri     (1000)    56953 2024-04-16 21:31:08.000000 pyracf-0.8.4/src/pyracf/__init__.py
+-rw-rw-r--   0 henri     (1000) henri     (1000)     1829 2024-04-15 10:15:48.000000 pyracf-0.8.4/src/pyracf/getOffsets.py
+-rw-rw-r--   0 henri     (1000) henri     (1000)   253950 2024-04-15 10:15:48.000000 pyracf-0.8.4/src/pyracf/offsets.json
+drwxrwxr-x   0 henri     (1000) henri     (1000)        0 2024-04-16 21:33:11.184994 pyracf-0.8.4/src/pyracf.egg-info/
+-rw-r--r--   0 henri     (1000) henri     (1000)    15118 2024-04-16 21:33:11.000000 pyracf-0.8.4/src/pyracf.egg-info/PKG-INFO
+-rw-rw-r--   0 henri     (1000) henri     (1000)      279 2024-04-16 21:33:11.000000 pyracf-0.8.4/src/pyracf.egg-info/SOURCES.txt
+-rw-rw-r--   0 henri     (1000) henri     (1000)        1 2024-04-16 21:33:11.000000 pyracf-0.8.4/src/pyracf.egg-info/dependency_links.txt
+-rw-rw-r--   0 henri     (1000) henri     (1000)       38 2024-04-16 21:33:11.000000 pyracf-0.8.4/src/pyracf.egg-info/requires.txt
+-rw-rw-r--   0 henri     (1000) henri     (1000)        7 2024-04-16 21:33:11.000000 pyracf-0.8.4/src/pyracf.egg-info/top_level.txt
```

### Comparing `pyracf-0.8.3/LICENSE` & `pyracf-0.8.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pyracf-0.8.3/PKG-INFO` & `pyracf-0.8.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyracf
-Version: 0.8.3
+Version: 0.8.4
 Summary: Parsing IRRDBU00 unloads in panda dataframes.
 Home-page: https://github.com/wizardofzos/pyracf
 Author: Wizard of z/OS
 Author-email: wizard@zdevops.com
 Project-URL: Bug Tracker, https://github.com/wizardofzos/pyracf/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `pyracf-0.8.3/README.md` & `pyracf-0.8.4/README.md`

 * *Files identical despite different names*

### Comparing `pyracf-0.8.3/setup.py` & `pyracf-0.8.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pyracf",
-    version="0.8.3",
+    version="0.8.4",
     author="Wizard of z/OS",
     author_email="wizard@zdevops.com",
     description="Parsing IRRDBU00 unloads in panda dataframes.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/wizardofzos/pyracf",
     project_urls={
```

### Comparing `pyracf-0.8.3/src/pyracf/__init__.py` & `pyracf-0.8.4/src/pyracf/__init__.py`

 * *Files identical despite different names*

### Comparing `pyracf-0.8.3/src/pyracf/getOffsets.py` & `pyracf-0.8.4/src/pyracf/getOffsets.py`

 * *Files identical despite different names*

### Comparing `pyracf-0.8.3/src/pyracf/offsets.json` & `pyracf-0.8.4/src/pyracf/offsets.json`

 * *Files identical despite different names*

### Comparing `pyracf-0.8.3/src/pyracf.egg-info/PKG-INFO` & `pyracf-0.8.4/src/pyracf.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyracf
-Version: 0.8.3
+Version: 0.8.4
 Summary: Parsing IRRDBU00 unloads in panda dataframes.
 Home-page: https://github.com/wizardofzos/pyracf
 Author: Wizard of z/OS
 Author-email: wizard@zdevops.com
 Project-URL: Bug Tracker, https://github.com/wizardofzos/pyracf/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
```

