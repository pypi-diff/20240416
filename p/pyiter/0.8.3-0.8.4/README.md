# Comparing `tmp/pyiter-0.8.3.tar.gz` & `tmp/pyiter-0.8.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyiter-0.8.3.tar", last modified: Sat Apr 13 12:58:53 2024, max compression
+gzip compressed data, was "pyiter-0.8.4.tar", last modified: Mon Apr 15 14:22:33 2024, max compression
```

## Comparing `pyiter-0.8.3.tar` & `pyiter-0.8.4.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 yish      (1000) yish      (1000)        0 2024-04-13 12:58:53.648203 pyiter-0.8.3/
--rw-r--r--   0 yish      (1000) yish      (1000)    11357 2023-09-09 01:32:37.000000 pyiter-0.8.3/LICENSE-APACHE
--rw-r--r--   0 yish      (1000) yish      (1000)     1062 2023-09-08 13:21:33.000000 pyiter-0.8.3/LICENSE-MIT
--rw-r--r--   0 yish      (1000) yish      (1000)     2900 2024-04-13 12:58:53.648203 pyiter-0.8.3/PKG-INFO
--rw-r--r--   0 yish      (1000) yish      (1000)     2346 2024-04-13 12:58:27.000000 pyiter-0.8.3/README.md
--rw-r--r--   0 yish      (1000) yish      (1000)       84 2023-10-12 09:06:56.000000 pyiter-0.8.3/pyproject.toml
--rw-r--r--   0 yish      (1000) yish      (1000)       38 2024-04-13 12:58:53.648203 pyiter-0.8.3/setup.cfg
--rw-r--r--   0 yish      (1000) yish      (1000)      846 2024-04-13 12:58:02.000000 pyiter-0.8.3/setup.py
-drwxr-xr-x   0 yish      (1000) yish      (1000)        0 2024-04-13 12:58:53.648203 pyiter-0.8.3/src/
-drwxr-xr-x   0 yish      (1000) yish      (1000)        0 2024-04-13 12:58:53.648203 pyiter-0.8.3/src/pyiter/
--rw-r--r--   0 yish      (1000) yish      (1000)      624 2024-03-26 03:31:01.000000 pyiter-0.8.3/src/pyiter/__init__.py
--rw-r--r--   0 yish      (1000) yish      (1000)    93117 2024-04-08 05:32:25.000000 pyiter-0.8.3/src/pyiter/sequence.py
-drwxr-xr-x   0 yish      (1000) yish      (1000)        0 2024-04-13 12:58:53.648203 pyiter-0.8.3/src/pyiter.egg-info/
--rw-r--r--   0 yish      (1000) yish      (1000)     2900 2024-04-13 12:58:53.000000 pyiter-0.8.3/src/pyiter.egg-info/PKG-INFO
--rw-r--r--   0 yish      (1000) yish      (1000)      275 2024-04-13 12:58:53.000000 pyiter-0.8.3/src/pyiter.egg-info/SOURCES.txt
--rw-r--r--   0 yish      (1000) yish      (1000)        1 2024-04-13 12:58:53.000000 pyiter-0.8.3/src/pyiter.egg-info/dependency_links.txt
--rw-r--r--   0 yish      (1000) yish      (1000)       11 2024-04-13 12:58:53.000000 pyiter-0.8.3/src/pyiter.egg-info/requires.txt
--rw-r--r--   0 yish      (1000) yish      (1000)        7 2024-04-13 12:58:53.000000 pyiter-0.8.3/src/pyiter.egg-info/top_level.txt
+drwxr-xr-x   0 yish      (1000) yish      (1000)        0 2024-04-15 14:22:33.387252 pyiter-0.8.4/
+-rw-r--r--   0 yish      (1000) yish      (1000)    11357 2023-09-09 01:32:37.000000 pyiter-0.8.4/LICENSE-APACHE
+-rw-r--r--   0 yish      (1000) yish      (1000)     1062 2023-09-08 13:21:33.000000 pyiter-0.8.4/LICENSE-MIT
+-rw-r--r--   0 yish      (1000) yish      (1000)     2900 2024-04-15 14:22:33.387252 pyiter-0.8.4/PKG-INFO
+-rw-r--r--   0 yish      (1000) yish      (1000)     2346 2024-04-13 12:58:27.000000 pyiter-0.8.4/README.md
+-rw-r--r--   0 yish      (1000) yish      (1000)       84 2023-10-12 09:06:56.000000 pyiter-0.8.4/pyproject.toml
+-rw-r--r--   0 yish      (1000) yish      (1000)       38 2024-04-15 14:22:33.387252 pyiter-0.8.4/setup.cfg
+-rw-r--r--   0 yish      (1000) yish      (1000)      846 2024-04-15 14:22:21.000000 pyiter-0.8.4/setup.py
+drwxr-xr-x   0 yish      (1000) yish      (1000)        0 2024-04-15 14:22:33.387252 pyiter-0.8.4/src/
+drwxr-xr-x   0 yish      (1000) yish      (1000)        0 2024-04-15 14:22:33.387252 pyiter-0.8.4/src/pyiter/
+-rw-r--r--   0 yish      (1000) yish      (1000)      624 2024-03-26 03:31:01.000000 pyiter-0.8.4/src/pyiter/__init__.py
+-rw-r--r--   0 yish      (1000) yish      (1000)    95751 2024-04-15 14:20:42.000000 pyiter-0.8.4/src/pyiter/sequence.py
+drwxr-xr-x   0 yish      (1000) yish      (1000)        0 2024-04-15 14:22:33.387252 pyiter-0.8.4/src/pyiter.egg-info/
+-rw-r--r--   0 yish      (1000) yish      (1000)     2900 2024-04-15 14:22:33.000000 pyiter-0.8.4/src/pyiter.egg-info/PKG-INFO
+-rw-r--r--   0 yish      (1000) yish      (1000)      275 2024-04-15 14:22:33.000000 pyiter-0.8.4/src/pyiter.egg-info/SOURCES.txt
+-rw-r--r--   0 yish      (1000) yish      (1000)        1 2024-04-15 14:22:33.000000 pyiter-0.8.4/src/pyiter.egg-info/dependency_links.txt
+-rw-r--r--   0 yish      (1000) yish      (1000)       11 2024-04-15 14:22:33.000000 pyiter-0.8.4/src/pyiter.egg-info/requires.txt
+-rw-r--r--   0 yish      (1000) yish      (1000)        7 2024-04-15 14:22:33.000000 pyiter-0.8.4/src/pyiter.egg-info/top_level.txt
```

### Comparing `pyiter-0.8.3/LICENSE-APACHE` & `pyiter-0.8.4/LICENSE-APACHE`

 * *Files identical despite different names*

### Comparing `pyiter-0.8.3/LICENSE-MIT` & `pyiter-0.8.4/LICENSE-MIT`

 * *Files identical despite different names*

### Comparing `pyiter-0.8.3/PKG-INFO` & `pyiter-0.8.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyiter
-Version: 0.8.3
+Version: 0.8.4
 Summary: PyIter is a Python package for iterative operations inspired by the Kotlin、CSharp(linq)、TypeSrcipt and Rust . Enables strong typing and type inference for iterative operations.
 Home-page: https://github.com/mokeyish/pyiter
 Author: YISH
 Author-email: mokeyish@hotmail.com
 License: MIT
 Keywords: linq,iterator,typing,lazy evaluation,type inference
 Requires-Python: >=3.8
```

### Comparing `pyiter-0.8.3/README.md` & `pyiter-0.8.4/README.md`

 * *Files identical despite different names*

### Comparing `pyiter-0.8.3/setup.py` & `pyiter-0.8.4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r", encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name='pyiter',
-    version='0.8.3',
+    version='0.8.4',
     keywords=['linq', 'iterator', 'typing', 'lazy evaluation', 'type inference'],
     description='PyIter is a Python package for iterative operations inspired by the Kotlin、CSharp(linq)、TypeSrcipt '
                 'and Rust . Enables strong typing and type inference for iterative operations.',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='YISH',
     author_email="mokeyish@hotmail.com",
```

### Comparing `pyiter-0.8.3/src/pyiter/__init__.py` & `pyiter-0.8.4/src/pyiter/__init__.py`

 * *Files identical despite different names*

### Comparing `pyiter-0.8.3/src/pyiter/sequence.py` & `pyiter-0.8.4/src/pyiter/sequence.py`

 * *Files 2% similar despite different names*

```diff
@@ -498,113 +498,191 @@
         True
         """
         last: Optional[T] = None
         for i in self if predicate is None else self.filter(predicate):
             last = i
         return last
     
+    def index_of_or_none(self, element: T) -> Optional[int]:
+        """
+        Returns first index of [element], or None if the collection does not contain element.
+
+        Example 1:
+        >>> lst = ['a', 'b', 'c']
+        >>> it(lst).index_of_or_none('b')
+        1
+
+        Example 2:
+        >>> lst = ['a', 'b', 'c']
+        >>> it(lst).index_of_or_none('d')
+        """
+        for i, x in enumerate(self._iter):
+            if x == element:
+                return i
+        return None
+
     def index_of(self, element: T) -> int:
         """
         Returns first index of [element], or -1 if the collection does not contain element.
          
         Example 1:
         >>> lst = ['a', 'b', 'c']
         >>> it(lst).index_of('b')
         1
 
         Example 2:
         >>> lst = ['a', 'b', 'c']
         >>> it(lst).index_of('d')
         -1
         """
-        for i, x in enumerate(self._iter):
-            if x == element:
-                return i
-        return -1
+        return self.index_of_or_none(element) or -1
     
-    def last_index_of(self, element: T) -> int:
+    def last_index_of_or_none(self, element: T) -> Optional[int]:
         """
-         Returns last index of [element], or -1 if the collection does not contain element.
-         
+         Returns last index of [element], or None if the collection does not contain element.
+
         Example 1:
         >>> lst = ['a', 'b', 'c', 'b']
-        >>> it(lst).last_index_of('b')
+        >>> it(lst).last_index_of_or_none('b')
         3
 
         Example 2:
         >>> lst = ['a', 'b', 'c']
-        >>> it(lst).last_index_of('d')
-        -1
+        >>> it(lst).last_index_of_or_none('d')
         """
         seq = self.reversed()
         last_idx = len(seq) - 1;
         for i, x in enumerate(seq):
             if x == element:
                 return last_idx - i
-        return -1
-    
+        return None
+
+    def last_index_of(self, element: T) -> int:
+        """
+         Returns last index of [element], or -1 if the collection does not contain element.
+
+        Example 1:
+        >>> lst = ['a', 'b', 'c', 'b']
+        >>> it(lst).last_index_of('b')
+        3
+
+        Example 2:
+        >>> lst = ['a', 'b', 'c']
+        >>> it(lst).last_index_of('d')
+        -1
+        """
+        return self.last_index_of_or_none(element) or -1
+
+    @overload
+    def index_of_first_or_none(self, predicate: Callable[[T], bool]) -> Optional[int]:
+        ...
+    @overload
+    def index_of_first_or_none(self, predicate: Callable[[T, int], bool]) -> Optional[int]:
+        ...
+    @overload
+    def index_of_first_or_none(self, predicate: Callable[[T, int, Sequence[T]], bool]) -> Optional[int]:
+        ...
+    def index_of_first_or_none(self, predicate: Callable[..., bool]) -> Optional[int]:
+        """
+        Returns first index of element matching the given [predicate], or None if no such element was found.
+
+        Example 1:
+        >>> lst = ['a', 'b', 'c']
+        >>> it(lst).index_of_first_or_none(lambda x: x == 'b')
+        1
+
+        Example 2:
+        >>> lst = ['a', 'b', 'c']
+        >>> it(lst).index_of_first_or_none(lambda x: x == 'd')
+        """
+        predicate = self._callback_overload_warpper(predicate)
+        for i, x in enumerate(self._iter):
+            if predicate(x):
+                return i
+        return None
+
     @overload
     def index_of_first(self, predicate: Callable[[T], bool]) -> int:
         ...
     @overload
     def index_of_first(self, predicate: Callable[[T, int], bool]) -> int:
         ...
     @overload
     def index_of_first(self, predicate: Callable[[T, int, Sequence[T]], bool]) -> int:
         ...
     def index_of_first(self, predicate: Callable[..., bool]) -> int:
         """
         Returns first index of element matching the given [predicate], or -1 if no such element was found.
-         
+
         Example 1:
         >>> lst = ['a', 'b', 'c']
         >>> it(lst).index_of_first(lambda x: x == 'b')
         1
 
         Example 2:
         >>> lst = ['a', 'b', 'c']
         >>> it(lst).index_of_first(lambda x: x == 'd')
         -1
         """
+        return self.index_of_first_or_none(predicate) or -1
+
+    @overload
+    def index_of_last_or_none(self, predicate: Callable[[T], bool]) -> Optional[int]:
+        ...
+    @overload
+    def index_of_last_or_none(self, predicate: Callable[[T, int], bool]) -> Optional[int]:
+        ...
+    @overload
+    def index_of_last_or_none(self, predicate: Callable[[T, int, Sequence[T]], bool]) -> Optional[int]:
+        ...
+    def index_of_last_or_none(self, predicate: Callable[..., bool]) -> Optional[int]:
+        """
+        Returns last index of element matching the given [predicate], or -1 if no such element was found.
+
+        Example 1:
+        >>> lst = ['a', 'b', 'c', 'b']
+        >>> it(lst).index_of_last_or_none(lambda x: x == 'b')
+        3
+
+        Example 2:
+        >>> lst = ['a', 'b', 'c']
+        >>> it(lst).index_of_last_or_none(lambda x: x == 'd')
+        """
+        seq = self.reversed()
+        last_idx = len(seq) - 1
         predicate = self._callback_overload_warpper(predicate)
-        for i, x in enumerate(self._iter):
+        for i, x in enumerate(seq):
             if predicate(x):
-                return i
-        return -1
-    
+                return last_idx - i
+        return None
+
     @overload
     def index_of_last(self, predicate: Callable[[T], bool]) -> int:
         ...
     @overload
     def index_of_last(self, predicate: Callable[[T, int], bool]) -> int:
         ...
     @overload
     def index_of_last(self, predicate: Callable[[T, int, Sequence[T]], bool]) -> int:
         ...
     def index_of_last(self, predicate: Callable[..., bool]) -> int:
         """
         Returns last index of element matching the given [predicate], or -1 if no such element was found.
-         
+
         Example 1:
         >>> lst = ['a', 'b', 'c', 'b']
         >>> it(lst).index_of_last(lambda x: x == 'b')
         3
 
         Example 2:
         >>> lst = ['a', 'b', 'c']
         >>> it(lst).index_of_last(lambda x: x == 'd')
         -1
         """
-        seq = self.reversed()
-        last_idx = len(seq) - 1;
-        predicate = self._callback_overload_warpper(predicate)
-        for i, x in enumerate(seq):
-            if predicate(x):
-                return last_idx - i
-        return -1
+        return self.index_of_last_or_none(predicate) or -1
 
     @overload
     def single(self) -> T:
         ...
     @overload
     def single(self, predicate: Callable[[T], bool]) -> T:
         ...
```

### Comparing `pyiter-0.8.3/src/pyiter.egg-info/PKG-INFO` & `pyiter-0.8.4/src/pyiter.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyiter
-Version: 0.8.3
+Version: 0.8.4
 Summary: PyIter is a Python package for iterative operations inspired by the Kotlin、CSharp(linq)、TypeSrcipt and Rust . Enables strong typing and type inference for iterative operations.
 Home-page: https://github.com/mokeyish/pyiter
 Author: YISH
 Author-email: mokeyish@hotmail.com
 License: MIT
 Keywords: linq,iterator,typing,lazy evaluation,type inference
 Requires-Python: >=3.8
```

