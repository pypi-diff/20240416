# Comparing `tmp/zodbpickle-3.2.tar.gz` & `tmp/zodbpickle-3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zodbpickle-3.2.tar", last modified: Fri Feb 16 07:37:36 2024, max compression
+gzip compressed data, was "zodbpickle-3.3.tar", last modified: Tue Apr 16 06:21:42 2024, max compression
```

## Comparing `zodbpickle-3.2.tar` & `zodbpickle-3.3.tar`

### file list

```diff
@@ -1,40 +1,39 @@
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2024-02-16 07:37:36.194570 zodbpickle-3.2/
--rw-r--r--   0 m.howitz   (502) staff       (20)      584 2024-02-16 07:37:35.000000 zodbpickle-3.2/.coveragerc
--rwxr-xr-x   0 m.howitz   (502) staff       (20)     2255 2024-02-16 07:37:35.000000 zodbpickle-3.2/.manylinux-install.sh
--rwxr-xr-x   0 m.howitz   (502) staff       (20)      509 2024-02-16 07:37:35.000000 zodbpickle-3.2/.manylinux.sh
--rw-r--r--   0 m.howitz   (502) staff       (20)     5742 2024-02-16 07:37:35.000000 zodbpickle-3.2/CHANGES.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)      799 2024-02-16 07:37:35.000000 zodbpickle-3.2/CONTRIBUTING.md
--rw-r--r--   0 m.howitz   (502) staff       (20)     4824 2024-02-16 07:37:35.000000 zodbpickle-3.2/LICENSE.txt
--rw-r--r--   0 m.howitz   (502) staff       (20)      304 2024-02-16 07:37:35.000000 zodbpickle-3.2/MANIFEST.in
--rw-r--r--   0 m.howitz   (502) staff       (20)    13079 2024-02-16 07:37:36.194427 zodbpickle-3.2/PKG-INFO
--rw-r--r--   0 m.howitz   (502) staff       (20)     5914 2024-02-16 07:37:35.000000 zodbpickle-3.2/README.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)     1965 2024-02-16 07:37:35.000000 zodbpickle-3.2/appveyor.yml
--rw-r--r--   0 m.howitz   (502) staff       (20)      196 2024-02-16 07:37:35.000000 zodbpickle-3.2/buildout.cfg
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2024-02-16 07:37:36.189159 zodbpickle-3.2/patches/
--rw-r--r--   0 m.howitz   (502) staff       (20)     4450 2024-02-16 07:37:35.000000 zodbpickle-3.2/patches/pickle_bytes_code.diff
--rw-r--r--   0 m.howitz   (502) staff       (20)     5287 2024-02-16 07:37:35.000000 zodbpickle-3.2/patches/pickle_bytes_tests.diff
--rw-r--r--   0 m.howitz   (502) staff       (20)      685 2024-02-16 07:37:36.194870 zodbpickle-3.2/setup.cfg
--rw-r--r--   0 m.howitz   (502) staff       (20)     3038 2024-02-16 07:37:35.000000 zodbpickle-3.2/setup.py
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2024-02-16 07:37:36.186709 zodbpickle-3.2/src/
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2024-02-16 07:37:36.191673 zodbpickle-3.2/src/zodbpickle/
--rw-r--r--   0 m.howitz   (502) staff       (20)       44 2024-02-16 07:37:35.000000 zodbpickle-3.2/src/zodbpickle/__init__.py
--rw-r--r--   0 m.howitz   (502) staff       (20)   204576 2024-02-16 07:37:35.000000 zodbpickle-3.2/src/zodbpickle/_pickle_33.c
--rw-r--r--   0 m.howitz   (502) staff       (20)      891 2024-02-16 07:37:35.000000 zodbpickle-3.2/src/zodbpickle/fastpickle.py
--rw-r--r--   0 m.howitz   (502) staff       (20)       24 2024-02-16 07:37:35.000000 zodbpickle-3.2/src/zodbpickle/pickle.py
--rw-r--r--   0 m.howitz   (502) staff       (20)    52163 2024-02-16 07:37:35.000000 zodbpickle-3.2/src/zodbpickle/pickle_3.py
--rw-r--r--   0 m.howitz   (502) staff       (20)    87531 2024-02-16 07:37:35.000000 zodbpickle-3.2/src/zodbpickle/pickletools_3.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     1061 2024-02-16 07:37:35.000000 zodbpickle-3.2/src/zodbpickle/slowpickle.py
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2024-02-16 07:37:36.193724 zodbpickle-3.2/src/zodbpickle/tests/
--rw-r--r--   0 m.howitz   (502) staff       (20)      212 2024-02-16 07:37:35.000000 zodbpickle-3.2/src/zodbpickle/tests/__init__.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     5271 2024-02-16 07:37:35.000000 zodbpickle-3.2/src/zodbpickle/tests/pickle_3_tests.py
--rw-r--r--   0 m.howitz   (502) staff       (20)    68946 2024-02-16 07:37:35.000000 zodbpickle-3.2/src/zodbpickle/tests/pickletester_3.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     1363 2024-02-16 07:37:35.000000 zodbpickle-3.2/src/zodbpickle/tests/test_compile_flags.py
--rw-r--r--   0 m.howitz   (502) staff       (20)     1161 2024-02-16 07:37:35.000000 zodbpickle-3.2/src/zodbpickle/tests/test_pickle.py
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2024-02-16 07:37:36.193942 zodbpickle-3.2/src/zodbpickle.egg-info/
--rw-r--r--   0 m.howitz   (502) staff       (20)    13079 2024-02-16 07:37:36.000000 zodbpickle-3.2/src/zodbpickle.egg-info/PKG-INFO
--rw-r--r--   0 m.howitz   (502) staff       (20)      839 2024-02-16 07:37:36.000000 zodbpickle-3.2/src/zodbpickle.egg-info/SOURCES.txt
--rw-r--r--   0 m.howitz   (502) staff       (20)        1 2024-02-16 07:37:36.000000 zodbpickle-3.2/src/zodbpickle.egg-info/dependency_links.txt
--rw-r--r--   0 m.howitz   (502) staff       (20)        1 2024-02-16 07:37:36.000000 zodbpickle-3.2/src/zodbpickle.egg-info/not-zip-safe
--rw-r--r--   0 m.howitz   (502) staff       (20)       35 2024-02-16 07:37:36.000000 zodbpickle-3.2/src/zodbpickle.egg-info/requires.txt
--rw-r--r--   0 m.howitz   (502) staff       (20)       11 2024-02-16 07:37:36.000000 zodbpickle-3.2/src/zodbpickle.egg-info/top_level.txt
--rw-r--r--   0 m.howitz   (502) staff       (20)     1562 2024-02-16 07:37:35.000000 zodbpickle-3.2/tox.ini
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2024-04-16 06:21:42.430591 zodbpickle-3.3/
+-rw-r--r--   0 m.howitz   (502) staff       (20)      584 2024-04-16 06:21:42.000000 zodbpickle-3.3/.coveragerc
+-rwxr-xr-x   0 m.howitz   (502) staff       (20)     2255 2024-04-16 06:21:42.000000 zodbpickle-3.3/.manylinux-install.sh
+-rwxr-xr-x   0 m.howitz   (502) staff       (20)      509 2024-04-16 06:21:42.000000 zodbpickle-3.3/.manylinux.sh
+-rw-r--r--   0 m.howitz   (502) staff       (20)     5867 2024-04-16 06:21:42.000000 zodbpickle-3.3/CHANGES.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      799 2024-04-16 06:21:42.000000 zodbpickle-3.3/CONTRIBUTING.md
+-rw-r--r--   0 m.howitz   (502) staff       (20)     4824 2024-04-16 06:21:42.000000 zodbpickle-3.3/LICENSE.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)      283 2024-04-16 06:21:42.000000 zodbpickle-3.3/MANIFEST.in
+-rw-r--r--   0 m.howitz   (502) staff       (20)    13204 2024-04-16 06:21:42.430302 zodbpickle-3.3/PKG-INFO
+-rw-r--r--   0 m.howitz   (502) staff       (20)     5914 2024-04-16 06:21:42.000000 zodbpickle-3.3/README.rst
+-rw-r--r--   0 m.howitz   (502) staff       (20)      196 2024-04-16 06:21:42.000000 zodbpickle-3.3/buildout.cfg
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2024-04-16 06:21:42.426366 zodbpickle-3.3/patches/
+-rw-r--r--   0 m.howitz   (502) staff       (20)     4450 2024-04-16 06:21:42.000000 zodbpickle-3.3/patches/pickle_bytes_code.diff
+-rw-r--r--   0 m.howitz   (502) staff       (20)     5287 2024-04-16 06:21:42.000000 zodbpickle-3.3/patches/pickle_bytes_tests.diff
+-rw-r--r--   0 m.howitz   (502) staff       (20)      656 2024-04-16 06:21:42.430868 zodbpickle-3.3/setup.cfg
+-rw-r--r--   0 m.howitz   (502) staff       (20)     3038 2024-04-16 06:21:42.000000 zodbpickle-3.3/setup.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2024-04-16 06:21:42.423953 zodbpickle-3.3/src/
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2024-04-16 06:21:42.427872 zodbpickle-3.3/src/zodbpickle/
+-rw-r--r--   0 m.howitz   (502) staff       (20)       44 2024-04-16 06:21:42.000000 zodbpickle-3.3/src/zodbpickle/__init__.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)   205193 2024-04-16 06:21:42.000000 zodbpickle-3.3/src/zodbpickle/_pickle_33.c
+-rw-r--r--   0 m.howitz   (502) staff       (20)      891 2024-04-16 06:21:42.000000 zodbpickle-3.3/src/zodbpickle/fastpickle.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)       24 2024-04-16 06:21:42.000000 zodbpickle-3.3/src/zodbpickle/pickle.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)    52163 2024-04-16 06:21:42.000000 zodbpickle-3.3/src/zodbpickle/pickle_3.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)    87531 2024-04-16 06:21:42.000000 zodbpickle-3.3/src/zodbpickle/pickletools_3.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1061 2024-04-16 06:21:42.000000 zodbpickle-3.3/src/zodbpickle/slowpickle.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2024-04-16 06:21:42.429800 zodbpickle-3.3/src/zodbpickle/tests/
+-rw-r--r--   0 m.howitz   (502) staff       (20)      212 2024-04-16 06:21:42.000000 zodbpickle-3.3/src/zodbpickle/tests/__init__.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     5271 2024-04-16 06:21:42.000000 zodbpickle-3.3/src/zodbpickle/tests/pickle_3_tests.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)    68946 2024-04-16 06:21:42.000000 zodbpickle-3.3/src/zodbpickle/tests/pickletester_3.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1363 2024-04-16 06:21:42.000000 zodbpickle-3.3/src/zodbpickle/tests/test_compile_flags.py
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1161 2024-04-16 06:21:42.000000 zodbpickle-3.3/src/zodbpickle/tests/test_pickle.py
+drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2024-04-16 06:21:42.430005 zodbpickle-3.3/src/zodbpickle.egg-info/
+-rw-r--r--   0 m.howitz   (502) staff       (20)    13204 2024-04-16 06:21:42.000000 zodbpickle-3.3/src/zodbpickle.egg-info/PKG-INFO
+-rw-r--r--   0 m.howitz   (502) staff       (20)      826 2024-04-16 06:21:42.000000 zodbpickle-3.3/src/zodbpickle.egg-info/SOURCES.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        1 2024-04-16 06:21:42.000000 zodbpickle-3.3/src/zodbpickle.egg-info/dependency_links.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)        1 2024-04-16 06:21:42.000000 zodbpickle-3.3/src/zodbpickle.egg-info/not-zip-safe
+-rw-r--r--   0 m.howitz   (502) staff       (20)       35 2024-04-16 06:21:42.000000 zodbpickle-3.3/src/zodbpickle.egg-info/requires.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)       11 2024-04-16 06:21:42.000000 zodbpickle-3.3/src/zodbpickle.egg-info/top_level.txt
+-rw-r--r--   0 m.howitz   (502) staff       (20)     1614 2024-04-16 06:21:42.000000 zodbpickle-3.3/tox.ini
```

### Comparing `zodbpickle-3.2/.coveragerc` & `zodbpickle-3.3/.coveragerc`

 * *Files identical despite different names*

### Comparing `zodbpickle-3.2/.manylinux-install.sh` & `zodbpickle-3.3/.manylinux-install.sh`

 * *Files identical despite different names*

### Comparing `zodbpickle-3.2/CHANGES.rst` & `zodbpickle-3.3/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,19 @@
 ===========
  Changelog
 ===========
 
+3.3 (2024-04-16)
+================
+
+- Build Windows wheels on GHA.
+
+- Add preliminary support for Python 3.13 as of 3.13a5.
+
+
 3.2 (2024-02-16)
 ================
 
 - Add preliminary support for Python 3.13 as of 3.13a3.
 
 
 3.1 (2023-10-05)
```

### Comparing `zodbpickle-3.2/CONTRIBUTING.md` & `zodbpickle-3.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `zodbpickle-3.2/LICENSE.txt` & `zodbpickle-3.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `zodbpickle-3.2/PKG-INFO` & `zodbpickle-3.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zodbpickle
-Version: 3.2
+Version: 3.3
 Summary: Fork of Python 3 pickle module.
 Home-page: https://github.com/zopefoundation/zodbpickle
 Author: Python and Zope Foundation
 Author-email: zodb-dev@zope.dev
 License: PSFL 2 and ZPL 2.1
 Keywords: zodb pickle
 Platform: any
@@ -200,14 +200,22 @@
 This module provides a ``noload()`` method again.
 
 
 ===========
  Changelog
 ===========
 
+3.3 (2024-04-16)
+================
+
+- Build Windows wheels on GHA.
+
+- Add preliminary support for Python 3.13 as of 3.13a5.
+
+
 3.2 (2024-02-16)
 ================
 
 - Add preliminary support for Python 3.13 as of 3.13a3.
 
 
 3.1 (2023-10-05)
```

### Comparing `zodbpickle-3.2/README.rst` & `zodbpickle-3.3/README.rst`

 * *Files identical despite different names*

### Comparing `zodbpickle-3.2/patches/pickle_bytes_code.diff` & `zodbpickle-3.3/patches/pickle_bytes_code.diff`

 * *Files identical despite different names*

### Comparing `zodbpickle-3.2/patches/pickle_bytes_tests.diff` & `zodbpickle-3.3/patches/pickle_bytes_tests.diff`

 * *Files identical despite different names*

### Comparing `zodbpickle-3.2/setup.cfg` & `zodbpickle-3.3/setup.cfg`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-[bdist_wheel]
-universal = 0
-
 [zest.releaser]
 create-wheel = no
 
 [flake8]
 doctests = 1
 per-file-ignores = 
 	src/zodbpickle/fastpickle.py: F401 F403
```

### Comparing `zodbpickle-3.2/setup.py` & `zodbpickle-3.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 else:
     ext_modules = [Extension(name='zodbpickle._pickle',
                              sources=[EXT])]
 
 
 setup(
     name='zodbpickle',
-    version='3.2',
+    version='3.3',
     description='Fork of Python 3 pickle module.',
     author='Python and Zope Foundation',
     author_email='zodb-dev@zope.dev',
     url='https://github.com/zopefoundation/zodbpickle',
     license='PSFL 2 and ZPL 2.1',
     long_description=README,
     classifiers=[
```

### Comparing `zodbpickle-3.2/src/zodbpickle/_pickle_33.c` & `zodbpickle-3.3/src/zodbpickle/_pickle_33.c`

 * *Files 0% similar despite different names*

```diff
@@ -11,23 +11,45 @@
      && !defined(__cplusplus) && !defined(inline))
 #  define PYCAPI_COMPAT_INLINE(TYPE static __inline TYPE
 #else
 #  define PYCAPI_COMPAT_STATIC_INLINE(TYPE) static inline TYPE
 #endif
 
 #if PY_VERSION_HEX < 0x030900A4 && !defined(Py_SET_SIZE) /* 3.9.0a4 */
+
 PYCAPI_COMPAT_STATIC_INLINE(void)
 _Py_SET_SIZE(PyVarObject *ob, Py_ssize_t size)
 {
     ob->ob_size = size;
 }
+
 #define Py_SET_SIZE(ob, size) _Py_SET_SIZE((PyVarObject*)(ob), size)
+
+#endif
+
+#if (PY_VERSION_HEX >= 0x30D00A5) /* 3.13.0a5 */
+
+/**
+ * In 3.13a5 ``_PyLong_AsByteArray`` got a new ``with_exceptions`` argument.
+ * See https://github.com/python/cpython/commit/7861dfd26a41e40c2b4361eb0bb1356b9b4a064b
+ */
+static int _PyLong_AsByteArray_compat(PyLongObject* v,
+    unsigned char* bytes, size_t n,
+    int little_endian, int is_signed)
+{
+    return _PyLong_AsByteArray(
+        v, bytes, n, little_endian, is_signed, 1 /* with_exceptions */
+    );
+}
+
+#define _PyLong_AsByteArray(v, bytes, n, little_endian, is_signed) _PyLong_AsByteArray_compat(v, bytes, n, little_endian, is_signed)
 #endif
 
 #if (PY_VERSION_HEX >= 0x30D00A1) /* 3.13.0a1 */
+
 /**
  * In 3.13a1 ``_PyObject_LookupAttrId`` was removed.
  * See https://github.com/python/cpython/commit/579aa89e68a6607398317a50586af781981e89fb
  * See also the explanation for 3.10 below.
  */
 static int _PyObject_HasAttrId(PyObject* obj, void* id)
 {
@@ -37,35 +59,39 @@
         return -1;
     }
     PyObject* attr_val;
     result = PyObject_GetOptionalAttr(obj, oname, &attr_val);
     Py_XDECREF(attr_val);
     return result;
 }
+
 /*
 * This declaration was moved to the internal API only accessible for building
 * CPython itself. But the implementation is still in `Objects/longobject.c` and
 * Pythons own `Modules/_pickle.c` still uses it.
 */
 PyAPI_FUNC(size_t) _PyLong_NumBits(PyObject *v);
+
 #elif (PY_VERSION_HEX >= 0x30A00B1) /* 3.10.0b1 */
+
 /**
  * The function ``_PyObject_LookupAttrId`` function replaces the combo of
  * ``_PyObject_HasAttrId`` followed by ``_PyObject_GetAttrId``; our code isn't
  * structured to take advantage of that, so for now we throw away the
  * resulting attribute value and continue to make the extra ``Get`` call.
  */
 static int _PyObject_HasAttrId(PyObject* obj, void* id)
 {
     int result;
     PyObject* attr_val;
     result = _PyObject_LookupAttrId(obj, id, &attr_val);
     Py_XDECREF(attr_val);
     return result;
 }
+
 #endif
 
 #if (PY_VERSION_HEX < 0x30B00A7) /* 3.11.0a7 */
 #  define PyFloat_Pack8 _PyFloat_Pack8
 #  define PyFloat_Unpack8 _PyFloat_Unpack8
 #endif
```

### Comparing `zodbpickle-3.2/src/zodbpickle/fastpickle.py` & `zodbpickle-3.3/src/zodbpickle/fastpickle.py`

 * *Files identical despite different names*

### Comparing `zodbpickle-3.2/src/zodbpickle/pickle_3.py` & `zodbpickle-3.3/src/zodbpickle/pickle_3.py`

 * *Files identical despite different names*

### Comparing `zodbpickle-3.2/src/zodbpickle/pickletools_3.py` & `zodbpickle-3.3/src/zodbpickle/pickletools_3.py`

 * *Files identical despite different names*

### Comparing `zodbpickle-3.2/src/zodbpickle/slowpickle.py` & `zodbpickle-3.3/src/zodbpickle/slowpickle.py`

 * *Files identical despite different names*

### Comparing `zodbpickle-3.2/src/zodbpickle/tests/pickle_3_tests.py` & `zodbpickle-3.3/src/zodbpickle/tests/pickle_3_tests.py`

 * *Files identical despite different names*

### Comparing `zodbpickle-3.2/src/zodbpickle/tests/pickletester_3.py` & `zodbpickle-3.3/src/zodbpickle/tests/pickletester_3.py`

 * *Files identical despite different names*

### Comparing `zodbpickle-3.2/src/zodbpickle/tests/test_compile_flags.py` & `zodbpickle-3.3/src/zodbpickle/tests/test_compile_flags.py`

 * *Files identical despite different names*

### Comparing `zodbpickle-3.2/src/zodbpickle/tests/test_pickle.py` & `zodbpickle-3.3/src/zodbpickle/tests/test_pickle.py`

 * *Files identical despite different names*

### Comparing `zodbpickle-3.2/src/zodbpickle.egg-info/PKG-INFO` & `zodbpickle-3.3/src/zodbpickle.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zodbpickle
-Version: 3.2
+Version: 3.3
 Summary: Fork of Python 3 pickle module.
 Home-page: https://github.com/zopefoundation/zodbpickle
 Author: Python and Zope Foundation
 Author-email: zodb-dev@zope.dev
 License: PSFL 2 and ZPL 2.1
 Keywords: zodb pickle
 Platform: any
@@ -200,14 +200,22 @@
 This module provides a ``noload()`` method again.
 
 
 ===========
  Changelog
 ===========
 
+3.3 (2024-04-16)
+================
+
+- Build Windows wheels on GHA.
+
+- Add preliminary support for Python 3.13 as of 3.13a5.
+
+
 3.2 (2024-02-16)
 ================
 
 - Add preliminary support for Python 3.13 as of 3.13a3.
 
 
 3.1 (2023-10-05)
```

### Comparing `zodbpickle-3.2/src/zodbpickle.egg-info/SOURCES.txt` & `zodbpickle-3.3/src/zodbpickle.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 .manylinux-install.sh
 .manylinux.sh
 CHANGES.rst
 CONTRIBUTING.md
 LICENSE.txt
 MANIFEST.in
 README.rst
-appveyor.yml
 buildout.cfg
 setup.cfg
 setup.py
 tox.ini
 patches/pickle_bytes_code.diff
 patches/pickle_bytes_tests.diff
 src/zodbpickle/__init__.py
```

### Comparing `zodbpickle-3.2/tox.ini` & `zodbpickle-3.3/tox.ini`

 * *Files 2% similar despite different names*

```diff
@@ -50,15 +50,15 @@
     build
     check-manifest
     check-python-versions >= 0.20.0
     wheel
 commands_pre =
 commands =
     check-manifest
-    check-python-versions
+    check-python-versions --only setup.py,tox.ini,.github/workflows/tests.yml
     python -m build --sdist --no-isolation
     twine check dist/*
 
 [testenv:lint]
 basepython = python3
 skip_install = true
 deps =
```

