# Comparing `tmp/shares-3.1.8.tar.gz` & `tmp/shares-3.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shares-3.1.8.tar", last modified: Thu Feb  1 06:07:13 2024, max compression
+gzip compressed data, was "shares-3.1.9.tar", last modified: Thu Feb  1 06:12:23 2024, max compression
```

## Comparing `shares-3.1.8.tar` & `shares-3.1.9.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 veganeco  (1000) veganeco  (1000)        0 2024-02-01 06:07:13.408573 shares-3.1.8/
--rw-r--r--   0 veganeco  (1000) veganeco  (1000)     3642 2024-02-01 06:07:13.408573 shares-3.1.8/PKG-INFO
-drwxr-xr-x   0 veganeco  (1000) veganeco  (1000)        0 2024-02-01 06:07:13.399574 shares-3.1.8/lands/
-drwxr-xr-x   0 veganeco  (1000) veganeco  (1000)        0 2024-02-01 06:07:13.399574 shares-3.1.8/lands/structures_local/
-drwxr-xr-x   0 veganeco  (1000) veganeco  (1000)        0 2024-02-01 06:07:13.401574 shares-3.1.8/lands/structures_local/shares/
-drwxr-xr-x   0 veganeco  (1000) veganeco  (1000)        0 2024-02-01 06:07:13.402574 shares-3.1.8/lands/structures_local/shares/$ company/
--rw-r--r--   0 veganeco  (1000) veganeco  (1000)     1190 2024-01-27 05:31:08.000000 shares-3.1.8/lands/structures_local/shares/$ company/company.s.HTML
--rw-r--r--   0 veganeco  (1000) veganeco  (1000)     2448 2024-01-31 18:48:00.000000 shares-3.1.8/lands/structures_local/shares/__init__.py
--rw-r--r--   0 veganeco  (1000) veganeco  (1000)     1115 2024-01-31 18:49:47.000000 shares-3.1.8/lands/structures_local/shares/_clique.py
-drwxr-xr-x   0 veganeco  (1000) veganeco  (1000)        0 2024-02-01 06:07:13.403574 shares-3.1.8/lands/structures_local/shares/_license/
--rw-r--r--   0 veganeco  (1000) veganeco  (1000)      180 2023-12-16 19:42:15.000000 shares-3.1.8/lands/structures_local/shares/_license/license.s.HTML
-drwxr-xr-x   0 veganeco  (1000) veganeco  (1000)        0 2024-02-01 06:07:13.403574 shares-3.1.8/lands/structures_local/shares/_status/
-drwxr-xr-x   0 veganeco  (1000) veganeco  (1000)        0 2024-02-01 06:07:13.399574 shares-3.1.8/lands/structures_local/shares/_status/checks/
-drwxr-xr-x   0 veganeco  (1000) veganeco  (1000)        0 2024-02-01 06:07:13.404574 shares-3.1.8/lands/structures_local/shares/_status/checks/1/
-drwxr-xr-x   0 veganeco  (1000) veganeco  (1000)        0 2024-02-01 06:07:13.405573 shares-3.1.8/lands/structures_local/shares/_status/checks/1/shares/
--rw-r--r--   0 veganeco  (1000) veganeco  (1000)       24 2024-01-26 17:38:56.000000 shares-3.1.8/lands/structures_local/shares/_status/checks/1/shares/shares 1.s.HTML
--rw-r--r--   0 veganeco  (1000) veganeco  (1000)       24 2024-01-26 17:38:52.000000 shares-3.1.8/lands/structures_local/shares/_status/checks/1/shares/shares 2.s.HTML
--rw-r--r--   0 veganeco  (1000) veganeco  (1000)      529 2024-01-27 05:29:44.000000 shares-3.1.8/lands/structures_local/shares/_status/checks/1/status_1.py
--rw-r--r--   0 veganeco  (1000) veganeco  (1000)     1227 2024-01-26 17:39:18.000000 shares-3.1.8/lands/structures_local/shares/_status/status.proc.py
-drwxr-xr-x   0 veganeco  (1000) veganeco  (1000)        0 2024-02-01 06:07:13.406574 shares-3.1.8/lands/structures_local/shares/basin/
--rw-r--r--   0 veganeco  (1000) veganeco  (1000)     2544 2024-01-31 18:51:45.000000 shares-3.1.8/lands/structures_local/shares/basin/__init__.py
--rw-r--r--   0 veganeco  (1000) veganeco  (1000)     3550 2024-01-27 06:34:27.000000 shares-3.1.8/lands/structures_local/shares/basin/treasury.py
--rw-r--r--   0 veganeco  (1000) veganeco  (1000)     3222 2024-01-31 19:06:24.000000 shares-3.1.8/lands/structures_local/shares/module.MD
-drwxr-xr-x   0 veganeco  (1000) veganeco  (1000)        0 2024-02-01 06:07:13.400574 shares-3.1.8/lands/structures_local/shares/modules/
-drwxr-xr-x   0 veganeco  (1000) veganeco  (1000)        0 2024-02-01 06:07:13.407574 shares-3.1.8/lands/structures_local/shares/modules/law_dictionary/
--rw-r--r--   0 veganeco  (1000) veganeco  (1000)     2750 2024-01-27 05:26:32.000000 shares-3.1.8/lands/structures_local/shares/modules/law_dictionary/__init__.py
--rw-r--r--   0 veganeco  (1000) veganeco  (1000)      391 2024-01-27 05:13:57.000000 shares-3.1.8/lands/structures_local/shares/modules/law_dictionary/dictionary_laws.s.HTML
--rw-r--r--   0 veganeco  (1000) veganeco  (1000)     1783 2024-01-27 05:13:57.000000 shares-3.1.8/lands/structures_local/shares/modules/law_dictionary/status_1.py
--rw-r--r--   0 veganeco  (1000) veganeco  (1000)     1059 2024-01-27 05:13:57.000000 shares-3.1.8/lands/structures_local/shares/modules/law_dictionary/status_broken_1.py
--rw-r--r--   0 veganeco  (1000) veganeco  (1000)     1651 2024-01-15 04:17:07.000000 shares-3.1.8/lands/structures_local/shares/shares.s.HTML
-drwxr-xr-x   0 veganeco  (1000) veganeco  (1000)        0 2024-02-01 06:07:13.408573 shares-3.1.8/lands/structures_local/shares.egg-info/
--rw-r--r--   0 veganeco  (1000) veganeco  (1000)     3642 2024-02-01 06:07:13.000000 shares-3.1.8/lands/structures_local/shares.egg-info/PKG-INFO
--rw-r--r--   0 veganeco  (1000) veganeco  (1000)     1236 2024-02-01 06:07:13.000000 shares-3.1.8/lands/structures_local/shares.egg-info/SOURCES.txt
--rw-r--r--   0 veganeco  (1000) veganeco  (1000)        1 2024-02-01 06:07:13.000000 shares-3.1.8/lands/structures_local/shares.egg-info/dependency_links.txt
--rw-r--r--   0 veganeco  (1000) veganeco  (1000)       41 2024-02-01 06:07:13.000000 shares-3.1.8/lands/structures_local/shares.egg-info/entry_points.txt
--rw-r--r--   0 veganeco  (1000) veganeco  (1000)       52 2024-02-01 06:07:13.000000 shares-3.1.8/lands/structures_local/shares.egg-info/requires.txt
--rw-r--r--   0 veganeco  (1000) veganeco  (1000)        7 2024-02-01 06:07:13.000000 shares-3.1.8/lands/structures_local/shares.egg-info/top_level.txt
--rw-r--r--   0 veganeco  (1000) veganeco  (1000)     1403 2024-02-01 06:07:09.000000 shares-3.1.8/pyproject.toml
--rw-r--r--   0 veganeco  (1000) veganeco  (1000)       38 2024-02-01 06:07:13.408573 shares-3.1.8/setup.cfg
+drwxr-xr-x   0 veganeco  (1000) veganeco  (1000)        0 2024-02-01 06:12:23.727539 shares-3.1.9/
+-rw-r--r--   0 veganeco  (1000) veganeco  (1000)     3612 2024-02-01 06:12:23.727539 shares-3.1.9/PKG-INFO
+drwxr-xr-x   0 veganeco  (1000) veganeco  (1000)        0 2024-02-01 06:12:23.724539 shares-3.1.9/lands/
+drwxr-xr-x   0 veganeco  (1000) veganeco  (1000)        0 2024-02-01 06:12:23.724539 shares-3.1.9/lands/structures_local/
+drwxr-xr-x   0 veganeco  (1000) veganeco  (1000)        0 2024-02-01 06:12:23.725539 shares-3.1.9/lands/structures_local/shares/
+drwxr-xr-x   0 veganeco  (1000) veganeco  (1000)        0 2024-02-01 06:12:23.725539 shares-3.1.9/lands/structures_local/shares/$ company/
+-rw-r--r--   0 veganeco  (1000) veganeco  (1000)     1190 2024-01-27 05:31:08.000000 shares-3.1.9/lands/structures_local/shares/$ company/company.s.HTML
+-rw-r--r--   0 veganeco  (1000) veganeco  (1000)     2449 2024-02-01 06:09:26.000000 shares-3.1.9/lands/structures_local/shares/__init__.py
+-rw-r--r--   0 veganeco  (1000) veganeco  (1000)     1115 2024-01-31 18:49:47.000000 shares-3.1.9/lands/structures_local/shares/_clique.py
+drwxr-xr-x   0 veganeco  (1000) veganeco  (1000)        0 2024-02-01 06:12:23.726539 shares-3.1.9/lands/structures_local/shares/_license/
+-rw-r--r--   0 veganeco  (1000) veganeco  (1000)      180 2023-12-16 19:42:15.000000 shares-3.1.9/lands/structures_local/shares/_license/license.s.HTML
+drwxr-xr-x   0 veganeco  (1000) veganeco  (1000)        0 2024-02-01 06:12:23.726539 shares-3.1.9/lands/structures_local/shares/_status/
+drwxr-xr-x   0 veganeco  (1000) veganeco  (1000)        0 2024-02-01 06:12:23.724539 shares-3.1.9/lands/structures_local/shares/_status/checks/
+drwxr-xr-x   0 veganeco  (1000) veganeco  (1000)        0 2024-02-01 06:12:23.726539 shares-3.1.9/lands/structures_local/shares/_status/checks/1/
+drwxr-xr-x   0 veganeco  (1000) veganeco  (1000)        0 2024-02-01 06:12:23.726539 shares-3.1.9/lands/structures_local/shares/_status/checks/1/shares/
+-rw-r--r--   0 veganeco  (1000) veganeco  (1000)       24 2024-01-26 17:38:56.000000 shares-3.1.9/lands/structures_local/shares/_status/checks/1/shares/shares 1.s.HTML
+-rw-r--r--   0 veganeco  (1000) veganeco  (1000)       24 2024-01-26 17:38:52.000000 shares-3.1.9/lands/structures_local/shares/_status/checks/1/shares/shares 2.s.HTML
+-rw-r--r--   0 veganeco  (1000) veganeco  (1000)      529 2024-01-27 05:29:44.000000 shares-3.1.9/lands/structures_local/shares/_status/checks/1/status_1.py
+-rw-r--r--   0 veganeco  (1000) veganeco  (1000)     1227 2024-01-26 17:39:18.000000 shares-3.1.9/lands/structures_local/shares/_status/status.proc.py
+drwxr-xr-x   0 veganeco  (1000) veganeco  (1000)        0 2024-02-01 06:12:23.726539 shares-3.1.9/lands/structures_local/shares/basin/
+-rw-r--r--   0 veganeco  (1000) veganeco  (1000)     2544 2024-01-31 18:51:45.000000 shares-3.1.9/lands/structures_local/shares/basin/__init__.py
+-rw-r--r--   0 veganeco  (1000) veganeco  (1000)     3550 2024-01-27 06:34:27.000000 shares-3.1.9/lands/structures_local/shares/basin/treasury.py
+-rw-r--r--   0 veganeco  (1000) veganeco  (1000)     3222 2024-01-31 19:06:24.000000 shares-3.1.9/lands/structures_local/shares/module.MD
+drwxr-xr-x   0 veganeco  (1000) veganeco  (1000)        0 2024-02-01 06:12:23.724539 shares-3.1.9/lands/structures_local/shares/modules/
+drwxr-xr-x   0 veganeco  (1000) veganeco  (1000)        0 2024-02-01 06:12:23.727539 shares-3.1.9/lands/structures_local/shares/modules/law_dictionary/
+-rw-r--r--   0 veganeco  (1000) veganeco  (1000)     2750 2024-01-27 05:26:32.000000 shares-3.1.9/lands/structures_local/shares/modules/law_dictionary/__init__.py
+-rw-r--r--   0 veganeco  (1000) veganeco  (1000)      391 2024-01-27 05:13:57.000000 shares-3.1.9/lands/structures_local/shares/modules/law_dictionary/dictionary_laws.s.HTML
+-rw-r--r--   0 veganeco  (1000) veganeco  (1000)     1783 2024-01-27 05:13:57.000000 shares-3.1.9/lands/structures_local/shares/modules/law_dictionary/status_1.py
+-rw-r--r--   0 veganeco  (1000) veganeco  (1000)     1059 2024-01-27 05:13:57.000000 shares-3.1.9/lands/structures_local/shares/modules/law_dictionary/status_broken_1.py
+-rw-r--r--   0 veganeco  (1000) veganeco  (1000)     1651 2024-01-15 04:17:07.000000 shares-3.1.9/lands/structures_local/shares/shares.s.HTML
+drwxr-xr-x   0 veganeco  (1000) veganeco  (1000)        0 2024-02-01 06:12:23.727539 shares-3.1.9/lands/structures_local/shares.egg-info/
+-rw-r--r--   0 veganeco  (1000) veganeco  (1000)     3612 2024-02-01 06:12:23.000000 shares-3.1.9/lands/structures_local/shares.egg-info/PKG-INFO
+-rw-r--r--   0 veganeco  (1000) veganeco  (1000)     1236 2024-02-01 06:12:23.000000 shares-3.1.9/lands/structures_local/shares.egg-info/SOURCES.txt
+-rw-r--r--   0 veganeco  (1000) veganeco  (1000)        1 2024-02-01 06:12:23.000000 shares-3.1.9/lands/structures_local/shares.egg-info/dependency_links.txt
+-rw-r--r--   0 veganeco  (1000) veganeco  (1000)       41 2024-02-01 06:12:23.000000 shares-3.1.9/lands/structures_local/shares.egg-info/entry_points.txt
+-rw-r--r--   0 veganeco  (1000) veganeco  (1000)       37 2024-02-01 06:12:23.000000 shares-3.1.9/lands/structures_local/shares.egg-info/requires.txt
+-rw-r--r--   0 veganeco  (1000) veganeco  (1000)        7 2024-02-01 06:12:23.000000 shares-3.1.9/lands/structures_local/shares.egg-info/top_level.txt
+-rw-r--r--   0 veganeco  (1000) veganeco  (1000)     1411 2024-02-01 06:12:05.000000 shares-3.1.9/pyproject.toml
+-rw-r--r--   0 veganeco  (1000) veganeco  (1000)       38 2024-02-01 06:12:23.727539 shares-3.1.9/setup.cfg
```

### Comparing `shares-3.1.8/PKG-INFO` & `shares-3.1.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: shares
-Version: 3.1.8
+Version: 3.1.9
 Summary: documentation framework that serves all '.s.HTML' that are found in the cwd.
 License: GPL 3.0
 Project-URL: GitLab, https://gitlab.com/reptilian_climates/modules_series_2/shares
 Description-Content-Type: text/markdown
 Requires-Dist: body_scan
-Requires-Dist: law_dictionary
 Requires-Dist: mako
 Requires-Dist: flask
 Requires-Dist: jsonschema
 Requires-Dist: rich
 
 
 ---
```

### Comparing `shares-3.1.8/lands/structures_local/shares/$ company/company.s.HTML` & `shares-3.1.9/lands/structures_local/shares/$ company/company.s.HTML`

 * *Files identical despite different names*

### Comparing `shares-3.1.8/lands/structures_local/shares/__init__.py` & `shares-3.1.9/lands/structures_local/shares/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 import os
 import pathlib
 import rich
 
 import shares.basin as basin
 from shares._clique import clique
 
-import shares.modules.law_dictionary as law_dictionary
+#import shares.modules.law_dictionary as law_dictionary
 
 def retrieve_directory ():
 	return os.getcwd ()
 	
 	return os.path.dirname (
 		os.path.abspath ((inspect.stack ()[1]) [1])
 	)
```

### Comparing `shares-3.1.8/lands/structures_local/shares/_clique.py` & `shares-3.1.9/lands/structures_local/shares/_clique.py`

 * *Files identical despite different names*

### Comparing `shares-3.1.8/lands/structures_local/shares/_status/checks/1/status_1.py` & `shares-3.1.9/lands/structures_local/shares/_status/checks/1/status_1.py`

 * *Files identical despite different names*

### Comparing `shares-3.1.8/lands/structures_local/shares/_status/status.proc.py` & `shares-3.1.9/lands/structures_local/shares/_status/status.proc.py`

 * *Files identical despite different names*

### Comparing `shares-3.1.8/lands/structures_local/shares/basin/__init__.py` & `shares-3.1.9/lands/structures_local/shares/basin/__init__.py`

 * *Files identical despite different names*

### Comparing `shares-3.1.8/lands/structures_local/shares/basin/treasury.py` & `shares-3.1.9/lands/structures_local/shares/basin/treasury.py`

 * *Files identical despite different names*

### Comparing `shares-3.1.8/lands/structures_local/shares/module.MD` & `shares-3.1.9/lands/structures_local/shares/module.MD`

 * *Files identical despite different names*

### Comparing `shares-3.1.8/lands/structures_local/shares/modules/law_dictionary/__init__.py` & `shares-3.1.9/lands/structures_local/shares/modules/law_dictionary/__init__.py`

 * *Files identical despite different names*

### Comparing `shares-3.1.8/lands/structures_local/shares/modules/law_dictionary/status_1.py` & `shares-3.1.9/lands/structures_local/shares/modules/law_dictionary/status_1.py`

 * *Files identical despite different names*

### Comparing `shares-3.1.8/lands/structures_local/shares/modules/law_dictionary/status_broken_1.py` & `shares-3.1.9/lands/structures_local/shares/modules/law_dictionary/status_broken_1.py`

 * *Files identical despite different names*

### Comparing `shares-3.1.8/lands/structures_local/shares/shares.s.HTML` & `shares-3.1.9/lands/structures_local/shares/shares.s.HTML`

 * *Files identical despite different names*

### Comparing `shares-3.1.8/lands/structures_local/shares.egg-info/PKG-INFO` & `shares-3.1.9/lands/structures_local/shares.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: shares
-Version: 3.1.8
+Version: 3.1.9
 Summary: documentation framework that serves all '.s.HTML' that are found in the cwd.
 License: GPL 3.0
 Project-URL: GitLab, https://gitlab.com/reptilian_climates/modules_series_2/shares
 Description-Content-Type: text/markdown
 Requires-Dist: body_scan
-Requires-Dist: law_dictionary
 Requires-Dist: mako
 Requires-Dist: flask
 Requires-Dist: jsonschema
 Requires-Dist: rich
 
 
 ---
```

### Comparing `shares-3.1.8/lands/structures_local/shares.egg-info/SOURCES.txt` & `shares-3.1.9/lands/structures_local/shares.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `shares-3.1.8/pyproject.toml` & `shares-3.1.9/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,29 +1,31 @@
 
 
 
 #
 #	How to Publish:
 #
+#
+#		# install the local modules
+#
 #		python3 lands/structures_local/shares/_status/status.proc.py
 #		python3 status_E2E/status.proc.py
 #		cp lands/structures_local/shares/module.MD readme.md
-#		(rm -rf dist && python3 -m build --sdist && twine upload dist/*)
+#		(rm -rf dist && python3 -m build && twine upload dist/*)
 #
 
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "shares"
-version = "3.1.8"
+version = "3.1.9"
 dependencies = [
 	"body_scan",
-	"law_dictionary",
 
 	"mako",
 	"flask",	
 	"jsonschema",
 	"rich"
 ]
```

