# Comparing `tmp/furthrmind-0.1b2.tar.gz` & `tmp/furthrmind-0.1b3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "furthrmind-0.1b2.tar", max compression
+gzip compressed data, was "furthrmind-0.1b3.tar", max compression
```

## Comparing `furthrmind-0.1b2.tar` & `furthrmind-0.1b3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rwxr-xr-x   0        0        0    35823 2024-03-07 10:34:57.137547 furthrmind-0.1b2/LICENSE
--rwxr-xr-x   0        0        0     2869 2024-04-15 16:25:04.221154 furthrmind-0.1b2/README.md
--rwxr-xr-x   0        0        0     1876 2024-04-15 16:12:36.272916 furthrmind-0.1b2/furthrmind/__init__.py
--rwxr-xr-x   0        0        0      471 2024-03-15 09:10:04.917117 furthrmind-0.1b2/furthrmind/collection/__init__.py
--rwxr-xr-x   0        0        0    19254 2024-04-15 16:12:36.344833 furthrmind-0.1b2/furthrmind/collection/baseclass.py
--rwxr-xr-x   0        0        0     2157 2024-04-15 16:12:36.211301 furthrmind-0.1b2/furthrmind/collection/category.py
--rwxr-xr-x   0        0        0     5824 2024-04-15 16:12:36.294403 furthrmind-0.1b2/furthrmind/collection/column.py
--rwxr-xr-x   0        0        0     5946 2024-04-15 16:12:36.330101 furthrmind-0.1b2/furthrmind/collection/comboboxentry.py
--rwxr-xr-x   0        0        0     6775 2024-04-15 16:12:36.362346 furthrmind-0.1b2/furthrmind/collection/datatable.py
--rwxr-xr-x   0        0        0     6085 2024-04-15 16:12:36.202385 furthrmind-0.1b2/furthrmind/collection/experiment.py
--rwxr-xr-x   0        0        0     4805 2024-04-15 16:12:36.283804 furthrmind-0.1b2/furthrmind/collection/field.py
--rwxr-xr-x   0        0        0    10119 2024-04-15 16:12:36.242521 furthrmind-0.1b2/furthrmind/collection/fielddata.py
--rwxr-xr-x   0        0        0     1553 2024-04-15 16:12:36.336627 furthrmind-0.1b2/furthrmind/collection/file.py
--rwxr-xr-x   0        0        0     4114 2024-04-15 16:12:36.310225 furthrmind-0.1b2/furthrmind/collection/group.py
--rwxr-xr-x   0        0        0        1 2024-03-13 11:54:06.300443 furthrmind-0.1b2/furthrmind/collection/import_collection.py
--rwxr-xr-x   0        0        0     2803 2024-04-15 16:12:36.192946 furthrmind-0.1b2/furthrmind/collection/project.py
--rwxr-xr-x   0        0        0     9392 2024-04-15 16:12:36.353089 furthrmind-0.1b2/furthrmind/collection/researchitem.py
--rwxr-xr-x   0        0        0     6138 2024-04-15 16:12:36.219089 furthrmind-0.1b2/furthrmind/collection/sample.py
--rwxr-xr-x   0        0        0     4226 2024-04-15 16:12:36.302470 furthrmind-0.1b2/furthrmind/collection/unit.py
--rwxr-xr-x   0        0        0     9478 2024-03-22 14:47:35.501823 furthrmind-0.1b2/furthrmind/file_loader.py
--rwxr-xr-x   0        0        0     1058 2024-03-15 14:50:00.492475 furthrmind-0.1b2/furthrmind/utils.py
--rwxr-xr-x   0        0        0      723 2024-04-15 16:28:01.241448 furthrmind-0.1b2/pyproject.toml
--rw-r--r--   0        0        0     3706 1970-01-01 00:00:00.000000 furthrmind-0.1b2/PKG-INFO
+-rwxr-xr-x   0        0        0    35823 2024-03-07 10:34:57.137547 furthrmind-0.1b3/LICENSE
+-rwxr-xr-x   0        0        0     2869 2024-04-15 16:25:04.221154 furthrmind-0.1b3/README.md
+-rwxr-xr-x   0        0        0     2353 2024-04-15 18:16:46.911920 furthrmind-0.1b3/furthrmind/__init__.py
+-rwxr-xr-x   0        0        0      471 2024-03-15 09:10:04.917117 furthrmind-0.1b3/furthrmind/collection/__init__.py
+-rwxr-xr-x   0        0        0    19254 2024-04-15 16:12:36.344833 furthrmind-0.1b3/furthrmind/collection/baseclass.py
+-rwxr-xr-x   0        0        0     2157 2024-04-15 16:12:36.211301 furthrmind-0.1b3/furthrmind/collection/category.py
+-rwxr-xr-x   0        0        0     5824 2024-04-15 16:12:36.294403 furthrmind-0.1b3/furthrmind/collection/column.py
+-rwxr-xr-x   0        0        0     5946 2024-04-15 16:12:36.330101 furthrmind-0.1b3/furthrmind/collection/comboboxentry.py
+-rwxr-xr-x   0        0        0     6775 2024-04-15 16:12:36.362346 furthrmind-0.1b3/furthrmind/collection/datatable.py
+-rwxr-xr-x   0        0        0     6085 2024-04-15 16:12:36.202385 furthrmind-0.1b3/furthrmind/collection/experiment.py
+-rwxr-xr-x   0        0        0     4805 2024-04-15 16:12:36.283804 furthrmind-0.1b3/furthrmind/collection/field.py
+-rwxr-xr-x   0        0        0    10119 2024-04-15 16:12:36.242521 furthrmind-0.1b3/furthrmind/collection/fielddata.py
+-rwxr-xr-x   0        0        0     1553 2024-04-15 16:12:36.336627 furthrmind-0.1b3/furthrmind/collection/file.py
+-rwxr-xr-x   0        0        0     4114 2024-04-15 16:12:36.310225 furthrmind-0.1b3/furthrmind/collection/group.py
+-rwxr-xr-x   0        0        0        1 2024-03-13 11:54:06.300443 furthrmind-0.1b3/furthrmind/collection/import_collection.py
+-rwxr-xr-x   0        0        0     2803 2024-04-15 16:12:36.192946 furthrmind-0.1b3/furthrmind/collection/project.py
+-rwxr-xr-x   0        0        0     9392 2024-04-15 16:12:36.353089 furthrmind-0.1b3/furthrmind/collection/researchitem.py
+-rwxr-xr-x   0        0        0     6138 2024-04-15 16:12:36.219089 furthrmind-0.1b3/furthrmind/collection/sample.py
+-rwxr-xr-x   0        0        0     4226 2024-04-15 16:12:36.302470 furthrmind-0.1b3/furthrmind/collection/unit.py
+-rwxr-xr-x   0        0        0     9478 2024-03-22 14:47:35.501823 furthrmind-0.1b3/furthrmind/file_loader.py
+-rwxr-xr-x   0        0        0     1058 2024-03-15 14:50:00.492475 furthrmind-0.1b3/furthrmind/utils.py
+-rwxr-xr-x   0        0        0      723 2024-04-15 18:20:03.904352 furthrmind-0.1b3/pyproject.toml
+-rw-r--r--   0        0        0     3706 1970-01-01 00:00:00.000000 furthrmind-0.1b3/PKG-INFO
```

### Comparing `furthrmind-0.1b2/LICENSE` & `furthrmind-0.1b3/LICENSE`

 * *Files identical despite different names*

### Comparing `furthrmind-0.1b2/README.md` & `furthrmind-0.1b3/README.md`

 * *Files identical despite different names*

### Comparing `furthrmind-0.1b2/furthrmind/collection/baseclass.py` & `furthrmind-0.1b3/furthrmind/collection/baseclass.py`

 * *Files identical despite different names*

### Comparing `furthrmind-0.1b2/furthrmind/collection/category.py` & `furthrmind-0.1b3/furthrmind/collection/category.py`

 * *Files identical despite different names*

### Comparing `furthrmind-0.1b2/furthrmind/collection/column.py` & `furthrmind-0.1b3/furthrmind/collection/column.py`

 * *Files identical despite different names*

### Comparing `furthrmind-0.1b2/furthrmind/collection/comboboxentry.py` & `furthrmind-0.1b3/furthrmind/collection/comboboxentry.py`

 * *Files identical despite different names*

### Comparing `furthrmind-0.1b2/furthrmind/collection/datatable.py` & `furthrmind-0.1b3/furthrmind/collection/datatable.py`

 * *Files identical despite different names*

### Comparing `furthrmind-0.1b2/furthrmind/collection/experiment.py` & `furthrmind-0.1b3/furthrmind/collection/experiment.py`

 * *Files identical despite different names*

### Comparing `furthrmind-0.1b2/furthrmind/collection/field.py` & `furthrmind-0.1b3/furthrmind/collection/field.py`

 * *Files identical despite different names*

### Comparing `furthrmind-0.1b2/furthrmind/collection/fielddata.py` & `furthrmind-0.1b3/furthrmind/collection/fielddata.py`

 * *Files identical despite different names*

### Comparing `furthrmind-0.1b2/furthrmind/collection/file.py` & `furthrmind-0.1b3/furthrmind/collection/file.py`

 * *Files identical despite different names*

### Comparing `furthrmind-0.1b2/furthrmind/collection/group.py` & `furthrmind-0.1b3/furthrmind/collection/group.py`

 * *Files identical despite different names*

### Comparing `furthrmind-0.1b2/furthrmind/collection/project.py` & `furthrmind-0.1b3/furthrmind/collection/project.py`

 * *Files identical despite different names*

### Comparing `furthrmind-0.1b2/furthrmind/collection/researchitem.py` & `furthrmind-0.1b3/furthrmind/collection/researchitem.py`

 * *Files identical despite different names*

### Comparing `furthrmind-0.1b2/furthrmind/collection/sample.py` & `furthrmind-0.1b3/furthrmind/collection/sample.py`

 * *Files identical despite different names*

### Comparing `furthrmind-0.1b2/furthrmind/collection/unit.py` & `furthrmind-0.1b3/furthrmind/collection/unit.py`

 * *Files identical despite different names*

### Comparing `furthrmind-0.1b2/furthrmind/file_loader.py` & `furthrmind-0.1b3/furthrmind/file_loader.py`

 * *Files identical despite different names*

### Comparing `furthrmind-0.1b2/furthrmind/utils.py` & `furthrmind-0.1b3/furthrmind/utils.py`

 * *Files identical despite different names*

### Comparing `furthrmind-0.1b2/pyproject.toml` & `furthrmind-0.1b3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "furthrmind"
-version = "0.1b2"
+version = "0.1b3"
 description = "Official python wrapper for the FURTHRmind rest api."
 authors = ["Daniel Menne"]
 license = "GNU GENERAL PUBLIC LICENSE Version 3"
 readme = "README.md"
 repository = "https://github.com/FURTHRresearch/furthrmind-sdk"
 
 [tool.poetry.dependencies]
```

### Comparing `furthrmind-0.1b2/PKG-INFO` & `furthrmind-0.1b3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: furthrmind
-Version: 0.1b2
+Version: 0.1b3
 Summary: Official python wrapper for the FURTHRmind rest api.
 Home-page: https://github.com/FURTHRresearch/furthrmind-sdk
 License: GNU GENERAL PUBLIC LICENSE Version 3
 Author: Daniel Menne
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

