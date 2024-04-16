# Comparing `tmp/pyapi_server-0.6.0.tar.gz` & `tmp/pyapi_server-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyapi_server-0.6.0.tar", last modified: Mon Apr 15 22:19:32 2024, max compression
+gzip compressed data, was "pyapi_server-0.7.0.tar", last modified: Tue Apr 16 18:43:53 2024, max compression
```

## Comparing `pyapi_server-0.6.0.tar` & `pyapi_server-0.7.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1072 2024-04-15 22:19:24.595759 pyapi_server-0.6.0/README.md
--rw-r--r--   0        0        0     7400 2024-04-15 22:19:24.595759 pyapi_server-0.6.0/pyapi/server/__init__.py
--rw-r--r--   0        0        0        0 2024-04-15 22:19:24.595759 pyapi_server-0.6.0/pyapi/server/py.typed
--rw-r--r--   0        0        0     2513 2024-04-15 22:19:24.595759 pyapi_server-0.6.0/pyapi/server/spec.py
--rw-r--r--   0        0        0     3259 2024-04-15 22:19:24.595759 pyapi_server-0.6.0/pyapi/server/validation.py
--rw-r--r--   0        0        0     3234 2024-04-15 22:19:32.947658 pyapi_server-0.6.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-15 22:19:24.599759 pyapi_server-0.6.0/tests/__init__.py
--rw-r--r--   0        0        0      402 2024-04-15 22:19:24.599759 pyapi_server-0.6.0/tests/conftest.py
--rw-r--r--   0        0        0      560 2024-04-15 22:19:24.599759 pyapi_server-0.6.0/tests/endpoints.py
--rw-r--r--   0        0        0     2737 2024-04-15 22:19:24.599759 pyapi_server-0.6.0/tests/openapi.json
--rw-r--r--   0        0        0        0 2024-04-15 22:19:24.599759 pyapi_server-0.6.0/tests/openapi.unknown
--rw-r--r--   0        0        0     1941 2024-04-15 22:19:24.599759 pyapi_server-0.6.0/tests/openapi.yaml
--rw-r--r--   0        0        0     1919 2024-04-15 22:19:24.599759 pyapi_server-0.6.0/tests/test_app.py
--rw-r--r--   0        0        0     3709 2024-04-15 22:19:24.599759 pyapi_server-0.6.0/tests/test_endpoints.py
--rw-r--r--   0        0        0     1765 2024-04-15 22:19:24.599759 pyapi_server-0.6.0/tests/test_service.py
--rw-r--r--   0        0        0      752 2024-04-15 22:19:24.599759 pyapi_server-0.6.0/tests/test_spec.py
--rw-r--r--   0        0        0     1827 1970-01-01 00:00:00.000000 pyapi_server-0.6.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-16 18:43:45.102545 pyapi_server-0.7.0/README.md
+-rw-r--r--   0        0        0     7460 2024-04-16 18:43:45.102545 pyapi_server-0.7.0/pyapi/server/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-16 18:43:45.102545 pyapi_server-0.7.0/pyapi/server/py.typed
+-rw-r--r--   0        0        0     2550 2024-04-16 18:43:45.102545 pyapi_server-0.7.0/pyapi/server/spec.py
+-rw-r--r--   0        0        0     3248 2024-04-16 18:43:45.102545 pyapi_server-0.7.0/pyapi/server/validation.py
+-rw-r--r--   0        0        0     3355 2024-04-16 18:43:53.218731 pyapi_server-0.7.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-16 18:43:45.102545 pyapi_server-0.7.0/tests/__init__.py
+-rw-r--r--   0        0        0      403 2024-04-16 18:43:45.102545 pyapi_server-0.7.0/tests/conftest.py
+-rw-r--r--   0        0        0      560 2024-04-16 18:43:45.102545 pyapi_server-0.7.0/tests/endpoints.py
+-rw-r--r--   0        0        0     2737 2024-04-16 18:43:45.102545 pyapi_server-0.7.0/tests/openapi.json
+-rw-r--r--   0        0        0        0 2024-04-16 18:43:45.102545 pyapi_server-0.7.0/tests/openapi.unknown
+-rw-r--r--   0        0        0     1941 2024-04-16 18:43:45.102545 pyapi_server-0.7.0/tests/openapi.yaml
+-rw-r--r--   0        0        0     1919 2024-04-16 18:43:45.102545 pyapi_server-0.7.0/tests/test_app.py
+-rw-r--r--   0        0        0     3709 2024-04-16 18:43:45.102545 pyapi_server-0.7.0/tests/test_endpoints.py
+-rw-r--r--   0        0        0     1764 2024-04-16 18:43:45.102545 pyapi_server-0.7.0/tests/test_service.py
+-rw-r--r--   0        0        0      752 2024-04-16 18:43:45.102545 pyapi_server-0.7.0/tests/test_spec.py
+-rw-r--r--   0        0        0     1948 1970-01-01 00:00:00.000000 pyapi_server-0.7.0/PKG-INFO
```

### Comparing `pyapi_server-0.6.0/README.md` & `pyapi_server-0.7.0/README.md`

 * *Files identical despite different names*

### Comparing `pyapi_server-0.6.0/pyapi/server/__init__.py` & `pyapi_server-0.7.0/pyapi/server/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,46 +1,47 @@
 """PyAPI Server."""
 
 from __future__ import annotations
 
+from collections.abc import Callable, Mapping
 from functools import wraps
 from http import HTTPStatus
 from importlib import import_module
 from inspect import iscoroutine
 from logging import getLogger
 from pathlib import Path
 from types import ModuleType
-from typing import Any, Callable, cast, Mapping, Optional, Union
+from typing import cast
 from urllib.parse import urlsplit
 
-from humps import decamelize
 from jsonschema_path import SchemaPath
 from openapi_core import validate_request, validate_response
 from openapi_core.exceptions import OpenAPIError
 from openapi_core.security.exceptions import SecurityProviderError
 from starlette.applications import Starlette
 from starlette.exceptions import HTTPException
+from stringcase import snakecase
 
 from .spec import get_spec_from_file, OperationSpec
 from .validation import JSONResponse, OpenAPIRequest, OpenAPIResponse, Request, Response
 
 log = getLogger(__name__)
 
 
 class Application(Starlette):
     """PyAPI server application."""
 
-    def __init__(
+    def __init__(  # noqa: PLR0913
         self,
-        spec: Union[SchemaPath, dict],
+        spec: SchemaPath | dict,
         *,
-        module: Optional[Union[str, ModuleType]] = None,
+        module: str | ModuleType | None = None,
         validate_responses: bool = True,
         enforce_case: bool = True,
-        custom_format_validators: Optional[Mapping[str, Callable]] = None,
+        custom_format_validators: Mapping[str, Callable] | None = None,
         spec_url: str = "",
         **kwargs,
     ):
         super().__init__(**kwargs)
         if isinstance(spec, dict):
             spec = SchemaPath.from_dict(spec, base_uri=spec_url)
         self.spec: SchemaPath = spec
@@ -59,26 +60,23 @@
                 name = operation_id
                 if "." in name:
                     base, name = name.rsplit(".", 1)
                     base_module = _load_module(f"{module.__name__}.{base}")
                 else:
                     base_module = module
                 if self.enforce_case:
-                    name = decamelize(name)
+                    name = snakecase(name)
                 try:
                     endpoint_fn = getattr(base_module, name)
                 except AttributeError as ex:
-                    raise RuntimeError(
-                        f"The function `{base_module.__name__}.{name}` does not exist!"
-                    ) from ex
+                    message = f"The function `{base_module.__name__}.{name}` does not exist!"
+                    raise RuntimeError(message) from ex
                 self.set_endpoint(endpoint_fn, operation_id=operation_id)
 
-    def set_endpoint(
-        self, endpoint_fn: Callable, *, operation_id: Optional[str] = None
-    ) -> None:
+    def set_endpoint(self, endpoint_fn: Callable, *, operation_id: str | None = None) -> None:
         """
         Sets endpoint function for a given `operationId`.
 
         If the `operation_id` is not given, it will try to determine it based on the
         function name.
 
         Args:
@@ -86,23 +84,24 @@
             operation_id: Optional ID of the operation to attach the callable to.
                           If omitted, the `operation_id` is determined based on
                           the callable's name.
         """
         if operation_id is None:
             operation_id = endpoint_fn.__name__
         if self.enforce_case and operation_id not in self._operations:
-            operation_id_key = {decamelize(op_id): op_id for op_id in self._operations}.get(
+            operation_id_key = {snakecase(op_id): op_id for op_id in self._operations}.get(
                 operation_id
             )
         else:
             operation_id_key = operation_id
         try:
             operation = self._operations[cast(str, operation_id_key)]
         except KeyError as ex:
-            raise ValueError(f"Unknown operationId: {operation_id}.") from ex
+            message = f"Unknown operationId: {operation_id}."
+            raise ValueError(message) from ex
 
         @wraps(endpoint_fn)
         async def wrapper(request: Request, **kwargs) -> Response:
             openapi_request = OpenAPIRequest(request)
             try:
                 validate_request(
                     request=openapi_request,
@@ -120,18 +119,19 @@
 
             response = endpoint_fn(request, **kwargs)
             if iscoroutine(response):
                 response = await response
             if isinstance(response, dict):
                 response = JSONResponse(response)
             elif not isinstance(response, Response):
-                raise ValueError(
+                message = (
                     f"The endpoint function `{endpoint_fn.__name__}` must return"
                     " either a dict or a Response instance."
                 )
+                raise TypeError(message)
 
             # TODO: pass a list of operation IDs to specify which responses not to validate
             if self.validate_responses:
                 validate_response(
                     request=openapi_request,
                     response=OpenAPIResponse(response),
                     spec=self.spec,
@@ -140,15 +140,15 @@
             return response
 
         for server_path in self._server_paths:
             self.add_route(
                 server_path + operation.path, wrapper, [operation.method], name=operation_id
             )
 
-    def endpoint(self, operation_id: Union[Callable, str]):
+    def endpoint(self, operation_id: Callable | str):
         """
         Decorator for setting endpoints.
 
         If used without arguments, it will try to determine the `operationId` based on the
         decorated function name:
 
             @app.endpoint
@@ -171,15 +171,15 @@
         def decorator(endpoint_fn):
             self.set_endpoint(endpoint_fn, operation_id=operation_id)
             return endpoint_fn
 
         return decorator
 
     @classmethod
-    def from_file(cls, path: Union[Path, str], *args, **kwargs) -> Application:
+    def from_file(cls, path: Path | str, *args, **kwargs) -> Application:
         """
         Creates an instance of the class by loading the spec from a local file.
 
         Args:
             path: Path of the OpenAPI spec file.
             args: Positional arguments are passed on to the class constructor.
             kwargs: Keyword arguments are passed on to the class constructor.
@@ -189,10 +189,11 @@
 
 
 def _load_module(name: str) -> ModuleType:
     """Helper function to load a module based on its dotted-string name."""
     try:
         module = import_module(name)
     except ModuleNotFoundError as ex:
-        raise RuntimeError(f"The module `{name}` does not exist!") from ex
+        message = f"The module `{name}` does not exist!"
+        raise RuntimeError(message) from ex
     else:
         return module
```

### Comparing `pyapi_server-0.6.0/pyapi/server/spec.py` & `pyapi_server-0.7.0/pyapi/server/spec.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 """Utility classes and functions."""
 
 from __future__ import annotations
 
 import json
 from collections import defaultdict
+from collections.abc import Callable, Mapping, Sequence
 from enum import Enum
 from itertools import chain
 from pathlib import Path
-from typing import Callable, Dict, Mapping, Sequence
 
 import yaml
-from humps import camelize
 from jsonschema_path import SchemaPath
+from stringcase import camelcase
 
 
 class OperationSpec:
     """Utility class for defining API operations."""
 
     def __init__(
         self, path: str, method: str, spec: dict, parameters: Mapping | Sequence | None = None
@@ -34,20 +34,20 @@
         """
         Looks for values of the specification fields.
 
         If the exact match of a name fails, also checks for the camel case version.
         """
         if name in self.spec:
             return self.spec[name]
-        if (camelcase_name := camelize(name)) in self.spec:
+        if (camelcase_name := camelcase(name)) in self.spec:
             return self.spec[camelcase_name]
         return super().__getattribute__(name)
 
     @classmethod
-    def get_all(cls, spec: SchemaPath) -> Dict[str, OperationSpec]:
+    def get_all(cls, spec: SchemaPath) -> dict[str, OperationSpec]:
         """Builds a dict of all operations in the spec."""
         return {
             op_spec["operationId"]: cls(
                 path,
                 method,
                 op_spec,
                 path_spec.get("parameters", []) + op_spec.get("parameters", []),
@@ -70,14 +70,15 @@
     suffix = path.suffix[1:].lower()
 
     if suffix in SpecFileTypes.JSON:
         spec_load: Callable = json.load
     elif suffix in SpecFileTypes.YAML:
         spec_load = yaml.safe_load
     else:
-        raise RuntimeError(
+        message = (
             f"Unknown specification file type."
             f" Accepted types: {', '.join(chain(*SpecFileTypes))}"
         )
+        raise RuntimeError(message)
 
-    with open(path, encoding="utf-8") as spec_file:
+    with path.open(encoding="utf-8") as spec_file:
         return spec_load(spec_file)
```

### Comparing `pyapi_server-0.6.0/pyapi/server/validation.py` & `pyapi_server-0.7.0/pyapi/server/validation.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,27 @@
 """OpenAPI request and response wrappers; adapted from openapi-core."""
 
+from __future__ import annotations
+
 import asyncio
 from concurrent.futures import ThreadPoolExecutor
-from typing import Optional, Union
 
 from openapi_core import protocols
 from openapi_core.validation.request.datatypes import RequestParameters
 from starlette.datastructures import Headers
 from starlette.requests import Request
 from starlette.responses import JSONResponse, Response  # noqa: F401
 
 
 class OpenAPIRequest(protocols.Request):
     """Wrapper for PyAPI Server requests."""
 
     def __init__(self, request: Request):
         self.request = request
-        self._body: Optional[Union[str, bytes]] = None
+        self._body: str | bytes | None = None
         self.parameters = RequestParameters(
             query=self.request.query_params,
             header=self.request.headers,
             cookie=self.request.cookies,
             path=self.request.path_params,
         )
         self._body_task = None
@@ -46,15 +47,15 @@
 
     @property
     def method(self) -> str:
         """Return the request HTTP method."""
         return self.request.method.lower()
 
     @property
-    def body(self) -> Optional[bytes]:
+    def body(self) -> bytes | None:
         """Return the request body as string, if present."""
         if isinstance(self._body, str):
             return self._body.encode("utf-8")
         return self._body
 
     @property
     def mimetype(self) -> str:
```

### Comparing `pyapi_server-0.6.0/pyproject.toml` & `pyapi_server-0.7.0/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,40 @@
 [project]
 name = "pyapi-server"
-version = "0.6.0"
+version = "0.7.0"
 description = "Lightweight API framework using an OpenAPI spec for routing and validation."
 readme = "README.md"
 authors = [
     { name = "Berislav Lopac", email = "berislav@lopac.net" },
 ]
-requires-python = ">=3.8,<4.0"
+requires-python = ">=3.8"
 dependencies = [
     "PyYAML>=6.0.1",
     "openapi-core>=0.19.1",
     "starlette>=0.37.2",
     "jsonschema-path>=0.3.2",
-    "pyhumps>=3.8.0",
+    "stringcase>=1.2.0",
 ]
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 homepage = "https://pyapi-server.readthedocs.io"
 documentation = "https://pyapi-server.readthedocs.io"
 repository = "https://github.com/berislavlopac/pyapi-server"
 
 [project.optional-dependencies]
 uvicorn = [
     "uvicorn>=0.18.3",
 ]
+docs = [
+    "mkdocs>=1.3.0",
+    "mkdocs-material>=9.5.17",
+]
 
 [build-system]
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
@@ -53,18 +57,14 @@
     "pytest-cov>=3.0.0",
     "pytest-spec>=3.2.0",
     "pytest-asyncio>=0.18.3",
     "requests>=2.27.1",
     "tox>=4.4.6",
     "tox-pdm>=0.6.1",
 ]
-docs = [
-    "mkdocs>=1.3.0",
-    "mkdocs-material>=9.5.17",
-]
 
 [tool.pdm.scripts.tests]
 cmd = "pytest --spec --cov"
 help = "Run unit tests and coverage."
 
 [tool.pdm.scripts.tests-quick]
 cmd = "pytest -m 'not api_request'"
@@ -129,42 +129,55 @@
 profile = "black"
 line_length = 96
 filter_files = true
 force_alphabetical_sort_within_sections = true
 
 [tool.ruff]
 line-length = 96
-target-version = "py311"
 output-format = "grouped"
 
 [tool.ruff.lint]
 select = [
     "E4",
     "E7",
     "E9",
     "W",
     "F",
     "D",
+    "N",
+    "PLR",
+    "PTH",
+    "UP",
+    "BLE",
+    "B",
+    "A",
+    "C4",
+    "DTZ",
+    "PIE",
+    "TRY",
+    "PERF",
+    "RUF",
 ]
 ignore = [
-    "D104",
     "D107",
     "D203",
+    "D211",
     "D212",
     "D401",
     "D407",
     "D413",
 ]
 
 [tool.ruff.lint.per-file-ignores]
 "__init__.py" = [
     "F401",
 ]
 "tests/*" = [
     "D",
+    "N802",
 ]
 "example/*" = [
     "D",
 ]
 
 [tool.mypy]
 mypy_path = "pyapi/"
```

### Comparing `pyapi_server-0.6.0/tests/endpoints.py` & `pyapi_server-0.7.0/tests/endpoints.py`

 * *Files identical despite different names*

### Comparing `pyapi_server-0.6.0/tests/openapi.json` & `pyapi_server-0.7.0/tests/openapi.json`

 * *Files identical despite different names*

### Comparing `pyapi_server-0.6.0/tests/openapi.yaml` & `pyapi_server-0.7.0/tests/openapi.yaml`

 * *Files identical despite different names*

### Comparing `pyapi_server-0.6.0/tests/test_app.py` & `pyapi_server-0.7.0/tests/test_app.py`

 * *Files identical despite different names*

### Comparing `pyapi_server-0.6.0/tests/test_endpoints.py` & `pyapi_server-0.7.0/tests/test_endpoints.py`

 * *Files identical despite different names*

### Comparing `pyapi_server-0.6.0/tests/test_service.py` & `pyapi_server-0.7.0/tests/test_service.py`

 * *Files 5% similar despite different names*

```diff
@@ -60,9 +60,9 @@
     monkeypatch.setattr(endpoints, "dummy_test_endpoint", lambda request: "sdfsdfsfds")
 
     path = "/test"
     app = Application(spec_dict, module=config.endpoint_base)
 
     route, request = _prepare(app, path)
 
-    with pytest.raises(ValueError):
+    with pytest.raises(TypeError):
         await route.endpoint(request)
```

### Comparing `pyapi_server-0.6.0/tests/test_spec.py` & `pyapi_server-0.7.0/tests/test_spec.py`

 * *Files identical despite different names*

### Comparing `pyapi_server-0.6.0/PKG-INFO` & `pyapi_server-0.7.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,28 @@
 Metadata-Version: 2.1
 Name: pyapi-server
-Version: 0.6.0
+Version: 0.7.0
 Summary: Lightweight API framework using an OpenAPI spec for routing and validation.
 Home-page: https://pyapi-server.readthedocs.io
 Author-Email: Berislav Lopac <berislav@lopac.net>
 License: MIT
 Project-URL: Homepage, https://pyapi-server.readthedocs.io
 Project-URL: Documentation, https://pyapi-server.readthedocs.io
 Project-URL: Repository, https://github.com/berislavlopac/pyapi-server
-Requires-Python: <4.0,>=3.8
+Requires-Python: >=3.8
 Requires-Dist: PyYAML>=6.0.1
 Requires-Dist: openapi-core>=0.19.1
 Requires-Dist: starlette>=0.37.2
 Requires-Dist: jsonschema-path>=0.3.2
-Requires-Dist: pyhumps>=3.8.0
+Requires-Dist: stringcase>=1.2.0
 Requires-Dist: uvicorn>=0.18.3; extra == "uvicorn"
+Requires-Dist: mkdocs>=1.3.0; extra == "docs"
+Requires-Dist: mkdocs-material>=9.5.17; extra == "docs"
 Provides-Extra: uvicorn
+Provides-Extra: docs
 Description-Content-Type: text/markdown
 
 # PyAPI Server
 
 [![Build Status](https://b11c.semaphoreci.com/badges/pyapi-server/branches/main.svg?style=shields&key=e9eeb9d2-6487-4aba-9207-e46c84f9bc6f)](https://b11c.semaphoreci.com/projects/pyapi-server)
 [![Documentation Status](https://readthedocs.org/projects/pyapi-server/badge/?version=latest)](https://pyapi-server.readthedocs.io/en/latest/?badge=latest)
```

