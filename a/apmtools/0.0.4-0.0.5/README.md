# Comparing `tmp/apmtools-0.0.4.tar.gz` & `tmp/apmtools-0.0.5.tar.gz`

## Comparing `apmtools-0.0.4.tar` & `apmtools-0.0.5.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apmtools-0.0.4/src/apmtools/__init__.py
--rw-r--r--   0        0        0     9107 2020-02-02 00:00:00.000000 apmtools-0.0.4/src/apmtools/classes.py
--rw-r--r--   0        0        0    17745 2020-02-02 00:00:00.000000 apmtools-0.0.4/src/apmtools/data_processing.py
--rw-r--r--   0        0        0     2632 2020-02-02 00:00:00.000000 apmtools-0.0.4/src/apmtools/functions.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 apmtools-0.0.4/.gitignore
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 apmtools-0.0.4/LICENSE
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 apmtools-0.0.4/README.md
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 apmtools-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      567 2020-02-02 00:00:00.000000 apmtools-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 apmtools-0.0.5/src/apmtools/__init__.py
+-rw-r--r--   0        0        0     9091 2020-02-02 00:00:00.000000 apmtools-0.0.5/src/apmtools/classes.py
+-rw-r--r--   0        0        0    17745 2020-02-02 00:00:00.000000 apmtools-0.0.5/src/apmtools/data_processing.py
+-rw-r--r--   0        0        0     2632 2020-02-02 00:00:00.000000 apmtools-0.0.5/src/apmtools/functions.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 apmtools-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 apmtools-0.0.5/LICENSE
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 apmtools-0.0.5/README.md
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 apmtools-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      568 2020-02-02 00:00:00.000000 apmtools-0.0.5/PKG-INFO
```

### Comparing `apmtools-0.0.4/src/apmtools/classes.py` & `apmtools-0.0.5/src/apmtools/classes.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         if type(filter_dict) != type(dict()):
             print("subset function error: type filter_dict should be dict")
             return
         return_dict = self
         for i, j in filter_dict.items():
             a = {}
             for key, value in return_dict.items():
-                if hasattr(value, 'meta') & (type(value.metadata) == type({})) & (i in value.metadata.keys()):
+                if hasattr(value, 'meta') & (type(value.meta) == type({})) & (i in value.meta.keys()):
                     try:
                         if value.__getattr__('meta')[i] in j:
                             a[key] = value
                     except:
                         pass
                 else:
                     try:
@@ -51,15 +51,15 @@
 
     def set_attrib(self, attribute):
         """
         returns the set of attribute values for dictionary
         """
         return_set = set()
         for i in self.values():
-            if hasattr(i, 'meta') & (type(i.metadata) == type({})) & (attribute in i.metadata.keys()):
+            if hasattr(i, 'meta') & (type(i.meta) == type({})) & (attribute in i.meta.keys()):
                 try:
                     return_set.add(i.__getattr__('meta')[attribute])
                 except:
                     pass
             else:
                 try:
                     return_set.add(i.__getattr__(attribute))
```

### Comparing `apmtools-0.0.4/src/apmtools/data_processing.py` & `apmtools-0.0.5/src/apmtools/data_processing.py`

 * *Files identical despite different names*

### Comparing `apmtools-0.0.4/src/apmtools/functions.py` & `apmtools-0.0.5/src/apmtools/functions.py`

 * *Files identical despite different names*

### Comparing `apmtools-0.0.4/LICENSE` & `apmtools-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `apmtools-0.0.4/pyproject.toml` & `apmtools-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "apmtools"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Federico Lorenzetti", email="lorenzetti.federico@gmail.com" },
 ]
 description = "A collection of tools for processing air pollution monitoring data"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `apmtools-0.0.4/PKG-INFO` & `apmtools-0.0.5/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 Metadata-Version: 2.3
 Name: apmtools
-Version: 0.0.4
+Version: 0.0.5
 Summary: A collection of tools for processing air pollution monitoring data
 Project-URL: Homepage, https://github.com/federlorenz/apmtools
 Author-email: Federico Lorenzetti <lorenzetti.federico@gmail.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 # apmtools
-A collection of tools for processing air pollution monitoring data
+A collection of tools for processing air pollution monitoring data.
```

