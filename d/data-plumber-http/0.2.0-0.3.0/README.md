# Comparing `tmp/data-plumber-http-0.2.0.tar.gz` & `tmp/data-plumber-http-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data-plumber-http-0.2.0.tar", last modified: Mon Apr 15 21:02:34 2024, max compression
+gzip compressed data, was "data-plumber-http-0.3.0.tar", last modified: Tue Apr 16 21:28:06 2024, max compression
```

## Comparing `data-plumber-http-0.2.0.tar` & `data-plumber-http-0.3.0.tar`

### file list

```diff
@@ -1,33 +1,34 @@
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-15 21:02:34.791844 data-plumber-http-0.2.0/
--rwxrwxrwx   0 root         (0) root         (0)     1080 2024-01-22 19:31:33.000000 data-plumber-http-0.2.0/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)    10476 2024-04-15 21:02:34.791637 data-plumber-http-0.2.0/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     9284 2024-04-15 21:02:26.000000 data-plumber-http-0.2.0/README.md
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-15 21:02:34.782919 data-plumber-http-0.2.0/data_plumber_http/
--rwxrwxrwx   0 root         (0) root         (0)       41 2024-04-14 11:44:45.000000 data-plumber-http-0.2.0/data_plumber_http/__init__.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-15 21:02:34.785386 data-plumber-http-0.2.0/data_plumber_http/decorators/
--rwxrwxrwx   0 root         (0) root         (0)      329 2024-04-14 11:13:20.000000 data-plumber-http-0.2.0/data_plumber_http/decorators/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1503 2024-04-14 22:14:15.000000 data-plumber-http-0.2.0/data_plumber_http/decorators/flask_input.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-15 21:02:34.786697 data-plumber-http-0.2.0/data_plumber_http/keys/
--rwxrwxrwx   0 root         (0) root         (0)      163 2024-04-14 09:01:26.000000 data-plumber-http-0.2.0/data_plumber_http/keys/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)       62 2024-04-14 09:02:00.000000 data-plumber-http-0.2.0/data_plumber_http/keys/all_of.py
--rwxrwxrwx   0 root         (0) root         (0)       62 2024-04-14 09:01:53.000000 data-plumber-http-0.2.0/data_plumber_http/keys/one_of.py
--rwxrwxrwx   0 root         (0) root         (0)     1443 2024-04-14 22:14:00.000000 data-plumber-http-0.2.0/data_plumber_http/keys/property.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-15 21:02:34.791016 data-plumber-http-0.2.0/data_plumber_http/types/
--rwxrwxrwx   0 root         (0) root         (0)     3952 2024-04-15 21:02:26.000000 data-plumber-http-0.2.0/data_plumber_http/types/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     1318 2024-04-15 21:02:26.000000 data-plumber-http-0.2.0/data_plumber_http/types/array.py
--rwxrwxrwx   0 root         (0) root         (0)      354 2024-04-14 22:13:32.000000 data-plumber-http-0.2.0/data_plumber_http/types/boolean.py
--rwxrwxrwx   0 root         (0) root         (0)     3094 2024-04-15 21:02:26.000000 data-plumber-http-0.2.0/data_plumber_http/types/file_system_object.py
--rwxrwxrwx   0 root         (0) root         (0)     1608 2024-04-14 20:05:12.000000 data-plumber-http-0.2.0/data_plumber_http/types/float.py
--rwxrwxrwx   0 root         (0) root         (0)     1603 2024-04-14 20:04:49.000000 data-plumber-http-0.2.0/data_plumber_http/types/integer.py
--rwxrwxrwx   0 root         (0) root         (0)      908 2024-04-14 22:13:42.000000 data-plumber-http-0.2.0/data_plumber_http/types/number.py
--rwxrwxrwx   0 root         (0) root         (0)    13720 2024-04-14 22:13:45.000000 data-plumber-http-0.2.0/data_plumber_http/types/object.py
--rwxrwxrwx   0 root         (0) root         (0)     1500 2024-04-14 22:13:52.000000 data-plumber-http-0.2.0/data_plumber_http/types/string.py
--rwxrwxrwx   0 root         (0) root         (0)     2093 2024-04-15 21:02:26.000000 data-plumber-http-0.2.0/data_plumber_http/types/url.py
-drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-15 21:02:34.784748 data-plumber-http-0.2.0/data_plumber_http.egg-info/
--rwxrwxrwx   0 root         (0) root         (0)    10476 2024-04-15 21:02:34.000000 data-plumber-http-0.2.0/data_plumber_http.egg-info/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)      832 2024-04-15 21:02:34.000000 data-plumber-http-0.2.0/data_plumber_http.egg-info/SOURCES.txt
--rwxrwxrwx   0 root         (0) root         (0)        1 2024-04-15 21:02:34.000000 data-plumber-http-0.2.0/data_plumber_http.egg-info/dependency_links.txt
--rwxrwxrwx   0 root         (0) root         (0)       76 2024-04-15 21:02:34.000000 data-plumber-http-0.2.0/data_plumber_http.egg-info/requires.txt
--rwxrwxrwx   0 root         (0) root         (0)       18 2024-04-15 21:02:34.000000 data-plumber-http-0.2.0/data_plumber_http.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)       38 2024-04-15 21:02:34.791947 data-plumber-http-0.2.0/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1924 2024-04-15 21:02:26.000000 data-plumber-http-0.2.0/setup.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-16 21:28:06.590482 data-plumber-http-0.3.0/
+-rwxrwxrwx   0 root         (0) root         (0)     1080 2024-01-22 19:31:33.000000 data-plumber-http-0.3.0/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)    10758 2024-04-16 21:28:06.590299 data-plumber-http-0.3.0/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     9284 2024-04-15 21:02:26.000000 data-plumber-http-0.3.0/README.md
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-16 21:28:06.581728 data-plumber-http-0.3.0/data_plumber_http/
+-rwxrwxrwx   0 root         (0) root         (0)       41 2024-04-14 11:44:45.000000 data-plumber-http-0.3.0/data_plumber_http/__init__.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-16 21:28:06.584313 data-plumber-http-0.3.0/data_plumber_http/decorators/
+-rwxrwxrwx   0 root         (0) root         (0)      329 2024-04-14 11:13:20.000000 data-plumber-http-0.3.0/data_plumber_http/decorators/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1503 2024-04-14 22:14:15.000000 data-plumber-http-0.3.0/data_plumber_http/decorators/flask_input.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-16 21:28:06.585690 data-plumber-http-0.3.0/data_plumber_http/keys/
+-rwxrwxrwx   0 root         (0) root         (0)      163 2024-04-14 09:01:26.000000 data-plumber-http-0.3.0/data_plumber_http/keys/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)       62 2024-04-14 09:02:00.000000 data-plumber-http-0.3.0/data_plumber_http/keys/all_of.py
+-rwxrwxrwx   0 root         (0) root         (0)       62 2024-04-14 09:01:53.000000 data-plumber-http-0.3.0/data_plumber_http/keys/one_of.py
+-rwxrwxrwx   0 root         (0) root         (0)     1881 2024-04-16 21:27:48.000000 data-plumber-http-0.3.0/data_plumber_http/keys/property.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-16 21:28:06.589732 data-plumber-http-0.3.0/data_plumber_http/types/
+-rwxrwxrwx   0 root         (0) root         (0)     3983 2024-04-16 21:27:48.000000 data-plumber-http-0.3.0/data_plumber_http/types/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     1318 2024-04-15 21:02:26.000000 data-plumber-http-0.3.0/data_plumber_http/types/array.py
+-rwxrwxrwx   0 root         (0) root         (0)      354 2024-04-14 22:13:32.000000 data-plumber-http-0.3.0/data_plumber_http/types/boolean.py
+-rwxrwxrwx   0 root         (0) root         (0)     3094 2024-04-15 21:02:26.000000 data-plumber-http-0.3.0/data_plumber_http/types/file_system_object.py
+-rwxrwxrwx   0 root         (0) root         (0)     1608 2024-04-14 20:05:12.000000 data-plumber-http-0.3.0/data_plumber_http/types/float.py
+-rwxrwxrwx   0 root         (0) root         (0)     1603 2024-04-14 20:04:49.000000 data-plumber-http-0.3.0/data_plumber_http/types/integer.py
+-rwxrwxrwx   0 root         (0) root         (0)      383 2024-04-16 21:27:48.000000 data-plumber-http-0.3.0/data_plumber_http/types/null.py
+-rwxrwxrwx   0 root         (0) root         (0)      908 2024-04-14 22:13:42.000000 data-plumber-http-0.3.0/data_plumber_http/types/number.py
+-rwxrwxrwx   0 root         (0) root         (0)    13793 2024-04-16 21:27:48.000000 data-plumber-http-0.3.0/data_plumber_http/types/object.py
+-rwxrwxrwx   0 root         (0) root         (0)     1500 2024-04-14 22:13:52.000000 data-plumber-http-0.3.0/data_plumber_http/types/string.py
+-rwxrwxrwx   0 root         (0) root         (0)     2093 2024-04-15 21:02:26.000000 data-plumber-http-0.3.0/data_plumber_http/types/url.py
+drwxrwxrwx   0 root         (0) root         (0)        0 2024-04-16 21:28:06.583613 data-plumber-http-0.3.0/data_plumber_http.egg-info/
+-rwxrwxrwx   0 root         (0) root         (0)    10758 2024-04-16 21:28:06.000000 data-plumber-http-0.3.0/data_plumber_http.egg-info/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)      864 2024-04-16 21:28:06.000000 data-plumber-http-0.3.0/data_plumber_http.egg-info/SOURCES.txt
+-rwxrwxrwx   0 root         (0) root         (0)        1 2024-04-16 21:28:06.000000 data-plumber-http-0.3.0/data_plumber_http.egg-info/dependency_links.txt
+-rwxrwxrwx   0 root         (0) root         (0)       76 2024-04-16 21:28:06.000000 data-plumber-http-0.3.0/data_plumber_http.egg-info/requires.txt
+-rwxrwxrwx   0 root         (0) root         (0)       18 2024-04-16 21:28:06.000000 data-plumber-http-0.3.0/data_plumber_http.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)       38 2024-04-16 21:28:06.590571 data-plumber-http-0.3.0/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1924 2024-04-16 21:27:48.000000 data-plumber-http-0.3.0/setup.py
```

### Comparing `data-plumber-http-0.2.0/LICENSE` & `data-plumber-http-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `data-plumber-http-0.2.0/PKG-INFO` & `data-plumber-http-0.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-plumber-http
-Version: 0.2.0
+Version: 0.3.0
 Summary: http extension for the data-plumber python framework
 Home-page: https://pypi.org/project/data-plumber-http/
 Author: Steffen Richters-Finger
 Author-email: srichters@uni-muenster.de
 License: MIT
 Project-URL: Source, https://github.com/RichtersFinger/data-plumber-http
 Platform: UNKNOWN
@@ -239,14 +239,25 @@
 
 Responses.BAD_VALUE.status = 405
 ```
 
 
 # Changelog
 
+## [0.3.0] - 2024-04-16
+
+### Added
+
+- added `Null`-type (`1657715`)
+
+### Fixed
+
+- fixed potentially problematic `Property` where the `name`-property is an empty string (`409551d`)
+- fixed issue where an `Object` with `model` causes crash when field is missing in input (`f7e30c2`)
+
 ## [0.2.0] - 2024-04-16
 
 ### Changed
 
 - changed `Array` constructor argument `items` to allow `None` (accept any content from JSON) (`ee24833`)
 
 ### Added
```

### Comparing `data-plumber-http-0.2.0/README.md` & `data-plumber-http-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `data-plumber-http-0.2.0/data_plumber_http/decorators/flask_input.py` & `data-plumber-http-0.3.0/data_plumber_http/decorators/flask_input.py`

 * *Files identical despite different names*

### Comparing `data-plumber-http-0.2.0/data_plumber_http/keys/property.py` & `data-plumber-http-0.3.0/data_plumber_http/keys/property.py`

 * *Files 18% similar despite different names*

```diff
@@ -29,12 +29,28 @@
         name: Optional[str] = None,
         default: Optional[Callable[[...], Any] | Any] = None,
         required: bool = False,
         fill_with_none: bool = False,
         validation_only: bool = False
     ) -> None:
         self.origin = origin
-        self.name = name or origin
+        if name is None:
+            self._name = origin
+        else:
+            self._name = name
+        if self._name == "":
+            raise ValueError("Empty Property-name is not allowed.")
         self.default = default
         self.required = required
         self.fill_with_none = fill_with_none
         self.validation_only = validation_only
+
+    @property
+    def name(self) -> str:
+        """`Property`'s `name`."""
+        return self._name
+
+    @name.setter
+    def name(self, value) -> None:
+        if value == "":
+            raise ValueError("Empty Property-name is not allowed.")
+        self._name = value
```

### Comparing `data-plumber-http-0.2.0/data_plumber_http/types/__init__.py` & `data-plumber-http-0.3.0/data_plumber_http/types/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -117,19 +117,20 @@
         self["kwargs"] = kwargs
 
 
 from .array import Array
 from .boolean import Boolean
 from .float import Float
 from .integer import Integer
+from .null import Null
 from .number import Number
 from .object import Object
 from .string import String
 from .url import Url
 from .file_system_object import FileSystemObject
 
 
 __all__ = [
     "Responses",
-    "Array", "Boolean", "Float", "Integer", "Number", "Object", "String",
-    "Url", "FileSystemObject",
+    "Array", "Boolean", "Float", "Integer", "Null", "Number", "Object",
+    "String", "Url", "FileSystemObject",
 ]
```

### Comparing `data-plumber-http-0.2.0/data_plumber_http/types/array.py` & `data-plumber-http-0.3.0/data_plumber_http/types/array.py`

 * *Files identical despite different names*

### Comparing `data-plumber-http-0.2.0/data_plumber_http/types/file_system_object.py` & `data-plumber-http-0.3.0/data_plumber_http/types/file_system_object.py`

 * *Files identical despite different names*

### Comparing `data-plumber-http-0.2.0/data_plumber_http/types/float.py` & `data-plumber-http-0.3.0/data_plumber_http/types/float.py`

 * *Files identical despite different names*

### Comparing `data-plumber-http-0.2.0/data_plumber_http/types/integer.py` & `data-plumber-http-0.3.0/data_plumber_http/types/integer.py`

 * *Files identical despite different names*

### Comparing `data-plumber-http-0.2.0/data_plumber_http/types/number.py` & `data-plumber-http-0.3.0/data_plumber_http/types/number.py`

 * *Files identical despite different names*

### Comparing `data-plumber-http-0.2.0/data_plumber_http/types/object.py` & `data-plumber-http-0.3.0/data_plumber_http/types/object.py`

 * *Files 2% similar despite different names*

```diff
@@ -288,16 +288,17 @@
             output.last_status or Responses.GOOD.status
         )
 
     def assemble(self, _loc: Optional[str] = None) -> Pipeline:
         """
         Returns `Pipeline` that processes a `json`-input.
         """
-        def finalizer(data, **kwargs):
-            data.value = self._model(**data.kwargs)
+        def finalizer(data, records, **kwargs):
+            if records[-1].status == Responses.GOOD.status:
+                data.value = self._model(**data.kwargs)
         p = Pipeline(
             exit_on_status=lambda status: status >= 400,
             initialize_output=Output,
             finalize_output=finalizer
         )
         __loc = _loc or "."
         if self._accept_only is not None:
```

### Comparing `data-plumber-http-0.2.0/data_plumber_http/types/string.py` & `data-plumber-http-0.3.0/data_plumber_http/types/string.py`

 * *Files identical despite different names*

### Comparing `data-plumber-http-0.2.0/data_plumber_http/types/url.py` & `data-plumber-http-0.3.0/data_plumber_http/types/url.py`

 * *Files identical despite different names*

### Comparing `data-plumber-http-0.2.0/data_plumber_http.egg-info/PKG-INFO` & `data-plumber-http-0.3.0/data_plumber_http.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-plumber-http
-Version: 0.2.0
+Version: 0.3.0
 Summary: http extension for the data-plumber python framework
 Home-page: https://pypi.org/project/data-plumber-http/
 Author: Steffen Richters-Finger
 Author-email: srichters@uni-muenster.de
 License: MIT
 Project-URL: Source, https://github.com/RichtersFinger/data-plumber-http
 Platform: UNKNOWN
@@ -239,14 +239,25 @@
 
 Responses.BAD_VALUE.status = 405
 ```
 
 
 # Changelog
 
+## [0.3.0] - 2024-04-16
+
+### Added
+
+- added `Null`-type (`1657715`)
+
+### Fixed
+
+- fixed potentially problematic `Property` where the `name`-property is an empty string (`409551d`)
+- fixed issue where an `Object` with `model` causes crash when field is missing in input (`f7e30c2`)
+
 ## [0.2.0] - 2024-04-16
 
 ### Changed
 
 - changed `Array` constructor argument `items` to allow `None` (accept any content from JSON) (`ee24833`)
 
 ### Added
```

### Comparing `data-plumber-http-0.2.0/data_plumber_http.egg-info/SOURCES.txt` & `data-plumber-http-0.3.0/data_plumber_http.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -15,11 +15,12 @@
 data_plumber_http/keys/property.py
 data_plumber_http/types/__init__.py
 data_plumber_http/types/array.py
 data_plumber_http/types/boolean.py
 data_plumber_http/types/file_system_object.py
 data_plumber_http/types/float.py
 data_plumber_http/types/integer.py
+data_plumber_http/types/null.py
 data_plumber_http/types/number.py
 data_plumber_http/types/object.py
 data_plumber_http/types/string.py
 data_plumber_http/types/url.py
```

### Comparing `data-plumber-http-0.2.0/setup.py` & `data-plumber-http-0.3.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 requirements = \
     (Path(__file__).parent / "requirements.txt") \
         .read_text(encoding="utf8") \
         .strip() \
         .split("\n")
 
 setup(
-    version="0.2.0",
+    version="0.3.0",
     name="data-plumber-http",
     description="http extension for the data-plumber python framework",
     long_description=long_description,
     long_description_content_type="text/markdown",
     author="Steffen Richters-Finger",
     author_email="srichters@uni-muenster.de",
     license="MIT",
```

