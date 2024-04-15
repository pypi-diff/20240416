# Comparing `tmp/synchronicity-0.6.6-py3-none-any.whl.zip` & `tmp/synchronicity-0.6.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,17 +1,17 @@
-Zip file size: 28555 bytes, number of entries: 15
--rw-r--r--  2.0 unx      100 b- defN 24-Feb-06 14:05 synchronicity/__init__.py
--rw-r--r--  2.0 unx     1188 b- defN 24-Feb-07 09:54 synchronicity/annotations.py
--rw-r--r--  2.0 unx     2582 b- defN 24-Mar-21 13:09 synchronicity/async_wrap.py
--rw-r--r--  2.0 unx     1485 b- defN 23-Jun-19 18:14 synchronicity/callback.py
--rw-r--r--  2.0 unx     2518 b- defN 24-Mar-13 16:28 synchronicity/combined_types.py
--rw-r--r--  2.0 unx     1303 b- defN 24-Mar-21 10:27 synchronicity/exceptions.py
--rw-r--r--  2.0 unx      331 b- defN 23-Jun-19 18:14 synchronicity/interface.py
--rw-r--r--  2.0 unx     1793 b- defN 24-Jan-26 13:32 synchronicity/overload_tracking.py
--rw-r--r--  2.0 unx    31176 b- defN 24-Apr-02 08:55 synchronicity/synchronizer.py
--rw-r--r--  2.0 unx    28057 b- defN 24-Mar-27 08:14 synchronicity/type_stubs.py
--rw-r--r--  2.0 unx    11357 b- defN 24-Apr-02 08:57 synchronicity-0.6.6.dist-info/LICENSE
--rw-r--r--  2.0 unx     7793 b- defN 24-Apr-02 08:57 synchronicity-0.6.6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Apr-02 08:57 synchronicity-0.6.6.dist-info/WHEEL
--rw-r--r--  2.0 unx       14 b- defN 24-Apr-02 08:57 synchronicity-0.6.6.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     1266 b- defN 24-Apr-02 08:57 synchronicity-0.6.6.dist-info/RECORD
-15 files, 91055 bytes uncompressed, 26457 bytes compressed:  70.9%
+Zip file size: 28608 bytes, number of entries: 15
+-rw-r--r--  2.0 unx      100 b- defN 23-May-10 14:24 synchronicity/__init__.py
+-rw-r--r--  2.0 unx     1188 b- defN 24-Mar-22 18:13 synchronicity/annotations.py
+-rw-r--r--  2.0 unx     2582 b- defN 24-Apr-12 21:43 synchronicity/async_wrap.py
+-rw-r--r--  2.0 unx     1485 b- defN 23-Mar-20 19:53 synchronicity/callback.py
+-rw-r--r--  2.0 unx     2518 b- defN 24-Mar-22 18:13 synchronicity/combined_types.py
+-rw-r--r--  2.0 unx     1303 b- defN 23-Mar-20 15:54 synchronicity/exceptions.py
+-rw-r--r--  2.0 unx      331 b- defN 23-Aug-01 07:57 synchronicity/interface.py
+-rw-r--r--  2.0 unx     1793 b- defN 24-Mar-22 18:13 synchronicity/overload_tracking.py
+-rw-r--r--  2.0 unx    31176 b- defN 24-Apr-12 21:35 synchronicity/synchronizer.py
+-rw-r--r--  2.0 unx    28265 b- defN 24-Apr-15 22:14 synchronicity/type_stubs.py
+-rw-r--r--  2.0 unx    11357 b- defN 24-Apr-15 22:18 synchronicity-0.6.7.dist-info/LICENSE
+-rw-r--r--  2.0 unx     7793 b- defN 24-Apr-15 22:18 synchronicity-0.6.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-15 22:18 synchronicity-0.6.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx       14 b- defN 24-Apr-15 22:18 synchronicity-0.6.7.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     1266 b- defN 24-Apr-15 22:18 synchronicity-0.6.7.dist-info/RECORD
+15 files, 91263 bytes uncompressed, 26510 bytes compressed:  71.0%
```

## zipnote {}

```diff
@@ -24,23 +24,23 @@
 
 Filename: synchronicity/synchronizer.py
 Comment: 
 
 Filename: synchronicity/type_stubs.py
 Comment: 
 
-Filename: synchronicity-0.6.6.dist-info/LICENSE
+Filename: synchronicity-0.6.7.dist-info/LICENSE
 Comment: 
 
-Filename: synchronicity-0.6.6.dist-info/METADATA
+Filename: synchronicity-0.6.7.dist-info/METADATA
 Comment: 
 
-Filename: synchronicity-0.6.6.dist-info/WHEEL
+Filename: synchronicity-0.6.7.dist-info/WHEEL
 Comment: 
 
-Filename: synchronicity-0.6.6.dist-info/top_level.txt
+Filename: synchronicity-0.6.7.dist-info/top_level.txt
 Comment: 
 
-Filename: synchronicity-0.6.6.dist-info/RECORD
+Filename: synchronicity-0.6.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## synchronicity/type_stubs.py

```diff
@@ -5,14 +5,15 @@
   implementation types directly (but translated to blocking).
 * Let synchronicity emit actual function bodies, to avoid runtime wrapping altogether
 """
 
 import collections
 import collections.abc
 import contextlib
+import enum
 import importlib
 import inspect
 import sys
 import typing
 from logging import getLogger
 from pathlib import Path
 from typing import Generic, TypeVar
@@ -154,14 +155,21 @@
         bases = []
         for b in cls.__dict__.get("__orig_bases__", cls.__bases__):
             bases.append(self._translate_global_annotation(b, cls))
         return bases
 
     def add_class(self, cls, name):
         self.global_types.add(name)
+
+        if issubclass(cls, enum.Enum):
+            # Do not translate Enum classes.
+            self.imports.add("enum")
+            self.parts.append(inspect.getsource(cls))
+            return
+
         bases = []
         for b in self._get_translated_class_bases(cls):
             if b is not object:
                 bases.append(self._formatannotation(b))
 
         bases_str = "" if not bases else "(" + ", ".join(bases) + ")"
         decl = f"class {name}{bases_str}:"
```

## Comparing `synchronicity-0.6.6.dist-info/LICENSE` & `synchronicity-0.6.7.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `synchronicity-0.6.6.dist-info/METADATA` & `synchronicity-0.6.7.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synchronicity
-Version: 0.6.6
+Version: 0.6.7
 Summary: Export blocking and async library versions from a single async implementation
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: sigtools ==4.0.1
 Requires-Dist: typing-extensions >=4.6
```

## Comparing `synchronicity-0.6.6.dist-info/RECORD` & `synchronicity-0.6.7.dist-info/RECORD`

 * *Files 11% similar despite different names*

```diff
@@ -3,13 +3,13 @@
 synchronicity/async_wrap.py,sha256=OcPo_ljrM6PxiL6qC9pg902wlTnZIHMcKr6AGtm5LFU,2582
 synchronicity/callback.py,sha256=ZPCfzrZkaepalwEmvxdfYewHEc059hDKFz_7oXIdIoY,1485
 synchronicity/combined_types.py,sha256=9qL8Ou_Mj7BFj68IjlltIromleLoanYIL3URa9834uk,2518
 synchronicity/exceptions.py,sha256=pJw_RhOvRSr-sMhSRLmCzNb1M5W36W4EFfeE0FD27OA,1303
 synchronicity/interface.py,sha256=OVodgsiXbzr9h_3q0bYc4T7qnbTaWQqorbkhYXdxwo0,331
 synchronicity/overload_tracking.py,sha256=VKOod5xYNJzK_JnujoUA2t7rTiz0qcJqvNNwDIX61eA,1793
 synchronicity/synchronizer.py,sha256=ecV03Wq8bC_8Nn2K9i5kAseC7pI0gx5yhZDy7bC17gw,31176
-synchronicity/type_stubs.py,sha256=CqzrszMx4TKUfIsSla-TAlx4RGRhwKmG9ROtXAeyN6Q,28057
-synchronicity-0.6.6.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
-synchronicity-0.6.6.dist-info/METADATA,sha256=0d_NZwWNQMsDbZblbKNYiJwmQNiyRZAS731McTPf9Y0,7793
-synchronicity-0.6.6.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
-synchronicity-0.6.6.dist-info/top_level.txt,sha256=pqAkRTgp1bdeADR7z1vhyQijkZNYCCsezJKpOwFizoE,14
-synchronicity-0.6.6.dist-info/RECORD,,
+synchronicity/type_stubs.py,sha256=ufty2YzhWR-BfxoFt7hi7wLM3wLmjZRdbfDmC_kS2Zg,28265
+synchronicity-0.6.7.dist-info/LICENSE,sha256=xx0jnfkXJvxRnG63LTGOxlggYnIysveWIZ6H3PNdCrQ,11357
+synchronicity-0.6.7.dist-info/METADATA,sha256=XoR9VRchZhG6g4MbBGamWHiwPNUj3EuZHOOhX0Q1hAU,7793
+synchronicity-0.6.7.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+synchronicity-0.6.7.dist-info/top_level.txt,sha256=pqAkRTgp1bdeADR7z1vhyQijkZNYCCsezJKpOwFizoE,14
+synchronicity-0.6.7.dist-info/RECORD,,
```

