# Comparing `tmp/perceval_public_inbox-0.1.9.tar.gz` & `tmp/perceval_public_inbox-0.1.9rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "perceval_public_inbox-0.1.9.tar", max compression
+gzip compressed data, was "perceval_public_inbox-0.1.9rc1.tar", max compression
```

## Comparing `perceval_public_inbox-0.1.9.tar` & `perceval_public_inbox-0.1.9rc1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0       87 2024-01-31 15:17:08.147202 perceval_public_inbox-0.1.9/AUTHORS
--rw-r--r--   0        0        0    35149 2024-01-31 15:17:08.147202 perceval_public_inbox-0.1.9/LICENSE
--rw-r--r--   0        0        0     1261 2024-01-31 15:17:08.147202 perceval_public_inbox-0.1.9/NEWS
--rw-r--r--   0        0        0     2291 2024-01-31 15:17:08.147202 perceval_public_inbox-0.1.9/README.md
--rw-r--r--   0        0        0        0 2024-01-31 15:17:08.147202 perceval_public_inbox-0.1.9/perceval/backends/public_inbox/__init__.py
--rw-r--r--   0        0        0       86 2024-01-31 15:17:08.147202 perceval_public_inbox-0.1.9/perceval/backends/public_inbox/_version.py
--rw-r--r--   0        0        0    12428 2024-01-31 15:17:08.147202 perceval_public_inbox-0.1.9/perceval/backends/public_inbox/public_inbox.py
--rw-r--r--   0        0        0     1429 2024-01-31 15:17:08.147202 perceval_public_inbox-0.1.9/pyproject.toml
--rw-r--r--   0        0        0    53248 2024-01-31 15:17:08.147202 perceval_public_inbox-0.1.9/tests/.coverage
--rw-r--r--   0        0        0        0 2024-01-31 15:17:08.147202 perceval_public_inbox-0.1.9/tests/__init__.py
--rw-r--r--   0        0        0    77686 2024-01-31 15:17:08.151202 perceval_public_inbox-0.1.9/tests/data/public_inbox/alternate-repos.tar.gz
--rw-r--r--   0        0        0    18463 2024-01-31 15:17:08.151202 perceval_public_inbox-0.1.9/tests/data/public_inbox/example-repo.git.tar.gz
--rwxr-xr-x   0        0        0     1017 2024-01-31 15:17:08.151202 perceval_public_inbox-0.1.9/tests/run_tests.py
--rw-r--r--   0        0        0    18717 2024-01-31 15:17:08.151202 perceval_public_inbox-0.1.9/tests/test_public_inbox.py
--rw-r--r--   0        0        0     3479 1970-01-01 00:00:00.000000 perceval_public_inbox-0.1.9/PKG-INFO
+-rw-r--r--   0        0        0       87 2024-01-31 11:19:59.158864 perceval_public_inbox-0.1.9rc1/AUTHORS
+-rw-r--r--   0        0        0    35149 2024-01-31 11:19:59.158864 perceval_public_inbox-0.1.9rc1/LICENSE
+-rw-r--r--   0        0        0     1168 2024-01-31 11:19:59.158864 perceval_public_inbox-0.1.9rc1/NEWS
+-rw-r--r--   0        0        0     2291 2024-01-31 11:19:59.158864 perceval_public_inbox-0.1.9rc1/README.md
+-rw-r--r--   0        0        0        0 2024-01-31 11:19:59.158864 perceval_public_inbox-0.1.9rc1/perceval/backends/public_inbox/__init__.py
+-rw-r--r--   0        0        0       91 2024-01-31 11:19:59.158864 perceval_public_inbox-0.1.9rc1/perceval/backends/public_inbox/_version.py
+-rw-r--r--   0        0        0    12428 2024-01-31 11:19:59.158864 perceval_public_inbox-0.1.9rc1/perceval/backends/public_inbox/public_inbox.py
+-rw-r--r--   0        0        0     1434 2024-01-31 11:19:59.158864 perceval_public_inbox-0.1.9rc1/pyproject.toml
+-rw-r--r--   0        0        0    53248 2024-01-31 11:19:59.162864 perceval_public_inbox-0.1.9rc1/tests/.coverage
+-rw-r--r--   0        0        0        0 2024-01-31 11:19:59.162864 perceval_public_inbox-0.1.9rc1/tests/__init__.py
+-rw-r--r--   0        0        0    77686 2024-01-31 11:19:59.162864 perceval_public_inbox-0.1.9rc1/tests/data/public_inbox/alternate-repos.tar.gz
+-rw-r--r--   0        0        0    18463 2024-01-31 11:19:59.162864 perceval_public_inbox-0.1.9rc1/tests/data/public_inbox/example-repo.git.tar.gz
+-rwxr-xr-x   0        0        0     1017 2024-01-31 11:19:59.162864 perceval_public_inbox-0.1.9rc1/tests/run_tests.py
+-rw-r--r--   0        0        0    18717 2024-01-31 11:19:59.162864 perceval_public_inbox-0.1.9rc1/tests/test_public_inbox.py
+-rw-r--r--   0        0        0     3482 1970-01-01 00:00:00.000000 perceval_public_inbox-0.1.9rc1/PKG-INFO
```

### Comparing `perceval_public_inbox-0.1.9/LICENSE` & `perceval_public_inbox-0.1.9rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `perceval_public_inbox-0.1.9/NEWS` & `perceval_public_inbox-0.1.9rc1/NEWS`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,9 @@
 # Releases
 
-  ## perceval-public-inbox 0.1.9 - (2024-01-31)
-  
-  * Update Poetry's package dependencies
-
   ## perceval-public-inbox 0.1.8 - (2023-12-26)
   
   * Update Poetry's package dependencies
 
   ## perceval-public-inbox 0.1.7 - (2023-11-17)
   
   * Update Poetry's package dependencies
```

### Comparing `perceval_public_inbox-0.1.9/README.md` & `perceval_public_inbox-0.1.9rc1/README.md`

 * *Files identical despite different names*

### Comparing `perceval_public_inbox-0.1.9/perceval/backends/public_inbox/public_inbox.py` & `perceval_public_inbox-0.1.9rc1/perceval/backends/public_inbox/public_inbox.py`

 * *Files identical despite different names*

### Comparing `perceval_public_inbox-0.1.9/pyproject.toml` & `perceval_public_inbox-0.1.9rc1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "perceval-public-inbox"
-version = "0.1.9"
+version = "0.1.9-rc.1"
 description = "Perceval backend for public-inbox."
 authors = [
     "GrimoireLab Developers"
 ]
 license = "GPL-3.0+"
 
 readme = "README.md"
```

### Comparing `perceval_public_inbox-0.1.9/tests/.coverage` & `perceval_public_inbox-0.1.9rc1/tests/.coverage`

 * *Files identical despite different names*

### Comparing `perceval_public_inbox-0.1.9/tests/data/public_inbox/alternate-repos.tar.gz` & `perceval_public_inbox-0.1.9rc1/tests/data/public_inbox/alternate-repos.tar.gz`

 * *Files identical despite different names*

### Comparing `perceval_public_inbox-0.1.9/tests/data/public_inbox/example-repo.git.tar.gz` & `perceval_public_inbox-0.1.9rc1/tests/data/public_inbox/example-repo.git.tar.gz`

 * *Files identical despite different names*

### Comparing `perceval_public_inbox-0.1.9/tests/run_tests.py` & `perceval_public_inbox-0.1.9rc1/tests/run_tests.py`

 * *Files identical despite different names*

### Comparing `perceval_public_inbox-0.1.9/tests/test_public_inbox.py` & `perceval_public_inbox-0.1.9rc1/tests/test_public_inbox.py`

 * *Files identical despite different names*

### Comparing `perceval_public_inbox-0.1.9/PKG-INFO` & `perceval_public_inbox-0.1.9rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: perceval-public-inbox
-Version: 0.1.9
+Version: 0.1.9rc1
 Summary: Perceval backend for public-inbox.
 Home-page: https://chaoss.github.io/grimoirelab/
 License: GPL-3.0+
 Keywords: development,grimoirelab
 Author: GrimoireLab Developers
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
```

