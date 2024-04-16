# Comparing `tmp/bezalel-0.0.8.tar.gz` & `tmp/bezalel-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bezalel-0.0.8.tar", last modified: Tue Jul  5 13:26:41 2022, max compression
+gzip compressed data, was "bezalel-0.0.9.tar", last modified: Fri Nov 11 14:45:56 2022, max compression
```

## Comparing `bezalel-0.0.8.tar` & `bezalel-0.0.9.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2022-07-05 13:26:41.281803 bezalel-0.0.8/
--rw-rw-rw-   0        0        0     1089 2022-07-05 13:15:11.000000 bezalel-0.0.8/LICENSE
--rw-rw-rw-   0        0        0     6437 2022-07-05 13:26:41.281803 bezalel-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0     5928 2022-07-05 13:10:26.000000 bezalel-0.0.8/README.md
--rw-rw-rw-   0        0        0       86 2022-07-05 13:10:26.000000 bezalel-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0      717 2022-07-05 13:26:41.297425 bezalel-0.0.8/setup.cfg
-drwxrwxrwx   0        0        0        0 2022-07-05 13:26:41.250604 bezalel-0.0.8/src/
-drwxrwxrwx   0        0        0        0 2022-07-05 13:26:41.266162 bezalel-0.0.8/src/bezalel/
--rw-rw-rw-   0        0        0      390 2022-07-05 13:10:26.000000 bezalel-0.0.8/src/bezalel/__init__.py
-drwxrwxrwx   0        0        0        0 2022-07-05 13:26:41.281803 bezalel-0.0.8/src/bezalel/impl/
--rw-rw-rw-   0        0        0      931 2022-07-05 13:10:26.000000 bezalel-0.0.8/src/bezalel/impl/BufferingIterator.py
--rw-rw-rw-   0        0        0     2033 2022-07-05 13:10:26.000000 bezalel-0.0.8/src/bezalel/impl/CursorApiIterator.py
--rw-rw-rw-   0        0        0     2495 2022-07-05 13:10:26.000000 bezalel-0.0.8/src/bezalel/impl/PaginatedApiIterator.py
--rw-rw-rw-   0        0        0        0 2022-07-05 13:10:26.000000 bezalel-0.0.8/src/bezalel/impl/__init__.py
--rw-rw-rw-   0        0        0     4013 2022-07-05 13:10:26.000000 bezalel-0.0.8/src/bezalel/impl/normalize_dicts.py
--rw-rw-rw-   0        0        0     3474 2022-07-05 13:10:26.000000 bezalel-0.0.8/src/bezalel/impl/normalize_with_prototype.py
--rw-rw-rw-   0        0        0     1327 2022-07-05 13:10:26.000000 bezalel-0.0.8/src/bezalel/impl/prepare_job.py
-drwxrwxrwx   0        0        0        0 2022-07-05 13:26:41.281803 bezalel-0.0.8/src/bezalel.egg-info/
--rw-rw-rw-   0        0        0     6437 2022-07-05 13:26:41.000000 bezalel-0.0.8/src/bezalel.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      499 2022-07-05 13:26:41.000000 bezalel-0.0.8/src/bezalel.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-07-05 13:26:41.000000 bezalel-0.0.8/src/bezalel.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2022-07-05 13:26:41.000000 bezalel-0.0.8/src/bezalel.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2022-07-05 13:26:41.000000 bezalel-0.0.8/src/bezalel.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2022-11-11 14:45:56.228285 bezalel-0.0.9/
+-rw-rw-rw-   0        0        0     1089 2022-07-05 13:15:11.000000 bezalel-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0     6687 2022-11-11 14:45:56.228285 bezalel-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     6178 2022-11-11 14:44:16.000000 bezalel-0.0.9/README.md
+-rw-rw-rw-   0        0        0      169 2022-11-11 13:03:42.000000 bezalel-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0      717 2022-11-11 14:45:56.229285 bezalel-0.0.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2022-11-11 14:45:56.210292 bezalel-0.0.9/src/
+drwxrwxrwx   0        0        0        0 2022-11-11 14:45:56.213285 bezalel-0.0.9/src/bezalel/
+-rw-rw-rw-   0        0        0      390 2022-07-05 13:10:26.000000 bezalel-0.0.9/src/bezalel/__init__.py
+drwxrwxrwx   0        0        0        0 2022-11-11 14:45:56.228285 bezalel-0.0.9/src/bezalel/impl/
+-rw-rw-rw-   0        0        0      931 2022-07-05 13:10:26.000000 bezalel-0.0.9/src/bezalel/impl/BufferingIterator.py
+-rw-rw-rw-   0        0        0     2033 2022-07-05 13:10:26.000000 bezalel-0.0.9/src/bezalel/impl/CursorApiIterator.py
+-rw-rw-rw-   0        0        0     2495 2022-07-05 13:10:26.000000 bezalel-0.0.9/src/bezalel/impl/PaginatedApiIterator.py
+-rw-rw-rw-   0        0        0        0 2022-07-05 13:10:26.000000 bezalel-0.0.9/src/bezalel/impl/__init__.py
+-rw-rw-rw-   0        0        0     4421 2022-11-11 11:50:23.000000 bezalel-0.0.9/src/bezalel/impl/normalize_dicts.py
+-rw-rw-rw-   0        0        0     3474 2022-07-05 13:10:26.000000 bezalel-0.0.9/src/bezalel/impl/normalize_with_prototype.py
+-rw-rw-rw-   0        0        0     1327 2022-07-05 13:10:26.000000 bezalel-0.0.9/src/bezalel/impl/prepare_job.py
+drwxrwxrwx   0        0        0        0 2022-11-11 14:45:56.225293 bezalel-0.0.9/src/bezalel.egg-info/
+-rw-rw-rw-   0        0        0     6687 2022-11-11 14:45:56.000000 bezalel-0.0.9/src/bezalel.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      499 2022-11-11 14:45:56.000000 bezalel-0.0.9/src/bezalel.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-11-11 14:45:56.000000 bezalel-0.0.9/src/bezalel.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2022-11-11 14:45:56.000000 bezalel-0.0.9/src/bezalel.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2022-11-11 14:45:56.000000 bezalel-0.0.9/src/bezalel.egg-info/top_level.txt
```

### Comparing `bezalel-0.0.8/LICENSE` & `bezalel-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `bezalel-0.0.8/PKG-INFO` & `bezalel-0.0.9/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bezalel
-Version: 0.0.8
+Version: 0.0.9
 Summary: A library for ingesting data provided by paginated HTTP APIs
 Home-page: https://github.com/bezalelsoft/bezalel
 Author: bezalelsoft
 Project-URL: Bug Tracker, https://github.com/bezalelsoft/bezalel/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -198,7 +198,11 @@
  {'id': 2, 'name': 'Sue Smith', 'pets.id': 201, 'pets.type': 'cat', 'pets.name': 'Kitten', 'pets.toys.name': 'toy5'},
  {'id': 2, 'name': 'Sue Smith', 'pets.id': 201, 'pets.type': 'cat', 'pets.name': 'Kitten', 'pets.toys.name': 'toy6'},
  {'id': 2, 'name': 'Sue Smith', 'pets.id': 202, 'pets.type': 'dog', 'pets.name': 'Fury'}]
 ```
 
 Presence of the last record can be controlled by flag `return_incomplete_records`. If `return_incomplete_records=False`
 then last record in the example would not have been returned.
+
+Additional options:
+- jsonify_lists - when set to True, then if a list is encountered (not in main path), it is dumped as a JSON string.
+- jsonify_dicts - list of paths for where to expect a dict. That dict will be then dumped as a JSON string.
```

### Comparing `bezalel-0.0.8/README.md` & `bezalel-0.0.9/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -184,7 +184,11 @@
  {'id': 2, 'name': 'Sue Smith', 'pets.id': 201, 'pets.type': 'cat', 'pets.name': 'Kitten', 'pets.toys.name': 'toy5'},
  {'id': 2, 'name': 'Sue Smith', 'pets.id': 201, 'pets.type': 'cat', 'pets.name': 'Kitten', 'pets.toys.name': 'toy6'},
  {'id': 2, 'name': 'Sue Smith', 'pets.id': 202, 'pets.type': 'dog', 'pets.name': 'Fury'}]
 ```
 
 Presence of the last record can be controlled by flag `return_incomplete_records`. If `return_incomplete_records=False`
 then last record in the example would not have been returned.
+
+Additional options:
+- jsonify_lists - when set to True, then if a list is encountered (not in main path), it is dumped as a JSON string.
+- jsonify_dicts - list of paths for where to expect a dict. That dict will be then dumped as a JSON string.
```

### Comparing `bezalel-0.0.8/setup.cfg` & `bezalel-0.0.9/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2062 657a 616c 656c 0d0a 7665 7273   = bezalel..vers
-00000020: 696f 6e20 3d20 302e 302e 380d 0a61 7574  ion = 0.0.8..aut
+00000020: 696f 6e20 3d20 302e 302e 390d 0a61 7574  ion = 0.0.9..aut
 00000030: 686f 7220 3d20 6265 7a61 6c65 6c73 6f66  hor = bezalelsof
 00000040: 740d 0a64 6573 6372 6970 7469 6f6e 203d  t..description =
 00000050: 2041 206c 6962 7261 7279 2066 6f72 2069   A library for i
 00000060: 6e67 6573 7469 6e67 2064 6174 6120 7072  ngesting data pr
 00000070: 6f76 6964 6564 2062 7920 7061 6769 6e61  ovided by pagina
 00000080: 7465 6420 4854 5450 2041 5049 730d 0a6c  ted HTTP APIs..l
 00000090: 6f6e 675f 6465 7363 7269 7074 696f 6e20  ong_description
```

### Comparing `bezalel-0.0.8/src/bezalel/impl/BufferingIterator.py` & `bezalel-0.0.9/src/bezalel/impl/BufferingIterator.py`

 * *Files identical despite different names*

### Comparing `bezalel-0.0.8/src/bezalel/impl/CursorApiIterator.py` & `bezalel-0.0.9/src/bezalel/impl/CursorApiIterator.py`

 * *Files identical despite different names*

### Comparing `bezalel-0.0.8/src/bezalel/impl/PaginatedApiIterator.py` & `bezalel-0.0.9/src/bezalel/impl/PaginatedApiIterator.py`

 * *Files identical despite different names*

### Comparing `bezalel-0.0.8/src/bezalel/impl/normalize_dicts.py` & `bezalel-0.0.9/src/bezalel/impl/normalize_dicts.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import json
 
 
-def normalize_dicts(records_list: list, path: list, separator=".", return_incomplete_records=True, jsonify_lists=False):
+def normalize_dicts(records_list: list, path: list, separator=".", return_incomplete_records=True, jsonify_lists=False,
+                    jsonify_dicts: list=[]):
     """
     Normalize list of nested python dicts to a list of one-level dicts.
 
     Example input:
     ```
     data = [
         {
@@ -38,26 +39,32 @@
     ```
 
     :param records_list: list of dicts to be normalized
     :param path: list of str, name of objects in nested dicts to follow when normalizing
     :param separator: str, (defaults to "."), it will be put in names of fields of resulting dicts.
     :param return_incomplete_records: bool (defaults to True), if following the `path` fails because there is no object
         at some level, this flag indicates if that incomplete record should be returned in result list.
+    :param jsonify_dicts: list (defaults to []) a list of paths (str) that point to dicts in each record that must not
+        be recurred into during unrolling.
     :return: list of normalized dicts.
     """
     def unroll_dict_rec(d: dict, prefix: str = "") -> dict:
         unrolled = {}
         for k, v in d.items():
-            if type(v) == dict:
-                for u_k, u_v in unroll_dict_rec(v, f"{prefix}{k}{separator}").items():
+            unrolled_key = f"{prefix}{k}"
+
+            if type(v) == dict and jsonify_dicts is not None and unrolled_key in jsonify_dicts:
+                unrolled[unrolled_key] = json.dumps(v)
+            elif type(v) == dict:
+                for u_k, u_v in unroll_dict_rec(v, f"{unrolled_key}{separator}").items():
                     unrolled[u_k] = u_v
             elif jsonify_lists and type(v) == list:
-                unrolled[f"{prefix}{k}"] = json.dumps(v)
+                unrolled[unrolled_key] = json.dumps(v)
             else:
-                unrolled[f"{prefix}{k}"] = v
+                unrolled[unrolled_key] = v
         return unrolled
 
     def normalize_dicts_rec(records_list: list, path: list, prefix: str = "") -> list:
         if records_list is None or len(records_list) == 0:
             records_list = [{}] if return_incomplete_records else []
         if type(records_list) != list:
             raise Exception(f"records_list is not a list at [{prefix}]")
```

### Comparing `bezalel-0.0.8/src/bezalel/impl/normalize_with_prototype.py` & `bezalel-0.0.9/src/bezalel/impl/normalize_with_prototype.py`

 * *Files identical despite different names*

### Comparing `bezalel-0.0.8/src/bezalel/impl/prepare_job.py` & `bezalel-0.0.9/src/bezalel/impl/prepare_job.py`

 * *Files identical despite different names*

### Comparing `bezalel-0.0.8/src/bezalel.egg-info/PKG-INFO` & `bezalel-0.0.9/src/bezalel.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bezalel
-Version: 0.0.8
+Version: 0.0.9
 Summary: A library for ingesting data provided by paginated HTTP APIs
 Home-page: https://github.com/bezalelsoft/bezalel
 Author: bezalelsoft
 Project-URL: Bug Tracker, https://github.com/bezalelsoft/bezalel/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -198,7 +198,11 @@
  {'id': 2, 'name': 'Sue Smith', 'pets.id': 201, 'pets.type': 'cat', 'pets.name': 'Kitten', 'pets.toys.name': 'toy5'},
  {'id': 2, 'name': 'Sue Smith', 'pets.id': 201, 'pets.type': 'cat', 'pets.name': 'Kitten', 'pets.toys.name': 'toy6'},
  {'id': 2, 'name': 'Sue Smith', 'pets.id': 202, 'pets.type': 'dog', 'pets.name': 'Fury'}]
 ```
 
 Presence of the last record can be controlled by flag `return_incomplete_records`. If `return_incomplete_records=False`
 then last record in the example would not have been returned.
+
+Additional options:
+- jsonify_lists - when set to True, then if a list is encountered (not in main path), it is dumped as a JSON string.
+- jsonify_dicts - list of paths for where to expect a dict. That dict will be then dumped as a JSON string.
```

