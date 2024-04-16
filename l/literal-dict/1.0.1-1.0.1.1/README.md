# Comparing `tmp/literal_dict-1.0.1.tar.gz` & `tmp/literal_dict-1.0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "literal_dict-1.0.1.tar", last modified: Sat Apr 13 15:22:19 2024, max compression
+gzip compressed data, was "literal_dict-1.0.1.1.tar", last modified: Tue Apr 16 11:29:14 2024, max compression
```

## Comparing `literal_dict-1.0.1.tar` & `literal_dict-1.0.1.1.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0     2823 2024-04-13 15:14:24.786745 literal_dict-1.0.1/README.md
--rw-r--r--   0        0        0      637 2024-04-13 15:22:19.825087 literal_dict-1.0.1/pyproject.toml
--rw-r--r--   0        0        0     1664 2024-04-13 14:33:47.507045 literal_dict-1.0.1/src/literal_dict.py
--rw-r--r--   0        0        0     2981 1970-01-01 00:00:00.000000 literal_dict-1.0.1/PKG-INFO
+-rw-r--r--   0        0        0     2823 2024-04-13 15:14:24.786745 literal_dict-1.0.1.1/README.md
+-rw-r--r--   0        0        0      639 2024-04-16 11:29:14.160271 literal_dict-1.0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1624 2024-04-16 11:29:05.117134 literal_dict-1.0.1.1/src/literal_dict.py
+-rw-r--r--   0        0        0     2983 1970-01-01 00:00:00.000000 literal_dict-1.0.1.1/PKG-INFO
```

### Comparing `literal_dict-1.0.1/README.md` & `literal_dict-1.0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `literal_dict-1.0.1/pyproject.toml` & `literal_dict-1.0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "literal-dict"
-version = "1.0.1"
+version = "1.0.1.1"
 description = "Use JavaScript-like object definition syntax in Python"
 authors = [
     { name = "Muspi Merol", email = "me@muspimerol.site" },
 ]
 dependencies = []
 requires-python = ">=3.6"
 readme = "README.md"
```

### Comparing `literal_dict-1.0.1/src/literal_dict.py` & `literal_dict-1.0.1.1/src/literal_dict.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 from inspect import currentframe
-from typing import Callable, Generic, Mapping, Sequence, TypeVar, Union, cast
+from typing import Callable, Generic, Sequence, TypeVar, Union, cast
 
 T = TypeVar("T")
-D = TypeVar("D", bound=Mapping)
+D = TypeVar("D")
 
 
 class DictBuilder(Generic[D]):
-    def __init__(self, mapping_constructor: Callable[[dict], D] = dict):
-        self.constructor = mapping_constructor
+    def __init__(self, constructor: Callable[[dict], D] = dict):
+        self.constructor = constructor
 
     def __getitem__(self, args: Union[slice, T, Sequence[Union[slice, T]]]) -> D:
         if not isinstance(args, tuple):
             args = (args,)  # type: ignore
 
         frame = currentframe()
         assert frame, "Unable to get the current frame."
```

### Comparing `literal_dict-1.0.1/PKG-INFO` & `literal_dict-1.0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: literal-dict
-Version: 1.0.1
+Version: 1.0.1.1
 Summary: Use JavaScript-like object definition syntax in Python
 Author-Email: Muspi Merol <me@muspimerol.site>
 License: MIT
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 
 # Literal Dict
```

