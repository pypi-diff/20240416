# Comparing `tmp/trial_IGNchinmay-0.0.8.tar.gz` & `tmp/trial_IGNchinmay-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trial_IGNchinmay-0.0.8.tar", last modified: Fri Apr 12 09:38:36 2024, max compression
+gzip compressed data, was "trial_IGNchinmay-0.0.9.tar", last modified: Fri Apr 12 09:47:04 2024, max compression
```

## Comparing `trial_IGNchinmay-0.0.8.tar` & `trial_IGNchinmay-0.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (996)        0 2024-04-12 09:38:36.412973 trial_IGNchinmay-0.0.8/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (996)    11356 2024-04-11 07:03:53.000000 trial_IGNchinmay-0.0.8/LICENSE
--rw-r--r--   0 gitlab-runner   (997) gitlab-runner   (996)      828 2024-04-12 09:38:36.412973 trial_IGNchinmay-0.0.8/PKG-INFO
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (996)      210 2024-04-11 11:08:55.000000 trial_IGNchinmay-0.0.8/README.md
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (996)      688 2024-04-12 09:37:40.000000 trial_IGNchinmay-0.0.8/pyproject.toml
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (996)       38 2024-04-12 09:38:36.412973 trial_IGNchinmay-0.0.8/setup.cfg
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (996)        0 2024-04-12 09:38:36.412973 trial_IGNchinmay-0.0.8/trial_IGNchinmay/
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (996)       41 2024-04-11 07:03:53.000000 trial_IGNchinmay-0.0.8/trial_IGNchinmay/__init__.py
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (996)     3058 2024-04-11 16:19:19.000000 trial_IGNchinmay-0.0.8/trial_IGNchinmay/json_utils.py
-drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (996)        0 2024-04-12 09:38:36.412973 trial_IGNchinmay-0.0.8/trial_IGNchinmay.egg-info/
--rw-r--r--   0 gitlab-runner   (997) gitlab-runner   (996)      828 2024-04-12 09:38:36.000000 trial_IGNchinmay-0.0.8/trial_IGNchinmay.egg-info/PKG-INFO
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (996)      252 2024-04-12 09:38:36.000000 trial_IGNchinmay-0.0.8/trial_IGNchinmay.egg-info/SOURCES.txt
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (996)        1 2024-04-12 09:38:36.000000 trial_IGNchinmay-0.0.8/trial_IGNchinmay.egg-info/dependency_links.txt
--rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (996)       17 2024-04-12 09:38:36.000000 trial_IGNchinmay-0.0.8/trial_IGNchinmay.egg-info/top_level.txt
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (996)        0 2024-04-12 09:47:04.531630 trial_IGNchinmay-0.0.9/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (996)    11356 2024-04-11 07:03:53.000000 trial_IGNchinmay-0.0.9/LICENSE
+-rw-r--r--   0 gitlab-runner   (997) gitlab-runner   (996)      828 2024-04-12 09:47:04.531630 trial_IGNchinmay-0.0.9/PKG-INFO
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (996)      210 2024-04-11 11:08:55.000000 trial_IGNchinmay-0.0.9/README.md
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (996)      688 2024-04-12 09:46:20.000000 trial_IGNchinmay-0.0.9/pyproject.toml
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (996)       38 2024-04-12 09:47:04.531630 trial_IGNchinmay-0.0.9/setup.cfg
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (996)        0 2024-04-12 09:47:04.527630 trial_IGNchinmay-0.0.9/trial_IGNchinmay/
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (996)       41 2024-04-11 07:03:53.000000 trial_IGNchinmay-0.0.9/trial_IGNchinmay/__init__.py
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (996)     3058 2024-04-11 16:19:19.000000 trial_IGNchinmay-0.0.9/trial_IGNchinmay/json_utils.py
+drwxrwxr-x   0 gitlab-runner   (997) gitlab-runner   (996)        0 2024-04-12 09:47:04.531630 trial_IGNchinmay-0.0.9/trial_IGNchinmay.egg-info/
+-rw-r--r--   0 gitlab-runner   (997) gitlab-runner   (996)      828 2024-04-12 09:47:04.000000 trial_IGNchinmay-0.0.9/trial_IGNchinmay.egg-info/PKG-INFO
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (996)      252 2024-04-12 09:47:04.000000 trial_IGNchinmay-0.0.9/trial_IGNchinmay.egg-info/SOURCES.txt
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (996)        1 2024-04-12 09:47:04.000000 trial_IGNchinmay-0.0.9/trial_IGNchinmay.egg-info/dependency_links.txt
+-rw-rw-r--   0 gitlab-runner   (997) gitlab-runner   (996)       17 2024-04-12 09:47:04.000000 trial_IGNchinmay-0.0.9/trial_IGNchinmay.egg-info/top_level.txt
```

### Comparing `trial_IGNchinmay-0.0.8/LICENSE` & `trial_IGNchinmay-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `trial_IGNchinmay-0.0.8/PKG-INFO` & `trial_IGNchinmay-0.0.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trial_IGNchinmay
-Version: 0.0.8
+Version: 0.0.9
 Summary: A small CV test package
 Author-email: Chinmay <chinmayananda.sahu@ignitarium.com>
 Project-URL: Homepage, https://gitlab.ignitarium.in/ign-ai/internal/ign_py_library/trial_IGNchinmay/-/tree/main?ref_type=heads
 Project-URL: Issues, https://gitlab.ignitarium.in/ign-ai/internal/ign_py_library/trial_IGNchinmay/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `trial_IGNchinmay-0.0.8/pyproject.toml` & `trial_IGNchinmay-0.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "trial_IGNchinmay"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="Chinmay", email="chinmayananda.sahu@ignitarium.com" },
 ]
 description = "A small CV test package"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `trial_IGNchinmay-0.0.8/trial_IGNchinmay/json_utils.py` & `trial_IGNchinmay-0.0.9/trial_IGNchinmay/json_utils.py`

 * *Files identical despite different names*

### Comparing `trial_IGNchinmay-0.0.8/trial_IGNchinmay.egg-info/PKG-INFO` & `trial_IGNchinmay-0.0.9/trial_IGNchinmay.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trial_IGNchinmay
-Version: 0.0.8
+Version: 0.0.9
 Summary: A small CV test package
 Author-email: Chinmay <chinmayananda.sahu@ignitarium.com>
 Project-URL: Homepage, https://gitlab.ignitarium.in/ign-ai/internal/ign_py_library/trial_IGNchinmay/-/tree/main?ref_type=heads
 Project-URL: Issues, https://gitlab.ignitarium.in/ign-ai/internal/ign_py_library/trial_IGNchinmay/-/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

