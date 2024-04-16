# Comparing `tmp/anyerplint-0.2.90.tar.gz` & `tmp/anyerplint-0.2.91.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anyerplint-0.2.90.tar", last modified: Thu Apr 11 05:37:03 2024, max compression
+gzip compressed data, was "anyerplint-0.2.91.tar", last modified: Tue Apr 16 12:48:50 2024, max compression
```

## Comparing `anyerplint-0.2.90.tar` & `anyerplint-0.2.91.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxrwxrwx   0        0        0        0 2024-04-11 05:37:03.559095 anyerplint-0.2.90/
--rw-rw-rw-   0        0        0      628 2024-04-11 05:37:03.558066 anyerplint-0.2.90/PKG-INFO
--rw-rw-rw-   0        0        0       91 2023-11-03 12:54:20.000000 anyerplint-0.2.90/README.md
-drwxrwxrwx   0        0        0        0 2024-04-11 05:37:03.531374 anyerplint-0.2.90/anyerplint/
--rw-rw-rw-   0        0        0      233 2023-09-20 08:47:10.000000 anyerplint-0.2.90/anyerplint/__init__.py
--rw-rw-rw-   0        0        0       80 2023-09-20 08:47:10.000000 anyerplint-0.2.90/anyerplint/__main__.py
--rw-rw-rw-   0        0        0      391 2024-03-20 13:30:36.000000 anyerplint-0.2.90/anyerplint/ast.py
--rw-rw-rw-   0        0        0    19517 2024-04-11 05:36:25.000000 anyerplint-0.2.90/anyerplint/business_logic.py
-drwxrwxrwx   0        0        0        0 2024-04-11 05:37:03.548651 anyerplint-0.2.90/anyerplint/cli/
--rw-rw-rw-   0        0        0        0 2023-09-20 08:47:10.000000 anyerplint-0.2.90/anyerplint/cli/__init__.py
--rw-rw-rw-   0        0        0     1107 2024-03-01 20:38:32.000000 anyerplint-0.2.90/anyerplint/cli/check.py
--rw-rw-rw-   0        0        0     1594 2024-03-20 13:30:36.000000 anyerplint-0.2.90/anyerplint/cli/importcmd.py
--rw-rw-rw-   0        0        0     1718 2024-03-20 13:30:36.000000 anyerplint-0.2.90/anyerplint/cli/initcmd.py
--rw-rw-rw-   0        0        0     1015 2024-03-20 13:30:28.000000 anyerplint-0.2.90/anyerplint/cli/main.py
--rw-rw-rw-   0        0        0     5390 2024-03-20 13:30:36.000000 anyerplint-0.2.90/anyerplint/cli/parsecmd.py
--rw-rw-rw-   0        0        0     2493 2024-03-20 13:30:36.000000 anyerplint-0.2.90/anyerplint/preprocessor.py
--rw-rw-rw-   0        0        0      107 2023-12-21 14:28:43.000000 anyerplint-0.2.90/anyerplint/recursive_list.py
--rw-rw-rw-   0        0        0     4852 2024-03-20 14:24:28.000000 anyerplint-0.2.90/anyerplint/tnex.py
--rw-rw-rw-   0        0        0     7531 2024-03-20 13:30:36.000000 anyerplint-0.2.90/anyerplint/translate.py
--rw-rw-rw-   0        0        0     2676 2024-01-09 08:12:37.000000 anyerplint-0.2.90/anyerplint/util.py
--rw-rw-rw-   0        0        0        8 2024-04-11 05:36:43.000000 anyerplint-0.2.90/anyerplint/version.txt
-drwxrwxrwx   0        0        0        0 2024-04-11 05:37:03.557033 anyerplint-0.2.90/anyerplint.egg-info/
--rw-rw-rw-   0        0        0      628 2024-04-11 05:37:03.000000 anyerplint-0.2.90/anyerplint.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      712 2024-04-11 05:37:03.000000 anyerplint-0.2.90/anyerplint.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-04-11 05:37:03.000000 anyerplint-0.2.90/anyerplint.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       56 2024-04-11 05:37:03.000000 anyerplint-0.2.90/anyerplint.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       20 2024-04-11 05:37:03.000000 anyerplint-0.2.90/anyerplint.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2024-04-11 05:37:03.000000 anyerplint-0.2.90/anyerplint.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1823 2024-03-20 14:24:28.000000 anyerplint-0.2.90/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-04-11 05:37:03.560127 anyerplint-0.2.90/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-04-11 05:37:03.554652 anyerplint-0.2.90/test/
--rw-rw-rw-   0        0        0     2617 2024-04-11 05:36:25.000000 anyerplint-0.2.90/test/test_business_logic.py
--rw-rw-rw-   0        0        0      589 2024-01-17 11:49:24.000000 anyerplint-0.2.90/test/test_preprocess.py
--rw-rw-rw-   0        0        0     3507 2024-03-20 13:30:36.000000 anyerplint-0.2.90/test/test_tnex.py
--rw-rw-rw-   0        0        0      674 2024-03-19 13:26:43.000000 anyerplint-0.2.90/test/test_translate.py
+drwxrwxrwx   0        0        0        0 2024-04-16 12:48:50.842743 anyerplint-0.2.91/
+-rw-rw-rw-   0        0        0      628 2024-04-16 12:48:50.840649 anyerplint-0.2.91/PKG-INFO
+-rw-rw-rw-   0        0        0       91 2023-11-03 12:54:20.000000 anyerplint-0.2.91/README.md
+drwxrwxrwx   0        0        0        0 2024-04-16 12:48:50.803254 anyerplint-0.2.91/anyerplint/
+-rw-rw-rw-   0        0        0      233 2023-09-20 08:47:10.000000 anyerplint-0.2.91/anyerplint/__init__.py
+-rw-rw-rw-   0        0        0       80 2023-09-20 08:47:10.000000 anyerplint-0.2.91/anyerplint/__main__.py
+-rw-rw-rw-   0        0        0      391 2024-03-20 13:30:36.000000 anyerplint-0.2.91/anyerplint/ast.py
+-rw-rw-rw-   0        0        0    19517 2024-04-11 05:36:25.000000 anyerplint-0.2.91/anyerplint/business_logic.py
+drwxrwxrwx   0        0        0        0 2024-04-16 12:48:50.828892 anyerplint-0.2.91/anyerplint/cli/
+-rw-rw-rw-   0        0        0        0 2023-09-20 08:47:10.000000 anyerplint-0.2.91/anyerplint/cli/__init__.py
+-rw-rw-rw-   0        0        0     1107 2024-03-01 20:38:32.000000 anyerplint-0.2.91/anyerplint/cli/check.py
+-rw-rw-rw-   0        0        0     1594 2024-03-20 13:30:36.000000 anyerplint-0.2.91/anyerplint/cli/importcmd.py
+-rw-rw-rw-   0        0        0     1718 2024-03-20 13:30:36.000000 anyerplint-0.2.91/anyerplint/cli/initcmd.py
+-rw-rw-rw-   0        0        0     1015 2024-03-20 13:30:28.000000 anyerplint-0.2.91/anyerplint/cli/main.py
+-rw-rw-rw-   0        0        0     5390 2024-03-20 13:30:36.000000 anyerplint-0.2.91/anyerplint/cli/parsecmd.py
+-rw-rw-rw-   0        0        0     2493 2024-03-20 13:30:36.000000 anyerplint-0.2.91/anyerplint/preprocessor.py
+-rw-rw-rw-   0        0        0      107 2023-12-21 14:28:43.000000 anyerplint-0.2.91/anyerplint/recursive_list.py
+-rw-rw-rw-   0        0        0     4852 2024-03-20 14:24:28.000000 anyerplint-0.2.91/anyerplint/tnex.py
+-rw-rw-rw-   0        0        0     7556 2024-04-16 12:42:35.000000 anyerplint-0.2.91/anyerplint/translate.py
+-rw-rw-rw-   0        0        0     2676 2024-01-09 08:12:37.000000 anyerplint-0.2.91/anyerplint/util.py
+-rw-rw-rw-   0        0        0        8 2024-04-16 12:48:30.000000 anyerplint-0.2.91/anyerplint/version.txt
+drwxrwxrwx   0        0        0        0 2024-04-16 12:48:50.839615 anyerplint-0.2.91/anyerplint.egg-info/
+-rw-rw-rw-   0        0        0      628 2024-04-16 12:48:50.000000 anyerplint-0.2.91/anyerplint.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      712 2024-04-16 12:48:50.000000 anyerplint-0.2.91/anyerplint.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-16 12:48:50.000000 anyerplint-0.2.91/anyerplint.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       56 2024-04-16 12:48:50.000000 anyerplint-0.2.91/anyerplint.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       20 2024-04-16 12:48:50.000000 anyerplint-0.2.91/anyerplint.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2024-04-16 12:48:50.000000 anyerplint-0.2.91/anyerplint.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1823 2024-03-20 14:24:28.000000 anyerplint-0.2.91/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-16 12:48:50.842743 anyerplint-0.2.91/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-16 12:48:50.837520 anyerplint-0.2.91/test/
+-rw-rw-rw-   0        0        0     2617 2024-04-11 05:36:25.000000 anyerplint-0.2.91/test/test_business_logic.py
+-rw-rw-rw-   0        0        0      589 2024-01-17 11:49:24.000000 anyerplint-0.2.91/test/test_preprocess.py
+-rw-rw-rw-   0        0        0     3507 2024-03-20 13:30:36.000000 anyerplint-0.2.91/test/test_tnex.py
+-rw-rw-rw-   0        0        0      674 2024-03-19 13:26:43.000000 anyerplint-0.2.91/test/test_translate.py
```

### Comparing `anyerplint-0.2.90/PKG-INFO` & `anyerplint-0.2.91/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anyerplint
-Version: 0.2.90
+Version: 0.2.91
 Summary: anyerplint
 Project-URL: Homepage, https://github.com/Basware/anyerplint
 Project-URL: Repository, https://github.com/Basware/anyerplint
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `anyerplint-0.2.90/anyerplint/business_logic.py` & `anyerplint-0.2.91/anyerplint/business_logic.py`

 * *Files identical despite different names*

### Comparing `anyerplint-0.2.90/anyerplint/cli/check.py` & `anyerplint-0.2.91/anyerplint/cli/check.py`

 * *Files identical despite different names*

### Comparing `anyerplint-0.2.90/anyerplint/cli/importcmd.py` & `anyerplint-0.2.91/anyerplint/cli/importcmd.py`

 * *Files identical despite different names*

### Comparing `anyerplint-0.2.90/anyerplint/cli/initcmd.py` & `anyerplint-0.2.91/anyerplint/cli/initcmd.py`

 * *Files identical despite different names*

### Comparing `anyerplint-0.2.90/anyerplint/cli/main.py` & `anyerplint-0.2.91/anyerplint/cli/main.py`

 * *Files identical despite different names*

### Comparing `anyerplint-0.2.90/anyerplint/cli/parsecmd.py` & `anyerplint-0.2.91/anyerplint/cli/parsecmd.py`

 * *Files identical despite different names*

### Comparing `anyerplint-0.2.90/anyerplint/preprocessor.py` & `anyerplint-0.2.91/anyerplint/preprocessor.py`

 * *Files identical despite different names*

### Comparing `anyerplint-0.2.90/anyerplint/tnex.py` & `anyerplint-0.2.91/anyerplint/tnex.py`

 * *Files identical despite different names*

### Comparing `anyerplint-0.2.90/anyerplint/translate.py` & `anyerplint-0.2.91/anyerplint/translate.py`

 * *Files 2% similar despite different names*

```diff
@@ -29,14 +29,15 @@
 # some 'trivial' translations
 nullary_funcs = {
     "F,GUID",
     "F,NOW",
 }
 # these will be translated to name(arg1; arg2)
 nnary_funcs: dict[str, int | tuple[int, int]] = {
+    "F,ADDXML": (3, 4),
     "F,ADDXMLNS": 3,
     "F,CSV": (2, 3),
     "F,DATEADD": 3,
     "F,DATEDIFF": 3,
     "F,DBSELECT": (2, 999),
     "F,FLOOR": 1,
     "F,ISCHANGED": 2,
```

### Comparing `anyerplint-0.2.90/anyerplint/util.py` & `anyerplint-0.2.91/anyerplint/util.py`

 * *Files identical despite different names*

### Comparing `anyerplint-0.2.90/anyerplint.egg-info/PKG-INFO` & `anyerplint-0.2.91/anyerplint.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: anyerplint
-Version: 0.2.90
+Version: 0.2.91
 Summary: anyerplint
 Project-URL: Homepage, https://github.com/Basware/anyerplint
 Project-URL: Repository, https://github.com/Basware/anyerplint
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `anyerplint-0.2.90/anyerplint.egg-info/SOURCES.txt` & `anyerplint-0.2.91/anyerplint.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `anyerplint-0.2.90/pyproject.toml` & `anyerplint-0.2.91/pyproject.toml`

 * *Files identical despite different names*

### Comparing `anyerplint-0.2.90/test/test_business_logic.py` & `anyerplint-0.2.91/test/test_business_logic.py`

 * *Files identical despite different names*

### Comparing `anyerplint-0.2.90/test/test_preprocess.py` & `anyerplint-0.2.91/test/test_preprocess.py`

 * *Files identical despite different names*

### Comparing `anyerplint-0.2.90/test/test_tnex.py` & `anyerplint-0.2.91/test/test_tnex.py`

 * *Files identical despite different names*

### Comparing `anyerplint-0.2.90/test/test_translate.py` & `anyerplint-0.2.91/test/test_translate.py`

 * *Files identical despite different names*

