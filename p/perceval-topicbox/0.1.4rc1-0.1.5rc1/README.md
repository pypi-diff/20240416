# Comparing `tmp/perceval_topicbox-0.1.4rc1.tar.gz` & `tmp/perceval_topicbox-0.1.5rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "perceval_topicbox-0.1.4rc1.tar", max compression
+gzip compressed data, was "perceval_topicbox-0.1.5rc1.tar", max compression
```

## Comparing `perceval_topicbox-0.1.4rc1.tar` & `perceval_topicbox-0.1.5rc1.tar`

### file list

```diff
@@ -1,16 +1,16 @@
--rw-r--r--   0        0        0       50 2024-03-27 15:45:25.326117 perceval_topicbox-0.1.4rc1/AUTHORS
--rw-r--r--   0        0        0    35149 2024-03-27 15:45:25.326117 perceval_topicbox-0.1.4rc1/LICENSE
--rw-r--r--   0        0        0      899 2024-03-27 15:45:25.326117 perceval_topicbox-0.1.4rc1/NEWS
--rw-r--r--   0        0        0     2161 2024-03-27 15:45:25.326117 perceval_topicbox-0.1.4rc1/README.md
--rw-r--r--   0        0        0        0 2024-03-27 15:45:25.326117 perceval_topicbox-0.1.4rc1/perceval/backends/topicbox/__init__.py
--rw-r--r--   0        0        0       91 2024-03-27 15:45:25.326117 perceval_topicbox-0.1.4rc1/perceval/backends/topicbox/_version.py
--rw-r--r--   0        0        0    10326 2024-03-27 15:45:25.326117 perceval_topicbox-0.1.4rc1/perceval/backends/topicbox/topicbox.py
--rw-r--r--   0        0        0     1384 2024-03-27 15:45:25.326117 perceval_topicbox-0.1.4rc1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-27 15:45:25.330117 perceval_topicbox-0.1.4rc1/tests/__init__.py
--rw-r--r--   0        0        0     3456 2024-03-27 15:45:25.330117 perceval_topicbox-0.1.4rc1/tests/data/topicbox/topicbox_groups.json
--rw-r--r--   0        0        0     6696 2024-03-27 15:45:25.330117 perceval_topicbox-0.1.4rc1/tests/data/topicbox/topicbox_messages.json
--rw-r--r--   0        0        0     4732 2024-03-27 15:45:25.330117 perceval_topicbox-0.1.4rc1/tests/data/topicbox/topicbox_messages_page_1.json
--rw-r--r--   0        0        0     2852 2024-03-27 15:45:25.330117 perceval_topicbox-0.1.4rc1/tests/data/topicbox/topicbox_messages_page_2.json
--rwxr-xr-x   0        0        0     1021 2024-03-27 15:45:25.330117 perceval_topicbox-0.1.4rc1/tests/run_tests.py
--rw-r--r--   0        0        0    16236 2024-03-27 15:45:25.330117 perceval_topicbox-0.1.4rc1/tests/test_topicbox.py
--rw-r--r--   0        0        0     3249 1970-01-01 00:00:00.000000 perceval_topicbox-0.1.4rc1/PKG-INFO
+-rw-r--r--   0        0        0       50 2024-04-16 08:13:53.124553 perceval_topicbox-0.1.5rc1/AUTHORS
+-rw-r--r--   0        0        0    35149 2024-04-16 08:13:53.124553 perceval_topicbox-0.1.5rc1/LICENSE
+-rw-r--r--   0        0        0      988 2024-04-16 08:13:53.124553 perceval_topicbox-0.1.5rc1/NEWS
+-rw-r--r--   0        0        0     2161 2024-04-16 08:13:53.124553 perceval_topicbox-0.1.5rc1/README.md
+-rw-r--r--   0        0        0        0 2024-04-16 08:13:53.124553 perceval_topicbox-0.1.5rc1/perceval/backends/topicbox/__init__.py
+-rw-r--r--   0        0        0       91 2024-04-16 08:13:53.124553 perceval_topicbox-0.1.5rc1/perceval/backends/topicbox/_version.py
+-rw-r--r--   0        0        0    10326 2024-04-16 08:13:53.124553 perceval_topicbox-0.1.5rc1/perceval/backends/topicbox/topicbox.py
+-rw-r--r--   0        0        0     1384 2024-04-16 08:13:53.124553 perceval_topicbox-0.1.5rc1/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-16 08:13:53.128553 perceval_topicbox-0.1.5rc1/tests/__init__.py
+-rw-r--r--   0        0        0     3456 2024-04-16 08:13:53.128553 perceval_topicbox-0.1.5rc1/tests/data/topicbox/topicbox_groups.json
+-rw-r--r--   0        0        0     6696 2024-04-16 08:13:53.128553 perceval_topicbox-0.1.5rc1/tests/data/topicbox/topicbox_messages.json
+-rw-r--r--   0        0        0     4732 2024-04-16 08:13:53.128553 perceval_topicbox-0.1.5rc1/tests/data/topicbox/topicbox_messages_page_1.json
+-rw-r--r--   0        0        0     2852 2024-04-16 08:13:53.128553 perceval_topicbox-0.1.5rc1/tests/data/topicbox/topicbox_messages_page_2.json
+-rwxr-xr-x   0        0        0     1021 2024-04-16 08:13:53.128553 perceval_topicbox-0.1.5rc1/tests/run_tests.py
+-rw-r--r--   0        0        0    16236 2024-04-16 08:13:53.128553 perceval_topicbox-0.1.5rc1/tests/test_topicbox.py
+-rw-r--r--   0        0        0     3249 1970-01-01 00:00:00.000000 perceval_topicbox-0.1.5rc1/PKG-INFO
```

### Comparing `perceval_topicbox-0.1.4rc1/LICENSE` & `perceval_topicbox-0.1.5rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `perceval_topicbox-0.1.4rc1/NEWS` & `perceval_topicbox-0.1.5rc1/NEWS`

 * *Files 15% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # Releases
 
+  ## perceval-topicbox 0.1.4 - (2024-04-01)
+  
+  * Update Poetry's package dependencies
+
   ## perceval-topicbox 0.1.3 - (2024-03-12)
   
   * Update Poetry's package dependencies
 
   ## perceval-topicbox 0.1.2 - (2024-03-04)
   
   * Update Poetry's package dependencies
```

### Comparing `perceval_topicbox-0.1.4rc1/README.md` & `perceval_topicbox-0.1.5rc1/README.md`

 * *Files identical despite different names*

### Comparing `perceval_topicbox-0.1.4rc1/perceval/backends/topicbox/topicbox.py` & `perceval_topicbox-0.1.5rc1/perceval/backends/topicbox/topicbox.py`

 * *Files identical despite different names*

### Comparing `perceval_topicbox-0.1.4rc1/pyproject.toml` & `perceval_topicbox-0.1.5rc1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "perceval-topicbox"
-version = "0.1.4-rc.1"
+version = "0.1.5-rc.1"
 description = "Perceval backend for Topicbox"
 authors = [
     "Bitergia Developers"
 ]
 license = "GPL-3.0+"
 readme = "README.md"
```

### Comparing `perceval_topicbox-0.1.4rc1/tests/data/topicbox/topicbox_groups.json` & `perceval_topicbox-0.1.5rc1/tests/data/topicbox/topicbox_groups.json`

 * *Files identical despite different names*

### Comparing `perceval_topicbox-0.1.4rc1/tests/data/topicbox/topicbox_messages.json` & `perceval_topicbox-0.1.5rc1/tests/data/topicbox/topicbox_messages.json`

 * *Files identical despite different names*

### Comparing `perceval_topicbox-0.1.4rc1/tests/data/topicbox/topicbox_messages_page_1.json` & `perceval_topicbox-0.1.5rc1/tests/data/topicbox/topicbox_messages_page_1.json`

 * *Files identical despite different names*

### Comparing `perceval_topicbox-0.1.4rc1/tests/data/topicbox/topicbox_messages_page_2.json` & `perceval_topicbox-0.1.5rc1/tests/data/topicbox/topicbox_messages_page_2.json`

 * *Files identical despite different names*

### Comparing `perceval_topicbox-0.1.4rc1/tests/run_tests.py` & `perceval_topicbox-0.1.5rc1/tests/run_tests.py`

 * *Files identical despite different names*

### Comparing `perceval_topicbox-0.1.4rc1/tests/test_topicbox.py` & `perceval_topicbox-0.1.5rc1/tests/test_topicbox.py`

 * *Files identical despite different names*

### Comparing `perceval_topicbox-0.1.4rc1/PKG-INFO` & `perceval_topicbox-0.1.5rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: perceval-topicbox
-Version: 0.1.4rc1
+Version: 0.1.5rc1
 Summary: Perceval backend for Topicbox
 Home-page: https://chaoss.github.io/grimoirelab/
 License: GPL-3.0+
 Keywords: development,grimoirelab
 Author: Bitergia Developers
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
```

