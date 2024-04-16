# Comparing `tmp/logiclayer-0.3.0.tar.gz` & `tmp/logiclayer-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logiclayer-0.3.0.tar", max compression
+gzip compressed data, was "logiclayer-0.3.1.tar", max compression
```

## Comparing `logiclayer-0.3.0.tar` & `logiclayer-0.3.1.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1072 2024-03-01 23:04:24.806041 logiclayer-0.3.0/LICENSE
--rw-r--r--   0        0        0     3574 2024-03-01 23:04:24.806041 logiclayer-0.3.0/PACKAGE.md
--rw-r--r--   0        0        0      359 2024-03-01 23:04:24.806041 logiclayer-0.3.0/logiclayer/__init__.py
--rw-r--r--   0        0        0      623 2024-03-01 23:04:24.806041 logiclayer-0.3.0/logiclayer/common.py
--rw-r--r--   0        0        0     2689 2024-03-01 23:04:24.806041 logiclayer-0.3.0/logiclayer/decorators.py
--rw-r--r--   0        0        0     5709 2024-03-01 23:04:24.806041 logiclayer-0.3.0/logiclayer/logiclayer.py
--rw-r--r--   0        0        0     3740 2024-03-01 23:04:24.806041 logiclayer-0.3.0/logiclayer/module.py
--rw-r--r--   0        0        0    88370 2024-03-01 23:04:24.806041 logiclayer-0.3.0/logiclayer/poetry.lock
--rw-r--r--   0        0        0      579 2024-03-01 23:04:24.806041 logiclayer-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     4406 1970-01-01 00:00:00.000000 logiclayer-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-16 17:20:42.343942 logiclayer-0.3.1/LICENSE
+-rw-r--r--   0        0        0     3574 2024-04-16 17:20:42.343942 logiclayer-0.3.1/PACKAGE.md
+-rw-r--r--   0        0        0      474 2024-04-16 17:20:42.343942 logiclayer-0.3.1/logiclayer/__init__.py
+-rw-r--r--   0        0        0      896 2024-04-16 17:20:42.343942 logiclayer-0.3.1/logiclayer/auth.py
+-rw-r--r--   0        0        0      623 2024-04-16 17:20:42.343942 logiclayer-0.3.1/logiclayer/common.py
+-rw-r--r--   0        0        0     2689 2024-04-16 17:20:42.343942 logiclayer-0.3.1/logiclayer/decorators.py
+-rw-r--r--   0        0        0     5886 2024-04-16 17:20:42.343942 logiclayer-0.3.1/logiclayer/logiclayer.py
+-rw-r--r--   0        0        0     3878 2024-04-16 17:20:42.343942 logiclayer-0.3.1/logiclayer/module.py
+-rw-r--r--   0        0        0      580 2024-04-16 17:20:42.347942 logiclayer-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     4407 1970-01-01 00:00:00.000000 logiclayer-0.3.1/PKG-INFO
```

### Comparing `logiclayer-0.3.0/LICENSE` & `logiclayer-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `logiclayer-0.3.0/PACKAGE.md` & `logiclayer-0.3.1/PACKAGE.md`

 * *Files identical despite different names*

### Comparing `logiclayer-0.3.0/logiclayer/common.py` & `logiclayer-0.3.1/logiclayer/common.py`

 * *Files identical despite different names*

### Comparing `logiclayer-0.3.0/logiclayer/decorators.py` & `logiclayer-0.3.1/logiclayer/decorators.py`

 * *Files identical despite different names*

### Comparing `logiclayer-0.3.0/logiclayer/logiclayer.py` & `logiclayer-0.3.1/logiclayer/logiclayer.py`

 * *Files 6% similar despite different names*

```diff
@@ -160,7 +160,14 @@
             await asyncio.gather(*gen)
         except Exception as exc:
             logger.error("Healthcheck failure", exc_info=exc)
         else:
             return Response(status_code=HTTP_204_NO_CONTENT)
 
         raise HTTPException(500, "One of the healthchecks failed.")
+
+    def route(self, path: str, **kwargs):
+        def route_decorator(fn):
+            self.add_route(path, fn, **kwargs)
+            return fn
+
+        return route_decorator
```

### Comparing `logiclayer-0.3.0/logiclayer/module.py` & `logiclayer-0.3.1/logiclayer/module.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import dataclasses
 from collections import defaultdict
 from enum import Enum, auto
-from typing import TYPE_CHECKING, Any, Dict, Tuple, Type
+from typing import TYPE_CHECKING, Any, Dict, Optional, Tuple, Type
 
 from fastapi import APIRouter
 
+from .auth import AuthProvider, VoidAuthProvider
 from .common import LOGICLAYER_METHOD_ATTR, CallableMayReturnCoroutine
 
 if TYPE_CHECKING:
     from .logiclayer import LogicLayer
 
 
 class MethodType(Enum):
@@ -71,33 +72,35 @@
 class LogicLayerModule(metaclass=ModuleMeta):
     """Base class for LogicLayer Modules.
 
     Modules must inherit from this class to be used in LogicLayer.
     Routes can be set using the provided decorators on any instance method.
     """
 
+    auth: AuthProvider
     router: APIRouter
     _llexceptions: Dict[Type[Exception], ModuleMethod]
     _llhealthchecks: Tuple[ModuleMethod, ...]
     _llroutes: Tuple[ModuleMethod, ...]
     _llshutdown: Tuple[ModuleMethod, ...]
     _llstartup: Tuple[ModuleMethod, ...]
 
-    def __init__(self, **kwargs):
+    def __init__(self, *, auth: Optional[AuthProvider] = None, **kwargs):
+        self.auth = auth or VoidAuthProvider()
         self.router = APIRouter(**kwargs)
 
     @property
     def name(self):
         return type(self).__name__
 
     @property
     def route_paths(self):
         return (item.path for item in self._llroutes)
 
-    def include_into(self, layer: "LogicLayer", *, prefix: str, **kwargs):
+    def include_into(self, layer: "LogicLayer", **kwargs):
         app = layer.app
         router = self.router
 
         for exc_cls, method in self._llexceptions.items():
             app.add_exception_handler(exc_cls, method.bound_to(self))
 
         for item in self._llhealthchecks:
@@ -105,8 +108,8 @@
 
         router.on_startup.extend(item.bound_to(self) for item in self._llstartup)
         router.on_shutdown.extend(item.bound_to(self) for item in self._llshutdown)
 
         for item in self._llroutes:
             router.add_api_route(item.path, item.bound_to(self), **item.kwargs)
 
-        app.include_router(router, prefix=prefix, **kwargs)
+        app.include_router(router, **kwargs)
```

### Comparing `logiclayer-0.3.0/pyproject.toml` & `logiclayer-0.3.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 [tool.poetry]
 name = "logiclayer"
-version = "0.3.0"
+version = "0.3.1"
 description = "A framework to quickly compose and use multiple functionalities as endpoints."
 authors = ["Francisco Abarzua <francisco@datawheel.us>"]
 license = "MIT"
 readme = "PACKAGE.md"
 repository = "https://github.com/Datawheel/logiclayer"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 asyncio = "^3.4.0"
-fastapi = ">=0.75 <1.0"
+fastapi = ">=0.100 <1.0"
 
 [tool.poetry.group.dev.dependencies]
 httpx = ">=0.20.0"
 pytest = "^8.0.2"
 ruff = "^0.3.0"
 uvicorn = "^0.27.0"
```

### Comparing `logiclayer-0.3.0/PKG-INFO` & `logiclayer-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: logiclayer
-Version: 0.3.0
+Version: 0.3.1
 Summary: A framework to quickly compose and use multiple functionalities as endpoints.
 Home-page: https://github.com/Datawheel/logiclayer
 License: MIT
 Author: Francisco Abarzua
 Author-email: francisco@datawheel.us
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: asyncio (>=3.4.0,<4.0.0)
-Requires-Dist: fastapi (>=0.75,<1.0)
+Requires-Dist: fastapi (>=0.100,<1.0)
 Project-URL: Repository, https://github.com/Datawheel/logiclayer
 Description-Content-Type: text/markdown
 
 A simple framework to quickly compose and use multiple functionalities as endpoints.  
 LogicLayer is built upon FastAPI to provide a simple way to group functionalities into reusable modules.
 
 <p>
```

