# Comparing `tmp/monteprediction-1.0.3.tar.gz` & `tmp/monteprediction-1.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "monteprediction-1.0.3.tar", last modified: Wed Apr 10 03:36:47 2024, max compression
+gzip compressed data, was "monteprediction-1.0.5.tar", last modified: Tue Apr 16 00:15:21 2024, max compression
```

## Comparing `monteprediction-1.0.3.tar` & `monteprediction-1.0.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:36:47.065123 monteprediction-1.0.3/
--rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-10 03:36:36.000000 monteprediction-1.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-10 03:36:47.065123 monteprediction-1.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-10 03:36:36.000000 monteprediction-1.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:36:47.061123 monteprediction-1.0.3/monteprediction/
--rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-10 03:36:36.000000 monteprediction-1.0.3/monteprediction/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-10 03:36:36.000000 monteprediction-1.0.3/monteprediction/api.py
--rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-10 03:36:36.000000 monteprediction-1.0.3/monteprediction/calendarutil.py
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-10 03:36:36.000000 monteprediction-1.0.3/monteprediction/scoring.py
--rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-04-10 03:36:36.000000 monteprediction-1.0.3/monteprediction/submission.py
--rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-10 03:36:36.000000 monteprediction-1.0.3/monteprediction/truth.py
--rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-10 03:36:36.000000 monteprediction-1.0.3/monteprediction/verification.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:36:47.065123 monteprediction-1.0.3/monteprediction.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-10 03:36:47.000000 monteprediction-1.0.3/monteprediction.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-10 03:36:47.000000 monteprediction-1.0.3/monteprediction.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-10 03:36:47.000000 monteprediction-1.0.3/monteprediction.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-10 03:36:47.000000 monteprediction-1.0.3/monteprediction.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-10 03:36:47.000000 monteprediction-1.0.3/monteprediction.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-10 03:36:47.000000 monteprediction-1.0.3/monteprediction.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-10 03:36:47.065123 monteprediction-1.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-10 03:36:36.000000 monteprediction-1.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-10 03:36:47.065123 monteprediction-1.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-04-10 03:36:36.000000 monteprediction-1.0.3/tests/test_calendarutil.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 00:15:21.193455 monteprediction-1.0.5/
+-rw-r--r--   0 runner    (1001) docker     (127)     1069 2024-04-16 00:15:13.000000 monteprediction-1.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-16 00:15:21.193455 monteprediction-1.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-16 00:15:13.000000 monteprediction-1.0.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 00:15:21.193455 monteprediction-1.0.5/monteprediction/
+-rw-r--r--   0 runner    (1001) docker     (127)      236 2024-04-16 00:15:13.000000 monteprediction-1.0.5/monteprediction/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      275 2024-04-16 00:15:13.000000 monteprediction-1.0.5/monteprediction/api.py
+-rw-r--r--   0 runner    (1001) docker     (127)      505 2024-04-16 00:15:13.000000 monteprediction-1.0.5/monteprediction/calendarutil.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-16 00:15:13.000000 monteprediction-1.0.5/monteprediction/scoring.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1557 2024-04-16 00:15:13.000000 monteprediction-1.0.5/monteprediction/submission.py
+-rw-r--r--   0 runner    (1001) docker     (127)      528 2024-04-16 00:15:13.000000 monteprediction-1.0.5/monteprediction/truth.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1061 2024-04-16 00:15:13.000000 monteprediction-1.0.5/monteprediction/verification.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 00:15:21.193455 monteprediction-1.0.5/monteprediction.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)      565 2024-04-16 00:15:21.000000 monteprediction-1.0.5/monteprediction.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      486 2024-04-16 00:15:21.000000 monteprediction-1.0.5/monteprediction.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 00:15:21.000000 monteprediction-1.0.5/monteprediction.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       66 2024-04-16 00:15:21.000000 monteprediction-1.0.5/monteprediction.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-16 00:15:21.000000 monteprediction-1.0.5/monteprediction.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       16 2024-04-16 00:15:21.000000 monteprediction-1.0.5/monteprediction.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 00:15:21.193455 monteprediction-1.0.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-16 00:15:13.000000 monteprediction-1.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 00:15:21.193455 monteprediction-1.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-04-16 00:15:13.000000 monteprediction-1.0.5/tests/test_calendarutil.py
```

### Comparing `monteprediction-1.0.3/LICENSE` & `monteprediction-1.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `monteprediction-1.0.3/PKG-INFO` & `monteprediction-1.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monteprediction
-Version: 1.0.3
+Version: 1.0.5
 Summary: A Weekly Monte Carlo Game
 Home-page: https://github.com/microprediction/monteprediction
 Author: microprediction
 Author-email: peter.cotton@microprediction.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `monteprediction-1.0.3/monteprediction/submission.py` & `monteprediction-1.0.5/monteprediction/submission.py`

 * *Files identical despite different names*

### Comparing `monteprediction-1.0.3/monteprediction/truth.py` & `monteprediction-1.0.5/monteprediction/truth.py`

 * *Files identical despite different names*

### Comparing `monteprediction-1.0.3/monteprediction/verification.py` & `monteprediction-1.0.5/monteprediction/verification.py`

 * *Files identical despite different names*

### Comparing `monteprediction-1.0.3/monteprediction.egg-info/PKG-INFO` & `monteprediction-1.0.5/monteprediction.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: monteprediction
-Version: 1.0.3
+Version: 1.0.5
 Summary: A Weekly Monte Carlo Game
 Home-page: https://github.com/microprediction/monteprediction
 Author: microprediction
 Author-email: peter.cotton@microprediction.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `monteprediction-1.0.3/setup.py` & `monteprediction-1.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 HERE = pathlib.Path(__file__).parent
 
 README = (HERE / "README.md").read_text()
 
 setup(
     name="monteprediction",
-    version="1.0.3",
+    version="1.0.5",
     description="A Weekly Monte Carlo Game",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/microprediction/monteprediction",
     author="microprediction",
     author_email="peter.cotton@microprediction.com",
     license="MIT",
```

### Comparing `monteprediction-1.0.3/tests/test_calendarutil.py` & `monteprediction-1.0.5/tests/test_calendarutil.py`

 * *Files identical despite different names*

