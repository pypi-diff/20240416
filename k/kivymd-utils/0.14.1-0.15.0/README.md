# Comparing `tmp/kivymd_utils-0.14.1.tar.gz` & `tmp/kivymd_utils-0.15.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kivymd_utils-0.14.1.tar", max compression
+gzip compressed data, was "kivymd_utils-0.15.0.tar", max compression
```

## Comparing `kivymd_utils-0.14.1.tar` & `kivymd_utils-0.15.0.tar`

### file list

```diff
@@ -1,25 +1,15 @@
--rw-r--r--   0        0        0     9970 2024-04-08 14:28:51.783893 kivymd_utils-0.14.1/README.md
--rw-r--r--   0        0        0       87 2024-04-08 13:05:21.394440 kivymd_utils-0.14.1/kivymd_utils/coroutine/__init__.py
--rw-r--r--   0        0        0      326 2024-04-08 14:00:42.877251 kivymd_utils-0.14.1/kivymd_utils/coroutine/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     4146 2024-04-08 14:00:42.880585 kivymd_utils-0.14.1/kivymd_utils/coroutine/__pycache__/coroutineBuilder.cpython-311.pyc
--rw-r--r--   0        0        0     1614 2024-04-08 13:05:01.503980 kivymd_utils-0.14.1/kivymd_utils/coroutine/coroutineBuilder.py
--rw-r--r--   0        0        0      126 2024-04-08 13:04:51.743754 kivymd_utils-0.14.1/kivymd_utils/redrawAble/__init__.py
--rw-r--r--   0        0        0      376 2024-04-08 14:00:42.893918 kivymd_utils-0.14.1/kivymd_utils/redrawAble/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1100 2024-04-03 14:47:45.322557 kivymd_utils-0.14.1/kivymd_utils/redrawAble/__pycache__/notifyListeners.cpython-311.pyc
--rw-r--r--   0        0        0     2294 2024-04-08 14:00:42.893918 kivymd_utils-0.14.1/kivymd_utils/redrawAble/__pycache__/redrawAble.cpython-311.pyc
--rw-r--r--   0        0        0      272 2024-04-03 14:19:25.831870 kivymd_utils-0.14.1/kivymd_utils/redrawAble/notifyListeners.py
--rw-r--r--   0        0        0     1058 2024-04-08 13:04:48.060336 kivymd_utils-0.14.1/kivymd_utils/redrawAble/redrawAble.py
--rw-r--r--   0        0        0      164 2024-04-08 13:05:29.157953 kivymd_utils-0.14.1/kivymd_utils/router/__init__.py
--rw-r--r--   0        0        0      469 2024-04-08 13:09:32.980348 kivymd_utils-0.14.1/kivymd_utils/router/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0        0        0     1533 2024-04-04 09:49:01.862213 kivymd_utils-0.14.1/kivymd_utils/router/__pycache__/error_page.cpython-311.pyc
--rw-r--r--   0        0        0     1339 2024-04-03 16:56:36.213490 kivymd_utils-0.14.1/kivymd_utils/router/__pycache__/path_utils.cpython-311.pyc
--rw-r--r--   0        0        0     7321 2024-04-08 13:32:38.210070 kivymd_utils-0.14.1/kivymd_utils/router/__pycache__/route.cpython-311.pyc
--rw-r--r--   0        0        0     6577 2024-04-08 13:11:05.535886 kivymd_utils-0.14.1/kivymd_utils/router/__pycache__/router.cpython-311.pyc
--rw-r--r--   0        0        0     2393 2024-04-08 13:09:33.243688 kivymd_utils-0.14.1/kivymd_utils/router/__pycache__/state.cpython-311.pyc
--rw-r--r--   0        0        0      561 2024-04-04 09:48:59.355519 kivymd_utils-0.14.1/kivymd_utils/router/error_page.py
--rw-r--r--   0        0        0      569 2024-04-03 16:56:34.050126 kivymd_utils-0.14.1/kivymd_utils/router/path_utils.py
--rw-r--r--   0        0        0     3968 2024-04-08 13:32:17.356334 kivymd_utils-0.14.1/kivymd_utils/router/route.py
--rw-r--r--   0        0        0     3633 2024-04-08 13:10:29.315022 kivymd_utils-0.14.1/kivymd_utils/router/router.py
--rw-r--r--   0        0        0     1683 2024-04-08 13:05:46.818364 kivymd_utils-0.14.1/kivymd_utils/router/state.py
--rw-r--r--   0        0        0      327 2024-04-08 14:29:16.647571 kivymd_utils-0.14.1/pyproject.toml
--rw-r--r--   0        0        0    10430 1970-01-01 00:00:00.000000 kivymd_utils-0.14.1/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-04-14 14:59:12.472183 kivymd_utils-0.15.0/LICENSE
+-rw-r--r--   0        0        0     9970 2024-04-08 14:28:51.783893 kivymd_utils-0.15.0/README.md
+-rw-r--r--   0        0        0       87 2024-04-08 13:05:21.394440 kivymd_utils-0.15.0/kivymd_utils/coroutine/__init__.py
+-rw-r--r--   0        0        0     1614 2024-04-08 13:05:01.503980 kivymd_utils-0.15.0/kivymd_utils/coroutine/coroutineBuilder.py
+-rw-r--r--   0        0        0      126 2024-04-08 13:04:51.743754 kivymd_utils-0.15.0/kivymd_utils/redrawAble/__init__.py
+-rw-r--r--   0        0        0      272 2024-04-03 14:19:25.831870 kivymd_utils-0.15.0/kivymd_utils/redrawAble/notifyListeners.py
+-rw-r--r--   0        0        0     1058 2024-04-08 13:04:48.060336 kivymd_utils-0.15.0/kivymd_utils/redrawAble/redrawAble.py
+-rw-r--r--   0        0        0      164 2024-04-08 13:05:29.157953 kivymd_utils-0.15.0/kivymd_utils/router/__init__.py
+-rw-r--r--   0        0        0      561 2024-04-04 09:48:59.355519 kivymd_utils-0.15.0/kivymd_utils/router/error_page.py
+-rw-r--r--   0        0        0      569 2024-04-03 16:56:34.050126 kivymd_utils-0.15.0/kivymd_utils/router/path_utils.py
+-rw-r--r--   0        0        0     4018 2024-04-16 11:38:02.610055 kivymd_utils-0.15.0/kivymd_utils/router/route.py
+-rw-r--r--   0        0        0     3676 2024-04-16 11:21:08.555478 kivymd_utils-0.15.0/kivymd_utils/router/router.py
+-rw-r--r--   0        0        0     1683 2024-04-08 13:05:46.818364 kivymd_utils-0.15.0/kivymd_utils/router/state.py
+-rw-r--r--   0        0        0      327 2024-04-16 11:38:57.000300 kivymd_utils-0.15.0/pyproject.toml
+-rw-r--r--   0        0        0    10430 1970-01-01 00:00:00.000000 kivymd_utils-0.15.0/PKG-INFO
```

### Comparing `kivymd_utils-0.14.1/README.md` & `kivymd_utils-0.15.0/README.md`

 * *Files identical despite different names*

### Comparing `kivymd_utils-0.14.1/kivymd_utils/coroutine/coroutineBuilder.py` & `kivymd_utils-0.15.0/kivymd_utils/coroutine/coroutineBuilder.py`

 * *Files identical despite different names*

### Comparing `kivymd_utils-0.14.1/kivymd_utils/redrawAble/redrawAble.py` & `kivymd_utils-0.15.0/kivymd_utils/redrawAble/redrawAble.py`

 * *Files identical despite different names*

### Comparing `kivymd_utils-0.14.1/kivymd_utils/router/error_page.py` & `kivymd_utils-0.15.0/kivymd_utils/router/error_page.py`

 * *Files identical despite different names*

### Comparing `kivymd_utils-0.14.1/kivymd_utils/router/path_utils.py` & `kivymd_utils-0.15.0/kivymd_utils/router/path_utils.py`

 * *Files identical despite different names*

### Comparing `kivymd_utils-0.14.1/kivymd_utils/router/route.py` & `kivymd_utils-0.15.0/kivymd_utils/router/route.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,14 +102,16 @@
         return matches
     
     def build(self, state, *args, **kwargs):
         route = state.get_route(self.routes, reconsume=True)
         if route is None:
             return None
         child = route.build(state, *args, **kwargs)
+        if child is None:
+            return None
         print(f"building shellroute {child}")
         return self.builder(state, child, *args, **kwargs)
     
 from kivymd_utils.router.error_page import ErrorPage
 class ErrorRoute(RouteBase):
     def __init__(self, path: str = "", builder = lambda state, path, *args, **kwargs: ErrorPage(path, *args, **kwargs) ) -> None:
         super().__init__([], builder)
```

### Comparing `kivymd_utils-0.14.1/kivymd_utils/router/router.py` & `kivymd_utils-0.15.0/kivymd_utils/router/router.py`

 * *Files 4% similar despite different names*

```diff
@@ -56,14 +56,15 @@
         self._pop()
     
         
 
     def build(self, path: str = None, is_push= False, initial_dict: dict = None):
         if path is None:
             path = self.path
+        print(f"trying to display {path}")
             
         self.path = path
         state = RouteState(path)
         if initial_dict is not None:
             state.parameters = initial_dict
         
         route = state.get_route(self.routes)
```

### Comparing `kivymd_utils-0.14.1/kivymd_utils/router/state.py` & `kivymd_utils-0.15.0/kivymd_utils/router/state.py`

 * *Files identical despite different names*

### Comparing `kivymd_utils-0.14.1/PKG-INFO` & `kivymd_utils-0.15.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kivymd-utils
-Version: 0.14.1
+Version: 0.15.0
 Summary: 
 Author: MilanR
 Author-email: milan.rombouts23@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

