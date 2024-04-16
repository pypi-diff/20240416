# Comparing `tmp/serializor-1.0.0.tar.gz` & `tmp/serializor-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "serializor-1.0.0.tar", last modified: Tue Apr 16 07:38:01 2024, max compression
+gzip compressed data, was "serializor-1.0.1.tar", last modified: Tue Apr 16 08:21:18 2024, max compression
```

## Comparing `serializor-1.0.0.tar` & `serializor-1.0.1.tar`

### file list

```diff
@@ -1,35 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:38:01.108797 serializor-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (127)    11981 2024-04-16 07:37:49.000000 serializor-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-16 07:37:49.000000 serializor-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     3025 2024-04-16 07:38:01.108797 serializor-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-04-16 07:37:49.000000 serializor-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-16 07:37:49.000000 serializor-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)      845 2024-04-16 07:38:01.108797 serializor-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-04-16 07:37:49.000000 serializor-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:38:01.100797 serializor-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:38:01.108797 serializor-1.0.0/src/serializor/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 07:37:49.000000 serializor-1.0.0/src/serializor/__init__.pxd
--rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-16 07:37:49.000000 serializor-1.0.0/src/serializor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   558221 2024-04-16 07:37:58.000000 serializor-1.0.0/src/serializor/crypto.c
--rw-r--r--   0 runner    (1001) docker     (127)      144 2024-04-16 07:37:49.000000 serializor-1.0.0/src/serializor/crypto.pxd
--rw-r--r--   0 runner    (1001) docker     (127)     3547 2024-04-16 07:37:49.000000 serializor-1.0.0/src/serializor/crypto.py
--rw-r--r--   0 runner    (1001) docker     (127)  1204573 2024-04-16 07:37:59.000000 serializor-1.0.0/src/serializor/deserialize.c
--rw-r--r--   0 runner    (1001) docker     (127)     5415 2024-04-16 07:37:49.000000 serializor-1.0.0/src/serializor/deserialize.pxd
--rw-r--r--   0 runner    (1001) docker     (127)    77945 2024-04-16 07:37:49.000000 serializor-1.0.0/src/serializor/deserialize.py
--rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-16 07:37:49.000000 serializor-1.0.0/src/serializor/errors.py
--rw-r--r--   0 runner    (1001) docker     (127)   413334 2024-04-16 07:37:59.000000 serializor-1.0.0/src/serializor/prefix.c
--rw-r--r--   0 runner    (1001) docker     (127)     3422 2024-04-16 07:37:49.000000 serializor-1.0.0/src/serializor/prefix.pxd
--rw-r--r--   0 runner    (1001) docker     (127)     8970 2024-04-16 07:37:49.000000 serializor-1.0.0/src/serializor/prefix.py
--rw-r--r--   0 runner    (1001) docker     (127)  1284364 2024-04-16 07:38:00.000000 serializor-1.0.0/src/serializor/serialize.c
--rw-r--r--   0 runner    (1001) docker     (127)     2921 2024-04-16 07:37:49.000000 serializor-1.0.0/src/serializor/serialize.pxd
--rw-r--r--   0 runner    (1001) docker     (127)    72165 2024-04-16 07:37:49.000000 serializor-1.0.0/src/serializor/serialize.py
--rw-r--r--   0 runner    (1001) docker     (127)   238142 2024-04-16 07:38:00.000000 serializor-1.0.0/src/serializor/typeref.c
--rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-16 07:37:49.000000 serializor-1.0.0/src/serializor/typeref.pxd
--rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-04-16 07:37:49.000000 serializor-1.0.0/src/serializor/typeref.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 07:38:01.108797 serializor-1.0.0/src/serializor.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     3025 2024-04-16 07:38:01.000000 serializor-1.0.0/src/serializor.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-16 07:38:01.000000 serializor-1.0.0/src/serializor.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 07:38:01.000000 serializor-1.0.0/src/serializor.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 07:38:00.000000 serializor-1.0.0/src/serializor.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-16 07:38:01.000000 serializor-1.0.0/src/serializor.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-16 07:38:01.000000 serializor-1.0.0/src/serializor.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:21:18.086000 serializor-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (127)    11981 2024-04-16 08:21:06.000000 serializor-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)      120 2024-04-16 08:21:06.000000 serializor-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     3025 2024-04-16 08:21:18.086000 serializor-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2329 2024-04-16 08:21:06.000000 serializor-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      160 2024-04-16 08:21:06.000000 serializor-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)      845 2024-04-16 08:21:18.086000 serializor-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1646 2024-04-16 08:21:06.000000 serializor-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:21:18.074000 serializor-1.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:21:18.082000 serializor-1.0.1/src/serializor/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 08:21:06.000000 serializor-1.0.1/src/serializor/__init__.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-16 08:21:06.000000 serializor-1.0.1/src/serializor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   558221 2024-04-16 08:21:15.000000 serializor-1.0.1/src/serializor/crypto.c
+-rw-r--r--   0 runner    (1001) docker     (127)      145 2024-04-16 08:21:06.000000 serializor-1.0.1/src/serializor/crypto.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     3547 2024-04-16 08:21:06.000000 serializor-1.0.1/src/serializor/crypto.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1204573 2024-04-16 08:21:16.000000 serializor-1.0.1/src/serializor/deserialize.c
+-rw-r--r--   0 runner    (1001) docker     (127)     5416 2024-04-16 08:21:06.000000 serializor-1.0.1/src/serializor/deserialize.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)    77945 2024-04-16 08:21:06.000000 serializor-1.0.1/src/serializor/deserialize.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1286 2024-04-16 08:21:06.000000 serializor-1.0.1/src/serializor/errors.py
+-rw-r--r--   0 runner    (1001) docker     (127)   413582 2024-04-16 08:21:16.000000 serializor-1.0.1/src/serializor/prefix.c
+-rw-r--r--   0 runner    (1001) docker     (127)     3422 2024-04-16 08:21:06.000000 serializor-1.0.1/src/serializor/prefix.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     9038 2024-04-16 08:21:06.000000 serializor-1.0.1/src/serializor/prefix.py
+-rw-r--r--   0 runner    (1001) docker     (127)  1284376 2024-04-16 08:21:17.000000 serializor-1.0.1/src/serializor/serialize.c
+-rw-r--r--   0 runner    (1001) docker     (127)     2922 2024-04-16 08:21:06.000000 serializor-1.0.1/src/serializor/serialize.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)    72173 2024-04-16 08:21:06.000000 serializor-1.0.1/src/serializor/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (127)   238142 2024-04-16 08:21:17.000000 serializor-1.0.1/src/serializor/typeref.c
+-rw-r--r--   0 runner    (1001) docker     (127)      602 2024-04-16 08:21:06.000000 serializor-1.0.1/src/serializor/typeref.pxd
+-rw-r--r--   0 runner    (1001) docker     (127)     1320 2024-04-16 08:21:06.000000 serializor-1.0.1/src/serializor/typeref.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 08:21:18.086000 serializor-1.0.1/src/serializor.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     3025 2024-04-16 08:21:18.000000 serializor-1.0.1/src/serializor.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      771 2024-04-16 08:21:18.000000 serializor-1.0.1/src/serializor.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 08:21:18.000000 serializor-1.0.1/src/serializor.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 08:21:17.000000 serializor-1.0.1/src/serializor.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-16 08:21:18.000000 serializor-1.0.1/src/serializor.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       11 2024-04-16 08:21:18.000000 serializor-1.0.1/src/serializor.egg-info/top_level.txt
```

### Comparing `serializor-1.0.0/LICENSE` & `serializor-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `serializor-1.0.0/PKG-INFO` & `serializor-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: serializor
-Version: 1.0.0
+Version: 1.0.1
 Summary: Serialization for common Python objects.
 Home-page: https://github.com/AresJef/Serializor
 Author: Jiefu Chen
 Author-email: keppa1991@163.com
 License: MIT license, Apache License 2.0
 Keywords: serialize,serialization,numpy,pandas,python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `serializor-1.0.0/README.md` & `serializor-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `serializor-1.0.0/setup.cfg` & `serializor-1.0.1/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = serializor
-version = 1.0.0
+version = 1.0.1
 author = Jiefu Chen
 author_email = keppa1991@163.com
 description = Serialization for common Python objects.
 url = https://github.com/AresJef/Serializor
 long_description = file: README.md
 long_description_content_type = text/markdown
 keywords = serialize, serialization, numpy, pandas, python
```

### Comparing `serializor-1.0.0/setup.py` & `serializor-1.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `serializor-1.0.0/src/serializor/__init__.py` & `serializor-1.0.1/src/serializor/__init__.py`

 * *Files identical despite different names*

### Comparing `serializor-1.0.0/src/serializor/crypto.c` & `serializor-1.0.1/src/serializor/crypto.c`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
                 "NPY_1_7_API_VERSION"
             ]
         ],
         "extra_compile_args": [
             "-Wno-unreachable-code"
         ],
         "include_dirs": [
-            "/tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/core/include"
+            "/tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/core/include"
         ],
         "name": "serializor.crypto",
         "sources": [
             "src/serializor/crypto.py"
         ]
     },
     "module_name": "serializor.crypto"
@@ -1535,177 +1535,177 @@
 /* ForceInitThreads.proto */
 #ifndef __PYX_FORCE_INIT_THREADS
   #define __PYX_FORCE_INIT_THREADS 0
 #endif
 
 /* #### Code section: numeric_typedefs ### */
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":730
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":730
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":731
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":731
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":732
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":732
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":733
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":733
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":737
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":737
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":738
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":738
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":739
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":739
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":740
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":740
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":744
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":744
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":745
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":745
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":754
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":754
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":755
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":755
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":757
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":757
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":758
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":758
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":760
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":760
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":761
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":761
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":763
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":763
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":764
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":764
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":765
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":765
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1734,42 +1734,42 @@
 #endif
 static CYTHON_INLINE __pyx_t_double_complex __pyx_t_double_complex_from_parts(double, double);
 
 /* #### Code section: type_declarations ### */
 
 /*--- Type declarations ---*/
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":767
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":767
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":768
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":768
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":769
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":769
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":771
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":771
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -3287,261 +3287,261 @@
 #define __pyx_tuple__3 __pyx_mstate_global->__pyx_tuple__3
 #define __pyx_tuple__7 __pyx_mstate_global->__pyx_tuple__7
 #define __pyx_tuple__9 __pyx_mstate_global->__pyx_tuple__9
 #define __pyx_codeobj__8 __pyx_mstate_global->__pyx_codeobj__8
 #define __pyx_codeobj__10 __pyx_mstate_global->__pyx_codeobj__10
 /* #### Code section: module_code ### */
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":245
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_7ndarray_4base_base(PyArrayObject *__pyx_v_self) {
   PyObject *__pyx_r;
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":248
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":248
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  *             return PyArray_BASE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_BASE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":245
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":251
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
 static CYTHON_INLINE PyArray_Descr *__pyx_f_5numpy_7ndarray_5descr_descr(PyArrayObject *__pyx_v_self) {
   PyArray_Descr *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyArray_Descr *__pyx_t_1;
   __Pyx_RefNannySetupContext("descr", 1);
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":254
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":254
  *             """Returns an owned reference to the dtype of the array.
  *             """
  *             return <dtype>PyArray_DESCR(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __Pyx_XDECREF((PyObject *)__pyx_r);
   __pyx_t_1 = PyArray_DESCR(__pyx_v_self);
   __Pyx_INCREF((PyObject *)((PyArray_Descr *)__pyx_t_1));
   __pyx_r = ((PyArray_Descr *)__pyx_t_1);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":251
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":257
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_7ndarray_4ndim_ndim(PyArrayObject *__pyx_v_self) {
   int __pyx_r;
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":260
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":260
  *             """Returns the number of dimensions in the array.
  *             """
  *             return PyArray_NDIM(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_NDIM(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":257
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":263
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_5shape_shape(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":268
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":268
  *             Can return NULL for 0-dimensional arrays.
  *             """
  *             return PyArray_DIMS(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_DIMS(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":263
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":271
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_7strides_strides(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":275
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":275
  *             The number of elements matches the number of dimensions of the array (ndim).
  *             """
  *             return PyArray_STRIDES(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_STRIDES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":271
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":278
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
 static CYTHON_INLINE npy_intp __pyx_f_5numpy_7ndarray_4size_size(PyArrayObject *__pyx_v_self) {
   npy_intp __pyx_r;
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":281
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":281
  *             """Returns the total size (in number of elements) of the array.
  *             """
  *             return PyArray_SIZE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_SIZE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":278
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":284
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
 static CYTHON_INLINE char *__pyx_f_5numpy_7ndarray_4data_data(PyArrayObject *__pyx_v_self) {
   char *__pyx_r;
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":290
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":290
  *             of `PyArray_DATA()` instead, which returns a 'void*'.
  *             """
  *             return PyArray_BYTES(self)             # <<<<<<<<<<<<<<
  * 
  *     ctypedef unsigned char      npy_bool
  */
   __pyx_r = PyArray_BYTES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":284
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":773
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -3550,29 +3550,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 1);
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":774
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":774
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 774, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":773
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -3583,15 +3583,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":776
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":776
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -3600,29 +3600,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 1);
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":777
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":777
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 777, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":776
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":776
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -3633,15 +3633,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":779
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -3650,29 +3650,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 1);
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":780
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":780
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 780, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":779
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -3683,15 +3683,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":782
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -3700,29 +3700,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 1);
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":783
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":783
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 783, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":782
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -3733,15 +3733,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":785
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -3750,29 +3750,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 1);
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":786
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":786
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 786, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":785
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -3783,217 +3783,217 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":788
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 1);
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":789
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = PyDataType_HASSUBARRAY(__pyx_v_d);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":790
+    /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":790
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":789
+    /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":792
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":792
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":788
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":968
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":968
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":969
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":969
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":970
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":970
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   __pyx_t_1 = PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(0, 970, __pyx_L1_error)
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":968
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":968
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_AddTraceback("numpy.set_array_base", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_L0:;
 }
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":972
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":972
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 1);
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":973
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":973
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":974
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":974
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = (__pyx_v_base == NULL);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":975
+    /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":975
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":974
+    /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":974
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":976
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":976
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":972
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":972
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":980
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":980
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -4009,15 +4009,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 1);
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":981
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -4025,68 +4025,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":982
+      /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":982
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(0, 982, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":981
+      /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":983
+    /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":983
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(0, 983, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":984
+      /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":984
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 984, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(0, 984, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":981
+    /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -4094,15 +4094,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":980
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":980
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -4117,15 +4117,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":986
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":986
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4141,15 +4141,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 1);
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":987
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -4157,68 +4157,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":988
+      /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":988
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(0, 988, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":987
+      /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":989
+    /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":989
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(0, 989, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":990
+      /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":990
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 990, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(0, 990, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":987
+    /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -4226,15 +4226,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":986
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":986
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4249,15 +4249,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":992
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":992
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4273,15 +4273,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 1);
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":993
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -4289,68 +4289,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":994
+      /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":994
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(0, 994, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":993
+      /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":995
+    /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":995
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(0, 995, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":996
+      /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":996
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * 
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(0, 996, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(0, 996, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":993
+    /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -4358,15 +4358,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":992
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":992
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4381,170 +4381,170 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":999
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":999
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1011
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1011
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":999
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":999
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1014
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1014
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1026
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1026
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1014
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1014
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1029
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1029
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1036
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1036
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1029
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1029
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1039
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1039
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1043
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1043
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1039
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1039
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1046
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1046
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1050
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1050
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1046
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1046
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -8144,26 +8144,26 @@
 }
 /* #### Code section: cached_constants ### */
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":984
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":984
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple_)) __PYX_ERR(0, 984, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple_);
   __Pyx_GIVEREF(__pyx_tuple_);
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":990
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":990
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(0, 990, __pyx_L1_error)
```

### Comparing `serializor-1.0.0/src/serializor/crypto.py` & `serializor-1.0.1/src/serializor/crypto.py`

 * *Files identical despite different names*

### Comparing `serializor-1.0.0/src/serializor/deserialize.c` & `serializor-1.0.1/src/serializor/deserialize.c`

 * *Files 0% similar despite different names*

```diff
@@ -10,15 +10,15 @@
             ]
         ],
         "depends": [],
         "extra_compile_args": [
             "-Wno-unreachable-code"
         ],
         "include_dirs": [
-            "/tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/core/include"
+            "/tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/core/include"
         ],
         "name": "serializor.deserialize",
         "sources": [
             "src/serializor/deserialize.py"
         ]
     },
     "module_name": "serializor.deserialize"
@@ -1611,177 +1611,177 @@
 /* ForceInitThreads.proto */
 #ifndef __PYX_FORCE_INIT_THREADS
   #define __PYX_FORCE_INIT_THREADS 0
 #endif
 
 /* #### Code section: numeric_typedefs ### */
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":730
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":730
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":731
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":731
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":732
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":732
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":733
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":733
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":737
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":737
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":738
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":738
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":739
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":739
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":740
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":740
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":744
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":744
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":745
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":745
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":754
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":754
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":755
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":755
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":757
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":757
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":758
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":758
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":760
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":760
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":761
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":761
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":763
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":763
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":764
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":764
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":765
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":765
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1836,42 +1836,42 @@
  *     or the provided default value if no such value was found.
  */
 struct __pyx_opt_args_7cpython_11contextvars_get_value_no_default {
   int __pyx_n;
   PyObject *default_value;
 };
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":767
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":767
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":768
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":768
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":769
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":769
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":771
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":771
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -4176,261 +4176,261 @@
 #define __pyx_tuple__2 __pyx_mstate_global->__pyx_tuple__2
 #define __pyx_tuple__3 __pyx_mstate_global->__pyx_tuple__3
 #define __pyx_tuple__4 __pyx_mstate_global->__pyx_tuple__4
 #define __pyx_tuple__7 __pyx_mstate_global->__pyx_tuple__7
 #define __pyx_codeobj__8 __pyx_mstate_global->__pyx_codeobj__8
 /* #### Code section: module_code ### */
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":245
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_7ndarray_4base_base(PyArrayObject *__pyx_v_self) {
   PyObject *__pyx_r;
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":248
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":248
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  *             return PyArray_BASE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_BASE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":245
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":251
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
 static CYTHON_INLINE PyArray_Descr *__pyx_f_5numpy_7ndarray_5descr_descr(PyArrayObject *__pyx_v_self) {
   PyArray_Descr *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyArray_Descr *__pyx_t_1;
   __Pyx_RefNannySetupContext("descr", 1);
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":254
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":254
  *             """Returns an owned reference to the dtype of the array.
  *             """
  *             return <dtype>PyArray_DESCR(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __Pyx_XDECREF((PyObject *)__pyx_r);
   __pyx_t_1 = PyArray_DESCR(__pyx_v_self);
   __Pyx_INCREF((PyObject *)((PyArray_Descr *)__pyx_t_1));
   __pyx_r = ((PyArray_Descr *)__pyx_t_1);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":251
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":257
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_7ndarray_4ndim_ndim(PyArrayObject *__pyx_v_self) {
   int __pyx_r;
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":260
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":260
  *             """Returns the number of dimensions in the array.
  *             """
  *             return PyArray_NDIM(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_NDIM(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":257
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":263
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_5shape_shape(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":268
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":268
  *             Can return NULL for 0-dimensional arrays.
  *             """
  *             return PyArray_DIMS(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_DIMS(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":263
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":271
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_7strides_strides(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":275
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":275
  *             The number of elements matches the number of dimensions of the array (ndim).
  *             """
  *             return PyArray_STRIDES(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_STRIDES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":271
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":278
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
 static CYTHON_INLINE npy_intp __pyx_f_5numpy_7ndarray_4size_size(PyArrayObject *__pyx_v_self) {
   npy_intp __pyx_r;
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":281
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":281
  *             """Returns the total size (in number of elements) of the array.
  *             """
  *             return PyArray_SIZE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_SIZE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":278
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":284
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
 static CYTHON_INLINE char *__pyx_f_5numpy_7ndarray_4data_data(PyArrayObject *__pyx_v_self) {
   char *__pyx_r;
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":290
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":290
  *             of `PyArray_DATA()` instead, which returns a 'void*'.
  *             """
  *             return PyArray_BYTES(self)             # <<<<<<<<<<<<<<
  * 
  *     ctypedef unsigned char      npy_bool
  */
   __pyx_r = PyArray_BYTES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":284
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":773
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -4439,29 +4439,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 1);
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":774
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":774
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 774, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":773
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -4472,15 +4472,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":776
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":776
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -4489,29 +4489,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 1);
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":777
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":777
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 777, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":776
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":776
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -4522,15 +4522,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":779
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -4539,29 +4539,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 1);
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":780
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":780
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 780, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":779
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -4572,15 +4572,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":782
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -4589,29 +4589,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 1);
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":783
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":783
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 783, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":782
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -4622,15 +4622,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":785
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -4639,29 +4639,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 1);
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":786
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":786
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 786, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":785
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -4672,217 +4672,217 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":788
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 1);
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":789
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = PyDataType_HASSUBARRAY(__pyx_v_d);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":790
+    /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":790
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":789
+    /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":792
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":792
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":788
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":968
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":968
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":969
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":969
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":970
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":970
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   __pyx_t_1 = PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(1, 970, __pyx_L1_error)
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":968
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":968
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_AddTraceback("numpy.set_array_base", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_L0:;
 }
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":972
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":972
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 1);
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":973
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":973
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":974
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":974
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = (__pyx_v_base == NULL);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":975
+    /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":975
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":974
+    /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":974
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":976
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":976
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":972
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":972
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":980
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":980
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -4898,15 +4898,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 1);
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":981
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -4914,68 +4914,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":982
+      /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":982
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 982, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":981
+      /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":983
+    /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":983
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 983, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":984
+      /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":984
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 984, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 984, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":981
+    /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -4983,15 +4983,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":980
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":980
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -5006,15 +5006,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":986
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":986
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -5030,15 +5030,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 1);
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":987
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -5046,68 +5046,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":988
+      /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":988
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 988, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":987
+      /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":989
+    /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":989
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 989, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":990
+      /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":990
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 990, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 990, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":987
+    /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -5115,15 +5115,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":986
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":986
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -5138,15 +5138,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":992
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":992
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -5162,15 +5162,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 1);
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":993
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -5178,68 +5178,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":994
+      /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":994
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 994, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":993
+      /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":995
+    /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":995
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 995, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":996
+      /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":996
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * 
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 996, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 996, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":993
+    /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -5247,15 +5247,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":992
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":992
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -5270,170 +5270,170 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":999
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":999
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1011
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1011
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":999
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":999
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1014
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1014
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1026
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1026
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1014
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1014
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1029
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1029
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1036
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1036
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1029
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1029
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1039
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1039
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1043
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1043
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1039
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1039
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1046
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1046
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1050
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1050
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1046
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1046
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -24261,26 +24261,26 @@
 }
 /* #### Code section: cached_constants ### */
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":984
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":984
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple_)) __PYX_ERR(1, 984, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple_);
   __Pyx_GIVEREF(__pyx_tuple_);
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":990
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":990
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 990, __pyx_L1_error)
```

### Comparing `serializor-1.0.0/src/serializor/deserialize.pxd` & `serializor-1.0.1/src/serializor/deserialize.pxd`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -135,8 +135,8 @@
     # Not found.
     raise ValueError(
         "Failed to locate the next close bracket ']' "
         "that is preceded by a non-escaped '\"' "
         "from:\n%s" % slice_to_unicode(data, start, end) )
 
 # Deserialize
-cdef object capi_deserialize(str obj)
+cdef object capi_deserialize(str obj)
```

### Comparing `serializor-1.0.0/src/serializor/deserialize.py` & `serializor-1.0.1/src/serializor/deserialize.py`

 * *Files identical despite different names*

### Comparing `serializor-1.0.0/src/serializor/errors.py` & `serializor-1.0.1/src/serializor/errors.py`

 * *Files identical despite different names*

### Comparing `serializor-1.0.0/src/serializor/prefix.c` & `serializor-1.0.1/src/serializor/prefix.c`

 * *Files 2% similar despite different names*

```diff
@@ -3564,15 +3564,15 @@
   __Pyx_GIVEREF(__pyx_tuple__6);
 
   /* "serializor/prefix.py":112
  * NDARRAY_DTYPE_COMPLEX: str = np.array(1 + 1j, dtype=np.complex128).dtype.kind  # 'c'
  * NDARRAY_DTYPE_BYTES: str = np.array(b"", dtype="S").dtype.kind  # 'S'
  * NDARRAY_DTYPE_UNICODE: str = np.array("", dtype="U").dtype.kind  # 'U'             # <<<<<<<<<<<<<<
  * # . identifier
- * NDARRAY_ID: cython.Py_UCS4 = str_loc(NDARRAY, 0)
+ * NDARRAY_ID: cython.Py_UCS4 = read_char(NDARRAY, 0)
  */
   __pyx_tuple__7 = PyTuple_Pack(1, __pyx_kp_u__5); if (unlikely(!__pyx_tuple__7)) __PYX_ERR(0, 112, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__7);
   __Pyx_GIVEREF(__pyx_tuple__7);
   __Pyx_RefNannyFinishContext();
   return 0;
   __pyx_L1_error:;
@@ -4273,83 +4273,83 @@
   __Pyx_GIVEREF(__pyx_n_u_i);
 
   /* "serializor/prefix.py":17
  * FLOAT: str = "f"
  * INT: str = "i"
  * NONE: str = "n"             # <<<<<<<<<<<<<<
  * # . identifier
- * STR_ID: cython.Py_UCS4 = str_loc(STR, 0)
+ * STR_ID: cython.Py_UCS4 = read_char(STR, 0)
  */
   __Pyx_INCREF(__pyx_n_u_n);
   __Pyx_XGOTREF(__pyx_v_10serializor_6prefix_NONE);
   __Pyx_DECREF_SET(__pyx_v_10serializor_6prefix_NONE, __pyx_n_u_n);
   __Pyx_GIVEREF(__pyx_n_u_n);
 
   /* "serializor/prefix.py":19
  * NONE: str = "n"
  * # . identifier
- * STR_ID: cython.Py_UCS4 = str_loc(STR, 0)             # <<<<<<<<<<<<<<
- * BOOL_ID: cython.Py_UCS4 = str_loc(BOOL, 0)
- * FLOAT_ID: cython.Py_UCS4 = str_loc(FLOAT, 0)
+ * STR_ID: cython.Py_UCS4 = read_char(STR, 0)             # <<<<<<<<<<<<<<
+ * BOOL_ID: cython.Py_UCS4 = read_char(BOOL, 0)
+ * FLOAT_ID: cython.Py_UCS4 = read_char(FLOAT, 0)
  */
   __pyx_t_2 = __pyx_v_10serializor_6prefix_STR;
   __Pyx_INCREF(__pyx_t_2);
   __pyx_v_10serializor_6prefix_STR_ID = PyUnicode_READ_CHAR(__pyx_t_2, 0);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "serializor/prefix.py":20
  * # . identifier
- * STR_ID: cython.Py_UCS4 = str_loc(STR, 0)
- * BOOL_ID: cython.Py_UCS4 = str_loc(BOOL, 0)             # <<<<<<<<<<<<<<
- * FLOAT_ID: cython.Py_UCS4 = str_loc(FLOAT, 0)
- * INT_ID: cython.Py_UCS4 = str_loc(INT, 0)
+ * STR_ID: cython.Py_UCS4 = read_char(STR, 0)
+ * BOOL_ID: cython.Py_UCS4 = read_char(BOOL, 0)             # <<<<<<<<<<<<<<
+ * FLOAT_ID: cython.Py_UCS4 = read_char(FLOAT, 0)
+ * INT_ID: cython.Py_UCS4 = read_char(INT, 0)
  */
   __pyx_t_2 = __pyx_v_10serializor_6prefix_BOOL;
   __Pyx_INCREF(__pyx_t_2);
   __pyx_v_10serializor_6prefix_BOOL_ID = PyUnicode_READ_CHAR(__pyx_t_2, 0);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "serializor/prefix.py":21
- * STR_ID: cython.Py_UCS4 = str_loc(STR, 0)
- * BOOL_ID: cython.Py_UCS4 = str_loc(BOOL, 0)
- * FLOAT_ID: cython.Py_UCS4 = str_loc(FLOAT, 0)             # <<<<<<<<<<<<<<
- * INT_ID: cython.Py_UCS4 = str_loc(INT, 0)
- * NONE_ID: cython.Py_UCS4 = str_loc(NONE, 0)
+ * STR_ID: cython.Py_UCS4 = read_char(STR, 0)
+ * BOOL_ID: cython.Py_UCS4 = read_char(BOOL, 0)
+ * FLOAT_ID: cython.Py_UCS4 = read_char(FLOAT, 0)             # <<<<<<<<<<<<<<
+ * INT_ID: cython.Py_UCS4 = read_char(INT, 0)
+ * NONE_ID: cython.Py_UCS4 = read_char(NONE, 0)
  */
   __pyx_t_2 = __pyx_v_10serializor_6prefix_FLOAT;
   __Pyx_INCREF(__pyx_t_2);
   __pyx_v_10serializor_6prefix_FLOAT_ID = PyUnicode_READ_CHAR(__pyx_t_2, 0);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "serializor/prefix.py":22
- * BOOL_ID: cython.Py_UCS4 = str_loc(BOOL, 0)
- * FLOAT_ID: cython.Py_UCS4 = str_loc(FLOAT, 0)
- * INT_ID: cython.Py_UCS4 = str_loc(INT, 0)             # <<<<<<<<<<<<<<
- * NONE_ID: cython.Py_UCS4 = str_loc(NONE, 0)
+ * BOOL_ID: cython.Py_UCS4 = read_char(BOOL, 0)
+ * FLOAT_ID: cython.Py_UCS4 = read_char(FLOAT, 0)
+ * INT_ID: cython.Py_UCS4 = read_char(INT, 0)             # <<<<<<<<<<<<<<
+ * NONE_ID: cython.Py_UCS4 = read_char(NONE, 0)
  * # . variant
  */
   __pyx_t_2 = __pyx_v_10serializor_6prefix_INT;
   __Pyx_INCREF(__pyx_t_2);
   __pyx_v_10serializor_6prefix_INT_ID = PyUnicode_READ_CHAR(__pyx_t_2, 0);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "serializor/prefix.py":23
- * FLOAT_ID: cython.Py_UCS4 = str_loc(FLOAT, 0)
- * INT_ID: cython.Py_UCS4 = str_loc(INT, 0)
- * NONE_ID: cython.Py_UCS4 = str_loc(NONE, 0)             # <<<<<<<<<<<<<<
+ * FLOAT_ID: cython.Py_UCS4 = read_char(FLOAT, 0)
+ * INT_ID: cython.Py_UCS4 = read_char(INT, 0)
+ * NONE_ID: cython.Py_UCS4 = read_char(NONE, 0)             # <<<<<<<<<<<<<<
  * # . variant
  * BOOL_TRUE: str = BOOL + "1"  # 'o1'
  */
   __pyx_t_2 = __pyx_v_10serializor_6prefix_NONE;
   __Pyx_INCREF(__pyx_t_2);
   __pyx_v_10serializor_6prefix_NONE_ID = PyUnicode_READ_CHAR(__pyx_t_2, 0);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "serializor/prefix.py":25
- * NONE_ID: cython.Py_UCS4 = str_loc(NONE, 0)
+ * NONE_ID: cython.Py_UCS4 = read_char(NONE, 0)
  * # . variant
  * BOOL_TRUE: str = BOOL + "1"  # 'o1'             # <<<<<<<<<<<<<<
  * BOOL_FALSE: str = BOOL + "0"  # 'o0'
  * 
  */
   __pyx_t_2 = __Pyx_PyUnicode_ConcatSafe(__pyx_v_10serializor_6prefix_BOOL, __pyx_kp_u_1); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 25, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
@@ -4409,61 +4409,61 @@
   __Pyx_GIVEREF(__pyx_n_u_z);
 
   /* "serializor/prefix.py":32
  * TIME: str = "t"
  * DATETIME: str = "z"
  * TIMEDELTA: str = "l"             # <<<<<<<<<<<<<<
  * # . identifier
- * DATE_ID: cython.Py_UCS4 = str_loc(DATE, 0)
+ * DATE_ID: cython.Py_UCS4 = read_char(DATE, 0)
  */
   __Pyx_INCREF(__pyx_n_u_l);
   __Pyx_XGOTREF(__pyx_v_10serializor_6prefix_TIMEDELTA);
   __Pyx_DECREF_SET(__pyx_v_10serializor_6prefix_TIMEDELTA, __pyx_n_u_l);
   __Pyx_GIVEREF(__pyx_n_u_l);
 
   /* "serializor/prefix.py":34
  * TIMEDELTA: str = "l"
  * # . identifier
- * DATE_ID: cython.Py_UCS4 = str_loc(DATE, 0)             # <<<<<<<<<<<<<<
- * TIME_ID: cython.Py_UCS4 = str_loc(TIME, 0)
- * DATETIME_ID: cython.Py_UCS4 = str_loc(DATETIME, 0)
+ * DATE_ID: cython.Py_UCS4 = read_char(DATE, 0)             # <<<<<<<<<<<<<<
+ * TIME_ID: cython.Py_UCS4 = read_char(TIME, 0)
+ * DATETIME_ID: cython.Py_UCS4 = read_char(DATETIME, 0)
  */
   __pyx_t_2 = __pyx_v_10serializor_6prefix_DATE;
   __Pyx_INCREF(__pyx_t_2);
   __pyx_v_10serializor_6prefix_DATE_ID = PyUnicode_READ_CHAR(__pyx_t_2, 0);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "serializor/prefix.py":35
  * # . identifier
- * DATE_ID: cython.Py_UCS4 = str_loc(DATE, 0)
- * TIME_ID: cython.Py_UCS4 = str_loc(TIME, 0)             # <<<<<<<<<<<<<<
- * DATETIME_ID: cython.Py_UCS4 = str_loc(DATETIME, 0)
- * TIMEDELTA_ID: cython.Py_UCS4 = str_loc(TIMEDELTA, 0)
+ * DATE_ID: cython.Py_UCS4 = read_char(DATE, 0)
+ * TIME_ID: cython.Py_UCS4 = read_char(TIME, 0)             # <<<<<<<<<<<<<<
+ * DATETIME_ID: cython.Py_UCS4 = read_char(DATETIME, 0)
+ * TIMEDELTA_ID: cython.Py_UCS4 = read_char(TIMEDELTA, 0)
  */
   __pyx_t_2 = __pyx_v_10serializor_6prefix_TIME;
   __Pyx_INCREF(__pyx_t_2);
   __pyx_v_10serializor_6prefix_TIME_ID = PyUnicode_READ_CHAR(__pyx_t_2, 0);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "serializor/prefix.py":36
- * DATE_ID: cython.Py_UCS4 = str_loc(DATE, 0)
- * TIME_ID: cython.Py_UCS4 = str_loc(TIME, 0)
- * DATETIME_ID: cython.Py_UCS4 = str_loc(DATETIME, 0)             # <<<<<<<<<<<<<<
- * TIMEDELTA_ID: cython.Py_UCS4 = str_loc(TIMEDELTA, 0)
+ * DATE_ID: cython.Py_UCS4 = read_char(DATE, 0)
+ * TIME_ID: cython.Py_UCS4 = read_char(TIME, 0)
+ * DATETIME_ID: cython.Py_UCS4 = read_char(DATETIME, 0)             # <<<<<<<<<<<<<<
+ * TIMEDELTA_ID: cython.Py_UCS4 = read_char(TIMEDELTA, 0)
  * 
  */
   __pyx_t_2 = __pyx_v_10serializor_6prefix_DATETIME;
   __Pyx_INCREF(__pyx_t_2);
   __pyx_v_10serializor_6prefix_DATETIME_ID = PyUnicode_READ_CHAR(__pyx_t_2, 0);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "serializor/prefix.py":37
- * TIME_ID: cython.Py_UCS4 = str_loc(TIME, 0)
- * DATETIME_ID: cython.Py_UCS4 = str_loc(DATETIME, 0)
- * TIMEDELTA_ID: cython.Py_UCS4 = str_loc(TIMEDELTA, 0)             # <<<<<<<<<<<<<<
+ * TIME_ID: cython.Py_UCS4 = read_char(TIME, 0)
+ * DATETIME_ID: cython.Py_UCS4 = read_char(DATETIME, 0)
+ * TIMEDELTA_ID: cython.Py_UCS4 = read_char(TIMEDELTA, 0)             # <<<<<<<<<<<<<<
  * 
  * # Numeric Types ---------------------------------------------------------------------
  */
   __pyx_t_2 = __pyx_v_10serializor_6prefix_TIMEDELTA;
   __Pyx_INCREF(__pyx_t_2);
   __pyx_v_10serializor_6prefix_TIMEDELTA_ID = PyUnicode_READ_CHAR(__pyx_t_2, 0);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
@@ -4481,85 +4481,85 @@
   __Pyx_GIVEREF(__pyx_n_u_e);
 
   /* "serializor/prefix.py":41
  * # Numeric Types ---------------------------------------------------------------------
  * DECIMAL: str = "e"
  * COMPLEX: str = "c"             # <<<<<<<<<<<<<<
  * # . identifier
- * DECIMAL_ID: cython.Py_UCS4 = str_loc(DECIMAL, 0)
+ * DECIMAL_ID: cython.Py_UCS4 = read_char(DECIMAL, 0)
  */
   __Pyx_INCREF(__pyx_n_u_c);
   __Pyx_XGOTREF(__pyx_v_10serializor_6prefix_COMPLEX);
   __Pyx_DECREF_SET(__pyx_v_10serializor_6prefix_COMPLEX, __pyx_n_u_c);
   __Pyx_GIVEREF(__pyx_n_u_c);
 
   /* "serializor/prefix.py":43
  * COMPLEX: str = "c"
  * # . identifier
- * DECIMAL_ID: cython.Py_UCS4 = str_loc(DECIMAL, 0)             # <<<<<<<<<<<<<<
- * COMPLEX_ID: cython.Py_UCS4 = str_loc(COMPLEX, 0)
+ * DECIMAL_ID: cython.Py_UCS4 = read_char(DECIMAL, 0)             # <<<<<<<<<<<<<<
+ * COMPLEX_ID: cython.Py_UCS4 = read_char(COMPLEX, 0)
  * 
  */
   __pyx_t_2 = __pyx_v_10serializor_6prefix_DECIMAL;
   __Pyx_INCREF(__pyx_t_2);
   __pyx_v_10serializor_6prefix_DECIMAL_ID = PyUnicode_READ_CHAR(__pyx_t_2, 0);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "serializor/prefix.py":44
  * # . identifier
- * DECIMAL_ID: cython.Py_UCS4 = str_loc(DECIMAL, 0)
- * COMPLEX_ID: cython.Py_UCS4 = str_loc(COMPLEX, 0)             # <<<<<<<<<<<<<<
+ * DECIMAL_ID: cython.Py_UCS4 = read_char(DECIMAL, 0)
+ * COMPLEX_ID: cython.Py_UCS4 = read_char(COMPLEX, 0)             # <<<<<<<<<<<<<<
  * 
  * # Bytes Types -----------------------------------------------------------------------
  */
   __pyx_t_2 = __pyx_v_10serializor_6prefix_COMPLEX;
   __Pyx_INCREF(__pyx_t_2);
   __pyx_v_10serializor_6prefix_COMPLEX_ID = PyUnicode_READ_CHAR(__pyx_t_2, 0);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "serializor/prefix.py":47
  * 
  * # Bytes Types -----------------------------------------------------------------------
  * BYTES: str = "b"             # <<<<<<<<<<<<<<
  * # . identifier
- * BYTES_ID: cython.Py_UCS4 = str_loc(BYTES, 0)
+ * BYTES_ID: cython.Py_UCS4 = read_char(BYTES, 0)
  */
   __Pyx_INCREF(__pyx_n_u_b);
   __Pyx_XGOTREF(__pyx_v_10serializor_6prefix_BYTES);
   __Pyx_DECREF_SET(__pyx_v_10serializor_6prefix_BYTES, __pyx_n_u_b);
   __Pyx_GIVEREF(__pyx_n_u_b);
 
   /* "serializor/prefix.py":49
  * BYTES: str = "b"
  * # . identifier
- * BYTES_ID: cython.Py_UCS4 = str_loc(BYTES, 0)             # <<<<<<<<<<<<<<
+ * BYTES_ID: cython.Py_UCS4 = read_char(BYTES, 0)             # <<<<<<<<<<<<<<
  * 
  * # Mapping ---------------------------------------------------------------------------
  */
   __pyx_t_2 = __pyx_v_10serializor_6prefix_BYTES;
   __Pyx_INCREF(__pyx_t_2);
   __pyx_v_10serializor_6prefix_BYTES_ID = PyUnicode_READ_CHAR(__pyx_t_2, 0);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "serializor/prefix.py":52
  * 
  * # Mapping ---------------------------------------------------------------------------
  * DICT: str = "D"             # <<<<<<<<<<<<<<
  * # . identifier
- * DICT_ID: cython.Py_UCS4 = str_loc(DICT, 0)
+ * DICT_ID: cython.Py_UCS4 = read_char(DICT, 0)
  */
   __Pyx_INCREF(__pyx_n_u_D);
   __Pyx_XGOTREF(__pyx_v_10serializor_6prefix_DICT);
   __Pyx_DECREF_SET(__pyx_v_10serializor_6prefix_DICT, __pyx_n_u_D);
   __Pyx_GIVEREF(__pyx_n_u_D);
 
   /* "serializor/prefix.py":54
  * DICT: str = "D"
  * # . identifier
- * DICT_ID: cython.Py_UCS4 = str_loc(DICT, 0)             # <<<<<<<<<<<<<<
+ * DICT_ID: cython.Py_UCS4 = read_char(DICT, 0)             # <<<<<<<<<<<<<<
  * 
  * # Sequence Types --------------------------------------------------------------------
  */
   __pyx_t_2 = __pyx_v_10serializor_6prefix_DICT;
   __Pyx_INCREF(__pyx_t_2);
   __pyx_v_10serializor_6prefix_DICT_ID = PyUnicode_READ_CHAR(__pyx_t_2, 0);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
@@ -4589,49 +4589,49 @@
   __Pyx_GIVEREF(__pyx_n_u_T);
 
   /* "serializor/prefix.py":59
  * LIST: str = "L"
  * TUPLE: str = "T"
  * SET: str = "E"             # <<<<<<<<<<<<<<
  * # . identifier
- * LIST_ID: cython.Py_UCS4 = str_loc(LIST, 0)
+ * LIST_ID: cython.Py_UCS4 = read_char(LIST, 0)
  */
   __Pyx_INCREF(__pyx_n_u_E);
   __Pyx_XGOTREF(__pyx_v_10serializor_6prefix_SET);
   __Pyx_DECREF_SET(__pyx_v_10serializor_6prefix_SET, __pyx_n_u_E);
   __Pyx_GIVEREF(__pyx_n_u_E);
 
   /* "serializor/prefix.py":61
  * SET: str = "E"
  * # . identifier
- * LIST_ID: cython.Py_UCS4 = str_loc(LIST, 0)             # <<<<<<<<<<<<<<
- * TUPLE_ID: cython.Py_UCS4 = str_loc(TUPLE, 0)
- * SET_ID: cython.Py_UCS4 = str_loc(SET, 0)
+ * LIST_ID: cython.Py_UCS4 = read_char(LIST, 0)             # <<<<<<<<<<<<<<
+ * TUPLE_ID: cython.Py_UCS4 = read_char(TUPLE, 0)
+ * SET_ID: cython.Py_UCS4 = read_char(SET, 0)
  */
   __pyx_t_2 = __pyx_v_10serializor_6prefix_LIST;
   __Pyx_INCREF(__pyx_t_2);
   __pyx_v_10serializor_6prefix_LIST_ID = PyUnicode_READ_CHAR(__pyx_t_2, 0);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "serializor/prefix.py":62
  * # . identifier
- * LIST_ID: cython.Py_UCS4 = str_loc(LIST, 0)
- * TUPLE_ID: cython.Py_UCS4 = str_loc(TUPLE, 0)             # <<<<<<<<<<<<<<
- * SET_ID: cython.Py_UCS4 = str_loc(SET, 0)
+ * LIST_ID: cython.Py_UCS4 = read_char(LIST, 0)
+ * TUPLE_ID: cython.Py_UCS4 = read_char(TUPLE, 0)             # <<<<<<<<<<<<<<
+ * SET_ID: cython.Py_UCS4 = read_char(SET, 0)
  * 
  */
   __pyx_t_2 = __pyx_v_10serializor_6prefix_TUPLE;
   __Pyx_INCREF(__pyx_t_2);
   __pyx_v_10serializor_6prefix_TUPLE_ID = PyUnicode_READ_CHAR(__pyx_t_2, 0);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "serializor/prefix.py":63
- * LIST_ID: cython.Py_UCS4 = str_loc(LIST, 0)
- * TUPLE_ID: cython.Py_UCS4 = str_loc(TUPLE, 0)
- * SET_ID: cython.Py_UCS4 = str_loc(SET, 0)             # <<<<<<<<<<<<<<
+ * LIST_ID: cython.Py_UCS4 = read_char(LIST, 0)
+ * TUPLE_ID: cython.Py_UCS4 = read_char(TUPLE, 0)
+ * SET_ID: cython.Py_UCS4 = read_char(SET, 0)             # <<<<<<<<<<<<<<
  * 
  * # Numpy Types -----------------------------------------------------------------------
  */
   __pyx_t_2 = __pyx_v_10serializor_6prefix_SET;
   __Pyx_INCREF(__pyx_t_2);
   __pyx_v_10serializor_6prefix_SET_ID = PyUnicode_READ_CHAR(__pyx_t_2, 0);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
@@ -4649,47 +4649,47 @@
   __Pyx_GIVEREF(__pyx_n_u_M);
 
   /* "serializor/prefix.py":67
  * # Numpy Types -----------------------------------------------------------------------
  * DATETIME64: str = "M"
  * TIMEDELTA64: str = "m"             # <<<<<<<<<<<<<<
  * # . identifier
- * DATETIME64_ID: cython.Py_UCS4 = str_loc(DATETIME64, 0)
+ * DATETIME64_ID: cython.Py_UCS4 = read_char(DATETIME64, 0)
  */
   __Pyx_INCREF(__pyx_n_u_m);
   __Pyx_XGOTREF(__pyx_v_10serializor_6prefix_TIMEDELTA64);
   __Pyx_DECREF_SET(__pyx_v_10serializor_6prefix_TIMEDELTA64, __pyx_n_u_m);
   __Pyx_GIVEREF(__pyx_n_u_m);
 
   /* "serializor/prefix.py":69
  * TIMEDELTA64: str = "m"
  * # . identifier
- * DATETIME64_ID: cython.Py_UCS4 = str_loc(DATETIME64, 0)             # <<<<<<<<<<<<<<
- * TIMEDELTA64_ID: cython.Py_UCS4 = str_loc(TIMEDELTA64, 0)
+ * DATETIME64_ID: cython.Py_UCS4 = read_char(DATETIME64, 0)             # <<<<<<<<<<<<<<
+ * TIMEDELTA64_ID: cython.Py_UCS4 = read_char(TIMEDELTA64, 0)
  * # . variant
  */
   __pyx_t_2 = __pyx_v_10serializor_6prefix_DATETIME64;
   __Pyx_INCREF(__pyx_t_2);
   __pyx_v_10serializor_6prefix_DATETIME64_ID = PyUnicode_READ_CHAR(__pyx_t_2, 0);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "serializor/prefix.py":70
  * # . identifier
- * DATETIME64_ID: cython.Py_UCS4 = str_loc(DATETIME64, 0)
- * TIMEDELTA64_ID: cython.Py_UCS4 = str_loc(TIMEDELTA64, 0)             # <<<<<<<<<<<<<<
+ * DATETIME64_ID: cython.Py_UCS4 = read_char(DATETIME64, 0)
+ * TIMEDELTA64_ID: cython.Py_UCS4 = read_char(TIMEDELTA64, 0)             # <<<<<<<<<<<<<<
  * # . variant
  * DATETIME64_Y: str = DATETIME64 + "Y"  # 'MY'
  */
   __pyx_t_2 = __pyx_v_10serializor_6prefix_TIMEDELTA64;
   __Pyx_INCREF(__pyx_t_2);
   __pyx_v_10serializor_6prefix_TIMEDELTA64_ID = PyUnicode_READ_CHAR(__pyx_t_2, 0);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "serializor/prefix.py":72
- * TIMEDELTA64_ID: cython.Py_UCS4 = str_loc(TIMEDELTA64, 0)
+ * TIMEDELTA64_ID: cython.Py_UCS4 = read_char(TIMEDELTA64, 0)
  * # . variant
  * DATETIME64_Y: str = DATETIME64 + "Y"  # 'MY'             # <<<<<<<<<<<<<<
  * DATETIME64_M: str = DATETIME64 + "M"  # 'MM'
  * DATETIME64_W: str = DATETIME64 + "W"  # 'MW'
  */
   __pyx_t_2 = __Pyx_PyUnicode_ConcatSafe(__pyx_v_10serializor_6prefix_DATETIME64, __pyx_n_u_Y); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 72, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
@@ -5407,15 +5407,15 @@
   __pyx_t_4 = 0;
 
   /* "serializor/prefix.py":112
  * NDARRAY_DTYPE_COMPLEX: str = np.array(1 + 1j, dtype=np.complex128).dtype.kind  # 'c'
  * NDARRAY_DTYPE_BYTES: str = np.array(b"", dtype="S").dtype.kind  # 'S'
  * NDARRAY_DTYPE_UNICODE: str = np.array("", dtype="U").dtype.kind  # 'U'             # <<<<<<<<<<<<<<
  * # . identifier
- * NDARRAY_ID: cython.Py_UCS4 = str_loc(NDARRAY, 0)
+ * NDARRAY_ID: cython.Py_UCS4 = read_char(NDARRAY, 0)
  */
   __Pyx_GetModuleGlobalName(__pyx_t_4, __pyx_n_s_np); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 112, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_4);
   __pyx_t_7 = __Pyx_PyObject_GetAttrStr(__pyx_t_4, __pyx_n_s_array); if (unlikely(!__pyx_t_7)) __PYX_ERR(0, 112, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_7);
   __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
   __pyx_t_4 = __Pyx_PyDict_NewPresized(1); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 112, __pyx_L1_error)
@@ -5436,145 +5436,145 @@
   __Pyx_DECREF_SET(__pyx_v_10serializor_6prefix_NDARRAY_DTYPE_UNICODE, ((PyObject*)__pyx_t_2));
   __Pyx_GIVEREF(__pyx_t_2);
   __pyx_t_2 = 0;
 
   /* "serializor/prefix.py":114
  * NDARRAY_DTYPE_UNICODE: str = np.array("", dtype="U").dtype.kind  # 'U'
  * # . identifier
- * NDARRAY_ID: cython.Py_UCS4 = str_loc(NDARRAY, 0)             # <<<<<<<<<<<<<<
- * NDARRAY_DTYPE_OBJECT_ID: cython.Py_UCS4 = str_loc(NDARRAY_DTYPE_OBJECT, 0)
- * NDARRAY_DTYPE_FLOAT_ID: cython.Py_UCS4 = str_loc(NDARRAY_DTYPE_FLOAT, 0)
+ * NDARRAY_ID: cython.Py_UCS4 = read_char(NDARRAY, 0)             # <<<<<<<<<<<<<<
+ * NDARRAY_DTYPE_OBJECT_ID: cython.Py_UCS4 = read_char(NDARRAY_DTYPE_OBJECT, 0)
+ * NDARRAY_DTYPE_FLOAT_ID: cython.Py_UCS4 = read_char(NDARRAY_DTYPE_FLOAT, 0)
  */
   __pyx_t_2 = __pyx_v_10serializor_6prefix_NDARRAY;
   __Pyx_INCREF(__pyx_t_2);
   __pyx_v_10serializor_6prefix_NDARRAY_ID = PyUnicode_READ_CHAR(__pyx_t_2, 0);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "serializor/prefix.py":115
  * # . identifier
- * NDARRAY_ID: cython.Py_UCS4 = str_loc(NDARRAY, 0)
- * NDARRAY_DTYPE_OBJECT_ID: cython.Py_UCS4 = str_loc(NDARRAY_DTYPE_OBJECT, 0)             # <<<<<<<<<<<<<<
- * NDARRAY_DTYPE_FLOAT_ID: cython.Py_UCS4 = str_loc(NDARRAY_DTYPE_FLOAT, 0)
- * NDARRAY_DTYPE_INT_ID: cython.Py_UCS4 = str_loc(NDARRAY_DTYPE_INT, 0)
+ * NDARRAY_ID: cython.Py_UCS4 = read_char(NDARRAY, 0)
+ * NDARRAY_DTYPE_OBJECT_ID: cython.Py_UCS4 = read_char(NDARRAY_DTYPE_OBJECT, 0)             # <<<<<<<<<<<<<<
+ * NDARRAY_DTYPE_FLOAT_ID: cython.Py_UCS4 = read_char(NDARRAY_DTYPE_FLOAT, 0)
+ * NDARRAY_DTYPE_INT_ID: cython.Py_UCS4 = read_char(NDARRAY_DTYPE_INT, 0)
  */
   __pyx_t_2 = __pyx_v_10serializor_6prefix_NDARRAY_DTYPE_OBJECT;
   __Pyx_INCREF(__pyx_t_2);
   __pyx_v_10serializor_6prefix_NDARRAY_DTYPE_OBJECT_ID = PyUnicode_READ_CHAR(__pyx_t_2, 0);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "serializor/prefix.py":116
- * NDARRAY_ID: cython.Py_UCS4 = str_loc(NDARRAY, 0)
- * NDARRAY_DTYPE_OBJECT_ID: cython.Py_UCS4 = str_loc(NDARRAY_DTYPE_OBJECT, 0)
- * NDARRAY_DTYPE_FLOAT_ID: cython.Py_UCS4 = str_loc(NDARRAY_DTYPE_FLOAT, 0)             # <<<<<<<<<<<<<<
- * NDARRAY_DTYPE_INT_ID: cython.Py_UCS4 = str_loc(NDARRAY_DTYPE_INT, 0)
- * NDARRAY_DTYPE_UINT_ID: cython.Py_UCS4 = str_loc(NDARRAY_DTYPE_UINT, 0)
+ * NDARRAY_ID: cython.Py_UCS4 = read_char(NDARRAY, 0)
+ * NDARRAY_DTYPE_OBJECT_ID: cython.Py_UCS4 = read_char(NDARRAY_DTYPE_OBJECT, 0)
+ * NDARRAY_DTYPE_FLOAT_ID: cython.Py_UCS4 = read_char(NDARRAY_DTYPE_FLOAT, 0)             # <<<<<<<<<<<<<<
+ * NDARRAY_DTYPE_INT_ID: cython.Py_UCS4 = read_char(NDARRAY_DTYPE_INT, 0)
+ * NDARRAY_DTYPE_UINT_ID: cython.Py_UCS4 = read_char(NDARRAY_DTYPE_UINT, 0)
  */
   __pyx_t_2 = __pyx_v_10serializor_6prefix_NDARRAY_DTYPE_FLOAT;
   __Pyx_INCREF(__pyx_t_2);
   __pyx_v_10serializor_6prefix_NDARRAY_DTYPE_FLOAT_ID = PyUnicode_READ_CHAR(__pyx_t_2, 0);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "serializor/prefix.py":117
- * NDARRAY_DTYPE_OBJECT_ID: cython.Py_UCS4 = str_loc(NDARRAY_DTYPE_OBJECT, 0)
- * NDARRAY_DTYPE_FLOAT_ID: cython.Py_UCS4 = str_loc(NDARRAY_DTYPE_FLOAT, 0)
- * NDARRAY_DTYPE_INT_ID: cython.Py_UCS4 = str_loc(NDARRAY_DTYPE_INT, 0)             # <<<<<<<<<<<<<<
- * NDARRAY_DTYPE_UINT_ID: cython.Py_UCS4 = str_loc(NDARRAY_DTYPE_UINT, 0)
- * NDARRAY_DTYPE_BOOL_ID: cython.Py_UCS4 = str_loc(NDARRAY_DTYPE_BOOL, 0)
+ * NDARRAY_DTYPE_OBJECT_ID: cython.Py_UCS4 = read_char(NDARRAY_DTYPE_OBJECT, 0)
+ * NDARRAY_DTYPE_FLOAT_ID: cython.Py_UCS4 = read_char(NDARRAY_DTYPE_FLOAT, 0)
+ * NDARRAY_DTYPE_INT_ID: cython.Py_UCS4 = read_char(NDARRAY_DTYPE_INT, 0)             # <<<<<<<<<<<<<<
+ * NDARRAY_DTYPE_UINT_ID: cython.Py_UCS4 = read_char(NDARRAY_DTYPE_UINT, 0)
+ * NDARRAY_DTYPE_BOOL_ID: cython.Py_UCS4 = read_char(NDARRAY_DTYPE_BOOL, 0)
  */
   __pyx_t_2 = __pyx_v_10serializor_6prefix_NDARRAY_DTYPE_INT;
   __Pyx_INCREF(__pyx_t_2);
   __pyx_v_10serializor_6prefix_NDARRAY_DTYPE_INT_ID = PyUnicode_READ_CHAR(__pyx_t_2, 0);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "serializor/prefix.py":118
- * NDARRAY_DTYPE_FLOAT_ID: cython.Py_UCS4 = str_loc(NDARRAY_DTYPE_FLOAT, 0)
- * NDARRAY_DTYPE_INT_ID: cython.Py_UCS4 = str_loc(NDARRAY_DTYPE_INT, 0)
- * NDARRAY_DTYPE_UINT_ID: cython.Py_UCS4 = str_loc(NDARRAY_DTYPE_UINT, 0)             # <<<<<<<<<<<<<<
- * NDARRAY_DTYPE_BOOL_ID: cython.Py_UCS4 = str_loc(NDARRAY_DTYPE_BOOL, 0)
- * NDARRAY_DTYPE_DT64_ID: cython.Py_UCS4 = str_loc(NDARRAY_DTYPE_DT64, 0)
+ * NDARRAY_DTYPE_FLOAT_ID: cython.Py_UCS4 = read_char(NDARRAY_DTYPE_FLOAT, 0)
+ * NDARRAY_DTYPE_INT_ID: cython.Py_UCS4 = read_char(NDARRAY_DTYPE_INT, 0)
+ * NDARRAY_DTYPE_UINT_ID: cython.Py_UCS4 = read_char(NDARRAY_DTYPE_UINT, 0)             # <<<<<<<<<<<<<<
+ * NDARRAY_DTYPE_BOOL_ID: cython.Py_UCS4 = read_char(NDARRAY_DTYPE_BOOL, 0)
+ * NDARRAY_DTYPE_DT64_ID: cython.Py_UCS4 = read_char(NDARRAY_DTYPE_DT64, 0)
  */
   __pyx_t_2 = __pyx_v_10serializor_6prefix_NDARRAY_DTYPE_UINT;
   __Pyx_INCREF(__pyx_t_2);
   __pyx_v_10serializor_6prefix_NDARRAY_DTYPE_UINT_ID = PyUnicode_READ_CHAR(__pyx_t_2, 0);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "serializor/prefix.py":119
- * NDARRAY_DTYPE_INT_ID: cython.Py_UCS4 = str_loc(NDARRAY_DTYPE_INT, 0)
- * NDARRAY_DTYPE_UINT_ID: cython.Py_UCS4 = str_loc(NDARRAY_DTYPE_UINT, 0)
- * NDARRAY_DTYPE_BOOL_ID: cython.Py_UCS4 = str_loc(NDARRAY_DTYPE_BOOL, 0)             # <<<<<<<<<<<<<<
- * NDARRAY_DTYPE_DT64_ID: cython.Py_UCS4 = str_loc(NDARRAY_DTYPE_DT64, 0)
- * NDARRAY_DTYPE_TD64_ID: cython.Py_UCS4 = str_loc(NDARRAY_DTYPE_TD64, 0)
+ * NDARRAY_DTYPE_INT_ID: cython.Py_UCS4 = read_char(NDARRAY_DTYPE_INT, 0)
+ * NDARRAY_DTYPE_UINT_ID: cython.Py_UCS4 = read_char(NDARRAY_DTYPE_UINT, 0)
+ * NDARRAY_DTYPE_BOOL_ID: cython.Py_UCS4 = read_char(NDARRAY_DTYPE_BOOL, 0)             # <<<<<<<<<<<<<<
+ * NDARRAY_DTYPE_DT64_ID: cython.Py_UCS4 = read_char(NDARRAY_DTYPE_DT64, 0)
+ * NDARRAY_DTYPE_TD64_ID: cython.Py_UCS4 = read_char(NDARRAY_DTYPE_TD64, 0)
  */
   __pyx_t_2 = __pyx_v_10serializor_6prefix_NDARRAY_DTYPE_BOOL;
   __Pyx_INCREF(__pyx_t_2);
   __pyx_v_10serializor_6prefix_NDARRAY_DTYPE_BOOL_ID = PyUnicode_READ_CHAR(__pyx_t_2, 0);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "serializor/prefix.py":120
- * NDARRAY_DTYPE_UINT_ID: cython.Py_UCS4 = str_loc(NDARRAY_DTYPE_UINT, 0)
- * NDARRAY_DTYPE_BOOL_ID: cython.Py_UCS4 = str_loc(NDARRAY_DTYPE_BOOL, 0)
- * NDARRAY_DTYPE_DT64_ID: cython.Py_UCS4 = str_loc(NDARRAY_DTYPE_DT64, 0)             # <<<<<<<<<<<<<<
- * NDARRAY_DTYPE_TD64_ID: cython.Py_UCS4 = str_loc(NDARRAY_DTYPE_TD64, 0)
- * NDARRAY_DTYPE_COMPLEX_ID: cython.Py_UCS4 = str_loc(NDARRAY_DTYPE_COMPLEX, 0)
+ * NDARRAY_DTYPE_UINT_ID: cython.Py_UCS4 = read_char(NDARRAY_DTYPE_UINT, 0)
+ * NDARRAY_DTYPE_BOOL_ID: cython.Py_UCS4 = read_char(NDARRAY_DTYPE_BOOL, 0)
+ * NDARRAY_DTYPE_DT64_ID: cython.Py_UCS4 = read_char(NDARRAY_DTYPE_DT64, 0)             # <<<<<<<<<<<<<<
+ * NDARRAY_DTYPE_TD64_ID: cython.Py_UCS4 = read_char(NDARRAY_DTYPE_TD64, 0)
+ * NDARRAY_DTYPE_COMPLEX_ID: cython.Py_UCS4 = read_char(NDARRAY_DTYPE_COMPLEX, 0)
  */
   __pyx_t_2 = __pyx_v_10serializor_6prefix_NDARRAY_DTYPE_DT64;
   __Pyx_INCREF(__pyx_t_2);
   __pyx_v_10serializor_6prefix_NDARRAY_DTYPE_DT64_ID = PyUnicode_READ_CHAR(__pyx_t_2, 0);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "serializor/prefix.py":121
- * NDARRAY_DTYPE_BOOL_ID: cython.Py_UCS4 = str_loc(NDARRAY_DTYPE_BOOL, 0)
- * NDARRAY_DTYPE_DT64_ID: cython.Py_UCS4 = str_loc(NDARRAY_DTYPE_DT64, 0)
- * NDARRAY_DTYPE_TD64_ID: cython.Py_UCS4 = str_loc(NDARRAY_DTYPE_TD64, 0)             # <<<<<<<<<<<<<<
- * NDARRAY_DTYPE_COMPLEX_ID: cython.Py_UCS4 = str_loc(NDARRAY_DTYPE_COMPLEX, 0)
- * NDARRAY_DTYPE_BYTES_ID: cython.Py_UCS4 = str_loc(NDARRAY_DTYPE_BYTES, 0)
+ * NDARRAY_DTYPE_BOOL_ID: cython.Py_UCS4 = read_char(NDARRAY_DTYPE_BOOL, 0)
+ * NDARRAY_DTYPE_DT64_ID: cython.Py_UCS4 = read_char(NDARRAY_DTYPE_DT64, 0)
+ * NDARRAY_DTYPE_TD64_ID: cython.Py_UCS4 = read_char(NDARRAY_DTYPE_TD64, 0)             # <<<<<<<<<<<<<<
+ * NDARRAY_DTYPE_COMPLEX_ID: cython.Py_UCS4 = read_char(NDARRAY_DTYPE_COMPLEX, 0)
+ * NDARRAY_DTYPE_BYTES_ID: cython.Py_UCS4 = read_char(NDARRAY_DTYPE_BYTES, 0)
  */
   __pyx_t_2 = __pyx_v_10serializor_6prefix_NDARRAY_DTYPE_TD64;
   __Pyx_INCREF(__pyx_t_2);
   __pyx_v_10serializor_6prefix_NDARRAY_DTYPE_TD64_ID = PyUnicode_READ_CHAR(__pyx_t_2, 0);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "serializor/prefix.py":122
- * NDARRAY_DTYPE_DT64_ID: cython.Py_UCS4 = str_loc(NDARRAY_DTYPE_DT64, 0)
- * NDARRAY_DTYPE_TD64_ID: cython.Py_UCS4 = str_loc(NDARRAY_DTYPE_TD64, 0)
- * NDARRAY_DTYPE_COMPLEX_ID: cython.Py_UCS4 = str_loc(NDARRAY_DTYPE_COMPLEX, 0)             # <<<<<<<<<<<<<<
- * NDARRAY_DTYPE_BYTES_ID: cython.Py_UCS4 = str_loc(NDARRAY_DTYPE_BYTES, 0)
- * NDARRAY_DTYPE_UNICODE_ID: cython.Py_UCS4 = str_loc(NDARRAY_DTYPE_UNICODE, 0)
+ * NDARRAY_DTYPE_DT64_ID: cython.Py_UCS4 = read_char(NDARRAY_DTYPE_DT64, 0)
+ * NDARRAY_DTYPE_TD64_ID: cython.Py_UCS4 = read_char(NDARRAY_DTYPE_TD64, 0)
+ * NDARRAY_DTYPE_COMPLEX_ID: cython.Py_UCS4 = read_char(NDARRAY_DTYPE_COMPLEX, 0)             # <<<<<<<<<<<<<<
+ * NDARRAY_DTYPE_BYTES_ID: cython.Py_UCS4 = read_char(NDARRAY_DTYPE_BYTES, 0)
+ * NDARRAY_DTYPE_UNICODE_ID: cython.Py_UCS4 = read_char(NDARRAY_DTYPE_UNICODE, 0)
  */
   __pyx_t_2 = __pyx_v_10serializor_6prefix_NDARRAY_DTYPE_COMPLEX;
   __Pyx_INCREF(__pyx_t_2);
   __pyx_v_10serializor_6prefix_NDARRAY_DTYPE_COMPLEX_ID = PyUnicode_READ_CHAR(__pyx_t_2, 0);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "serializor/prefix.py":123
- * NDARRAY_DTYPE_TD64_ID: cython.Py_UCS4 = str_loc(NDARRAY_DTYPE_TD64, 0)
- * NDARRAY_DTYPE_COMPLEX_ID: cython.Py_UCS4 = str_loc(NDARRAY_DTYPE_COMPLEX, 0)
- * NDARRAY_DTYPE_BYTES_ID: cython.Py_UCS4 = str_loc(NDARRAY_DTYPE_BYTES, 0)             # <<<<<<<<<<<<<<
- * NDARRAY_DTYPE_UNICODE_ID: cython.Py_UCS4 = str_loc(NDARRAY_DTYPE_UNICODE, 0)
+ * NDARRAY_DTYPE_TD64_ID: cython.Py_UCS4 = read_char(NDARRAY_DTYPE_TD64, 0)
+ * NDARRAY_DTYPE_COMPLEX_ID: cython.Py_UCS4 = read_char(NDARRAY_DTYPE_COMPLEX, 0)
+ * NDARRAY_DTYPE_BYTES_ID: cython.Py_UCS4 = read_char(NDARRAY_DTYPE_BYTES, 0)             # <<<<<<<<<<<<<<
+ * NDARRAY_DTYPE_UNICODE_ID: cython.Py_UCS4 = read_char(NDARRAY_DTYPE_UNICODE, 0)
  * # . variant dtype
  */
   __pyx_t_2 = __pyx_v_10serializor_6prefix_NDARRAY_DTYPE_BYTES;
   __Pyx_INCREF(__pyx_t_2);
   __pyx_v_10serializor_6prefix_NDARRAY_DTYPE_BYTES_ID = PyUnicode_READ_CHAR(__pyx_t_2, 0);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "serializor/prefix.py":124
- * NDARRAY_DTYPE_COMPLEX_ID: cython.Py_UCS4 = str_loc(NDARRAY_DTYPE_COMPLEX, 0)
- * NDARRAY_DTYPE_BYTES_ID: cython.Py_UCS4 = str_loc(NDARRAY_DTYPE_BYTES, 0)
- * NDARRAY_DTYPE_UNICODE_ID: cython.Py_UCS4 = str_loc(NDARRAY_DTYPE_UNICODE, 0)             # <<<<<<<<<<<<<<
+ * NDARRAY_DTYPE_COMPLEX_ID: cython.Py_UCS4 = read_char(NDARRAY_DTYPE_COMPLEX, 0)
+ * NDARRAY_DTYPE_BYTES_ID: cython.Py_UCS4 = read_char(NDARRAY_DTYPE_BYTES, 0)
+ * NDARRAY_DTYPE_UNICODE_ID: cython.Py_UCS4 = read_char(NDARRAY_DTYPE_UNICODE, 0)             # <<<<<<<<<<<<<<
  * # . variant dtype
  * NDARRAY_DTYPE_DT64_Y: str = NDARRAY_DTYPE_DT64 + "Y"  # 'MY'
  */
   __pyx_t_2 = __pyx_v_10serializor_6prefix_NDARRAY_DTYPE_UNICODE;
   __Pyx_INCREF(__pyx_t_2);
   __pyx_v_10serializor_6prefix_NDARRAY_DTYPE_UNICODE_ID = PyUnicode_READ_CHAR(__pyx_t_2, 0);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "serializor/prefix.py":126
- * NDARRAY_DTYPE_UNICODE_ID: cython.Py_UCS4 = str_loc(NDARRAY_DTYPE_UNICODE, 0)
+ * NDARRAY_DTYPE_UNICODE_ID: cython.Py_UCS4 = read_char(NDARRAY_DTYPE_UNICODE, 0)
  * # . variant dtype
  * NDARRAY_DTYPE_DT64_Y: str = NDARRAY_DTYPE_DT64 + "Y"  # 'MY'             # <<<<<<<<<<<<<<
  * NDARRAY_DTYPE_DT64_M: str = NDARRAY_DTYPE_DT64 + "M"  # 'MM'
  * NDARRAY_DTYPE_DT64_W: str = NDARRAY_DTYPE_DT64 + "W"  # 'MW'
  */
   __pyx_t_2 = __Pyx_PyUnicode_ConcatSafe(__pyx_v_10serializor_6prefix_NDARRAY_DTYPE_DT64, __pyx_n_u_Y); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 126, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
@@ -6086,71 +6086,71 @@
   __Pyx_GIVEREF(__pyx_n_u_Z);
 
   /* "serializor/prefix.py":166
  * # Pandas Types ----------------------------------------------------------------------
  * DATETIMEINDEX: str = "Z"
  * TIMEDELTAINDEX: str = "X"             # <<<<<<<<<<<<<<
  * # . identifier
- * DATETIMEINDEX_ID: cython.Py_UCS4 = str_loc(DATETIMEINDEX, 0)
+ * DATETIMEINDEX_ID: cython.Py_UCS4 = read_char(DATETIMEINDEX, 0)
  */
   __Pyx_INCREF(__pyx_n_u_X);
   __Pyx_XGOTREF(__pyx_v_10serializor_6prefix_TIMEDELTAINDEX);
   __Pyx_DECREF_SET(__pyx_v_10serializor_6prefix_TIMEDELTAINDEX, __pyx_n_u_X);
   __Pyx_GIVEREF(__pyx_n_u_X);
 
   /* "serializor/prefix.py":168
  * TIMEDELTAINDEX: str = "X"
  * # . identifier
- * DATETIMEINDEX_ID: cython.Py_UCS4 = str_loc(DATETIMEINDEX, 0)             # <<<<<<<<<<<<<<
- * TIMEDELTAINDEX_ID: cython.Py_UCS4 = str_loc(TIMEDELTAINDEX, 0)
+ * DATETIMEINDEX_ID: cython.Py_UCS4 = read_char(DATETIMEINDEX, 0)             # <<<<<<<<<<<<<<
+ * TIMEDELTAINDEX_ID: cython.Py_UCS4 = read_char(TIMEDELTAINDEX, 0)
  * 
  */
   __pyx_t_2 = __pyx_v_10serializor_6prefix_DATETIMEINDEX;
   __Pyx_INCREF(__pyx_t_2);
   __pyx_v_10serializor_6prefix_DATETIMEINDEX_ID = PyUnicode_READ_CHAR(__pyx_t_2, 0);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "serializor/prefix.py":169
  * # . identifier
- * DATETIMEINDEX_ID: cython.Py_UCS4 = str_loc(DATETIMEINDEX, 0)
- * TIMEDELTAINDEX_ID: cython.Py_UCS4 = str_loc(TIMEDELTAINDEX, 0)             # <<<<<<<<<<<<<<
+ * DATETIMEINDEX_ID: cython.Py_UCS4 = read_char(DATETIMEINDEX, 0)
+ * TIMEDELTAINDEX_ID: cython.Py_UCS4 = read_char(TIMEDELTAINDEX, 0)             # <<<<<<<<<<<<<<
  * 
  * # Pandas.Series ---------------------------------------------------------------------
  */
   __pyx_t_2 = __pyx_v_10serializor_6prefix_TIMEDELTAINDEX;
   __Pyx_INCREF(__pyx_t_2);
   __pyx_v_10serializor_6prefix_TIMEDELTAINDEX_ID = PyUnicode_READ_CHAR(__pyx_t_2, 0);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "serializor/prefix.py":172
  * 
  * # Pandas.Series ---------------------------------------------------------------------
  * SERIES: str = "I"             # <<<<<<<<<<<<<<
  * # . identifier
- * SERIES_ID: cython.Py_UCS4 = str_loc(SERIES, 0)
+ * SERIES_ID: cython.Py_UCS4 = read_char(SERIES, 0)
  */
   __Pyx_INCREF(__pyx_n_u_I);
   __Pyx_XGOTREF(__pyx_v_10serializor_6prefix_SERIES);
   __Pyx_DECREF_SET(__pyx_v_10serializor_6prefix_SERIES, __pyx_n_u_I);
   __Pyx_GIVEREF(__pyx_n_u_I);
 
   /* "serializor/prefix.py":174
  * SERIES: str = "I"
  * # . identifier
- * SERIES_ID: cython.Py_UCS4 = str_loc(SERIES, 0)             # <<<<<<<<<<<<<<
+ * SERIES_ID: cython.Py_UCS4 = read_char(SERIES, 0)             # <<<<<<<<<<<<<<
  * # . variant
  * SERIES_OBJECT: str = SERIES + NDARRAY_DTYPE_OBJECT  # 'IO'
  */
   __pyx_t_2 = __pyx_v_10serializor_6prefix_SERIES;
   __Pyx_INCREF(__pyx_t_2);
   __pyx_v_10serializor_6prefix_SERIES_ID = PyUnicode_READ_CHAR(__pyx_t_2, 0);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "serializor/prefix.py":176
- * SERIES_ID: cython.Py_UCS4 = str_loc(SERIES, 0)
+ * SERIES_ID: cython.Py_UCS4 = read_char(SERIES, 0)
  * # . variant
  * SERIES_OBJECT: str = SERIES + NDARRAY_DTYPE_OBJECT  # 'IO'             # <<<<<<<<<<<<<<
  * SERIES_FLOAT: str = SERIES + NDARRAY_DTYPE_FLOAT  # 'If'
  * SERIES_INT: str = SERIES + NDARRAY_DTYPE_INT  # 'Ii'
  */
   __pyx_t_2 = __Pyx_PyUnicode_ConcatSafe(__pyx_v_10serializor_6prefix_SERIES, __pyx_v_10serializor_6prefix_NDARRAY_DTYPE_OBJECT); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 176, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
@@ -6258,35 +6258,35 @@
   __pyx_t_2 = 0;
 
   /* "serializor/prefix.py":186
  * 
  * # Pandas.DataFrame ------------------------------------------------------------------
  * DATAFRAME: str = "F"             # <<<<<<<<<<<<<<
  * # . identifier
- * DATAFRAME_ID: cython.Py_UCS4 = str_loc(DATAFRAME, 0)
+ * DATAFRAME_ID: cython.Py_UCS4 = read_char(DATAFRAME, 0)
  */
   __Pyx_INCREF(__pyx_n_u_F);
   __Pyx_XGOTREF(__pyx_v_10serializor_6prefix_DATAFRAME);
   __Pyx_DECREF_SET(__pyx_v_10serializor_6prefix_DATAFRAME, __pyx_n_u_F);
   __Pyx_GIVEREF(__pyx_n_u_F);
 
   /* "serializor/prefix.py":188
  * DATAFRAME: str = "F"
  * # . identifier
- * DATAFRAME_ID: cython.Py_UCS4 = str_loc(DATAFRAME, 0)             # <<<<<<<<<<<<<<
+ * DATAFRAME_ID: cython.Py_UCS4 = read_char(DATAFRAME, 0)             # <<<<<<<<<<<<<<
  * # . variant
  * DATAFRAME_COL_OBJECT: str = NDARRAY_DTYPE_OBJECT  # 'O'
  */
   __pyx_t_2 = __pyx_v_10serializor_6prefix_DATAFRAME;
   __Pyx_INCREF(__pyx_t_2);
   __pyx_v_10serializor_6prefix_DATAFRAME_ID = PyUnicode_READ_CHAR(__pyx_t_2, 0);
   __Pyx_DECREF(__pyx_t_2); __pyx_t_2 = 0;
 
   /* "serializor/prefix.py":190
- * DATAFRAME_ID: cython.Py_UCS4 = str_loc(DATAFRAME, 0)
+ * DATAFRAME_ID: cython.Py_UCS4 = read_char(DATAFRAME, 0)
  * # . variant
  * DATAFRAME_COL_OBJECT: str = NDARRAY_DTYPE_OBJECT  # 'O'             # <<<<<<<<<<<<<<
  * DATAFRAME_COL_FLOAT: str = NDARRAY_DTYPE_FLOAT  # 'f'
  * DATAFRAME_COL_INT: str = NDARRAY_DTYPE_INT  # 'i'
  */
   __Pyx_INCREF(__pyx_v_10serializor_6prefix_NDARRAY_DTYPE_OBJECT);
   __Pyx_XGOTREF(__pyx_v_10serializor_6prefix_DATAFRAME_COL_OBJECT);
```

### Comparing `serializor-1.0.0/src/serializor/prefix.pxd` & `serializor-1.0.1/src/serializor/prefix.pxd`

 * *Files identical despite different names*

### Comparing `serializor-1.0.0/src/serializor/prefix.py` & `serializor-1.0.1/src/serializor/prefix.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,77 +1,77 @@
 # cython: language_level=3
 # cython: wraparound=False
 # cython: boundscheck=False
 
 # Cython imports
 import cython
-from cython.cimports.cpython.unicode import PyUnicode_READ_CHAR as str_loc  # type: ignore
+from cython.cimports.cpython.unicode import PyUnicode_READ_CHAR as read_char  # type: ignore
 
 # Python imports
 import numpy as np
 
 # Basic Types -----------------------------------------------------------------------
 STR: str = "s"
 BOOL: str = "o"
 FLOAT: str = "f"
 INT: str = "i"
 NONE: str = "n"
 # . identifier
-STR_ID: cython.Py_UCS4 = str_loc(STR, 0)
-BOOL_ID: cython.Py_UCS4 = str_loc(BOOL, 0)
-FLOAT_ID: cython.Py_UCS4 = str_loc(FLOAT, 0)
-INT_ID: cython.Py_UCS4 = str_loc(INT, 0)
-NONE_ID: cython.Py_UCS4 = str_loc(NONE, 0)
+STR_ID: cython.Py_UCS4 = read_char(STR, 0)
+BOOL_ID: cython.Py_UCS4 = read_char(BOOL, 0)
+FLOAT_ID: cython.Py_UCS4 = read_char(FLOAT, 0)
+INT_ID: cython.Py_UCS4 = read_char(INT, 0)
+NONE_ID: cython.Py_UCS4 = read_char(NONE, 0)
 # . variant
 BOOL_TRUE: str = BOOL + "1"  # 'o1'
 BOOL_FALSE: str = BOOL + "0"  # 'o0'
 
 # Date&Time Types -------------------------------------------------------------------
 DATE: str = "d"
 TIME: str = "t"
 DATETIME: str = "z"
 TIMEDELTA: str = "l"
 # . identifier
-DATE_ID: cython.Py_UCS4 = str_loc(DATE, 0)
-TIME_ID: cython.Py_UCS4 = str_loc(TIME, 0)
-DATETIME_ID: cython.Py_UCS4 = str_loc(DATETIME, 0)
-TIMEDELTA_ID: cython.Py_UCS4 = str_loc(TIMEDELTA, 0)
+DATE_ID: cython.Py_UCS4 = read_char(DATE, 0)
+TIME_ID: cython.Py_UCS4 = read_char(TIME, 0)
+DATETIME_ID: cython.Py_UCS4 = read_char(DATETIME, 0)
+TIMEDELTA_ID: cython.Py_UCS4 = read_char(TIMEDELTA, 0)
 
 # Numeric Types ---------------------------------------------------------------------
 DECIMAL: str = "e"
 COMPLEX: str = "c"
 # . identifier
-DECIMAL_ID: cython.Py_UCS4 = str_loc(DECIMAL, 0)
-COMPLEX_ID: cython.Py_UCS4 = str_loc(COMPLEX, 0)
+DECIMAL_ID: cython.Py_UCS4 = read_char(DECIMAL, 0)
+COMPLEX_ID: cython.Py_UCS4 = read_char(COMPLEX, 0)
 
 # Bytes Types -----------------------------------------------------------------------
 BYTES: str = "b"
 # . identifier
-BYTES_ID: cython.Py_UCS4 = str_loc(BYTES, 0)
+BYTES_ID: cython.Py_UCS4 = read_char(BYTES, 0)
 
 # Mapping ---------------------------------------------------------------------------
 DICT: str = "D"
 # . identifier
-DICT_ID: cython.Py_UCS4 = str_loc(DICT, 0)
+DICT_ID: cython.Py_UCS4 = read_char(DICT, 0)
 
 # Sequence Types --------------------------------------------------------------------
 LIST: str = "L"
 TUPLE: str = "T"
 SET: str = "E"
 # . identifier
-LIST_ID: cython.Py_UCS4 = str_loc(LIST, 0)
-TUPLE_ID: cython.Py_UCS4 = str_loc(TUPLE, 0)
-SET_ID: cython.Py_UCS4 = str_loc(SET, 0)
+LIST_ID: cython.Py_UCS4 = read_char(LIST, 0)
+TUPLE_ID: cython.Py_UCS4 = read_char(TUPLE, 0)
+SET_ID: cython.Py_UCS4 = read_char(SET, 0)
 
 # Numpy Types -----------------------------------------------------------------------
 DATETIME64: str = "M"
 TIMEDELTA64: str = "m"
 # . identifier
-DATETIME64_ID: cython.Py_UCS4 = str_loc(DATETIME64, 0)
-TIMEDELTA64_ID: cython.Py_UCS4 = str_loc(TIMEDELTA64, 0)
+DATETIME64_ID: cython.Py_UCS4 = read_char(DATETIME64, 0)
+TIMEDELTA64_ID: cython.Py_UCS4 = read_char(TIMEDELTA64, 0)
 # . variant
 DATETIME64_Y: str = DATETIME64 + "Y"  # 'MY'
 DATETIME64_M: str = DATETIME64 + "M"  # 'MM'
 DATETIME64_W: str = DATETIME64 + "W"  # 'MW'
 DATETIME64_D: str = DATETIME64 + "D"  # 'MD'
 DATETIME64_B: str = DATETIME64 + "B"  # 'MB'
 DATETIME64_H: str = DATETIME64 + "h"  # 'Mh'
@@ -107,25 +107,25 @@
 NDARRAY_DTYPE_BOOL: str = np.array(1, dtype=np.bool_).dtype.kind  # 'b'
 NDARRAY_DTYPE_DT64: str = np.array(1, dtype="datetime64[ns]").dtype.kind  # 'M'
 NDARRAY_DTYPE_TD64: str = np.array(1, dtype="timedelta64[ns]").dtype.kind  # 'm'
 NDARRAY_DTYPE_COMPLEX: str = np.array(1 + 1j, dtype=np.complex128).dtype.kind  # 'c'
 NDARRAY_DTYPE_BYTES: str = np.array(b"", dtype="S").dtype.kind  # 'S'
 NDARRAY_DTYPE_UNICODE: str = np.array("", dtype="U").dtype.kind  # 'U'
 # . identifier
-NDARRAY_ID: cython.Py_UCS4 = str_loc(NDARRAY, 0)
-NDARRAY_DTYPE_OBJECT_ID: cython.Py_UCS4 = str_loc(NDARRAY_DTYPE_OBJECT, 0)
-NDARRAY_DTYPE_FLOAT_ID: cython.Py_UCS4 = str_loc(NDARRAY_DTYPE_FLOAT, 0)
-NDARRAY_DTYPE_INT_ID: cython.Py_UCS4 = str_loc(NDARRAY_DTYPE_INT, 0)
-NDARRAY_DTYPE_UINT_ID: cython.Py_UCS4 = str_loc(NDARRAY_DTYPE_UINT, 0)
-NDARRAY_DTYPE_BOOL_ID: cython.Py_UCS4 = str_loc(NDARRAY_DTYPE_BOOL, 0)
-NDARRAY_DTYPE_DT64_ID: cython.Py_UCS4 = str_loc(NDARRAY_DTYPE_DT64, 0)
-NDARRAY_DTYPE_TD64_ID: cython.Py_UCS4 = str_loc(NDARRAY_DTYPE_TD64, 0)
-NDARRAY_DTYPE_COMPLEX_ID: cython.Py_UCS4 = str_loc(NDARRAY_DTYPE_COMPLEX, 0)
-NDARRAY_DTYPE_BYTES_ID: cython.Py_UCS4 = str_loc(NDARRAY_DTYPE_BYTES, 0)
-NDARRAY_DTYPE_UNICODE_ID: cython.Py_UCS4 = str_loc(NDARRAY_DTYPE_UNICODE, 0)
+NDARRAY_ID: cython.Py_UCS4 = read_char(NDARRAY, 0)
+NDARRAY_DTYPE_OBJECT_ID: cython.Py_UCS4 = read_char(NDARRAY_DTYPE_OBJECT, 0)
+NDARRAY_DTYPE_FLOAT_ID: cython.Py_UCS4 = read_char(NDARRAY_DTYPE_FLOAT, 0)
+NDARRAY_DTYPE_INT_ID: cython.Py_UCS4 = read_char(NDARRAY_DTYPE_INT, 0)
+NDARRAY_DTYPE_UINT_ID: cython.Py_UCS4 = read_char(NDARRAY_DTYPE_UINT, 0)
+NDARRAY_DTYPE_BOOL_ID: cython.Py_UCS4 = read_char(NDARRAY_DTYPE_BOOL, 0)
+NDARRAY_DTYPE_DT64_ID: cython.Py_UCS4 = read_char(NDARRAY_DTYPE_DT64, 0)
+NDARRAY_DTYPE_TD64_ID: cython.Py_UCS4 = read_char(NDARRAY_DTYPE_TD64, 0)
+NDARRAY_DTYPE_COMPLEX_ID: cython.Py_UCS4 = read_char(NDARRAY_DTYPE_COMPLEX, 0)
+NDARRAY_DTYPE_BYTES_ID: cython.Py_UCS4 = read_char(NDARRAY_DTYPE_BYTES, 0)
+NDARRAY_DTYPE_UNICODE_ID: cython.Py_UCS4 = read_char(NDARRAY_DTYPE_UNICODE, 0)
 # . variant dtype
 NDARRAY_DTYPE_DT64_Y: str = NDARRAY_DTYPE_DT64 + "Y"  # 'MY'
 NDARRAY_DTYPE_DT64_M: str = NDARRAY_DTYPE_DT64 + "M"  # 'MM'
 NDARRAY_DTYPE_DT64_W: str = NDARRAY_DTYPE_DT64 + "W"  # 'MW'
 NDARRAY_DTYPE_DT64_D: str = NDARRAY_DTYPE_DT64 + "D"  # 'MD'
 NDARRAY_DTYPE_DT64_B: str = NDARRAY_DTYPE_DT64 + "B"  # 'MB'
 NDARRAY_DTYPE_DT64_H: str = NDARRAY_DTYPE_DT64 + "h"  # 'Mh'
@@ -161,35 +161,35 @@
 NDARRAY_BYTES: str = NDARRAY + NDARRAY_DTYPE_BYTES  # 'NS'
 NDARRAY_UNICODE: str = NDARRAY + NDARRAY_DTYPE_UNICODE  # 'NU'
 
 # Pandas Types ----------------------------------------------------------------------
 DATETIMEINDEX: str = "Z"
 TIMEDELTAINDEX: str = "X"
 # . identifier
-DATETIMEINDEX_ID: cython.Py_UCS4 = str_loc(DATETIMEINDEX, 0)
-TIMEDELTAINDEX_ID: cython.Py_UCS4 = str_loc(TIMEDELTAINDEX, 0)
+DATETIMEINDEX_ID: cython.Py_UCS4 = read_char(DATETIMEINDEX, 0)
+TIMEDELTAINDEX_ID: cython.Py_UCS4 = read_char(TIMEDELTAINDEX, 0)
 
 # Pandas.Series ---------------------------------------------------------------------
 SERIES: str = "I"
 # . identifier
-SERIES_ID: cython.Py_UCS4 = str_loc(SERIES, 0)
+SERIES_ID: cython.Py_UCS4 = read_char(SERIES, 0)
 # . variant
 SERIES_OBJECT: str = SERIES + NDARRAY_DTYPE_OBJECT  # 'IO'
 SERIES_FLOAT: str = SERIES + NDARRAY_DTYPE_FLOAT  # 'If'
 SERIES_INT: str = SERIES + NDARRAY_DTYPE_INT  # 'Ii'
 SERIES_UINT: str = SERIES + NDARRAY_DTYPE_UINT  # 'Iu'
 SERIES_BOOL: str = SERIES + NDARRAY_DTYPE_BOOL  # 'Ib'
 SERIES_COMPLEX: str = SERIES + NDARRAY_DTYPE_COMPLEX  # 'Ic'
 SERIES_BYTES: str = SERIES + NDARRAY_DTYPE_BYTES  # 'IS'
 SERIES_UNICODE: str = SERIES + NDARRAY_DTYPE_UNICODE  # 'IU'
 
 # Pandas.DataFrame ------------------------------------------------------------------
 DATAFRAME: str = "F"
 # . identifier
-DATAFRAME_ID: cython.Py_UCS4 = str_loc(DATAFRAME, 0)
+DATAFRAME_ID: cython.Py_UCS4 = read_char(DATAFRAME, 0)
 # . variant
 DATAFRAME_COL_OBJECT: str = NDARRAY_DTYPE_OBJECT  # 'O'
 DATAFRAME_COL_FLOAT: str = NDARRAY_DTYPE_FLOAT  # 'f'
 DATAFRAME_COL_INT: str = NDARRAY_DTYPE_INT  # 'i'
 DATAFRAME_COL_UINT: str = NDARRAY_DTYPE_UINT  # 'u'
 DATAFRAME_COL_BOOL: str = NDARRAY_DTYPE_BOOL  # 'b'
 DATAFRAME_COL_COMPLEX: str = NDARRAY_DTYPE_COMPLEX  # 'c'
```

### Comparing `serializor-1.0.0/src/serializor/serialize.c` & `serializor-1.0.1/src/serializor/serialize.c`

 * *Files 1% similar despite different names*

```diff
@@ -6,25 +6,25 @@
         "define_macros": [
             [
                 "NPY_NO_DEPRECATED_API",
                 "NPY_1_7_API_VERSION"
             ]
         ],
         "depends": [
-            "/tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "/tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "/tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "/tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/core/include/numpy/ufuncobject.h"
+            "/tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/core/include/numpy/ufuncobject.h"
         ],
         "extra_compile_args": [
             "-Wno-unreachable-code"
         ],
         "include_dirs": [
-            "/tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/core/include"
+            "/tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/core/include"
         ],
         "name": "serializor.serialize",
         "sources": [
             "src/serializor/serialize.py"
         ]
     },
     "module_name": "serializor.serialize"
@@ -1616,177 +1616,177 @@
 /* ForceInitThreads.proto */
 #ifndef __PYX_FORCE_INIT_THREADS
   #define __PYX_FORCE_INIT_THREADS 0
 #endif
 
 /* #### Code section: numeric_typedefs ### */
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":730
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":730
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":731
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":731
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":732
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":732
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":733
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":733
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":737
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":737
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":738
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":738
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":739
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":739
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":740
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":740
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":744
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":744
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":745
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":745
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":754
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":754
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":755
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":755
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":757
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":757
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":758
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":758
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":760
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":760
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":761
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":761
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":763
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":763
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":764
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":764
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":765
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":765
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1841,42 +1841,42 @@
  *     or the provided default value if no such value was found.
  */
 struct __pyx_opt_args_7cpython_11contextvars_get_value_no_default {
   int __pyx_n;
   PyObject *default_value;
 };
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":767
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":767
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":768
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":768
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":769
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":769
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":771
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":771
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -4410,261 +4410,261 @@
 #define __pyx_tuple__13 __pyx_mstate_global->__pyx_tuple__13
 #define __pyx_tuple__14 __pyx_mstate_global->__pyx_tuple__14
 #define __pyx_tuple__15 __pyx_mstate_global->__pyx_tuple__15
 #define __pyx_tuple__17 __pyx_mstate_global->__pyx_tuple__17
 #define __pyx_codeobj__18 __pyx_mstate_global->__pyx_codeobj__18
 /* #### Code section: module_code ### */
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":245
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_7ndarray_4base_base(PyArrayObject *__pyx_v_self) {
   PyObject *__pyx_r;
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":248
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":248
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  *             return PyArray_BASE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_BASE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":245
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":245
  * 
  *         @property
  *         cdef inline PyObject* base(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a borrowed reference to the object owning the data/memory.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":251
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
 static CYTHON_INLINE PyArray_Descr *__pyx_f_5numpy_7ndarray_5descr_descr(PyArrayObject *__pyx_v_self) {
   PyArray_Descr *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   PyArray_Descr *__pyx_t_1;
   __Pyx_RefNannySetupContext("descr", 1);
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":254
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":254
  *             """Returns an owned reference to the dtype of the array.
  *             """
  *             return <dtype>PyArray_DESCR(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __Pyx_XDECREF((PyObject *)__pyx_r);
   __pyx_t_1 = PyArray_DESCR(__pyx_v_self);
   __Pyx_INCREF((PyObject *)((PyArray_Descr *)__pyx_t_1));
   __pyx_r = ((PyArray_Descr *)__pyx_t_1);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":251
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":251
  * 
  *         @property
  *         cdef inline dtype descr(self):             # <<<<<<<<<<<<<<
  *             """Returns an owned reference to the dtype of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF((PyObject *)__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":257
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_7ndarray_4ndim_ndim(PyArrayObject *__pyx_v_self) {
   int __pyx_r;
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":260
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":260
  *             """Returns the number of dimensions in the array.
  *             """
  *             return PyArray_NDIM(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_NDIM(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":257
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":257
  * 
  *         @property
  *         cdef inline int ndim(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the number of dimensions in the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":263
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_5shape_shape(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":268
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":268
  *             Can return NULL for 0-dimensional arrays.
  *             """
  *             return PyArray_DIMS(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_DIMS(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":263
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":263
  * 
  *         @property
  *         cdef inline npy_intp *shape(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the dimensions/shape of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":271
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
 static CYTHON_INLINE npy_intp *__pyx_f_5numpy_7ndarray_7strides_strides(PyArrayObject *__pyx_v_self) {
   npy_intp *__pyx_r;
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":275
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":275
  *             The number of elements matches the number of dimensions of the array (ndim).
  *             """
  *             return PyArray_STRIDES(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_STRIDES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":271
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":271
  * 
  *         @property
  *         cdef inline npy_intp *strides(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns a pointer to the strides of the array.
  *             The number of elements matches the number of dimensions of the array (ndim).
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":278
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
 static CYTHON_INLINE npy_intp __pyx_f_5numpy_7ndarray_4size_size(PyArrayObject *__pyx_v_self) {
   npy_intp __pyx_r;
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":281
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":281
  *             """Returns the total size (in number of elements) of the array.
  *             """
  *             return PyArray_SIZE(self)             # <<<<<<<<<<<<<<
  * 
  *         @property
  */
   __pyx_r = PyArray_SIZE(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":278
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":278
  * 
  *         @property
  *         cdef inline npy_intp size(self) nogil:             # <<<<<<<<<<<<<<
  *             """Returns the total size (in number of elements) of the array.
  *             """
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":284
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
 static CYTHON_INLINE char *__pyx_f_5numpy_7ndarray_4data_data(PyArrayObject *__pyx_v_self) {
   char *__pyx_r;
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":290
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":290
  *             of `PyArray_DATA()` instead, which returns a 'void*'.
  *             """
  *             return PyArray_BYTES(self)             # <<<<<<<<<<<<<<
  * 
  *     ctypedef unsigned char      npy_bool
  */
   __pyx_r = PyArray_BYTES(__pyx_v_self);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":284
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":284
  * 
  *         @property
  *         cdef inline char* data(self) nogil:             # <<<<<<<<<<<<<<
  *             """The pointer to the data buffer as a char*.
  *             This is provided for legacy reasons to avoid direct struct field access.
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":773
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -4673,29 +4673,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 1);
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":774
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":774
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 774, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":773
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":773
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -4706,15 +4706,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":776
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":776
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -4723,29 +4723,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 1);
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":777
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":777
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 777, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":776
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":776
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -4756,15 +4756,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":779
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -4773,29 +4773,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 1);
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":780
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":780
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 780, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":779
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":779
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -4806,15 +4806,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":782
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -4823,29 +4823,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 1);
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":783
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":783
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 783, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":782
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":782
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -4856,15 +4856,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":785
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -4873,29 +4873,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 1);
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":786
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":786
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 786, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":785
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":785
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -4906,217 +4906,217 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":788
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 1);
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":789
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = PyDataType_HASSUBARRAY(__pyx_v_d);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":790
+    /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":790
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":789
+    /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":789
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":792
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":792
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":788
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":788
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":968
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":968
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   int __pyx_t_1;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":969
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":969
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":970
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":970
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   __pyx_t_1 = PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base); if (unlikely(__pyx_t_1 == ((int)-1))) __PYX_ERR(1, 970, __pyx_L1_error)
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":968
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":968
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   goto __pyx_L0;
   __pyx_L1_error:;
   __Pyx_AddTraceback("numpy.set_array_base", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_L0:;
 }
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":972
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":972
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 1);
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":973
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":973
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":974
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":974
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = (__pyx_v_base == NULL);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":975
+    /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":975
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":974
+    /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":974
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":976
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":976
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":972
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":972
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":980
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":980
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -5132,15 +5132,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 1);
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":981
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -5148,68 +5148,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":982
+      /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":982
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 982, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":981
+      /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":983
+    /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":983
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 983, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":984
+      /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":984
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple_, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 984, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 984, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":981
+    /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":981
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -5217,15 +5217,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":980
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":980
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -5240,15 +5240,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":986
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":986
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -5264,15 +5264,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 1);
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":987
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -5280,68 +5280,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":988
+      /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":988
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 988, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":987
+      /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":989
+    /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":989
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 989, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":990
+      /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":990
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 990, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 990, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":987
+    /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":987
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -5349,15 +5349,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":986
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":986
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -5372,15 +5372,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":992
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":992
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -5396,15 +5396,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 1);
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":993
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -5412,68 +5412,68 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":994
+      /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":994
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 994, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":993
+      /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":995
+    /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":995
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 995, __pyx_L5_except_error)
       __Pyx_XGOTREF(__pyx_t_5);
       __Pyx_XGOTREF(__pyx_t_6);
       __Pyx_XGOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":996
+      /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":996
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * 
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 996, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_8);
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 996, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
 
-    /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":993
+    /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":993
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __pyx_L5_except_error:;
@@ -5481,15 +5481,15 @@
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":992
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":992
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -5504,170 +5504,170 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":999
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":999
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1011
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1011
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":999
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":999
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1014
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1014
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1026
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1026
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1014
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1014
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1029
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1029
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1036
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1036
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1029
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1029
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1039
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1039
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1043
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1043
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1039
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1039
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1046
+/* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1046
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1050
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1050
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1046
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":1046
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -13034,15 +13034,15 @@
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("_serialize_ndarray", 0);
   __Pyx_INCREF((PyObject *)__pyx_v_obj);
 
   /* "serializor/serialize.py":675
  *     """
  *     # Get ndarray dtype
- *     dtype: cython.Py_UCS4 = str_loc(obj.dtype.kind, 0)             # <<<<<<<<<<<<<<
+ *     dtype: cython.Py_UCS4 = read_char(obj.dtype.kind, 0)             # <<<<<<<<<<<<<<
  * 
  *     # Get ndarray dimensions
  */
   __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_obj), __pyx_n_s_dtype); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 675, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_kind); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 675, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
@@ -19826,15 +19826,15 @@
   if (!(likely(((__pyx_t_1) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_1, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 1347, __pyx_L1_error)
   __pyx_v_values = ((PyArrayObject *)__pyx_t_1);
   __pyx_t_1 = 0;
 
   /* "serializor/serialize.py":1350
  * 
  *     # Get Series dtype
- *     dtype: cython.Py_UCS4 = str_loc(values.dtype.kind, 0)             # <<<<<<<<<<<<<<
+ *     dtype: cython.Py_UCS4 = read_char(values.dtype.kind, 0)             # <<<<<<<<<<<<<<
  * 
  *     # Get Series size
  */
   __pyx_t_1 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_values), __pyx_n_s_dtype); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1350, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_t_2 = __Pyx_PyObject_GetAttrStr(__pyx_t_1, __pyx_n_s_kind); if (unlikely(!__pyx_t_2)) __PYX_ERR(0, 1350, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_2);
@@ -21445,39 +21445,39 @@
     __pyx_t_3 = 0;
 
     /* "serializor/serialize.py":1611
  *     for _, col in obj.items():
  *         # . access column (Series) values
  *         values: np.ndarray = col.values             # <<<<<<<<<<<<<<
  *         # . get column (Series) dtype
- *         dtype: cython.Py_UCS4 = str_loc(values.dtype.kind, 0)
+ *         dtype: cython.Py_UCS4 = read_char(values.dtype.kind, 0)
  */
     __pyx_t_3 = __Pyx_PyObject_GetAttrStr(__pyx_v_col, __pyx_n_s_values); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1611, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     if (!(likely(((__pyx_t_3) == Py_None) || likely(__Pyx_TypeTest(__pyx_t_3, __pyx_ptype_5numpy_ndarray))))) __PYX_ERR(0, 1611, __pyx_L1_error)
     __Pyx_XDECREF_SET(__pyx_v_values, ((PyArrayObject *)__pyx_t_3));
     __pyx_t_3 = 0;
 
     /* "serializor/serialize.py":1613
  *         values: np.ndarray = col.values
  *         # . get column (Series) dtype
- *         dtype: cython.Py_UCS4 = str_loc(values.dtype.kind, 0)             # <<<<<<<<<<<<<<
+ *         dtype: cython.Py_UCS4 = read_char(values.dtype.kind, 0)             # <<<<<<<<<<<<<<
  *         # . `<object>`
  *         if dtype == prefix.NDARRAY_DTYPE_OBJECT_ID:
  */
     __pyx_t_3 = __Pyx_PyObject_GetAttrStr(((PyObject *)__pyx_v_values), __pyx_n_s_dtype); if (unlikely(!__pyx_t_3)) __PYX_ERR(0, 1613, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_3);
     __pyx_t_4 = __Pyx_PyObject_GetAttrStr(__pyx_t_3, __pyx_n_s_kind); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1613, __pyx_L1_error)
     __Pyx_GOTREF(__pyx_t_4);
     __Pyx_DECREF(__pyx_t_3); __pyx_t_3 = 0;
     __pyx_v_dtype = PyUnicode_READ_CHAR(__pyx_t_4, 0);
     __Pyx_DECREF(__pyx_t_4); __pyx_t_4 = 0;
 
     /* "serializor/serialize.py":1615
- *         dtype: cython.Py_UCS4 = str_loc(values.dtype.kind, 0)
+ *         dtype: cython.Py_UCS4 = read_char(values.dtype.kind, 0)
  *         # . `<object>`
  *         if dtype == prefix.NDARRAY_DTYPE_OBJECT_ID:             # <<<<<<<<<<<<<<
  *             val = _serialize_dataframe_object(values, rows)
  *         # . `<float>`
  */
     __pyx_t_6 = (__pyx_v_dtype == __pyx_v_10serializor_6prefix_NDARRAY_DTYPE_OBJECT_ID);
     if (__pyx_t_6) {
@@ -21491,15 +21491,15 @@
  */
       __pyx_t_4 = __pyx_f_10serializor_9serialize__serialize_dataframe_object(__pyx_v_values, __pyx_v_rows); if (unlikely(!__pyx_t_4)) __PYX_ERR(0, 1616, __pyx_L1_error)
       __Pyx_GOTREF(__pyx_t_4);
       __Pyx_XDECREF_SET(__pyx_v_val, ((PyObject*)__pyx_t_4));
       __pyx_t_4 = 0;
 
       /* "serializor/serialize.py":1615
- *         dtype: cython.Py_UCS4 = str_loc(values.dtype.kind, 0)
+ *         dtype: cython.Py_UCS4 = read_char(values.dtype.kind, 0)
  *         # . `<object>`
  *         if dtype == prefix.NDARRAY_DTYPE_OBJECT_ID:             # <<<<<<<<<<<<<<
  *             val = _serialize_dataframe_object(values, rows)
  *         # . `<float>`
  */
       goto __pyx_L7;
     }
@@ -25509,26 +25509,26 @@
 }
 /* #### Code section: cached_constants ### */
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":984
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":984
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple_ = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple_)) __PYX_ERR(1, 984, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple_);
   __Pyx_GIVEREF(__pyx_tuple_);
 
-  /* "../../../../../tmp/build-env-wv23z7az/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":990
+  /* "../../../../../tmp/build-env-i853fefs/lib/python3.12/site-packages/numpy/__init__.cython-30.pxd":990
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 990, __pyx_L1_error)
```

### Comparing `serializor-1.0.0/src/serializor/serialize.pxd` & `serializor-1.0.1/src/serializor/serialize.pxd`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -67,8 +67,8 @@
     return PyArray_SETITEM(arr, itemptr, item)
 
 cdef inline int ndarray_setitem_4d(np.ndarray arr, np.npy_intp i, np.npy_intp j, np.npy_intp k, np.npy_intp l, object item):
     cdef void* itemptr = <void*>PyArray_GETPTR4(arr, i, j, k, l)
     return PyArray_SETITEM(arr, itemptr, item)
 
 # Serialize
-cdef str capi_serialize(object obj)
+cdef str capi_serialize(object obj)
```

### Comparing `serializor-1.0.0/src/serializor/serialize.py` & `serializor-1.0.1/src/serializor/serialize.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # cython: boundscheck=False
 
 # Cython imports
 import cython
 from cython.cimports import numpy as np  # type: ignore
 from cython.cimports.cpython import datetime  # type: ignore
 from cython.cimports.libc.math import isnormal  # type: ignore
-from cython.cimports.cpython.unicode import PyUnicode_READ_CHAR as str_loc  # type: ignore
+from cython.cimports.cpython.unicode import PyUnicode_READ_CHAR as read_char  # type: ignore
 from cython.cimports.cpython.unicode import PyUnicode_GET_LENGTH as str_len  # type: ignore
 from cython.cimports.cpython.unicode import PyUnicode_Substring as str_substr  # type: ignore
 from cython.cimports.cpython.set import PySet_GET_SIZE as set_len  # type: ignore
 from cython.cimports.cpython.list import PyList_GET_SIZE as list_len  # type: ignore
 from cython.cimports.cpython.tuple import PyTuple_GET_SIZE as tuple_len  # type: ignore
 from cython.cimports.cpython.dict import PyDict_Keys as dict_getkeys  # type: ignore
 from cython.cimports.cpython.dict import PyDict_Values as dict_getvals  # type: ignore
@@ -668,15 +668,15 @@
          to serialize items as an 1-dimensional json array for maximum
          performance.
     - 5. For dtype of 'object', items are serialized one by one, similar
          to the serialization process of a list. For more detail, please
          refer to the `_serialize_ndarray_object()` function.
     """
     # Get ndarray dtype
-    dtype: cython.Py_UCS4 = str_loc(obj.dtype.kind, 0)
+    dtype: cython.Py_UCS4 = read_char(obj.dtype.kind, 0)
 
     # Get ndarray dimensions
     ndim: cython.Py_ssize_t = obj.ndim
     if ndim == 0:
         raise errors.SerializeTypeError(
             "<Serializor> Can't not serialize 0-dimensional `<ndarray>`."
         )
@@ -1343,15 +1343,15 @@
          to the serialization process of a list. For more details, please
          refer to the `_serialize_series_object()` function.
     """
     # Access Series values
     values: np.ndarray = obj.values
 
     # Get Series dtype
-    dtype: cython.Py_UCS4 = str_loc(values.dtype.kind, 0)
+    dtype: cython.Py_UCS4 = read_char(values.dtype.kind, 0)
 
     # Get Series size
     size: cython.Py_ssize_t = values.shape[0]
 
     # Serialize Series
     # . Series[object]
     if dtype == prefix.NDARRAY_DTYPE_OBJECT_ID:
@@ -1606,15 +1606,15 @@
 
     # Serialize DataFrame
     vals: list = []
     for _, col in obj.items():
         # . access column (Series) values
         values: np.ndarray = col.values
         # . get column (Series) dtype
-        dtype: cython.Py_UCS4 = str_loc(values.dtype.kind, 0)
+        dtype: cython.Py_UCS4 = read_char(values.dtype.kind, 0)
         # . `<object>`
         if dtype == prefix.NDARRAY_DTYPE_OBJECT_ID:
             val = _serialize_dataframe_object(values, rows)
         # . `<float>`
         elif dtype == prefix.NDARRAY_DTYPE_FLOAT_ID:
             if np.PyArray_TYPE(values) == np.NPY_FLOAT16:
                 values = np.PyArray_Cast(values, np.NPY_FLOAT32)
```

### Comparing `serializor-1.0.0/src/serializor/typeref.c` & `serializor-1.0.1/src/serializor/typeref.c`

 * *Files identical despite different names*

### Comparing `serializor-1.0.0/src/serializor/typeref.pxd` & `serializor-1.0.1/src/serializor/typeref.pxd`

 * *Files identical despite different names*

### Comparing `serializor-1.0.0/src/serializor/typeref.py` & `serializor-1.0.1/src/serializor/typeref.py`

 * *Files identical despite different names*

### Comparing `serializor-1.0.0/src/serializor.egg-info/PKG-INFO` & `serializor-1.0.1/src/serializor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: serializor
-Version: 1.0.0
+Version: 1.0.1
 Summary: Serialization for common Python objects.
 Home-page: https://github.com/AresJef/Serializor
 Author: Jiefu Chen
 Author-email: keppa1991@163.com
 License: MIT license, Apache License 2.0
 Keywords: serialize,serialization,numpy,pandas,python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `serializor-1.0.0/src/serializor.egg-info/SOURCES.txt` & `serializor-1.0.1/src/serializor.egg-info/SOURCES.txt`

 * *Files identical despite different names*

