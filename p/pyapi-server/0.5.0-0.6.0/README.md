# Comparing `tmp/pyapi_server-0.5.0.tar.gz` & `tmp/pyapi_server-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyapi_server-0.5.0.tar", last modified: Fri Apr  5 22:59:05 2024, max compression
+gzip compressed data, was "pyapi_server-0.6.0.tar", last modified: Mon Apr 15 22:19:32 2024, max compression
```

## Comparing `pyapi_server-0.5.0.tar` & `pyapi_server-0.6.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     1072 2024-04-05 22:58:56.640256 pyapi_server-0.5.0/README.md
--rw-r--r--   0        0        0     7402 2024-04-05 22:58:56.644256 pyapi_server-0.5.0/pyapi/server/__init__.py
--rw-r--r--   0        0        0        0 2024-04-05 22:58:56.644256 pyapi_server-0.5.0/pyapi/server/py.typed
--rw-r--r--   0        0        0     2520 2024-04-05 22:58:56.644256 pyapi_server-0.5.0/pyapi/server/spec.py
--rw-r--r--   0        0        0     3259 2024-04-05 22:58:56.644256 pyapi_server-0.5.0/pyapi/server/validation.py
--rw-r--r--   0        0        0     2625 2024-04-05 22:59:05.464253 pyapi_server-0.5.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-05 22:58:56.644256 pyapi_server-0.5.0/tests/__init__.py
--rw-r--r--   0        0        0      402 2024-04-05 22:58:56.644256 pyapi_server-0.5.0/tests/conftest.py
--rw-r--r--   0        0        0      560 2024-04-05 22:58:56.644256 pyapi_server-0.5.0/tests/endpoints.py
--rw-r--r--   0        0        0     2737 2024-04-05 22:58:56.644256 pyapi_server-0.5.0/tests/openapi.json
--rw-r--r--   0        0        0        0 2024-04-05 22:58:56.644256 pyapi_server-0.5.0/tests/openapi.unknown
--rw-r--r--   0        0        0     1941 2024-04-05 22:58:56.644256 pyapi_server-0.5.0/tests/openapi.yaml
--rw-r--r--   0        0        0     1919 2024-04-05 22:58:56.644256 pyapi_server-0.5.0/tests/test_app.py
--rw-r--r--   0        0        0     3709 2024-04-05 22:58:56.644256 pyapi_server-0.5.0/tests/test_endpoints.py
--rw-r--r--   0        0        0     1765 2024-04-05 22:58:56.644256 pyapi_server-0.5.0/tests/test_service.py
--rw-r--r--   0        0        0      752 2024-04-05 22:58:56.644256 pyapi_server-0.5.0/tests/test_spec.py
--rw-r--r--   0        0        0     1826 1970-01-01 00:00:00.000000 pyapi_server-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-15 22:19:24.595759 pyapi_server-0.6.0/README.md
+-rw-r--r--   0        0        0     7400 2024-04-15 22:19:24.595759 pyapi_server-0.6.0/pyapi/server/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-15 22:19:24.595759 pyapi_server-0.6.0/pyapi/server/py.typed
+-rw-r--r--   0        0        0     2513 2024-04-15 22:19:24.595759 pyapi_server-0.6.0/pyapi/server/spec.py
+-rw-r--r--   0        0        0     3259 2024-04-15 22:19:24.595759 pyapi_server-0.6.0/pyapi/server/validation.py
+-rw-r--r--   0        0        0     3234 2024-04-15 22:19:32.947658 pyapi_server-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-15 22:19:24.599759 pyapi_server-0.6.0/tests/__init__.py
+-rw-r--r--   0        0        0      402 2024-04-15 22:19:24.599759 pyapi_server-0.6.0/tests/conftest.py
+-rw-r--r--   0        0        0      560 2024-04-15 22:19:24.599759 pyapi_server-0.6.0/tests/endpoints.py
+-rw-r--r--   0        0        0     2737 2024-04-15 22:19:24.599759 pyapi_server-0.6.0/tests/openapi.json
+-rw-r--r--   0        0        0        0 2024-04-15 22:19:24.599759 pyapi_server-0.6.0/tests/openapi.unknown
+-rw-r--r--   0        0        0     1941 2024-04-15 22:19:24.599759 pyapi_server-0.6.0/tests/openapi.yaml
+-rw-r--r--   0        0        0     1919 2024-04-15 22:19:24.599759 pyapi_server-0.6.0/tests/test_app.py
+-rw-r--r--   0        0        0     3709 2024-04-15 22:19:24.599759 pyapi_server-0.6.0/tests/test_endpoints.py
+-rw-r--r--   0        0        0     1765 2024-04-15 22:19:24.599759 pyapi_server-0.6.0/tests/test_service.py
+-rw-r--r--   0        0        0      752 2024-04-15 22:19:24.599759 pyapi_server-0.6.0/tests/test_spec.py
+-rw-r--r--   0        0        0     1827 1970-01-01 00:00:00.000000 pyapi_server-0.6.0/PKG-INFO
```

### Comparing `pyapi_server-0.5.0/README.md` & `pyapi_server-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `pyapi_server-0.5.0/pyapi/server/__init__.py` & `pyapi_server-0.6.0/pyapi/server/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,21 +8,21 @@
 from inspect import iscoroutine
 from logging import getLogger
 from pathlib import Path
 from types import ModuleType
 from typing import Any, Callable, cast, Mapping, Optional, Union
 from urllib.parse import urlsplit
 
+from humps import decamelize
 from jsonschema_path import SchemaPath
 from openapi_core import validate_request, validate_response
 from openapi_core.exceptions import OpenAPIError
 from openapi_core.security.exceptions import SecurityProviderError
 from starlette.applications import Starlette
 from starlette.exceptions import HTTPException
-from stringcase import snakecase
 
 from .spec import get_spec_from_file, OperationSpec
 from .validation import JSONResponse, OpenAPIRequest, OpenAPIResponse, Request, Response
 
 log = getLogger(__name__)
 
 
@@ -59,15 +59,15 @@
                 name = operation_id
                 if "." in name:
                     base, name = name.rsplit(".", 1)
                     base_module = _load_module(f"{module.__name__}.{base}")
                 else:
                     base_module = module
                 if self.enforce_case:
-                    name = snakecase(name)
+                    name = decamelize(name)
                 try:
                     endpoint_fn = getattr(base_module, name)
                 except AttributeError as ex:
                     raise RuntimeError(
                         f"The function `{base_module.__name__}.{name}` does not exist!"
                     ) from ex
                 self.set_endpoint(endpoint_fn, operation_id=operation_id)
@@ -86,15 +86,15 @@
             operation_id: Optional ID of the operation to attach the callable to.
                           If omitted, the `operation_id` is determined based on
                           the callable's name.
         """
         if operation_id is None:
             operation_id = endpoint_fn.__name__
         if self.enforce_case and operation_id not in self._operations:
-            operation_id_key = {snakecase(op_id): op_id for op_id in self._operations}.get(
+            operation_id_key = {decamelize(op_id): op_id for op_id in self._operations}.get(
                 operation_id
             )
         else:
             operation_id_key = operation_id
         try:
             operation = self._operations[cast(str, operation_id_key)]
         except KeyError as ex:
```

### Comparing `pyapi_server-0.5.0/pyapi/server/spec.py` & `pyapi_server-0.6.0/pyapi/server/spec.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,16 @@
 from collections import defaultdict
 from enum import Enum
 from itertools import chain
 from pathlib import Path
 from typing import Callable, Dict, Mapping, Sequence
 
 import yaml
+from humps import camelize
 from jsonschema_path import SchemaPath
-from stringcase import camelcase
 
 
 class OperationSpec:
     """Utility class for defining API operations."""
 
     def __init__(
         self, path: str, method: str, spec: dict, parameters: Mapping | Sequence | None = None
@@ -34,15 +34,15 @@
         """
         Looks for values of the specification fields.
 
         If the exact match of a name fails, also checks for the camel case version.
         """
         if name in self.spec:
             return self.spec[name]
-        if (camelcase_name := camelcase(name)) in self.spec:
+        if (camelcase_name := camelize(name)) in self.spec:
             return self.spec[camelcase_name]
         return super().__getattribute__(name)
 
     @classmethod
     def get_all(cls, spec: SchemaPath) -> Dict[str, OperationSpec]:
         """Builds a dict of all operations in the spec."""
         return {
```

### Comparing `pyapi_server-0.5.0/pyapi/server/validation.py` & `pyapi_server-0.6.0/pyapi/server/validation.py`

 * *Files identical despite different names*

### Comparing `pyapi_server-0.5.0/pyproject.toml` & `pyapi_server-0.6.0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 [project]
 name = "pyapi-server"
-version = "0.5.0"
+version = "0.6.0"
 description = "Lightweight API framework using an OpenAPI spec for routing and validation."
 readme = "README.md"
 authors = [
     { name = "Berislav Lopac", email = "berislav@lopac.net" },
 ]
 requires-python = ">=3.8,<4.0"
 dependencies = [
-    "PyYAML>=5.4",
-    "stringcase>=1.2.0",
-    "openapi-core>=0.18",
-    "starlette>=0.21.0",
+    "PyYAML>=6.0.1",
+    "openapi-core>=0.19.1",
+    "starlette>=0.37.2",
     "jsonschema-path>=0.3.2",
+    "pyhumps>=3.8.0",
 ]
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 homepage = "https://pyapi-server.readthedocs.io"
@@ -37,54 +37,77 @@
 [tool.pdm.build]
 includes = [
     "pyapi/server/",
 ]
 
 [tool.pdm.dev-dependencies]
 dev = [
-    "pytest-asyncio>=0.18.3",
-    "pytest-cov>=3.0.0",
-    "pytest-flake8>=1.1.1",
-    "pytest-mypy>=0.9.1",
-    "requests>=2.27.1",
-    "pytest>=7.1.1",
-    "pydocstyle>=6.1.1",
+    "pipdeptree>=2.18.1",
+]
+checks = [
     "mypy>=0.942",
-    "toml>=0.10.2",
-    "pytest-spec>=3.2.0",
     "isort>=5.10.1",
+    "ruff>=0.0.253",
+]
+tests = [
+    "pytest>=7.1.1",
+    "pytest-cov>=3.0.0",
+    "pytest-spec>=3.2.0",
+    "pytest-asyncio>=0.18.3",
+    "requests>=2.27.1",
     "tox>=4.4.6",
     "tox-pdm>=0.6.1",
-    "ruff>=0.0.253",
 ]
 docs = [
     "mkdocs>=1.3.0",
-    "mkdocs-material>=8.5.6",
+    "mkdocs-material>=9.5.17",
 ]
 
 [tool.pdm.scripts.tests]
 cmd = "pytest --spec --cov"
+help = "Run unit tests and coverage."
 
-[tool.pdm.scripts.check-lint]
-shell = "    ruff check .\n    ruff format --check .\n    isort --check .\n"
+[tool.pdm.scripts.tests-quick]
+cmd = "pytest -m 'not api_request'"
+help = "Run unit tests without coverage and API request tests."
 
-[tool.pdm.scripts.reformat]
-shell = "    isort .\n    ruff format .\n"
+[tool.pdm.scripts.check-lint]
+shell = "    ruff format --check .\n    isort --check .\n    ruff check .\n"
+help = "Run linting and formating checks."
 
 [tool.pdm.scripts.check-typing]
 cmd = "mypy --install-types --non-interactive"
+help = "Run static typing analysis."
 
 [tool.pdm.scripts.checks]
 composite = [
     "check-lint",
     "check-typing",
 ]
+help = "Run all checks."
+
+[tool.pdm.scripts.ready]
+composite = [
+    "check-lint",
+    "check-typing",
+    "tests",
+]
+help = "Run all checks and tests."
+
+[tool.pdm.scripts.reformat]
+shell = "    isort .\n    ruff format .\n"
+help = "Reformat the code using isort and ruff."
+
+[tool.pdm.scripts.reqs]
+shell = "pdm export --prod --without-hashes"
+help = "Extract current production requirements. Save to a file with the `-o` option."
 
 [tool.pdm.scripts.new-commits]
 shell = "git log $(git describe --tags --abbrev=0)..HEAD --oneline --no-decorate"
+help = "List all commits since the last tag."
 
 [tool.pytest.ini_options]
 asyncio_mode = "auto"
 
 [tool.coverage.run]
 source = [
     "pyapi/",
```

### Comparing `pyapi_server-0.5.0/tests/endpoints.py` & `pyapi_server-0.6.0/tests/endpoints.py`

 * *Files identical despite different names*

### Comparing `pyapi_server-0.5.0/tests/openapi.json` & `pyapi_server-0.6.0/tests/openapi.json`

 * *Files identical despite different names*

### Comparing `pyapi_server-0.5.0/tests/openapi.yaml` & `pyapi_server-0.6.0/tests/openapi.yaml`

 * *Files identical despite different names*

### Comparing `pyapi_server-0.5.0/tests/test_app.py` & `pyapi_server-0.6.0/tests/test_app.py`

 * *Files identical despite different names*

### Comparing `pyapi_server-0.5.0/tests/test_endpoints.py` & `pyapi_server-0.6.0/tests/test_endpoints.py`

 * *Files identical despite different names*

### Comparing `pyapi_server-0.5.0/tests/test_service.py` & `pyapi_server-0.6.0/tests/test_service.py`

 * *Files identical despite different names*

### Comparing `pyapi_server-0.5.0/tests/test_spec.py` & `pyapi_server-0.6.0/tests/test_spec.py`

 * *Files identical despite different names*

### Comparing `pyapi_server-0.5.0/PKG-INFO` & `pyapi_server-0.6.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: pyapi-server
-Version: 0.5.0
+Version: 0.6.0
 Summary: Lightweight API framework using an OpenAPI spec for routing and validation.
 Home-page: https://pyapi-server.readthedocs.io
 Author-Email: Berislav Lopac <berislav@lopac.net>
 License: MIT
 Project-URL: Homepage, https://pyapi-server.readthedocs.io
 Project-URL: Documentation, https://pyapi-server.readthedocs.io
 Project-URL: Repository, https://github.com/berislavlopac/pyapi-server
 Requires-Python: <4.0,>=3.8
-Requires-Dist: PyYAML>=5.4
-Requires-Dist: stringcase>=1.2.0
-Requires-Dist: openapi-core>=0.18
-Requires-Dist: starlette>=0.21.0
+Requires-Dist: PyYAML>=6.0.1
+Requires-Dist: openapi-core>=0.19.1
+Requires-Dist: starlette>=0.37.2
 Requires-Dist: jsonschema-path>=0.3.2
+Requires-Dist: pyhumps>=3.8.0
 Requires-Dist: uvicorn>=0.18.3; extra == "uvicorn"
 Provides-Extra: uvicorn
 Description-Content-Type: text/markdown
 
 # PyAPI Server
 
 [![Build Status](https://b11c.semaphoreci.com/badges/pyapi-server/branches/main.svg?style=shields&key=e9eeb9d2-6487-4aba-9207-e46c84f9bc6f)](https://b11c.semaphoreci.com/projects/pyapi-server)
```

