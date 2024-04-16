# Comparing `tmp/imsosorrybutinc-0.6.0.tar.gz` & `tmp/imsosorrybutinc-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "imsosorrybutinc-0.6.0.tar", last modified: Sun Apr  7 15:04:36 2024, max compression
+gzip compressed data, was "imsosorrybutinc-0.7.0.tar", last modified: Tue Apr 16 01:14:55 2024, max compression
```

## Comparing `imsosorrybutinc-0.6.0.tar` & `imsosorrybutinc-0.7.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:04:36.363379 imsosorrybutinc-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-07 15:04:33.000000 imsosorrybutinc-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-07 15:04:33.000000 imsosorrybutinc-0.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-07 15:04:36.363379 imsosorrybutinc-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-07 15:04:33.000000 imsosorrybutinc-0.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-04-07 15:04:33.000000 imsosorrybutinc-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-07 15:04:36.363379 imsosorrybutinc-0.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-07 15:04:33.000000 imsosorrybutinc-0.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:04:36.359379 imsosorrybutinc-0.6.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:04:36.363379 imsosorrybutinc-0.6.0/src/imsosorrybutinc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-07 15:04:36.000000 imsosorrybutinc-0.6.0/src/imsosorrybutinc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-07 15:04:36.000000 imsosorrybutinc-0.6.0/src/imsosorrybutinc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-07 15:04:36.000000 imsosorrybutinc-0.6.0/src/imsosorrybutinc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-07 15:04:36.000000 imsosorrybutinc-0.6.0/src/imsosorrybutinc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-07 15:04:36.000000 imsosorrybutinc-0.6.0/src/imsosorrybutinc.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:04:36.363379 imsosorrybutinc-0.6.0/src/uwuifier/
--rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-07 15:04:33.000000 imsosorrybutinc-0.6.0/src/uwuifier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    51178 2024-04-07 15:04:33.000000 imsosorrybutinc-0.6.0/src/uwuifier/_uwuifier.c
--rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-07 15:04:33.000000 imsosorrybutinc-0.6.0/src/uwuifier/_uwuifier.pyi
--rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-07 15:04:33.000000 imsosorrybutinc-0.6.0/src/uwuifier/py.typed
--rw-r--r--   0 runner    (1001) docker     (127)    20515 2024-04-07 15:04:33.000000 imsosorrybutinc-0.6.0/src/uwuifier/uwuifier.stringlib.h
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-07 15:04:36.363379 imsosorrybutinc-0.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-04-07 15:04:33.000000 imsosorrybutinc-0.6.0/tests/test_uwuify.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 01:14:55.358030 imsosorrybutinc-0.7.0/
+-rw-r--r--   0 runner    (1001) docker     (127)     1074 2024-04-16 01:14:52.000000 imsosorrybutinc-0.7.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-16 01:14:52.000000 imsosorrybutinc-0.7.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-16 01:14:55.358030 imsosorrybutinc-0.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-16 01:14:52.000000 imsosorrybutinc-0.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-04-16 01:14:52.000000 imsosorrybutinc-0.7.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 01:14:55.358030 imsosorrybutinc-0.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)      273 2024-04-16 01:14:52.000000 imsosorrybutinc-0.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 01:14:55.354030 imsosorrybutinc-0.7.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 01:14:55.358030 imsosorrybutinc-0.7.0/src/imsosorrybutinc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1016 2024-04-16 01:14:55.000000 imsosorrybutinc-0.7.0/src/imsosorrybutinc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      421 2024-04-16 01:14:55.000000 imsosorrybutinc-0.7.0/src/imsosorrybutinc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 01:14:55.000000 imsosorrybutinc-0.7.0/src/imsosorrybutinc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      114 2024-04-16 01:14:55.000000 imsosorrybutinc-0.7.0/src/imsosorrybutinc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-16 01:14:55.000000 imsosorrybutinc-0.7.0/src/imsosorrybutinc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 01:14:55.358030 imsosorrybutinc-0.7.0/src/uwuifier/
+-rw-r--r--   0 runner    (1001) docker     (127)      261 2024-04-16 01:14:52.000000 imsosorrybutinc-0.7.0/src/uwuifier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    51231 2024-04-16 01:14:52.000000 imsosorrybutinc-0.7.0/src/uwuifier/_uwuifier.c
+-rw-r--r--   0 runner    (1001) docker     (127)      376 2024-04-16 01:14:52.000000 imsosorrybutinc-0.7.0/src/uwuifier/_uwuifier.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)       27 2024-04-16 01:14:52.000000 imsosorrybutinc-0.7.0/src/uwuifier/py.typed
+-rw-r--r--   0 runner    (1001) docker     (127)    20515 2024-04-16 01:14:52.000000 imsosorrybutinc-0.7.0/src/uwuifier/uwuifier.stringlib.h
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 01:14:55.358030 imsosorrybutinc-0.7.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)     1721 2024-04-16 01:14:52.000000 imsosorrybutinc-0.7.0/tests/test_uwuify.py
```

### Comparing `imsosorrybutinc-0.6.0/LICENSE` & `imsosorrybutinc-0.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `imsosorrybutinc-0.6.0/PKG-INFO` & `imsosorrybutinc-0.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imsosorrybutinc
-Version: 0.6.0
+Version: 0.7.0
 Summary: Sometimes it can be necessary to call upon the ancient arts... but in C!
 Author-email: Bradley Reynolds <bradley.reynolds@darbia.dev>
 License: MIT
 Project-URL: repository, https://github.com/letsbuilda/imsosorrybutinc/
 Project-URL: documentation, https://docs.letsbuilda.dev/imsosorrybutinc/
 Requires-Python: <3.14,>=3.10
 Description-Content-Type: text/markdown
```

### Comparing `imsosorrybutinc-0.6.0/pyproject.toml` & `imsosorrybutinc-0.7.0/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "imsosorrybutinc"
-version = "0.6.0"
+version = "0.7.0"
 description = "Sometimes it can be necessary to call upon the ancient arts... but in C!"
 authors = [
     { name = "Bradley Reynolds", email = "bradley.reynolds@darbia.dev" },
 ]
 license = { text = "MIT" }
 readme = "README.md"
 requires-python = ">=3.10,<3.14"
```

### Comparing `imsosorrybutinc-0.6.0/src/imsosorrybutinc.egg-info/PKG-INFO` & `imsosorrybutinc-0.7.0/src/imsosorrybutinc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: imsosorrybutinc
-Version: 0.6.0
+Version: 0.7.0
 Summary: Sometimes it can be necessary to call upon the ancient arts... but in C!
 Author-email: Bradley Reynolds <bradley.reynolds@darbia.dev>
 License: MIT
 Project-URL: repository, https://github.com/letsbuilda/imsosorrybutinc/
 Project-URL: documentation, https://docs.letsbuilda.dev/imsosorrybutinc/
 Requires-Python: <3.14,>=3.10
 Description-Content-Type: text/markdown
```

### Comparing `imsosorrybutinc-0.6.0/src/uwuifier/_uwuifier.c` & `imsosorrybutinc-0.7.0/src/uwuifier/_uwuifier.c`

 * *Files 0% similar despite different names*

```diff
@@ -162,15 +162,15 @@
 #undef STRINGLIB_FAST_MEMCHR
 
 #define STRINGLIB(F)            ucs4_##F
 #define STRINGLIB_SIZEOF_CHAR   4
 #define STRINGLIB_CHAR          Py_UCS4
 #if SIZEOF_WCHAR_T == 4
 #define STRINGLIB_FAST_MEMCHR(s, c, n)              \
-    (Py_UCS2 *)wmemchr((const wchar_t *)(s), c, n)
+    (Py_UCS4 *)wmemchr((const wchar_t *)(s), c, n)
 #endif
 #include "uwuifier.stringlib.h"
 #undef STRINGLIB
 #undef STRINGLIB_SIZEOF_CHAR
 #undef STRINGLIB_CHAR
 #undef STRINGLIB_FAST_MEMCHR
 
@@ -383,26 +383,30 @@
 ascii_askind(void const *data, Py_ssize_t len, int kind)
 {
     void *result;
 
     switch (kind) {
     case PyUnicode_2BYTE_KIND:
         result = PyMem_New(Py_UCS2, len);
-        if (UNLIKELY(!result))
-            return PyErr_NoMemory();
+        if (UNLIKELY(!result)) {
+            PyErr_NoMemory();
+            return NULL;
+        }
         CONVERT_BYTES(
             Py_UCS1, Py_UCS2,
             (const Py_UCS1 *)data,
             ((const Py_UCS1 *)data) + len,
             result);
         return result;
     case PyUnicode_4BYTE_KIND:
         result = PyMem_New(Py_UCS4, len);
-        if (UNLIKELY(!result))
-            return PyErr_NoMemory();
+        if (UNLIKELY(!result)) {
+            PyErr_NoMemory();
+            return NULL;
+        }
         CONVERT_BYTES(
             Py_UCS1, Py_UCS4,
             (const Py_UCS1 *)data,
             ((const Py_UCS1 *)data) + len,
             result);
         return result;
     default:
@@ -740,14 +744,15 @@
 
     if (UNLIKELY(count == 0)) {
         Py_DECREF(u);
         return Py_NewRef(text);
     }
     if (count != n) {
         if (UNLIKELY(PyUnicode_Resize(&u, ol + count) < 0)) {
+            Py_DECREF(u);
             return NULL;
         }
     }
 
     return u;
 }
 
@@ -956,14 +961,15 @@
 
     if (UNLIKELY(count == 0)) {
         Py_DECREF(u);
         return Py_NewRef(text);
     }
     if (count != n) {
         if (UNLIKELY(PyUnicode_Resize(&u, ol + count+count) < 0)) {
+            Py_DECREF(u);
             return NULL;
         }
     }
 
     return u;
 }
 
@@ -1206,14 +1212,15 @@
             }
             copy_fromU2p_to1B(PyUnicode_DATA(u),
                               PyUnicode_DATA(u2), new_size, ukind);
             Py_DECREF(u);
             u = u2;
         }
         else if (UNLIKELY(PyUnicode_Resize(&u, new_size) < 0)) {
+            Py_DECREF(u);
             return NULL;
         }
     }
 
     return u;
 }
 
@@ -1400,14 +1407,15 @@
 
     if (UNLIKELY(count == 0)) {
         Py_DECREF(u);
         return Py_NewRef(text);
     }
     if (count != n) {
         if (UNLIKELY(PyUnicode_Resize(&u, ol + count) < 0)) {
+            Py_DECREF(u);
             return NULL;
         }
     }
 
     return u;
 }
 
@@ -1526,19 +1534,19 @@
 /* Here we could use _PyLong_Sign() or other easy stuff from CPython to be
    faster, but of course it's totally taboo to have private, unstable,
    implementation-dependent functions. grr. ¬∧¬ */
 LOCAL(int)
 long_sign(PyObject *l)
 {
     PyObject *zero = PyLong_FromLong(0L);
-    if (UNLIKELY(zero == NULL)) {
-        return -1;
-    }
+    if (UNLIKELY(zero == NULL)) return -1;
+
     int res = PyObject_RichCompareBool(l, zero, Py_GT);
     Py_DECREF(zero);
+
     return res;
 }
 
 static PyObject *
 uwuify(PyObject *module,
        PyObject *const *args,
        Py_ssize_t nargs,
@@ -1610,17 +1618,15 @@
         text = args[0];
         goto skip_keyarg_checks;
     }
 
     if (has_SS) {
         if (PyLong_CheckExact(SS_o)) {
             int sign = long_sign(SS_o);
-            if (sign == -1) {
-                 return NULL;
-            }
+            if (sign == -1) return NULL;
             SS = sign > 0 ? 1. : 0.;
         }
         else if (PyFloat_CheckExact(SS_o)) {
             SS = PyFloat_AS_DOUBLE(SS_o);
         }
         else {
             FMT_ERROR_RET(Type,
@@ -1629,17 +1635,15 @@
                           Py_TYPE(SS_o)->tp_name);
         }
     }
 
     if (has_ES) {
         if (PyLong_CheckExact(ES_o)) {
             int sign = long_sign(ES_o);
-            if (sign == -1) {
-                 return NULL;
-            }
+            if (sign == -1) return NULL;
             ES = sign > 0 ? 1. : 0.;
         }
         else if (PyFloat_CheckExact(ES_o)) {
             ES = PyFloat_AS_DOUBLE(ES_o);
         }
         else {
             FMT_ERROR_RET(Type,
@@ -1648,17 +1652,15 @@
                           Py_TYPE(ES_o)->tp_name);
         }
     }
 
     if (has_TS) {
         if (PyLong_CheckExact(TS_o)) {
             int sign = long_sign(TS_o);
-            if (sign == -1) {
-                 return NULL;
-            }
+            if (sign == -1) return NULL;
             TS = sign > 0 ? 1. : 0.;
         }
         else if (PyFloat_CheckExact(TS_o)) {
             TS = PyFloat_AS_DOUBLE(TS_o);
         }
         else {
             FMT_ERROR_RET(Type,
@@ -1681,15 +1683,15 @@
     if (UNLIKELY(tmp == NULL)) { \
         Py_DECREF(text); \
         return NULL; \
     } \
     if (text != tmp) { \
         nochange = 0; \
         Py_SETREF(text, tmp); \
-    }
+    } \
 
     uwuifier_modstate *state = PyModule_GetState(module);
     assert(state != NULL);
     PyObject *tmp = PyObject_CallMethodNoArgs(text, state->lower__str__);
     if (UNLIKELY(tmp == NULL)) return NULL;
     text = tmp;
```

### Comparing `imsosorrybutinc-0.6.0/src/uwuifier/uwuifier.stringlib.h` & `imsosorrybutinc-0.7.0/src/uwuifier/uwuifier.stringlib.h`

 * *Files identical despite different names*

### Comparing `imsosorrybutinc-0.6.0/tests/test_uwuify.py` & `imsosorrybutinc-0.7.0/tests/test_uwuify.py`

 * *Files identical despite different names*

