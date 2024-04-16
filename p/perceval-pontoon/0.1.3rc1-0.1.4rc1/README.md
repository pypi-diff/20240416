# Comparing `tmp/perceval_pontoon-0.1.3rc1.tar.gz` & `tmp/perceval_pontoon-0.1.4rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "perceval_pontoon-0.1.3rc1.tar", max compression
+gzip compressed data, was "perceval_pontoon-0.1.4rc1.tar", max compression
```

## Comparing `perceval_pontoon-0.1.3rc1.tar` & `perceval_pontoon-0.1.4rc1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0       50 2024-03-27 15:45:56.930268 perceval_pontoon-0.1.3rc1/AUTHORS
--rw-r--r--   0        0        0    35149 2024-03-27 15:45:56.934268 perceval_pontoon-0.1.3rc1/LICENSE
--rw-r--r--   0        0        0      885 2024-03-27 15:45:56.934268 perceval_pontoon-0.1.3rc1/NEWS
--rw-r--r--   0        0        0     2301 2024-03-27 15:45:56.934268 perceval_pontoon-0.1.3rc1/README.md
--rw-r--r--   0        0        0        0 2024-03-27 15:45:56.934268 perceval_pontoon-0.1.3rc1/perceval/backends/pontoon/__init__.py
--rw-r--r--   0        0        0       91 2024-03-27 15:45:56.934268 perceval_pontoon-0.1.3rc1/perceval/backends/pontoon/_version.py
--rw-r--r--   0        0        0     9961 2024-03-27 15:45:56.934268 perceval_pontoon-0.1.3rc1/perceval/backends/pontoon/pontoon.py
--rw-r--r--   0        0        0     1380 2024-03-27 15:45:56.934268 perceval_pontoon-0.1.3rc1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-27 15:45:56.934268 perceval_pontoon-0.1.3rc1/tests/__init__.py
--rw-r--r--   0        0        0    10795 2024-03-27 15:45:56.934268 perceval_pontoon-0.1.3rc1/tests/data/pontoon/pontoon_entities.json
--rw-r--r--   0        0        0    11734 2024-03-27 15:45:56.934268 perceval_pontoon-0.1.3rc1/tests/data/pontoon/pontoon_entities_page_1.json
--rw-r--r--   0        0        0     9973 2024-03-27 15:45:56.934268 perceval_pontoon-0.1.3rc1/tests/data/pontoon/pontoon_entities_page_2.json
--rw-r--r--   0        0        0     2110 2024-03-27 15:45:56.934268 perceval_pontoon-0.1.3rc1/tests/data/pontoon/pontoon_history.json
--rw-r--r--   0        0        0      152 2024-03-27 15:45:56.934268 perceval_pontoon-0.1.3rc1/tests/data/pontoon/pontoon_locales.json
--rwxr-xr-x   0        0        0     1021 2024-03-27 15:45:56.934268 perceval_pontoon-0.1.3rc1/tests/run_tests.py
--rw-r--r--   0        0        0    13874 2024-03-27 15:45:56.934268 perceval_pontoon-0.1.3rc1/tests/test_pontoon.py
--rw-r--r--   0        0        0     3385 1970-01-01 00:00:00.000000 perceval_pontoon-0.1.3rc1/PKG-INFO
+-rw-r--r--   0        0        0       50 2024-04-16 08:15:48.414368 perceval_pontoon-0.1.4rc1/AUTHORS
+-rw-r--r--   0        0        0    35149 2024-04-16 08:15:48.414368 perceval_pontoon-0.1.4rc1/LICENSE
+-rw-r--r--   0        0        0     1097 2024-04-16 08:15:48.414368 perceval_pontoon-0.1.4rc1/NEWS
+-rw-r--r--   0        0        0     2301 2024-04-16 08:15:48.414368 perceval_pontoon-0.1.4rc1/README.md
+-rw-r--r--   0        0        0        0 2024-04-16 08:15:48.414368 perceval_pontoon-0.1.4rc1/perceval/backends/pontoon/__init__.py
+-rw-r--r--   0        0        0       91 2024-04-16 08:15:48.414368 perceval_pontoon-0.1.4rc1/perceval/backends/pontoon/_version.py
+-rw-r--r--   0        0        0     9961 2024-04-16 08:15:48.414368 perceval_pontoon-0.1.4rc1/perceval/backends/pontoon/pontoon.py
+-rw-r--r--   0        0        0     1380 2024-04-16 08:15:48.414368 perceval_pontoon-0.1.4rc1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-16 08:15:48.414368 perceval_pontoon-0.1.4rc1/tests/__init__.py
+-rw-r--r--   0        0        0    10795 2024-04-16 08:15:48.414368 perceval_pontoon-0.1.4rc1/tests/data/pontoon/pontoon_entities.json
+-rw-r--r--   0        0        0    11734 2024-04-16 08:15:48.414368 perceval_pontoon-0.1.4rc1/tests/data/pontoon/pontoon_entities_page_1.json
+-rw-r--r--   0        0        0     9973 2024-04-16 08:15:48.414368 perceval_pontoon-0.1.4rc1/tests/data/pontoon/pontoon_entities_page_2.json
+-rw-r--r--   0        0        0     2110 2024-04-16 08:15:48.414368 perceval_pontoon-0.1.4rc1/tests/data/pontoon/pontoon_history.json
+-rw-r--r--   0        0        0      152 2024-04-16 08:15:48.414368 perceval_pontoon-0.1.4rc1/tests/data/pontoon/pontoon_locales.json
+-rwxr-xr-x   0        0        0     1021 2024-04-16 08:15:48.414368 perceval_pontoon-0.1.4rc1/tests/run_tests.py
+-rw-r--r--   0        0        0    13874 2024-04-16 08:15:48.414368 perceval_pontoon-0.1.4rc1/tests/test_pontoon.py
+-rw-r--r--   0        0        0     3385 1970-01-01 00:00:00.000000 perceval_pontoon-0.1.4rc1/PKG-INFO
```

### Comparing `perceval_pontoon-0.1.3rc1/LICENSE` & `perceval_pontoon-0.1.4rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `perceval_pontoon-0.1.3rc1/NEWS` & `perceval_pontoon-0.1.4rc1/NEWS`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,18 @@
 # Releases
 
+## perceval-pontoon 0.1.3 - (2024-04-01)
+
+**Bug fixes:**
+
+ * Pontoon pagination updated\
+   Pontoon improved the pagination for performance. Integrate the recent
+   pagination enhancements in Perceval backend.
+
+
   ## perceval-pontoon 0.1.2 - (2024-03-12)
   
   * Update Poetry's package dependencies
 
   ## perceval-pontoon 0.1.1 - (2024-03-04)
   
   * Update Poetry's package dependencies
```

### Comparing `perceval_pontoon-0.1.3rc1/README.md` & `perceval_pontoon-0.1.4rc1/README.md`

 * *Files identical despite different names*

### Comparing `perceval_pontoon-0.1.3rc1/perceval/backends/pontoon/pontoon.py` & `perceval_pontoon-0.1.4rc1/perceval/backends/pontoon/pontoon.py`

 * *Files identical despite different names*

### Comparing `perceval_pontoon-0.1.3rc1/pyproject.toml` & `perceval_pontoon-0.1.4rc1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "perceval-pontoon"
-version = "0.1.3-rc.1"
+version = "0.1.4-rc.1"
 description = "Perceval backend for Pontoon"
 authors = [
     "Bitergia Developers"
 ]
 license = "GPL-3.0+"
 readme = "README.md"
```

### Comparing `perceval_pontoon-0.1.3rc1/tests/data/pontoon/pontoon_entities.json` & `perceval_pontoon-0.1.4rc1/tests/data/pontoon/pontoon_entities.json`

 * *Files identical despite different names*

### Comparing `perceval_pontoon-0.1.3rc1/tests/data/pontoon/pontoon_entities_page_1.json` & `perceval_pontoon-0.1.4rc1/tests/data/pontoon/pontoon_entities_page_1.json`

 * *Files identical despite different names*

### Comparing `perceval_pontoon-0.1.3rc1/tests/data/pontoon/pontoon_entities_page_2.json` & `perceval_pontoon-0.1.4rc1/tests/data/pontoon/pontoon_entities_page_2.json`

 * *Files identical despite different names*

### Comparing `perceval_pontoon-0.1.3rc1/tests/data/pontoon/pontoon_history.json` & `perceval_pontoon-0.1.4rc1/tests/data/pontoon/pontoon_history.json`

 * *Files identical despite different names*

### Comparing `perceval_pontoon-0.1.3rc1/tests/run_tests.py` & `perceval_pontoon-0.1.4rc1/tests/run_tests.py`

 * *Files identical despite different names*

### Comparing `perceval_pontoon-0.1.3rc1/tests/test_pontoon.py` & `perceval_pontoon-0.1.4rc1/tests/test_pontoon.py`

 * *Files identical despite different names*

### Comparing `perceval_pontoon-0.1.3rc1/PKG-INFO` & `perceval_pontoon-0.1.4rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: perceval-pontoon
-Version: 0.1.3rc1
+Version: 0.1.4rc1
 Summary: Perceval backend for Pontoon
 Home-page: https://chaoss.github.io/grimoirelab/
 License: GPL-3.0+
 Keywords: development,grimoirelab
 Author: Bitergia Developers
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
```

