# Comparing `tmp/pymeos_cffi-1.1.0rc2.post1.tar.gz` & `tmp/pymeos_cffi-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymeos_cffi-1.1.0rc2.post1.tar", last modified: Tue Mar 19 18:28:33 2024, max compression
+gzip compressed data, was "pymeos_cffi-1.1.1.tar", last modified: Mon Apr 15 22:23:21 2024, max compression
```

## Comparing `pymeos_cffi-1.1.0rc2.post1.tar` & `pymeos_cffi-1.1.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 diviloper  (1000) diviloper  (1000)        0 2024-03-19 18:28:33.703716 pymeos_cffi-1.1.0rc2.post1/
--rw-r--r--   0 diviloper  (1000) diviloper  (1000)     1603 2024-02-09 23:37:51.000000 pymeos_cffi-1.1.0rc2.post1/LICENSE
--rw-r--r--   0 diviloper  (1000) diviloper  (1000)       34 2024-02-09 23:37:51.000000 pymeos_cffi-1.1.0rc2.post1/MANIFEST.in
--rw-r--r--   0 diviloper  (1000) diviloper  (1000)     4347 2024-03-19 18:28:33.703716 pymeos_cffi-1.1.0rc2.post1/PKG-INFO
--rw-r--r--   0 diviloper  (1000) diviloper  (1000)     1343 2024-02-11 11:45:36.000000 pymeos_cffi-1.1.0rc2.post1/README.md
-drwxr-xr-x   0 diviloper  (1000) diviloper  (1000)        0 2024-03-19 18:28:33.693716 pymeos_cffi-1.1.0rc2.post1/pymeos_cffi/
--rw-r--r--   0 diviloper  (1000) diviloper  (1000)    56856 2024-03-19 18:28:12.000000 pymeos_cffi-1.1.0rc2.post1/pymeos_cffi/__init__.py
-drwxr-xr-x   0 diviloper  (1000) diviloper  (1000)        0 2024-03-19 18:28:33.703716 pymeos_cffi-1.1.0rc2.post1/pymeos_cffi/builder/
--rw-r--r--   0 diviloper  (1000) diviloper  (1000)        0 2024-02-09 23:37:51.000000 pymeos_cffi-1.1.0rc2.post1/pymeos_cffi/builder/__init__.py
--rw-r--r--   0 diviloper  (1000) diviloper  (1000)     3572 2024-02-11 11:45:36.000000 pymeos_cffi-1.1.0rc2.post1/pymeos_cffi/builder/build_header.py
--rw-r--r--   0 diviloper  (1000) diviloper  (1000)      468 2024-02-20 20:02:17.000000 pymeos_cffi-1.1.0rc2.post1/pymeos_cffi/builder/build_pymeos.py
--rw-r--r--   0 diviloper  (1000) diviloper  (1000)    20388 2024-03-19 18:28:08.000000 pymeos_cffi-1.1.0rc2.post1/pymeos_cffi/builder/build_pymeos_functions.py
--rw-r--r--   0 diviloper  (1000) diviloper  (1000)     3622 2024-02-24 09:07:52.000000 pymeos_cffi-1.1.0rc2.post1/pymeos_cffi/builder/build_pymeos_functions_modifiers.py
--rw-r--r--   0 diviloper  (1000) diviloper  (1000)   157880 2024-03-19 18:28:09.000000 pymeos_cffi-1.1.0rc2.post1/pymeos_cffi/builder/meos.h
--rw-r--r--   0 diviloper  (1000) diviloper  (1000)     3521 2024-02-11 11:45:36.000000 pymeos_cffi-1.1.0rc2.post1/pymeos_cffi/builder/objects.py
--rw-r--r--   0 diviloper  (1000) diviloper  (1000)     3682 2024-02-11 11:45:36.000000 pymeos_cffi-1.1.0rc2.post1/pymeos_cffi/enums.py
--rw-r--r--   0 diviloper  (1000) diviloper  (1000)     4078 2024-02-11 11:45:36.000000 pymeos_cffi-1.1.0rc2.post1/pymeos_cffi/errors.py
--rw-r--r--   0 diviloper  (1000) diviloper  (1000)   640066 2024-03-19 18:28:27.000000 pymeos_cffi-1.1.0rc2.post1/pymeos_cffi/functions.py
-drwxr-xr-x   0 diviloper  (1000) diviloper  (1000)        0 2024-03-19 18:28:33.703716 pymeos_cffi-1.1.0rc2.post1/pymeos_cffi.egg-info/
--rw-r--r--   0 diviloper  (1000) diviloper  (1000)     4347 2024-03-19 18:28:33.000000 pymeos_cffi-1.1.0rc2.post1/pymeos_cffi.egg-info/PKG-INFO
--rw-r--r--   0 diviloper  (1000) diviloper  (1000)      583 2024-03-19 18:28:33.000000 pymeos_cffi-1.1.0rc2.post1/pymeos_cffi.egg-info/SOURCES.txt
--rw-r--r--   0 diviloper  (1000) diviloper  (1000)        1 2024-03-19 18:28:33.000000 pymeos_cffi-1.1.0rc2.post1/pymeos_cffi.egg-info/dependency_links.txt
--rw-r--r--   0 diviloper  (1000) diviloper  (1000)       29 2024-03-19 18:28:33.000000 pymeos_cffi-1.1.0rc2.post1/pymeos_cffi.egg-info/requires.txt
--rw-r--r--   0 diviloper  (1000) diviloper  (1000)       23 2024-03-19 18:28:33.000000 pymeos_cffi-1.1.0rc2.post1/pymeos_cffi.egg-info/top_level.txt
--rw-r--r--   0 diviloper  (1000) diviloper  (1000)     1372 2024-02-11 11:45:36.000000 pymeos_cffi-1.1.0rc2.post1/pyproject.toml
--rw-r--r--   0 diviloper  (1000) diviloper  (1000)       38 2024-03-19 18:28:33.703716 pymeos_cffi-1.1.0rc2.post1/setup.cfg
--rw-r--r--   0 diviloper  (1000) diviloper  (1000)      190 2024-02-11 11:45:36.000000 pymeos_cffi-1.1.0rc2.post1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 22:23:21.612689 pymeos_cffi-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (127)     1603 2024-04-15 22:23:11.000000 pymeos_cffi-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       34 2024-04-15 22:23:11.000000 pymeos_cffi-1.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     4288 2024-04-15 22:23:21.612689 pymeos_cffi-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1343 2024-04-15 22:23:11.000000 pymeos_cffi-1.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 22:23:21.608689 pymeos_cffi-1.1.1/pymeos_cffi/
+-rw-r--r--   0 runner    (1001) docker     (127)    56847 2024-04-15 22:23:11.000000 pymeos_cffi-1.1.1/pymeos_cffi/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 22:23:21.612689 pymeos_cffi-1.1.1/pymeos_cffi/builder/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 22:23:11.000000 pymeos_cffi-1.1.1/pymeos_cffi/builder/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3970 2024-04-15 22:23:11.000000 pymeos_cffi-1.1.1/pymeos_cffi/builder/build_header.py
+-rw-r--r--   0 runner    (1001) docker     (127)      769 2024-04-15 22:23:11.000000 pymeos_cffi-1.1.1/pymeos_cffi/builder/build_pymeos.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20388 2024-04-15 22:23:11.000000 pymeos_cffi-1.1.1/pymeos_cffi/builder/build_pymeos_functions.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3980 2024-04-15 22:23:11.000000 pymeos_cffi-1.1.1/pymeos_cffi/builder/build_pymeos_functions_modifiers.py
+-rw-r--r--   0 runner    (1001) docker     (127)   157940 2024-04-15 22:23:11.000000 pymeos_cffi-1.1.1/pymeos_cffi/builder/meos.h
+-rw-r--r--   0 runner    (1001) docker     (127)     3521 2024-04-15 22:23:11.000000 pymeos_cffi-1.1.1/pymeos_cffi/builder/objects.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3682 2024-04-15 22:23:11.000000 pymeos_cffi-1.1.1/pymeos_cffi/enums.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4078 2024-04-15 22:23:11.000000 pymeos_cffi-1.1.1/pymeos_cffi/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)   640377 2024-04-15 22:23:11.000000 pymeos_cffi-1.1.1/pymeos_cffi/functions.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 22:23:21.612689 pymeos_cffi-1.1.1/pymeos_cffi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4288 2024-04-15 22:23:21.000000 pymeos_cffi-1.1.1/pymeos_cffi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      583 2024-04-15 22:23:21.000000 pymeos_cffi-1.1.1/pymeos_cffi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 22:23:21.000000 pymeos_cffi-1.1.1/pymeos_cffi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       29 2024-04-15 22:23:21.000000 pymeos_cffi-1.1.1/pymeos_cffi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-15 22:23:21.000000 pymeos_cffi-1.1.1/pymeos_cffi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)     1327 2024-04-15 22:23:11.000000 pymeos_cffi-1.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 22:23:21.612689 pymeos_cffi-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1156 2024-04-15 22:23:11.000000 pymeos_cffi-1.1.1/setup.py
```

### Comparing `pymeos_cffi-1.1.0rc2.post1/LICENSE` & `pymeos_cffi-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pymeos_cffi-1.1.0rc2.post1/PKG-INFO` & `pymeos_cffi-1.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymeos_cffi
-Version: 1.1.0rc2.post1
+Version: 1.1.1
 Summary: PyMEOS wrapper for the MEOS C Library.
 Author-email: Victor Divi <vdiviloper@gmail.com>
 License: PostgreSQL License
         
         -------------------------------------------------------------------------------
         This PyMEOS CFFI code is provided under The PostgreSQL License.
         
@@ -29,24 +29,23 @@
 Classifier: License :: OSI Approved :: PostgreSQL License
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: cffi
 Requires-Dist: python-dateutil
 Requires-Dist: shapely
 
 # ![MEOS Logo](https://raw.githubusercontent.com/MobilityDB/PyMEOS/master/docs/images/PyMEOS%20Logo.png)
```

### Comparing `pymeos_cffi-1.1.0rc2.post1/README.md` & `pymeos_cffi-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `pymeos_cffi-1.1.0rc2.post1/pymeos_cffi/__init__.py` & `pymeos_cffi-1.1.1/pymeos_cffi/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from .functions import *
 from .enums import *
 from .errors import *
 
-__version__ = "1.1.0rc2-post1"
+__version__ = "1.1.1"
 __all__ = [
     # Exceptions
     "MeosException",
     "MeosInternalError",
     "MeosArgumentError",
     "MeosIoError",
     "MeosInternalTypeError",
```

### Comparing `pymeos_cffi-1.1.0rc2.post1/pymeos_cffi/builder/build_header.py` & `pymeos_cffi-1.1.1/pymeos_cffi/builder/build_header.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 import os.path
+import platform
 import re
 import subprocess
 import sys
 from typing import Set, Tuple
 
 
 def get_defined_functions(library_path):
-    result = subprocess.check_output(["nm", "-gD", library_path])
+    result = subprocess.check_output(["nm", "-g", library_path])
     output = result.decode("utf-8")
     lines = output.splitlines()
     defined = {line.split(" ")[-1] for line in lines if " T " in line}
     return defined
 
 
 def remove_undefined_functions(content, so_path):
     defined = get_defined_functions(so_path)
     undefined_types = ["json_object"]
 
     def remove_if_not_defined(m):
         function = m.group(0).split("(")[0].strip().split(" ")[-1].strip("*")
-        if function in defined:
+        if function in defined or (
+            sys.platform == "darwin" and ("_" + function) in defined
+        ):
             for t in undefined_types:
                 if t in m.group(0):
                     print(f"Removing function due to undefined type {t}: {function}")
                     return f"/* {m.group(0)}  (undefined type {t}) */"
             return m.group(0)
         else:
             print(f"Removing undefined function: {function}")
@@ -97,8 +100,14 @@
         f.write(global_content)
 
 
 if __name__ == "__main__":
     if len(sys.argv) > 1:
         main(*sys.argv[1:])
     else:
-        main("/usr/local/include", "/usr/local/lib/libmeos.so")
+        if sys.platform == "linux":
+            main("/usr/local/include", "/usr/local/lib/libmeos.so")
+        elif sys.platform == "darwin":
+            if platform.processor() == "arm":
+                main("/opt/homebrew/include", "/opt/homebrew/lib/libmeos.dylib")
+            else:
+                main("/usr/local/include", "/usr/local/lib/libmeos.dylib")
```

### Comparing `pymeos_cffi-1.1.0rc2.post1/pymeos_cffi/builder/build_pymeos_functions.py` & `pymeos_cffi-1.1.1/pymeos_cffi/builder/build_pymeos_functions.py`

 * *Files identical despite different names*

### Comparing `pymeos_cffi-1.1.0rc2.post1/pymeos_cffi/builder/build_pymeos_functions_modifiers.py` & `pymeos_cffi-1.1.1/pymeos_cffi/builder/build_pymeos_functions_modifiers.py`

 * *Files 8% similar despite different names*

```diff
@@ -38,14 +38,22 @@
     return function.replace("_ffi.cast('const text *', x)", "cstring2text(x)").replace(
         "'List[const text]'", "List[str]"
     )
 
 
 def meos_initialize_modifier(_: str) -> str:
     return """def meos_initialize(tz_str: "Optional[str]") -> None:
+    
+    if "PROJ_DATA" not in os.environ and "PROJ_LIB" not in os.environ:
+        proj_dir = os.path.join(os.path.dirname(__file__), "proj_data")
+        if os.path.exists(proj_dir):
+            # Assume we are in a wheel and the PROJ data is in the package
+            os.environ["PROJ_DATA"] = proj_dir
+            os.environ["PROJ_LIB"] = proj_dir
+    
     tz_str_converted = tz_str.encode('utf-8') if tz_str is not None else _ffi.NULL
     _lib.meos_initialize(tz_str_converted, _lib.py_error_handler)"""
 
 
 def remove_error_check_modifier(function: str) -> str:
     return function.replace("    _check_error()\n", "")
```

### Comparing `pymeos_cffi-1.1.0rc2.post1/pymeos_cffi/builder/meos.h` & `pymeos_cffi-1.1.1/pymeos_cffi/builder/meos.h`

 * *Files 0% similar despite different names*

```diff
@@ -424,14 +424,15 @@
 } interpType;
 
 typedef enum
 {
   INTERSECTS =     0,
   CONTAINS =       1,
   TOUCHES =        2,
+  COVERS =         3,
 } spatialRel;
 
 typedef struct
 {
   int32 vl_len_;        
   uint8 temptype;       
   uint8 subtype;        
@@ -540,17 +541,17 @@
 extern int meos_errno(void);
 extern int meos_errno_set(int err);
 extern int meos_errno_restore(int err);
 extern int meos_errno_reset(void);
 
 typedef void (*error_handler_fn)(int, int, char *);
 
-extern void meos_initialize_timezone(const char *name);
+/* extern void meos_initialize_timezone(const char *name);  (undefined) */
 extern void meos_initialize_error_handler(error_handler_fn err_handler);
-extern void meos_finalize_timezone(void);
+/* extern void meos_finalize_timezone(void);  (undefined) */
 
 extern bool meos_set_datestyle(char *newval, void *extra);
 extern bool meos_set_intervalstyle(char *newval, int extra);
 extern char *meos_get_datestyle(void);
 extern char *meos_get_intervalstyle(void);
 
 extern void meos_initialize(const char *tz_str, error_handler_fn err_handler);
```

### Comparing `pymeos_cffi-1.1.0rc2.post1/pymeos_cffi/builder/objects.py` & `pymeos_cffi-1.1.1/pymeos_cffi/builder/objects.py`

 * *Files identical despite different names*

### Comparing `pymeos_cffi-1.1.0rc2.post1/pymeos_cffi/enums.py` & `pymeos_cffi-1.1.1/pymeos_cffi/enums.py`

 * *Files identical despite different names*

### Comparing `pymeos_cffi-1.1.0rc2.post1/pymeos_cffi/errors.py` & `pymeos_cffi-1.1.1/pymeos_cffi/errors.py`

 * *Files identical despite different names*

### Comparing `pymeos_cffi-1.1.0rc2.post1/pymeos_cffi/functions.py` & `pymeos_cffi-1.1.1/pymeos_cffi/functions.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 import logging
+import os
+
 from datetime import datetime, timedelta, date
 from typing import Any, Tuple, Optional, List
 
 import _meos_cffi
 import shapely.geometry as spg
 from dateutil.parser import parse
 from shapely import wkt, get_srid, set_srid
@@ -199,14 +201,20 @@
     result = _lib.meos_get_intervalstyle()
     _check_error()
     result = _ffi.string(result).decode("utf-8")
     return result if result != _ffi.NULL else None
 
 
 def meos_initialize(tz_str: "Optional[str]") -> None:
+    if "PROJ_DATA" not in os.environ and "PROJ_LIB" not in os.environ:
+        # Assume we are in a wheel and the PROJ data is in the package
+        proj_dir = os.path.join(os.path.dirname(__file__), "proj_data")
+        os.environ["PROJ_DATA"] = proj_dir
+        os.environ["PROJ_LIB"] = proj_dir
+
     tz_str_converted = tz_str.encode("utf-8") if tz_str is not None else _ffi.NULL
     _lib.meos_initialize(tz_str_converted, _lib.py_error_handler)
 
 
 def meos_finalize() -> None:
     _lib.meos_finalize()
     _check_error()
```

### Comparing `pymeos_cffi-1.1.0rc2.post1/pymeos_cffi.egg-info/PKG-INFO` & `pymeos_cffi-1.1.1/pymeos_cffi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymeos_cffi
-Version: 1.1.0rc2.post1
+Version: 1.1.1
 Summary: PyMEOS wrapper for the MEOS C Library.
 Author-email: Victor Divi <vdiviloper@gmail.com>
 License: PostgreSQL License
         
         -------------------------------------------------------------------------------
         This PyMEOS CFFI code is provided under The PostgreSQL License.
         
@@ -29,24 +29,23 @@
 Classifier: License :: OSI Approved :: PostgreSQL License
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: C
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Operating System :: POSIX
 Classifier: Operating System :: Unix
-Requires-Python: >=3.7
+Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: cffi
 Requires-Dist: python-dateutil
 Requires-Dist: shapely
 
 # ![MEOS Logo](https://raw.githubusercontent.com/MobilityDB/PyMEOS/master/docs/images/PyMEOS%20Logo.png)
```

### Comparing `pymeos_cffi-1.1.0rc2.post1/pymeos_cffi.egg-info/SOURCES.txt` & `pymeos_cffi-1.1.1/pymeos_cffi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pymeos_cffi-1.1.0rc2.post1/pyproject.toml` & `pymeos_cffi-1.1.1/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -16,28 +16,27 @@
     'License :: OSI Approved :: PostgreSQL License',
     'Development Status :: 4 - Beta',
     'Intended Audience :: Developers',
     'Intended Audience :: Science/Research',
     'Programming Language :: C',
     'Programming Language :: Python',
     'Programming Language :: Python :: 3',
-    'Programming Language :: Python :: 3.7',
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
     'Programming Language :: Python :: 3.11',
     'Programming Language :: Python :: 3 :: Only',
     'Programming Language :: Python :: Implementation :: CPython',
     'Operating System :: POSIX',
     'Operating System :: Unix'
 ]
 readme = 'README.md'
 license = { file = 'LICENSE' }
 
-requires-python = '>=3.7'
+requires-python = '>=3.8'
 dependencies = [
     'cffi',
     'python-dateutil',
     'shapely'
 ]
 
 [project.urls]
```

