# Comparing `tmp/law_dictionary-1.0.8.tar.gz` & `tmp/law_dictionary-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "law_dictionary-1.0.8.tar", last modified: Sun Feb  4 21:59:57 2024, max compression
+gzip compressed data, was "law_dictionary-1.0.9.tar", last modified: Fri Feb  9 01:02:46 2024, max compression
```

## Comparing `law_dictionary-1.0.8.tar` & `law_dictionary-1.0.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 veganeco  (1000) veganeco  (1000)        0 2024-02-04 21:59:57.812513 law_dictionary-1.0.8/
--rw-r--r--   0 veganeco  (1000) veganeco  (1000)     3456 2024-02-04 21:59:57.812513 law_dictionary-1.0.8/PKG-INFO
--rw-r--r--   0 veganeco  (1000) veganeco  (1000)     1220 2024-02-04 21:59:54.000000 law_dictionary-1.0.8/pyproject.toml
--rw-r--r--   0 veganeco  (1000) veganeco  (1000)     3217 2024-01-31 19:16:24.000000 law_dictionary-1.0.8/readme.md
--rw-r--r--   0 veganeco  (1000) veganeco  (1000)       38 2024-02-04 21:59:57.813513 law_dictionary-1.0.8/setup.cfg
-drwxr-xr-x   0 veganeco  (1000) veganeco  (1000)        0 2024-02-04 21:59:57.806513 law_dictionary-1.0.8/structures/
-drwxr-xr-x   0 veganeco  (1000) veganeco  (1000)        0 2024-02-04 21:59:57.806513 law_dictionary-1.0.8/structures/modules/
-drwxr-xr-x   0 veganeco  (1000) veganeco  (1000)        0 2024-02-04 21:59:57.808513 law_dictionary-1.0.8/structures/modules/law_dictionary/
--rw-r--r--   0 veganeco  (1000) veganeco  (1000)     3320 2024-01-31 18:38:48.000000 law_dictionary-1.0.8/structures/modules/law_dictionary/__init__.py
-drwxr-xr-x   0 veganeco  (1000) veganeco  (1000)        0 2024-02-04 21:59:57.809513 law_dictionary-1.0.8/structures/modules/law_dictionary/_clique/
--rw-r--r--   0 veganeco  (1000) veganeco  (1000)      297 2023-12-11 06:07:46.000000 law_dictionary-1.0.8/structures/modules/law_dictionary/_clique/__init__.py
-drwxr-xr-x   0 veganeco  (1000) veganeco  (1000)        0 2024-02-04 21:59:57.810513 law_dictionary-1.0.8/structures/modules/law_dictionary/_clique/group/
--rw-r--r--   0 veganeco  (1000) veganeco  (1000)      294 2023-12-01 19:53:30.000000 law_dictionary-1.0.8/structures/modules/law_dictionary/_clique/group/__init__.py
-drwxr-xr-x   0 veganeco  (1000) veganeco  (1000)        0 2024-02-04 21:59:57.806513 law_dictionary-1.0.8/structures/modules/law_dictionary/_license/
-drwxr-xr-x   0 veganeco  (1000) veganeco  (1000)        0 2024-02-04 21:59:57.810513 law_dictionary-1.0.8/structures/modules/law_dictionary/_license/licenses/
--rw-r--r--   0 veganeco  (1000) veganeco  (1000)    37279 2023-12-01 20:51:04.000000 law_dictionary-1.0.8/structures/modules/law_dictionary/_license/licenses/gpl-3.0-standalone.html
-drwxr-xr-x   0 veganeco  (1000) veganeco  (1000)        0 2024-02-04 21:59:57.812513 law_dictionary-1.0.8/structures/modules/law_dictionary/_status/
--rw-r--r--   0 veganeco  (1000) veganeco  (1000)     1317 2024-01-26 19:02:24.000000 law_dictionary-1.0.8/structures/modules/law_dictionary/_status/status.proc.py
--rw-r--r--   0 veganeco  (1000) veganeco  (1000)     1750 2024-01-27 23:09:17.000000 law_dictionary-1.0.8/structures/modules/law_dictionary/status_1.py
--rw-r--r--   0 veganeco  (1000) veganeco  (1000)     1359 2024-01-27 23:43:16.000000 law_dictionary-1.0.8/structures/modules/law_dictionary/status_2.py
--rw-r--r--   0 veganeco  (1000) veganeco  (1000)      757 2024-01-31 18:35:24.000000 law_dictionary-1.0.8/structures/modules/law_dictionary/status_3.py
--rw-r--r--   0 veganeco  (1000) veganeco  (1000)     1017 2024-01-27 23:10:19.000000 law_dictionary-1.0.8/structures/modules/law_dictionary/status_broken_1.py
--rw-r--r--   0 veganeco  (1000) veganeco  (1000)      600 2024-01-27 23:12:19.000000 law_dictionary-1.0.8/structures/modules/law_dictionary/status_broken_2.py
-drwxr-xr-x   0 veganeco  (1000) veganeco  (1000)        0 2024-02-04 21:59:57.812513 law_dictionary-1.0.8/structures/modules/law_dictionary.egg-info/
--rw-r--r--   0 veganeco  (1000) veganeco  (1000)     3456 2024-02-04 21:59:57.000000 law_dictionary-1.0.8/structures/modules/law_dictionary.egg-info/PKG-INFO
--rw-r--r--   0 veganeco  (1000) veganeco  (1000)      845 2024-02-04 21:59:57.000000 law_dictionary-1.0.8/structures/modules/law_dictionary.egg-info/SOURCES.txt
--rw-r--r--   0 veganeco  (1000) veganeco  (1000)        1 2024-02-04 21:59:57.000000 law_dictionary-1.0.8/structures/modules/law_dictionary.egg-info/dependency_links.txt
--rw-r--r--   0 veganeco  (1000) veganeco  (1000)       14 2024-02-04 21:59:57.000000 law_dictionary-1.0.8/structures/modules/law_dictionary.egg-info/requires.txt
--rw-r--r--   0 veganeco  (1000) veganeco  (1000)       15 2024-02-04 21:59:57.000000 law_dictionary-1.0.8/structures/modules/law_dictionary.egg-info/top_level.txt
+drwxrwxr-x   0 treasury-1  (1000) treasury-1  (1000)        0 2024-02-09 01:02:46.466160 law_dictionary-1.0.9/
+-rw-r--r--   0 treasury-1  (1000) treasury-1  (1000)     3456 2024-02-09 01:02:46.466160 law_dictionary-1.0.9/PKG-INFO
+-rw-r--r--   0 treasury-1  (1000) treasury-1  (1000)     1220 2024-02-09 01:02:38.000000 law_dictionary-1.0.9/pyproject.toml
+-rw-r--r--   0 treasury-1  (1000) treasury-1  (1000)     3217 2024-02-09 01:02:36.000000 law_dictionary-1.0.9/readme.md
+-rw-rw-r--   0 treasury-1  (1000) treasury-1  (1000)       38 2024-02-09 01:02:46.466160 law_dictionary-1.0.9/setup.cfg
+drwxrwxr-x   0 treasury-1  (1000) treasury-1  (1000)        0 2024-02-09 01:02:46.462160 law_dictionary-1.0.9/structures/
+drwxrwxr-x   0 treasury-1  (1000) treasury-1  (1000)        0 2024-02-09 01:02:46.462160 law_dictionary-1.0.9/structures/modules/
+drwxrwxr-x   0 treasury-1  (1000) treasury-1  (1000)        0 2024-02-09 01:02:46.466160 law_dictionary-1.0.9/structures/modules/law_dictionary/
+-rw-r--r--   0 treasury-1  (1000) treasury-1  (1000)     3321 2024-02-09 01:02:16.000000 law_dictionary-1.0.9/structures/modules/law_dictionary/__init__.py
+drwxrwxr-x   0 treasury-1  (1000) treasury-1  (1000)        0 2024-02-09 01:02:46.466160 law_dictionary-1.0.9/structures/modules/law_dictionary/_clique/
+-rw-r--r--   0 treasury-1  (1000) treasury-1  (1000)      297 2023-12-11 06:07:46.000000 law_dictionary-1.0.9/structures/modules/law_dictionary/_clique/__init__.py
+drwxrwxr-x   0 treasury-1  (1000) treasury-1  (1000)        0 2024-02-09 01:02:46.466160 law_dictionary-1.0.9/structures/modules/law_dictionary/_clique/group/
+-rw-r--r--   0 treasury-1  (1000) treasury-1  (1000)      294 2023-12-01 19:53:30.000000 law_dictionary-1.0.9/structures/modules/law_dictionary/_clique/group/__init__.py
+drwxrwxr-x   0 treasury-1  (1000) treasury-1  (1000)        0 2024-02-09 01:02:46.462160 law_dictionary-1.0.9/structures/modules/law_dictionary/_license/
+drwxrwxr-x   0 treasury-1  (1000) treasury-1  (1000)        0 2024-02-09 01:02:46.466160 law_dictionary-1.0.9/structures/modules/law_dictionary/_license/licenses/
+-rw-r--r--   0 treasury-1  (1000) treasury-1  (1000)    37279 2023-12-01 20:51:04.000000 law_dictionary-1.0.9/structures/modules/law_dictionary/_license/licenses/gpl-3.0-standalone.html
+drwxrwxr-x   0 treasury-1  (1000) treasury-1  (1000)        0 2024-02-09 01:02:46.466160 law_dictionary-1.0.9/structures/modules/law_dictionary/_status/
+-rw-r--r--   0 treasury-1  (1000) treasury-1  (1000)     1317 2024-01-26 19:02:24.000000 law_dictionary-1.0.9/structures/modules/law_dictionary/_status/status.proc.py
+-rw-r--r--   0 treasury-1  (1000) treasury-1  (1000)     1750 2024-01-27 23:09:17.000000 law_dictionary-1.0.9/structures/modules/law_dictionary/status_1.py
+-rw-r--r--   0 treasury-1  (1000) treasury-1  (1000)     1359 2024-01-27 23:43:16.000000 law_dictionary-1.0.9/structures/modules/law_dictionary/status_2.py
+-rw-r--r--   0 treasury-1  (1000) treasury-1  (1000)      757 2024-01-31 18:35:24.000000 law_dictionary-1.0.9/structures/modules/law_dictionary/status_3.py
+-rw-r--r--   0 treasury-1  (1000) treasury-1  (1000)     1017 2024-01-27 23:10:19.000000 law_dictionary-1.0.9/structures/modules/law_dictionary/status_broken_1.py
+-rw-r--r--   0 treasury-1  (1000) treasury-1  (1000)      600 2024-01-27 23:12:19.000000 law_dictionary-1.0.9/structures/modules/law_dictionary/status_broken_2.py
+drwxrwxr-x   0 treasury-1  (1000) treasury-1  (1000)        0 2024-02-09 01:02:46.466160 law_dictionary-1.0.9/structures/modules/law_dictionary.egg-info/
+-rw-r--r--   0 treasury-1  (1000) treasury-1  (1000)     3456 2024-02-09 01:02:46.000000 law_dictionary-1.0.9/structures/modules/law_dictionary.egg-info/PKG-INFO
+-rw-r--r--   0 treasury-1  (1000) treasury-1  (1000)      845 2024-02-09 01:02:46.000000 law_dictionary-1.0.9/structures/modules/law_dictionary.egg-info/SOURCES.txt
+-rw-r--r--   0 treasury-1  (1000) treasury-1  (1000)        1 2024-02-09 01:02:46.000000 law_dictionary-1.0.9/structures/modules/law_dictionary.egg-info/dependency_links.txt
+-rw-r--r--   0 treasury-1  (1000) treasury-1  (1000)       14 2024-02-09 01:02:46.000000 law_dictionary-1.0.9/structures/modules/law_dictionary.egg-info/requires.txt
+-rw-r--r--   0 treasury-1  (1000) treasury-1  (1000)       15 2024-02-09 01:02:46.000000 law_dictionary-1.0.9/structures/modules/law_dictionary.egg-info/top_level.txt
```

### Comparing `law_dictionary-1.0.8/PKG-INFO` & `law_dictionary-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: law_dictionary
-Version: 1.0.8
+Version: 1.0.9
 License: GPL 3.0
 Project-URL: GitLab, https://gitlab.com/offline-money/squash-1/law_dictionary
 Description-Content-Type: text/markdown
 Requires-Dist: clique
 Requires-Dist: onesie
```

### Comparing `law_dictionary-1.0.8/pyproject.toml` & `law_dictionary-1.0.9/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "law_dictionary"
-version = "1.0.8"
+version = "1.0.9"
 dependencies = [
 	'clique',
 	'onesie'
 ]
 
 # license = { text = "license" }
 # license = { file = "license.txt" }
```

### Comparing `law_dictionary-1.0.8/readme.md` & `law_dictionary-1.0.9/readme.md`

 * *Files identical despite different names*

### Comparing `law_dictionary-1.0.8/structures/modules/law_dictionary/__init__.py` & `law_dictionary-1.0.9/structures/modules/law_dictionary/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -95,15 +95,15 @@
 			required = True
 	
 	
 			'''
 			This determines whether the label in the laws is found in the dictionary.
 		'''
 		dictionary_has_law_label = law_label in dictionary;
-		print ("dictionary_has_law_label:", dictionary_has_law_label)
+		#print ("dictionary_has_law_label:", dictionary_has_law_label)
 	
 	
 	
 		if (required == True):
 			if (law_label not in dictionary):
 				return obstacle (f'The label "{ law_label }" was not found in the laws.')
```

### Comparing `law_dictionary-1.0.8/structures/modules/law_dictionary/_license/licenses/gpl-3.0-standalone.html` & `law_dictionary-1.0.9/structures/modules/law_dictionary/_license/licenses/gpl-3.0-standalone.html`

 * *Files identical despite different names*

### Comparing `law_dictionary-1.0.8/structures/modules/law_dictionary/_status/status.proc.py` & `law_dictionary-1.0.9/structures/modules/law_dictionary/_status/status.proc.py`

 * *Files identical despite different names*

### Comparing `law_dictionary-1.0.8/structures/modules/law_dictionary/status_1.py` & `law_dictionary-1.0.9/structures/modules/law_dictionary/status_1.py`

 * *Files identical despite different names*

### Comparing `law_dictionary-1.0.8/structures/modules/law_dictionary/status_2.py` & `law_dictionary-1.0.9/structures/modules/law_dictionary/status_2.py`

 * *Files identical despite different names*

### Comparing `law_dictionary-1.0.8/structures/modules/law_dictionary/status_3.py` & `law_dictionary-1.0.9/structures/modules/law_dictionary/status_3.py`

 * *Files identical despite different names*

### Comparing `law_dictionary-1.0.8/structures/modules/law_dictionary/status_broken_1.py` & `law_dictionary-1.0.9/structures/modules/law_dictionary/status_broken_1.py`

 * *Files identical despite different names*

### Comparing `law_dictionary-1.0.8/structures/modules/law_dictionary/status_broken_2.py` & `law_dictionary-1.0.9/structures/modules/law_dictionary/status_broken_2.py`

 * *Files identical despite different names*

### Comparing `law_dictionary-1.0.8/structures/modules/law_dictionary.egg-info/PKG-INFO` & `law_dictionary-1.0.9/structures/modules/law_dictionary.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: law_dictionary
-Version: 1.0.8
+Version: 1.0.9
 License: GPL 3.0
 Project-URL: GitLab, https://gitlab.com/offline-money/squash-1/law_dictionary
 Description-Content-Type: text/markdown
 Requires-Dist: clique
 Requires-Dist: onesie
```

### Comparing `law_dictionary-1.0.8/structures/modules/law_dictionary.egg-info/SOURCES.txt` & `law_dictionary-1.0.9/structures/modules/law_dictionary.egg-info/SOURCES.txt`

 * *Files identical despite different names*

