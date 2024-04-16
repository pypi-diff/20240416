# Comparing `tmp/json_write-0.0.1.tar.gz` & `tmp/json_write-0.0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "json_write-0.0.1.tar", max compression
+gzip compressed data, was "json_write-0.0.1.1.tar", max compression
```

## Comparing `json_write-0.0.1.tar` & `json_write-0.0.1.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rwxr-xr-x   0        0        0     1100 2024-01-29 04:51:11.346824 json_write-0.0.1/LICENSE
--rwxr-xr-x   0        0        0     8220 2024-04-16 05:44:45.470965 json_write-0.0.1/json_write.py
--rw-r--r--   0        0        0     1086 2024-04-16 05:51:57.470481 json_write-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      160 2024-04-16 05:49:52.935809 json_write-0.0.1/readme.md
--rw-r--r--   0        0        0     1636 1970-01-01 00:00:00.000000 json_write-0.0.1/PKG-INFO
+-rwxr-xr-x   0        0        0     1100 2024-01-29 04:51:11.346824 json_write-0.0.1.1/LICENSE
+-rwxr-xr-x   0        0        0     8218 2024-04-16 11:41:06.926096 json_write-0.0.1.1/json_write.py
+-rw-r--r--   0        0        0     1088 2024-04-16 11:43:10.310682 json_write-0.0.1.1/pyproject.toml
+-rw-r--r--   0        0        0      160 2024-04-16 05:49:52.935809 json_write-0.0.1.1/readme.md
+-rw-r--r--   0        0        0     1638 1970-01-01 00:00:00.000000 json_write-0.0.1.1/PKG-INFO
```

### Comparing `json_write-0.0.1/LICENSE` & `json_write-0.0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `json_write-0.0.1/json_write.py` & `json_write-0.0.1.1/json_write.py`

 * *Files 1% similar despite different names*

```diff
@@ -275,27 +275,27 @@
             if value is not None:
                 val = value(val)
             if not_first:
                 seek(-1, 1)
                 tpl = b",%s]"
             else:
                 tpl = b"[%s]"
-                not_first = False
+                not_first = True
             write(tpl % dumps(val))
     else:
         while True:
             val = yield
             if value is not None:
                 val = value(val)
             if not_first:
                 seek(-1, 1)
                 tpl = b",%s:%s}"
             else:
                 tpl = b"{%s:%s}"
-                not_first = False
+                not_first = True
             write(tpl % (dumps(str(key(val))), dumps(val)))
 
 
 def json_ensure_write(
     it: Iterable, 
     /, 
     path: PathType,
```

### Comparing `json_write-0.0.1/pyproject.toml` & `json_write-0.0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "json_write"
-version = "0.0.1"
+version = "0.0.1.1"
 description = "JSON write tools."
 authors = ["ChenyangGao <wosiwujm@gmail.com>"]
 license = "MIT"
 readme = "readme.md"
 homepage = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/json_write"
 repository = "https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/json_write"
 keywords = ["json", "write"]
```

### Comparing `json_write-0.0.1/PKG-INFO` & `json_write-0.0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: json_write
-Version: 0.0.1
+Version: 0.0.1.1
 Summary: JSON write tools.
 Home-page: https://github.com/ChenyangGao/web-mount-packs/tree/main/python-module/json_write
 License: MIT
 Keywords: json,write
 Author: ChenyangGao
 Author-email: wosiwujm@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
```

