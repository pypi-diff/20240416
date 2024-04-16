# Comparing `tmp/cachetools_async-0.0.2.tar.gz` & `tmp/cachetools_async-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cachetools_async-0.0.2.tar", max compression
+gzip compressed data, was "cachetools_async-0.0.3.tar", max compression
```

## Comparing `cachetools_async-0.0.2.tar` & `cachetools_async-0.0.3.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1067 2024-04-11 06:13:12.032951 cachetools_async-0.0.2/LICENSE
--rw-r--r--   0        0        0     2983 2024-04-13 07:30:33.705611 cachetools_async-0.0.2/README.md
--rw-r--r--   0        0        0      638 2024-04-13 15:51:18.078676 cachetools_async-0.0.2/pyproject.toml
--rw-r--r--   0        0        0       93 2024-04-12 06:36:03.383096 cachetools_async-0.0.2/src/cachetools_async/__init__.py
--rw-r--r--   0        0        0     4935 2024-04-13 15:38:48.095131 cachetools_async-0.0.2/src/cachetools_async/decorators.py
--rw-r--r--   0        0        0     3639 1970-01-01 00:00:00.000000 cachetools_async-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-04-11 06:13:12.032951 cachetools_async-0.0.3/LICENSE
+-rw-r--r--   0        0        0     2983 2024-04-13 07:30:33.705611 cachetools_async-0.0.3/README.md
+-rw-r--r--   0        0        0      638 2024-04-16 07:36:59.077116 cachetools_async-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0       94 2024-04-16 04:58:07.917379 cachetools_async-0.0.3/src/cachetools_async/__init__.py
+-rw-r--r--   0        0        0     5150 2024-04-16 07:36:53.637279 cachetools_async-0.0.3/src/cachetools_async/decorators.py
+-rw-r--r--   0        0        0     3639 1970-01-01 00:00:00.000000 cachetools_async-0.0.3/PKG-INFO
```

### Comparing `cachetools_async-0.0.2/LICENSE` & `cachetools_async-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cachetools_async-0.0.2/README.md` & `cachetools_async-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `cachetools_async-0.0.2/pyproject.toml` & `cachetools_async-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cachetools-async"
-version = "0.0.2"
+version = "0.0.3"
 description = "Provides decorators that are inspired by and work closely with cachetools' for caching asyncio functions and methods."
 authors = ["James Ward <james@notjam.es>"]
 license = "MIT"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `cachetools_async-0.0.2/src/cachetools_async/decorators.py` & `cachetools_async-0.0.3/src/cachetools_async/decorators.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,42 +3,50 @@
     TypeVar,
     Callable,
     Awaitable,
     Any,
     MutableMapping,
     Optional,
     ContextManager,
+    Protocol,
+    TYPE_CHECKING,
 )
 from inspect import iscoroutinefunction
 from asyncio import get_event_loop, shield, Future, Task
 
 from cachetools.keys import hashkey, methodkey
 
 
 _KT = TypeVar("_KT")
+_T = TypeVar("_T")
+
+
+class IdentityFunction(Protocol):
+    def __call__(self, x: _T, /) -> _T: ...
 
 
 def apply_task_result_to_future(task: Task, future: Future):
     if task.cancelled():
         future.cancel()
         return
 
-    if task.exception() is not None:
-        future.set_exception(task.exception())
+    exception = task.exception()
+    if exception is not None:
+        future.set_exception(exception)
         return
 
     future.set_result(task.result())
 
 
 def cached(
     cache: Optional[MutableMapping[_KT, Future]],
     key: Callable[..., _KT] = hashkey,
     lock: Optional[ContextManager[Any]] = None,
     info: bool = False,
-):
+) -> IdentityFunction:
     """
     Decorator to wrap a function with a memoizing callable that saves
     results in a cache.
     """
 
     if info:
         raise NotImplementedError("cachetools_async does not support `info`")
@@ -46,77 +54,72 @@
     if lock is not None:
         raise NotImplementedError("cachetools_async does not support `lock`")
 
     def decorator(fn: Callable[..., Awaitable]):
         if not iscoroutinefunction(fn):
             raise TypeError("Expected Coroutine function, got {}".format(fn))
 
-        if cache is None:
-
-            async def wrapper(*args, **kwargs):
+        async def wrapper(*args, **kwargs):
+            if cache is None:
+                # No cache available - run the method as normal
                 return await fn(*args, **kwargs)
 
-            def cache_clear():
-                pass
-
-        else:
+            k = key(*args, **kwargs)
 
-            async def wrapper(*args, **kwargs):
-                k = key(*args, **kwargs)
-
-                try:
-                    future = cache[k]
-                except KeyError:
-                    # key not found
-                    future = None
+            try:
+                future = cache[k]
+            except KeyError:
+                # key not found
+                future = None
 
-                if future is not None:
-                    if not future.done():
-                        return await shield(future)
+            if future is not None:
+                if not future.done():
+                    return await shield(future)
 
-                    if future.exception() is None:
-                        return future.result()
+                if future.exception() is None:
+                    return future.result()
 
-                coro = fn(*args, **kwargs)
+            coro = fn(*args, **kwargs)
 
-                loop = get_event_loop()
+            loop = get_event_loop()
 
-                # Crete a task that tracks the coroutine execution
-                task = loop.create_task(coro)
+            # Crete a task that tracks the coroutine execution
+            task = loop.create_task(coro)
 
-                # Create a future and then tie the future and task together
-                f = loop.create_future()
-                task.add_done_callback(lambda t: apply_task_result_to_future(t, f))
+            # Create a future and then tie the future and task together
+            f = loop.create_future()
+            task.add_done_callback(lambda t: apply_task_result_to_future(t, f))
 
-                try:
-                    cache[k] = f
-                except ValueError:
-                    # value too large
-                    pass
-                return await shield(f)
+            try:
+                cache[k] = f
+            except ValueError:
+                # value too large
+                pass
+            return await shield(f)
 
-            def cache_clear():
+        def cache_clear():
+            if cache is not None:
                 cache.clear()
 
-        wrapper.cache = cache
-        wrapper.cache_key = key
-        wrapper.cache_lock = None
-        wrapper.cache_clear = cache_clear
-        wrapper.cache_info = None
+        setattr(wrapper, "cache", cache)
+        setattr(wrapper, "cache_key", key)
+        setattr(wrapper, "cache_lock", None)
+        setattr(wrapper, "cache_clear", cache_clear)
+        setattr(wrapper, "cache_info", None)
 
         return update_wrapper(wrapper, fn)
 
-    return decorator
+    return decorator  # type: ignore
 
 
 def cachedmethod(
     cache: Callable[[Any], Optional[MutableMapping[_KT, Future]]],
     key: Callable[[Any], _KT] = methodkey,
     lock: Optional[Callable[[Any], ContextManager[Any]]] = None,
-):
+) -> IdentityFunction:
     """
     Decorator to wrap a class or instance method with a memoizing
     callable that saves results in a cache.
     """
 
     if lock is not None:
         raise NotImplementedError("cachetools_async does not support `lock`")
@@ -160,20 +163,20 @@
             try:
                 c[k] = future
             except ValueError:
                 # value too large
                 pass
             return await shield(future)
 
-        def clear(self):
+        def cache_clear(self):
             c = cache(self)
             if c is not None:
                 c.clear()
 
-        wrapper.cache = cache
-        wrapper.cache_key = key
-        wrapper.cache_lock = None
-        wrapper.cache_clear = clear
+        setattr(wrapper, "cache", cache)
+        setattr(wrapper, "cache_key", key)
+        setattr(wrapper, "cache_lock", None)
+        setattr(wrapper, "cache_clear", cache_clear)
 
         return update_wrapper(wrapper, method)
 
-    return decorator
+    return decorator  # type: ignore
```

### Comparing `cachetools_async-0.0.2/PKG-INFO` & `cachetools_async-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cachetools-async
-Version: 0.0.2
+Version: 0.0.3
 Summary: Provides decorators that are inspired by and work closely with cachetools' for caching asyncio functions and methods.
 License: MIT
 Author: James Ward
 Author-email: james@notjam.es
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

