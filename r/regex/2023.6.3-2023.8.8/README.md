# Comparing `tmp/regex-2023.6.3.tar.gz` & `tmp/regex-2023.8.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "regex-2023.6.3.tar", last modified: Sat Jun  3 17:05:03 2023, max compression
+gzip compressed data, was "regex-2023.8.8.tar", last modified: Tue Aug  8 20:38:00 2023, max compression
```

## Comparing `regex-2023.6.3.tar` & `regex-2023.8.8.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 17:05:03.085785 regex-2023.6.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11584 2023-06-03 17:05:01.000000 regex-2023.6.3/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-06-03 17:05:01.000000 regex-2023.6.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    40894 2023-06-03 17:05:03.081785 regex-2023.6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    39805 2023-06-03 17:05:01.000000 regex-2023.6.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 17:05:03.077785 regex-2023.6.3/docs/
--rw-r--r--   0 runner    (1001) docker     (123)   143294 2023-06-03 17:05:01.000000 regex-2023.6.3/docs/Features.html
--rw-r--r--   0 runner    (1001) docker     (123)    29426 2023-06-03 17:05:01.000000 regex-2023.6.3/docs/UnicodeProperties.rst
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-06-03 17:05:01.000000 regex-2023.6.3/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 17:05:03.081785 regex-2023.6.3/regex.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    40894 2023-06-03 17:05:02.000000 regex-2023.6.3/regex.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      415 2023-06-03 17:05:03.000000 regex-2023.6.3/regex.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-03 17:05:02.000000 regex-2023.6.3/regex.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-06-03 17:05:02.000000 regex-2023.6.3/regex.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 17:05:03.081785 regex-2023.6.3/regex_3/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-06-03 17:05:01.000000 regex-2023.6.3/regex_3/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   825160 2023-06-03 17:05:01.000000 regex-2023.6.3/regex_3/_regex.c
--rw-r--r--   0 runner    (1001) docker     (123)     6328 2023-06-03 17:05:01.000000 regex-2023.6.3/regex_3/_regex.h
--rw-r--r--   0 runner    (1001) docker     (123)   141150 2023-06-03 17:05:01.000000 regex-2023.6.3/regex_3/_regex_core.py
--rw-r--r--   0 runner    (1001) docker     (123)  1837887 2023-06-03 17:05:01.000000 regex-2023.6.3/regex_3/_regex_unicode.c
--rw-r--r--   0 runner    (1001) docker     (123)    10655 2023-06-03 17:05:01.000000 regex-2023.6.3/regex_3/_regex_unicode.h
--rw-r--r--   0 runner    (1001) docker     (123)    32811 2023-06-03 17:05:01.000000 regex-2023.6.3/regex_3/regex.py
--rw-r--r--   0 runner    (1001) docker     (123)   219948 2023-06-03 17:05:01.000000 regex-2023.6.3/regex_3/test_regex.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-03 17:05:03.085785 regex-2023.6.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-06-03 17:05:01.000000 regex-2023.6.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-03 17:05:03.081785 regex-2023.6.3/tools/
--rw-r--r--   0 runner    (1001) docker     (123)    55247 2023-06-03 17:05:01.000000 regex-2023.6.3/tools/build_regex_unicode.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:38:00.256177 regex-2023.8.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    11584 2023-08-08 20:37:59.000000 regex-2023.8.8/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-08-08 20:37:59.000000 regex-2023.8.8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    40945 2023-08-08 20:38:00.256177 regex-2023.8.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    39805 2023-08-08 20:37:59.000000 regex-2023.8.8/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:38:00.248177 regex-2023.8.8/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)   143294 2023-08-08 20:37:59.000000 regex-2023.8.8/docs/Features.html
+-rw-r--r--   0 runner    (1001) docker     (123)    29426 2023-08-08 20:37:59.000000 regex-2023.8.8/docs/UnicodeProperties.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-08-08 20:37:59.000000 regex-2023.8.8/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:38:00.248177 regex-2023.8.8/regex.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    40945 2023-08-08 20:38:00.000000 regex-2023.8.8/regex.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      415 2023-08-08 20:38:00.000000 regex-2023.8.8/regex.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-08-08 20:38:00.000000 regex-2023.8.8/regex.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-08-08 20:38:00.000000 regex-2023.8.8/regex.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:38:00.252177 regex-2023.8.8/regex_3/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-08-08 20:37:59.000000 regex-2023.8.8/regex_3/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   826026 2023-08-08 20:37:59.000000 regex-2023.8.8/regex_3/_regex.c
+-rw-r--r--   0 runner    (1001) docker     (123)     6328 2023-08-08 20:37:59.000000 regex-2023.8.8/regex_3/_regex.h
+-rw-r--r--   0 runner    (1001) docker     (123)   141166 2023-08-08 20:37:59.000000 regex-2023.8.8/regex_3/_regex_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)  1837887 2023-08-08 20:37:59.000000 regex-2023.8.8/regex_3/_regex_unicode.c
+-rw-r--r--   0 runner    (1001) docker     (123)    10655 2023-08-08 20:37:59.000000 regex-2023.8.8/regex_3/_regex_unicode.h
+-rw-r--r--   0 runner    (1001) docker     (123)    32811 2023-08-08 20:37:59.000000 regex-2023.8.8/regex_3/regex.py
+-rw-r--r--   0 runner    (1001) docker     (123)   220168 2023-08-08 20:37:59.000000 regex-2023.8.8/regex_3/test_regex.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-08-08 20:38:00.256177 regex-2023.8.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-08-08 20:37:59.000000 regex-2023.8.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-08-08 20:38:00.252177 regex-2023.8.8/tools/
+-rw-r--r--   0 runner    (1001) docker     (123)    55247 2023-08-08 20:37:59.000000 regex-2023.8.8/tools/build_regex_unicode.py
```

### Comparing `regex-2023.6.3/LICENSE.txt` & `regex-2023.8.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `regex-2023.6.3/PKG-INFO` & `regex-2023.8.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: regex
-Version: 2023.6.3
+Version: 2023.8.8
 Summary: Alternative regular expression module, to replace re.
 Home-page: https://github.com/mrabarnett/mrab-regex
 Author: Matthew Barnett
 Author-email: regex@mrabarnett.plus.com
 License: Apache Software License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -12,14 +12,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Text Processing
 Classifier: Topic :: Text Processing :: General
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
```

### Comparing `regex-2023.6.3/README.rst` & `regex-2023.8.8/README.rst`

 * *Files identical despite different names*

### Comparing `regex-2023.6.3/docs/Features.html` & `regex-2023.8.8/docs/Features.html`

 * *Files identical despite different names*

### Comparing `regex-2023.6.3/docs/UnicodeProperties.rst` & `regex-2023.8.8/docs/UnicodeProperties.rst`

 * *Files identical despite different names*

### Comparing `regex-2023.6.3/regex.egg-info/PKG-INFO` & `regex-2023.8.8/regex.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: regex
-Version: 2023.6.3
+Version: 2023.8.8
 Summary: Alternative regular expression module, to replace re.
 Home-page: https://github.com/mrabarnett/mrab-regex
 Author: Matthew Barnett
 Author-email: regex@mrabarnett.plus.com
 License: Apache Software License
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
@@ -12,14 +12,15 @@
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Text Processing
 Classifier: Topic :: Text Processing :: General
 Requires-Python: >=3.6
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
```

### Comparing `regex-2023.6.3/regex_3/_regex.c` & `regex-2023.8.8/regex_3/_regex.c`

 * *Files 0% similar despite different names*

```diff
@@ -18702,16 +18702,16 @@
         if (!result)
             return NULL;
 
         item = Py_BuildValue("n", self->match_start);
         if (!item)
             goto error;
 
-        /* PyList_SET_ITEM borrows the reference. */
-        PyList_SET_ITEM(result, 0, item);
+        /* PyList_SetItem borrows the reference. */
+        PyList_SetItem(result, 0, item);
 
         return result;
     }
 
     /* Capture group indexes are 1-based (excluding group 0, which is the
      * entire matched string).
      */
@@ -18722,16 +18722,16 @@
         return NULL;
 
     for (i = 0; i < group->count; i++) {
         item = Py_BuildValue("n", group->captures[i].start);
         if (!item)
             goto error;
 
-        /* PyList_SET_ITEM borrows the reference. */
-        PyList_SET_ITEM(result, i, item);
+        /* PyList_SetItem borrows the reference. */
+        PyList_SetItem(result, i, item);
     }
 
     return result;
 
 error:
     Py_DECREF(result);
     return NULL;
@@ -18782,16 +18782,16 @@
         if (!result)
             return NULL;
 
         item = Py_BuildValue("n", self->match_end);
         if (!item)
             goto error;
 
-        /* PyList_SET_ITEM borrows the reference. */
-        PyList_SET_ITEM(result, 0, item);
+        /* PyList_SetItem borrows the reference. */
+        PyList_SetItem(result, 0, item);
 
         return result;
     }
 
     /* Capture group indexes are 1-based (excluding group 0, which is the
      * entire matched string).
      */
@@ -18802,16 +18802,16 @@
         return NULL;
 
     for (i = 0; i < group->count; i++) {
         item = Py_BuildValue("n", group->captures[i].end);
         if (!item)
             goto error;
 
-        /* PyList_SET_ITEM borrows the reference. */
-        PyList_SET_ITEM(result, i, item);
+        /* PyList_SetItem borrows the reference. */
+        PyList_SetItem(result, i, item);
     }
 
     return result;
 
 error:
     Py_DECREF(result);
     return NULL;
@@ -18863,16 +18863,16 @@
         if (!result)
             return NULL;
 
         item = Py_BuildValue("nn", self->match_start, self->match_end);
         if (!item)
             goto error;
 
-        /* PyList_SET_ITEM borrows the reference. */
-        PyList_SET_ITEM(result, 0, item);
+        /* PyList_SetItem borrows the reference. */
+        PyList_SetItem(result, 0, item);
 
         return result;
     }
 
     /* Capture group indexes are 1-based (excluding group 0, which is the
      * entire matched string).
      */
@@ -18884,16 +18884,16 @@
 
     for (i = 0; i < group->count; i++) {
         item = Py_BuildValue("nn", group->captures[i].start,
           group->captures[i].end);
         if (!item)
             goto error;
 
-        /* PyList_SET_ITEM borrows the reference. */
-        PyList_SET_ITEM(result, i, item);
+        /* PyList_SetItem borrows the reference. */
+        PyList_SetItem(result, i, item);
     }
 
     return result;
 
 error:
     Py_DECREF(result);
     return NULL;
@@ -18919,16 +18919,16 @@
             return NULL;
 
         slice = get_slice(self->substring, self->match_start -
           self->substring_offset, self->match_end - self->substring_offset);
         if (!slice)
             goto error;
 
-        /* PyList_SET_ITEM borrows the reference. */
-        PyList_SET_ITEM(result, 0, slice);
+        /* PyList_SetItem borrows the reference. */
+        PyList_SetItem(result, 0, slice);
 
         return result;
     }
 
     /* Capture group indexes are 1-based (excluding group 0, which is the
      * entire matched string).
      */
@@ -18941,16 +18941,16 @@
     for (i = 0; i < group->count; i++) {
         slice = get_slice(self->substring, group->captures[i].start -
           self->substring_offset, group->captures[i].end -
           self->substring_offset);
         if (!slice)
             goto error;
 
-        /* PyList_SET_ITEM borrows the reference. */
-        PyList_SET_ITEM(result, i, slice);
+        /* PyList_SetItem borrows the reference. */
+        PyList_SetItem(result, i, slice);
     }
 
     return result;
 
 error:
     Py_DECREF(result);
     return NULL;
@@ -19278,21 +19278,21 @@
     if (!result || !self->pattern->groupindex)
         return result;
 
     keys = PyMapping_Keys(self->pattern->groupindex);
     if (!keys)
         goto failed;
 
-    for (g = 0; g < PyList_GET_SIZE(keys); g++) {
+    for (g = 0; g < PyList_Size(keys); g++) {
         PyObject* key;
         PyObject* value;
         int status;
 
-        /* PyList_GET_ITEM borrows a reference. */
-        key = PyList_GET_ITEM(keys, g);
+        /* PyList_GetItem borrows a reference. */
+        key = PyList_GetItem(keys, g);
         if (!key)
             goto failed;
 
         value = match_get_group(self, key, def, FALSE);
         if (!value)
             goto failed;
 
@@ -19322,22 +19322,22 @@
     if (!result || !self->pattern->groupindex)
         return result;
 
     keys = PyMapping_Keys(self->pattern->groupindex);
     if (!keys)
         goto failed;
 
-    for (g = 0; g < PyList_GET_SIZE(keys); g++) {
+    for (g = 0; g < PyList_Size(keys); g++) {
         PyObject* key;
         Py_ssize_t group;
         PyObject* captures;
         int status;
 
-        /* PyList_GET_ITEM borrows a reference. */
-        key = PyList_GET_ITEM(keys, g);
+        /* PyList_GetItem borrows a reference. */
+        key = PyList_GetItem(keys, g);
         if (!key)
             goto failed;
 
         group = match_get_group_index(self, key, FALSE);
         if (group < 0)
             goto failed;
 
@@ -19505,20 +19505,20 @@
     if (join_info->item) {
         join_info->list = PyList_New(2);
         if (!join_info->list) {
             status = RE_ERROR_MEMORY;
             goto error;
         }
 
-        /* PyList_SET_ITEM borrows the reference. */
-        PyList_SET_ITEM(join_info->list, 0, join_info->item);
+        /* PyList_SetItem borrows the reference. */
+        PyList_SetItem(join_info->list, 0, join_info->item);
         join_info->item = NULL;
 
-        /* PyList_SET_ITEM borrows the reference. */
-        PyList_SET_ITEM(join_info->list, 1, new_item);
+        /* PyList_SetItem borrows the reference. */
+        PyList_SetItem(join_info->list, 1, new_item);
         return 0;
     }
 
     /* This is the first item. */
     join_info->item = new_item;
 
     return 0;
@@ -19531,46 +19531,86 @@
 
 /* Clears the join list. */
 Py_LOCAL_INLINE(void) clear_join_list(RE_JoinInfo* join_info) {
     Py_XDECREF(join_info->list);
     Py_XDECREF(join_info->item);
 }
 
+/* Joins a list of bytestrings. */
+Py_LOCAL_INLINE(PyObject*) join_bytestrings(PyObject* list) {
+    Py_ssize_t count;
+    Py_ssize_t length;
+    Py_ssize_t i;
+    PyObject *result;
+    char* to_bytes;
+
+    count = PyList_Size(list);
+
+    /* How long will the result be? */
+    length = 0;
+
+    for (i = 0; i < count; i++)
+        length += PyBytes_Size(PyList_GetItem(list, i));
+
+    /* Create the resulting bytestring, but uninitialised. */
+    result = PyBytes_FromStringAndSize(NULL, length);
+    if (!result)
+        return NULL;
+
+    /* Fill the resulting bytestring. */
+    to_bytes = PyBytes_AsString(result);
+    length = 0;
+
+    for (i = 0; i < count; i++) {
+        PyObject* bytestring;
+        char* from_bytes;
+        Py_ssize_t from_length;
+
+        bytestring = PyList_GetItem(list, i);
+        from_bytes = PyBytes_AsString(bytestring);
+        from_length = PyBytes_Size(bytestring);
+        memmove(to_bytes + length, from_bytes, from_length);
+        length += from_length;
+    }
+
+    return result;
+}
+
+/* Joins a list of strings. */
+Py_LOCAL_INLINE(PyObject*) join_strings(PyObject* list) {
+    PyObject* joiner;
+    PyObject* result;
+
+    joiner = PyUnicode_FromString("");
+    if (!joiner)
+        return NULL;
+
+    result = PyUnicode_Join(joiner, list);
+    Py_DECREF(joiner);
+
+    return result;
+}
+
 /* Joins together a list of strings for pattern_subx. */
 Py_LOCAL_INLINE(PyObject*) join_list_info(RE_JoinInfo* join_info) {
     /* If the list already exists then just do the join. */
     if (join_info->list) {
-        PyObject* joiner;
         PyObject* result;
 
         if (join_info->reversed)
             /* The list needs to be reversed before being joined. */
             PyList_Reverse(join_info->list);
 
-        if (join_info->is_unicode) {
+        if (join_info->is_unicode)
             /* Concatenate the Unicode strings. */
-            joiner = PyUnicode_New(0, 0);
-            if (!joiner) {
-                clear_join_list(join_info);
-                return NULL;
-            }
-
-            result = PyUnicode_Join(joiner, join_info->list);
-        } else {
-            joiner = PyBytes_FromString("");
-            if (!joiner) {
-                clear_join_list(join_info);
-                return NULL;
-            }
-
+            result = join_strings(join_info->list);
+        else
             /* Concatenate the bytestrings. */
-            result = _PyBytes_Join(joiner, join_info->list);
-        }
+            result = join_bytestrings(join_info->list);
 
-        Py_DECREF(joiner);
         clear_join_list(join_info);
 
         return result;
     }
 
     /* If we have only 1 item, so we'll just return it. */
     if (join_info->item)
@@ -19647,21 +19687,21 @@
       PyTuple_Pack(2, self->pattern, str_template));
     if (!replacement)
         return NULL;
 
     init_join_list(&join_info, FALSE, PyUnicode_Check(self->string));
 
     /* Add each part of the template to the list. */
-    size = PyList_GET_SIZE(replacement);
+    size = PyList_Size(replacement);
     for (i = 0; i < size; i++) {
         PyObject* item;
         PyObject* str_item;
 
-        /* PyList_GET_ITEM borrows a reference. */
-        item = PyList_GET_ITEM(replacement, i);
+        /* PyList_GetItem borrows a reference. */
+        item = PyList_GetItem(replacement, i);
         str_item = get_match_replacement(self, item, self->group_count);
         if (!str_item)
             goto error;
 
         /* Add to the list. */
         if (str_item == Py_None)
             Py_DECREF(str_item);
@@ -19723,27 +19763,27 @@
     if (!keys)
         goto failed;
 
     values = PyMapping_Values(match->pattern->groupindex);
     if (!values)
         goto failed;
 
-    for (g = 0; g < PyList_GET_SIZE(keys); g++) {
+    for (g = 0; g < PyList_Size(keys); g++) {
         PyObject* key;
         PyObject* value;
         Py_ssize_t v;
         int status;
 
-        /* PyList_GET_ITEM borrows a reference. */
-        key = PyList_GET_ITEM(keys, g);
+        /* PyList_GetItem borrows a reference. */
+        key = PyList_GetItem(keys, g);
         if (!key)
             goto failed;
 
-        /* PyList_GET_ITEM borrows a reference. */
-        value = PyList_GET_ITEM(values, g);
+        /* PyList_GetItem borrows a reference. */
+        value = PyList_GetItem(values, g);
         if (!value)
             goto failed;
 
         v = PyLong_AsLong(value);
         if (v == -1 && PyErr_Occurred())
             goto failed;
 
@@ -21738,15 +21778,15 @@
         } else if (is_template) {
             /* The replacement is a list template. */
             Py_ssize_t count;
             Py_ssize_t index;
             Py_ssize_t step;
 
             /* Add each part of the template to the list. */
-            count = PyList_GET_SIZE(replacement);
+            count = PyList_Size(replacement);
             if (join_info.reversed) {
                 /* We're searching backwards, so we'll be reversing the list
                  * when it's complete. Therefore, we need to add the items of
                  * the template in reverse order for them to be in the correct
                  * order after the reversal.
                  */
                 index = count - 1;
@@ -21757,16 +21797,16 @@
                 step = 1;
             }
 
             while (count > 0) {
                 PyObject* item;
                 PyObject* str_item;
 
-                /* PyList_GET_ITEM borrows a reference. */
-                item = PyList_GET_ITEM(replacement, index);
+                /* PyList_GetItem borrows a reference. */
+                item = PyList_GetItem(replacement, index);
                 str_item = get_sub_replacement(item, string, &state,
                   self->public_group_count);
                 if (!str_item)
                     goto error;
 
                 /* Add the result to the list. */
                 if (str_item == Py_None)
@@ -25715,30 +25755,30 @@
             return NULL;
 
         unpacked = TRUE;
     } else
         unpacked = FALSE;
 
     /* Read the regex code. */
-    code_len = PyList_GET_SIZE(code_list);
+    code_len = PyList_Size(code_list);
     code = (RE_CODE*)re_alloc((size_t)code_len * sizeof(RE_CODE));
     if (!code) {
         if (unpacked) {
             /* code_list has been built from a packed code list. */
             Py_DECREF(code_list);
         }
         return NULL;
     }
 
     for (i = 0; i < code_len; i++) {
         PyObject* o;
         size_t value;
 
-        /* PyList_GET_ITEM borrows a reference. */
-        o = PyList_GET_ITEM(code_list, i);
+        /* PyList_GetItem borrows a reference. */
+        o = PyList_GetItem(code_list, i);
 
         value = PyLong_AsUnsignedLong(o);
         if ((Py_ssize_t)value == -1 && PyErr_Occurred())
             goto error;
 
         code[i] = (RE_CODE)value;
         if (code[i] != value)
```

### Comparing `regex-2023.6.3/regex_3/_regex.h` & `regex-2023.8.8/regex_3/_regex.h`

 * *Files identical despite different names*

### Comparing `regex-2023.6.3/regex_3/_regex_core.py` & `regex-2023.8.8/regex_3/_regex_core.py`

 * *Files 0% similar despite different names*

```diff
@@ -2996,26 +2996,27 @@
 
     def has_simple_start(self):
         return self.subpattern.has_simple_start()
 
     def _compile(self, reverse, fuzzy):
         code = []
 
-        key = self.group, reverse, fuzzy
-        ref = self.info.call_refs.get(key)
-        if ref is not None:
-            code += [(OP.CALL_REF, ref)]
-
         public_group = private_group = self.group
         if private_group < 0:
             public_group = self.info.private_groups[private_group]
             private_group = self.info.group_count - private_group
 
-        code += ([(OP.GROUP, int(not reverse), private_group, public_group)] +
-          self.subpattern.compile(reverse, fuzzy) + [(OP.END, )])
+        key = self.group, reverse, fuzzy
+        ref = self.info.call_refs.get(key)
+        if ref is not None:
+            code += [(OP.CALL_REF, ref)]
+
+        code += [(OP.GROUP, int(not reverse), private_group, public_group)]
+        code += self.subpattern.compile(reverse, fuzzy)
+        code += [(OP.END, )]
 
         if ref is not None:
             code += [(OP.END, )]
 
         return code
 
     def dump(self, indent, reverse):
```

### Comparing `regex-2023.6.3/regex_3/_regex_unicode.c` & `regex-2023.8.8/regex_3/_regex_unicode.c`

 * *Files identical despite different names*

### Comparing `regex-2023.6.3/regex_3/_regex_unicode.h` & `regex-2023.8.8/regex_3/_regex_unicode.h`

 * *Files identical despite different names*

### Comparing `regex-2023.6.3/regex_3/regex.py` & `regex-2023.8.8/regex_3/regex.py`

 * *Files 0% similar despite different names*

```diff
@@ -237,15 +237,15 @@
   "sub", "subf", "subfn", "subn", "template", "Scanner", "A", "ASCII", "B",
   "BESTMATCH", "D", "DEBUG", "E", "ENHANCEMATCH", "S", "DOTALL", "F",
   "FULLCASE", "I", "IGNORECASE", "L", "LOCALE", "M", "MULTILINE", "P", "POSIX",
   "R", "REVERSE", "T", "TEMPLATE", "U", "UNICODE", "V0", "VERSION0", "V1",
   "VERSION1", "X", "VERBOSE", "W", "WORD", "error", "Regex", "__version__",
   "__doc__", "RegexFlag"]
 
-__version__ = "2.5.129"
+__version__ = "2.5.132"
 
 # --------------------------------------------------------------------
 # Public interface.
 
 def match(pattern, string, flags=0, pos=None, endpos=None, partial=False,
   concurrent=None, timeout=None, ignore_unused=False, **kwargs):
     """Try to apply the pattern at the start of the string, returning a match
```

### Comparing `regex-2023.6.3/regex_3/test_regex.py` & `regex-2023.8.8/regex_3/test_regex.py`

 * *Files 0% similar despite different names*

```diff
@@ -3285,15 +3285,15 @@
         self.assertEqual(regex.search(r"(?:fe)?male", "female").group(),
           "female")
         self.assertEqual([m.group() for m in
           regex.finditer(r"(fe)?male: h(?(1)(er)|(is)) (\w+)",
           "female: her dog; male: his cat. asdsasda")], ['female: her dog',
           'male: his cat'])
 
-        # Hg issue 78: "Captures"doesn't work for recursive calls
+        # Hg issue 78: "Captures" doesn't work for recursive calls
         self.assertEqual(regex.search(r'(?<rec>\((?:[^()]++|(?&rec))*\))',
           'aaa(((1+0)+1)+1)bbb').captures('rec'), ['(1+0)', '((1+0)+1)',
           '(((1+0)+1)+1)'])
 
         # Hg issue 80: Escape characters throws an exception
         self.assertRaisesRegex(regex.error, self.BAD_ESCAPE, lambda:
           regex.sub('x', '\\', 'x'), )
@@ -3620,14 +3620,17 @@
         self.assertEqual(regex.findall(r'(?r)(\w\w\K\w\w)', 'abcdefgh'),
           ['efgh', 'abcd'])
 
         # Hg issue 152: Request: Request: (?(DEFINE)...).
         self.assertEqual(regex.search(r'(?(DEFINE)(?<quant>\d+)(?<item>\w+))(?&quant) (?&item)',
           '5 elephants')[0], '5 elephants')
 
+        self.assertEqual(regex.search(r'(?&routine)(?(DEFINE)(?<routine>.))', 'a').group('routine'), None)
+        self.assertEqual(regex.search(r'(?&routine)(?(DEFINE)(?<routine>.))', 'a').captures('routine'), ['a'])
+
         # Hg issue 153: Request: (*SKIP).
         self.assertEqual(regex.search(r'12(*FAIL)|3', '123')[0], '3')
         self.assertEqual(regex.search(r'(?r)12(*FAIL)|3', '123')[0], '3')
 
         self.assertEqual(regex.search(r'\d+(*PRUNE)\d', '123'), None)
         self.assertEqual(regex.search(r'\d+(?=(*PRUNE))\d', '123')[0], '123')
         self.assertEqual(regex.search(r'\d+(*PRUNE)bcd|[3d]', '123bcd')[0],
```

### Comparing `regex-2023.6.3/setup.py` & `regex-2023.8.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from os.path import join
 
 with open('README.rst') as file:
     long_description = file.read()
 
 setup(
     name='regex',
-    version='2023.6.3',
+    version='2023.8.8',
     description='Alternative regular expression module, to replace re.',
     long_description=long_description,
     long_description_content_type='text/x-rst',
     author='Matthew Barnett',
     author_email='regex@mrabarnett.plus.com',
     url='https://github.com/mrabarnett/mrab-regex',
     license='Apache Software License',
@@ -23,14 +23,15 @@
         'Operating System :: OS Independent',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
+        'Programming Language :: Python :: 3.12',
         'Topic :: Scientific/Engineering :: Information Analysis',
         'Topic :: Software Development :: Libraries :: Python Modules',
         'Topic :: Text Processing',
         'Topic :: Text Processing :: General',
     ],
     python_requires='>=3.6',
```

### Comparing `regex-2023.6.3/tools/build_regex_unicode.py` & `regex-2023.8.8/tools/build_regex_unicode.py`

 * *Files identical despite different names*

