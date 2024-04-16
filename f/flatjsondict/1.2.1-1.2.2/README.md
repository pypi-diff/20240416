# Comparing `tmp/flatjsondict-1.2.1.tar.gz` & `tmp/flatjsondict-1.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flatjsondict-1.2.1.tar", max compression
+gzip compressed data, was "flatjsondict-1.2.2.tar", max compression
```

## Comparing `flatjsondict-1.2.1.tar` & `flatjsondict-1.2.2.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1497 2024-04-10 18:33:35.334981 flatjsondict-1.2.1/LICENSE
--rw-r--r--   0        0        0     4278 2024-04-10 18:33:35.334981 flatjsondict-1.2.1/README.md
--rw-r--r--   0        0        0       58 2024-04-10 18:33:35.334981 flatjsondict-1.2.1/flatjsondict/__init__.py
--rw-r--r--   0        0        0    21477 2024-04-10 18:33:35.334981 flatjsondict-1.2.1/flatjsondict/flatjsondict.py
--rw-r--r--   0        0        0      546 2024-04-10 18:33:35.334981 flatjsondict-1.2.1/pyproject.toml
--rw-r--r--   0        0        0     5175 1970-01-01 00:00:00.000000 flatjsondict-1.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1497 2024-04-16 21:36:19.612819 flatjsondict-1.2.2/LICENSE
+-rw-r--r--   0        0        0     4278 2024-04-16 21:36:19.612819 flatjsondict-1.2.2/README.md
+-rw-r--r--   0        0        0       58 2024-04-16 21:36:19.612819 flatjsondict-1.2.2/flatjsondict/__init__.py
+-rw-r--r--   0        0        0    21600 2024-04-16 21:36:19.612819 flatjsondict-1.2.2/flatjsondict/flatjsondict.py
+-rw-r--r--   0        0        0      546 2024-04-16 21:36:19.612819 flatjsondict-1.2.2/pyproject.toml
+-rw-r--r--   0        0        0     5175 1970-01-01 00:00:00.000000 flatjsondict-1.2.2/PKG-INFO
```

### Comparing `flatjsondict-1.2.1/LICENSE` & `flatjsondict-1.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `flatjsondict-1.2.1/README.md` & `flatjsondict-1.2.2/README.md`

 * *Files identical despite different names*

### Comparing `flatjsondict-1.2.1/flatjsondict/flatjsondict.py` & `flatjsondict-1.2.2/flatjsondict/flatjsondict.py`

 * *Files 1% similar despite different names*

```diff
@@ -368,20 +368,23 @@
         return isinstance(key, str) and self._keypath_separator in key
 
     def _listkeys(self) -> list:
         """Return a list with `FlatJson` keys."""
         result = []
         for key, value in self._values.items():
             if isinstance(self._values[key], FlatJson):
-                subkeys = self._values[key]._listkeys()
-                for subkey in subkeys:
-                    result.append(
-                        [key] + subkey if isinstance(subkey, list)
-                        else [subkey]
-                    )
+                if len(value) == 0:
+                    result.append([key])
+                else:
+                    subkeys = self._values[key]._listkeys()
+                    for subkey in subkeys:
+                        result.append(
+                            [key] + subkey if isinstance(subkey, list)
+                            else [subkey]
+                        )
             else:
                 result.append([key])
         return result
 
     def _as_dict(self) -> dict:
         """Return nested dictionary with data from `FlatJson`."""
         out = {}
```

### Comparing `flatjsondict-1.2.1/pyproject.toml` & `flatjsondict-1.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "flatjsondict"
-version = "1.2.1"
+version = "1.2.2"
 description = "JSON-like data manipulation and transformation to and from nested parent-child and flat label-value data items."
 authors = ["Martins Bruvelis <martins.bruvelis@gmail.com>"]
 readme = "README.md"
 repository = "https://gitlab.com/martins-bruvelis/flatjsondict"
 documentation = "https://gitlab.com/martins-bruvelis/flatjsondict/-/blob/main/README.md"
 
 [tool.poetry.dependencies]
```

### Comparing `flatjsondict-1.2.1/PKG-INFO` & `flatjsondict-1.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flatjsondict
-Version: 1.2.1
+Version: 1.2.2
 Summary: JSON-like data manipulation and transformation to and from nested parent-child and flat label-value data items.
 Home-page: https://gitlab.com/martins-bruvelis/flatjsondict
 Author: Martins Bruvelis
 Author-email: martins.bruvelis@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

