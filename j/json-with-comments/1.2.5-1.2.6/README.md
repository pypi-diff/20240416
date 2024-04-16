# Comparing `tmp/json_with_comments-1.2.5.tar.gz` & `tmp/json_with_comments-1.2.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "json_with_comments-1.2.5.tar", max compression
+gzip compressed data, was "json_with_comments-1.2.6.tar", max compression
```

## Comparing `json_with_comments-1.2.5.tar` & `json_with_comments-1.2.6.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0     4924 2024-03-28 00:19:22.621248 json_with_comments-1.2.5/jsonc/__init__.py
--rw-r--r--   0        0        0     4311 2024-03-28 00:12:14.991592 json_with_comments-1.2.5/jsonc/_add_comments.py
--rw-r--r--   0        0        0     1269 2024-03-06 00:21:51.078785 json_with_comments-1.2.5/jsonc/_util.py
--rw-r--r--   0        0        0     1088 2024-02-05 00:29:56.953661 json_with_comments-1.2.5/LICENSE
--rw-r--r--   0        0        0     1220 2024-03-28 00:19:22.610278 json_with_comments-1.2.5/pyproject.toml
--rw-r--r--   0        0        0     1076 2024-02-05 00:29:56.969283 json_with_comments-1.2.5/README.md
--rw-r--r--   0        0        0     1894 1970-01-01 00:00:00.000000 json_with_comments-1.2.5/PKG-INFO
+-rw-r--r--   0        0        0     4997 2024-04-16 00:19:24.820726 json_with_comments-1.2.6/jsonc/__init__.py
+-rw-r--r--   0        0        0     4311 2024-03-28 00:12:14.991592 json_with_comments-1.2.6/jsonc/_add_comments.py
+-rw-r--r--   0        0        0      496 2024-04-16 00:14:30.586933 json_with_comments-1.2.6/jsonc/_types.py
+-rw-r--r--   0        0        0     1269 2024-03-06 00:21:51.078785 json_with_comments-1.2.6/jsonc/_util.py
+-rw-r--r--   0        0        0     1088 2024-02-05 00:29:56.953661 json_with_comments-1.2.6/LICENSE
+-rw-r--r--   0        0        0     1220 2024-04-16 00:19:24.807510 json_with_comments-1.2.6/pyproject.toml
+-rw-r--r--   0        0        0     1076 2024-02-05 00:29:56.969283 json_with_comments-1.2.6/README.md
+-rw-r--r--   0        0        0     1894 1970-01-01 00:00:00.000000 json_with_comments-1.2.6/PKG-INFO
```

### Comparing `json_with_comments-1.2.5/jsonc/__init__.py` & `json_with_comments-1.2.6/jsonc/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -19,32 +19,33 @@
 from typing import TYPE_CHECKING
 
 from jsonc._add_comments import _add_comments
 from jsonc._util import _add_trailing_comma, _remove_c_comment, _remove_trailing_comma
 
 if TYPE_CHECKING:
     from collections.abc import Callable
-    from typing import Any, TextIO
+    from typing import Any
 
     from jsonc._add_comments import Comments
+    from jsonc._types import SupportsRead, SupportsWrite
 
-__version__ = "1.2.5"
+__version__ = "1.2.6"
 __all__ = [
     "dump",
     "dumps",
     "load",
     "loads",
     "JSONDecoder",
     "JSONDecodeError",
     "JSONEncoder",
 ]
 
 
 def load(
-    fp: TextIO,
+    fp: SupportsRead[str],
     *,
     cls: type[json.JSONDecoder] | None = None,
     object_hook: Callable[[dict[Any, Any]], Any] | None = None,
     parse_float: Callable[[str], Any] | None = None,
     parse_int: Callable[[str], Any] | None = None,
     parse_constant: Callable[[str], Any] | None = None,
     object_pairs_hook: Callable[[list[tuple[Any, Any]]], Any] | None = None,
@@ -140,15 +141,15 @@
         return data
 
     return _add_comments(data, comments)
 
 
 def dump(
     obj: Any,
-    fp: TextIO,
+    fp: SupportsWrite[str],
     *,
     skipkeys=False,
     ensure_ascii=True,
     check_circular=True,
     allow_nan=True,
     cls: type[JSONEncoder] | None = None,
     indent: int | None = None,
```

### Comparing `json_with_comments-1.2.5/jsonc/_add_comments.py` & `json_with_comments-1.2.6/jsonc/_add_comments.py`

 * *Files identical despite different names*

### Comparing `json_with_comments-1.2.5/jsonc/_util.py` & `json_with_comments-1.2.6/jsonc/_util.py`

 * *Files identical despite different names*

### Comparing `json_with_comments-1.2.5/LICENSE` & `json_with_comments-1.2.6/LICENSE`

 * *Files identical despite different names*

### Comparing `json_with_comments-1.2.5/pyproject.toml` & `json_with_comments-1.2.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poetry-dynamic-versioning]
 enable = false
 
 [tool.poetry]
 name = "json-with-comments"
-version = "1.2.5"
+version = "1.2.6"
 description = "JSON with Comments for Python"
 license = "MIT"
 authors = ["Takumasa Nakamura <n.takumasa@gmail.com>"]
 readme = "README.md"
 repository = "https://github.com/n-takumasa/json-with-comments"
 classifiers = [
     "Topic :: Software Development :: Libraries :: Python Modules"
```

### Comparing `json_with_comments-1.2.5/README.md` & `json_with_comments-1.2.6/README.md`

 * *Files identical despite different names*

### Comparing `json_with_comments-1.2.5/PKG-INFO` & `json_with_comments-1.2.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: json-with-comments
-Version: 1.2.5
+Version: 1.2.6
 Summary: JSON with Comments for Python
 Home-page: https://github.com/n-takumasa/json-with-comments
 License: MIT
 Author: Takumasa Nakamura
 Author-email: n.takumasa@gmail.com
 Requires-Python: >=3.7
 Classifier: License :: OSI Approved :: MIT License
```

