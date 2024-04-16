# Comparing `tmp/anls_star-0.0.7.tar.gz` & `tmp/anls_star-0.0.8.tar.gz`

## Comparing `anls_star-0.0.7.tar` & `anls_star-0.0.8.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 anls_star-0.0.7/src/__init__.py
--rw-r--r--   0        0        0    11795 2020-02-02 00:00:00.000000 anls_star-0.0.7/src/anls_star.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 anls_star-0.0.7/tests/__init__.py
--rw-r--r--   0        0        0    13806 2020-02-02 00:00:00.000000 anls_star-0.0.7/tests/test_anls_star.py
--rw-r--r--   0        0        0     3135 2020-02-02 00:00:00.000000 anls_star-0.0.7/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 anls_star-0.0.7/LICENSE
--rw-r--r--   0        0        0     8115 2020-02-02 00:00:00.000000 anls_star-0.0.7/README.md
--rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 anls_star-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     8812 2020-02-02 00:00:00.000000 anls_star-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 anls_star-0.0.8/src/__init__.py
+-rw-r--r--   0        0        0    11795 2020-02-02 00:00:00.000000 anls_star-0.0.8/src/anls_star.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 anls_star-0.0.8/tests/__init__.py
+-rw-r--r--   0        0        0    13806 2020-02-02 00:00:00.000000 anls_star-0.0.8/tests/test_anls_star.py
+-rw-r--r--   0        0        0     3135 2020-02-02 00:00:00.000000 anls_star-0.0.8/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 anls_star-0.0.8/LICENSE
+-rw-r--r--   0        0        0     4469 2020-02-02 00:00:00.000000 anls_star-0.0.8/README.md
+-rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 anls_star-0.0.8/pyproject.toml
+-rw-r--r--   0        0        0     5166 2020-02-02 00:00:00.000000 anls_star-0.0.8/PKG-INFO
```

### Comparing `anls_star-0.0.7/src/anls_star.py` & `anls_star-0.0.8/src/anls_star.py`

 * *Files identical despite different names*

### Comparing `anls_star-0.0.7/tests/test_anls_star.py` & `anls_star-0.0.8/tests/test_anls_star.py`

 * *Files identical despite different names*

### Comparing `anls_star-0.0.7/.gitignore` & `anls_star-0.0.8/.gitignore`

 * *Files identical despite different names*

### Comparing `anls_star-0.0.7/LICENSE` & `anls_star-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `anls_star-0.0.7/pyproject.toml` & `anls_star-0.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 
 [project]
 name = "anls_star"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="David Peer", email="david.peer@deepopinion.ai" },
 ]
 description = "A universal metric for Generative Large Language Models (GLLMs)"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

