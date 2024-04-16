# Comparing `tmp/kivymd_utils-0.15.1.tar.gz` & `tmp/kivymd_utils-0.15.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kivymd_utils-0.15.1.tar", max compression
+gzip compressed data, was "kivymd_utils-0.15.2.tar", max compression
```

## Comparing `kivymd_utils-0.15.1.tar` & `kivymd_utils-0.15.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0     1068 2024-04-14 14:59:12.472183 kivymd_utils-0.15.1/LICENSE
--rw-r--r--   0        0        0     9970 2024-04-08 14:28:51.783893 kivymd_utils-0.15.1/README.md
--rw-r--r--   0        0        0       87 2024-04-08 13:05:21.394440 kivymd_utils-0.15.1/kivymd_utils/coroutine/__init__.py
--rw-r--r--   0        0        0     1614 2024-04-08 13:05:01.503980 kivymd_utils-0.15.1/kivymd_utils/coroutine/coroutineBuilder.py
--rw-r--r--   0        0        0      126 2024-04-08 13:04:51.743754 kivymd_utils-0.15.1/kivymd_utils/redrawAble/__init__.py
--rw-r--r--   0        0        0      272 2024-04-03 14:19:25.831870 kivymd_utils-0.15.1/kivymd_utils/redrawAble/notifyListeners.py
--rw-r--r--   0        0        0     1058 2024-04-08 13:04:48.060336 kivymd_utils-0.15.1/kivymd_utils/redrawAble/redrawAble.py
--rw-r--r--   0        0        0      164 2024-04-08 13:05:29.157953 kivymd_utils-0.15.1/kivymd_utils/router/__init__.py
--rw-r--r--   0        0        0      561 2024-04-04 09:48:59.355519 kivymd_utils-0.15.1/kivymd_utils/router/error_page.py
--rw-r--r--   0        0        0      569 2024-04-03 16:56:34.050126 kivymd_utils-0.15.1/kivymd_utils/router/path_utils.py
--rw-r--r--   0        0        0     4018 2024-04-16 11:38:02.610055 kivymd_utils-0.15.1/kivymd_utils/router/route.py
--rw-r--r--   0        0        0     4588 2024-04-16 12:08:47.251715 kivymd_utils-0.15.1/kivymd_utils/router/router.py
--rw-r--r--   0        0        0     1683 2024-04-08 13:05:46.818364 kivymd_utils-0.15.1/kivymd_utils/router/state.py
--rw-r--r--   0        0        0      327 2024-04-16 12:09:00.781776 kivymd_utils-0.15.1/pyproject.toml
--rw-r--r--   0        0        0    10430 1970-01-01 00:00:00.000000 kivymd_utils-0.15.1/PKG-INFO
+-rw-r--r--   0        0        0     1068 2024-04-14 14:59:12.472183 kivymd_utils-0.15.2/LICENSE
+-rw-r--r--   0        0        0     9970 2024-04-08 14:28:51.783893 kivymd_utils-0.15.2/README.md
+-rw-r--r--   0        0        0       87 2024-04-08 13:05:21.394440 kivymd_utils-0.15.2/kivymd_utils/coroutine/__init__.py
+-rw-r--r--   0        0        0     1614 2024-04-08 13:05:01.503980 kivymd_utils-0.15.2/kivymd_utils/coroutine/coroutineBuilder.py
+-rw-r--r--   0        0        0      126 2024-04-08 13:04:51.743754 kivymd_utils-0.15.2/kivymd_utils/redrawAble/__init__.py
+-rw-r--r--   0        0        0      272 2024-04-03 14:19:25.831870 kivymd_utils-0.15.2/kivymd_utils/redrawAble/notifyListeners.py
+-rw-r--r--   0        0        0     1058 2024-04-08 13:04:48.060336 kivymd_utils-0.15.2/kivymd_utils/redrawAble/redrawAble.py
+-rw-r--r--   0        0        0      164 2024-04-08 13:05:29.157953 kivymd_utils-0.15.2/kivymd_utils/router/__init__.py
+-rw-r--r--   0        0        0      561 2024-04-04 09:48:59.355519 kivymd_utils-0.15.2/kivymd_utils/router/error_page.py
+-rw-r--r--   0        0        0      569 2024-04-03 16:56:34.050126 kivymd_utils-0.15.2/kivymd_utils/router/path_utils.py
+-rw-r--r--   0        0        0     4018 2024-04-16 11:38:02.610055 kivymd_utils-0.15.2/kivymd_utils/router/route.py
+-rw-r--r--   0        0        0     4691 2024-04-16 12:14:25.659909 kivymd_utils-0.15.2/kivymd_utils/router/router.py
+-rw-r--r--   0        0        0     1683 2024-04-08 13:05:46.818364 kivymd_utils-0.15.2/kivymd_utils/router/state.py
+-rw-r--r--   0        0        0      327 2024-04-16 12:15:35.973560 kivymd_utils-0.15.2/pyproject.toml
+-rw-r--r--   0        0        0    10430 1970-01-01 00:00:00.000000 kivymd_utils-0.15.2/PKG-INFO
```

### Comparing `kivymd_utils-0.15.1/LICENSE` & `kivymd_utils-0.15.2/LICENSE`

 * *Files identical despite different names*

### Comparing `kivymd_utils-0.15.1/README.md` & `kivymd_utils-0.15.2/README.md`

 * *Files identical despite different names*

### Comparing `kivymd_utils-0.15.1/kivymd_utils/coroutine/coroutineBuilder.py` & `kivymd_utils-0.15.2/kivymd_utils/coroutine/coroutineBuilder.py`

 * *Files identical despite different names*

### Comparing `kivymd_utils-0.15.1/kivymd_utils/redrawAble/redrawAble.py` & `kivymd_utils-0.15.2/kivymd_utils/redrawAble/redrawAble.py`

 * *Files identical despite different names*

### Comparing `kivymd_utils-0.15.1/kivymd_utils/router/error_page.py` & `kivymd_utils-0.15.2/kivymd_utils/router/error_page.py`

 * *Files identical despite different names*

### Comparing `kivymd_utils-0.15.1/kivymd_utils/router/path_utils.py` & `kivymd_utils-0.15.2/kivymd_utils/router/path_utils.py`

 * *Files identical despite different names*

### Comparing `kivymd_utils-0.15.1/kivymd_utils/router/route.py` & `kivymd_utils-0.15.2/kivymd_utils/router/route.py`

 * *Files identical despite different names*

### Comparing `kivymd_utils-0.15.1/kivymd_utils/router/router.py` & `kivymd_utils-0.15.2/kivymd_utils/router/router.py`

 * *Files 2% similar despite different names*

```diff
@@ -58,19 +58,20 @@
         self._push_to_path(path, initial_dict=initial_attributes)
 
     def pop(self):
         self._pop()
     
         
 
-    def build(self, path: str = None, is_push= False, initial_dict: dict = None):
+    def build(self, path: str = None, is_push= False, initial_dict: dict = None, is_pop = False):
         if path is None:
             path = self.path
         if (self.debug):
             print(f"trying to display '{path}'")
+            print(f"push = {is_push}")
             
         self.path = path
         state = RouteState(path)
         if initial_dict is not None:
             state.parameters = initial_dict
         if (self.debug):
             print(f"assigning parameters '{state.parameters}'")
@@ -99,17 +100,17 @@
                 print(self.parameter_stack)
 
             return MDScreen(
                 self.error_route.build(state, router=self)
             )
         if is_push == False:
             self.page_stack.clear()
-
-        self.page_stack.append(path)
-        self.parameter_stack.append(self.parameters)
+        if is_pop == False:
+            self.page_stack.append(path)
+            self.parameter_stack.append(self.parameters)
             
         if (self.debug):
             print("stack is now")
             print(self.page_stack)
             print(self.parameter_stack)
         screen = MDScreen(
             item
@@ -127,15 +128,15 @@
     def _pop(self):
         #print("trying pop")
         if len(self.page_stack) == 1:
             return
         #print(f"got pop to {self.page_stack}")
         _ = self.page_stack.pop()
         _ = self.parameter_stack.pop()
-        self._switch_to(self.build(self.page_stack[-1], is_push=True, initial_dict=self.parameter_stack[-1]))
+        self._switch_to(self.build(self.page_stack[-1], is_push=True, initial_dict=self.parameter_stack[-1], is_pop=True))
 
     def _add_switch_manager(self, switch_manager):
         self._switch_to = switch_manager
```

### Comparing `kivymd_utils-0.15.1/kivymd_utils/router/state.py` & `kivymd_utils-0.15.2/kivymd_utils/router/state.py`

 * *Files identical despite different names*

### Comparing `kivymd_utils-0.15.1/PKG-INFO` & `kivymd_utils-0.15.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kivymd-utils
-Version: 0.15.1
+Version: 0.15.2
 Summary: 
 Author: MilanR
 Author-email: milan.rombouts23@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
```

