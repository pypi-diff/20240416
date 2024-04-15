# Comparing `tmp/momoa-0.2.1.tar.gz` & `tmp/momoa-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "momoa-0.2.1.tar", last modified: Thu Apr 20 15:03:06 2023, max compression
+gzip compressed data, was "momoa-0.2.3.tar", last modified: Mon Apr 15 23:20:47 2024, max compression
```

## Comparing `momoa-0.2.1.tar` & `momoa-0.2.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1244 2023-04-20 15:02:55.984472 momoa-0.2.1/README.md
--rw-r--r--   0        0        0     3125 2023-04-20 15:02:55.984472 momoa-0.2.1/momoa/__init__.py
--rw-r--r--   0        0        0      294 2023-04-20 15:02:55.984472 momoa-0.2.1/momoa/exceptions.py
--rw-r--r--   0        0        0     1977 2023-04-20 15:02:55.984472 momoa-0.2.1/momoa/format.py
--rw-r--r--   0        0        0     4278 2023-04-20 15:02:55.984472 momoa-0.2.1/momoa/model.py
--rw-r--r--   0        0        0        0 2023-04-20 15:02:55.984472 momoa-0.2.1/momoa/py.typed
--rw-r--r--   0        0        0     2605 2023-04-20 15:02:55.984472 momoa-0.2.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-20 15:02:55.984472 momoa-0.2.1/tests/__init__.py
--rw-r--r--   0        0        0      339 2023-04-20 15:02:55.984472 momoa-0.2.1/tests/conftest.py
--rw-r--r--   0        0        0      606 2023-04-20 15:02:55.984472 momoa-0.2.1/tests/test_data/action_description.json
--rw-r--r--   0        0        0      169 2023-04-20 15:02:55.984472 momoa-0.2.1/tests/test_data/action_input_schema.json
--rw-r--r--   0        0        0      180 2023-04-20 15:02:55.984472 momoa-0.2.1/tests/test_data/action_output_schema.json
--rw-r--r--   0        0        0     1410 2023-04-20 15:02:55.984472 momoa-0.2.1/tests/test_data/schema.json
--rw-r--r--   0        0        0      304 2023-04-20 15:02:55.984472 momoa-0.2.1/tests/test_data/valid.json
--rw-r--r--   0        0        0     4167 2023-04-20 15:02:55.984472 momoa-0.2.1/tests/test_deserialization.py
--rw-r--r--   0        0        0     2240 2023-04-20 15:02:55.984472 momoa-0.2.1/tests/test_format.py
--rw-r--r--   0        0        0     3476 2023-04-20 15:02:55.984472 momoa-0.2.1/tests/test_model.py
--rw-r--r--   0        0        0     1653 2023-04-20 15:02:55.984472 momoa-0.2.1/tests/test_schema.py
--rw-r--r--   0        0        0     3687 2023-04-20 15:02:55.984472 momoa-0.2.1/tests/test_serialization.py
--rw-r--r--   0        0        0     1660 1970-01-01 00:00:00.000000 momoa-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1244 2024-04-15 23:20:38.420282 momoa-0.2.3/README.md
+-rw-r--r--   0        0        0     3126 2024-04-15 23:20:38.420282 momoa-0.2.3/momoa/__init__.py
+-rw-r--r--   0        0        0      294 2024-04-15 23:20:38.420282 momoa-0.2.3/momoa/exceptions.py
+-rw-r--r--   0        0        0     1978 2024-04-15 23:20:38.420282 momoa-0.2.3/momoa/format.py
+-rw-r--r--   0        0        0     4272 2024-04-15 23:20:38.420282 momoa-0.2.3/momoa/model.py
+-rw-r--r--   0        0        0        0 2024-04-15 23:20:38.420282 momoa-0.2.3/momoa/py.typed
+-rw-r--r--   0        0        0     3615 2024-04-15 23:20:47.136371 momoa-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-15 23:20:38.420282 momoa-0.2.3/tests/__init__.py
+-rw-r--r--   0        0        0      339 2024-04-15 23:20:38.420282 momoa-0.2.3/tests/conftest.py
+-rw-r--r--   0        0        0      606 2024-04-15 23:20:38.420282 momoa-0.2.3/tests/test_data/action_description.json
+-rw-r--r--   0        0        0      169 2024-04-15 23:20:38.420282 momoa-0.2.3/tests/test_data/action_input_schema.json
+-rw-r--r--   0        0        0      180 2024-04-15 23:20:38.420282 momoa-0.2.3/tests/test_data/action_output_schema.json
+-rw-r--r--   0        0        0     1410 2024-04-15 23:20:38.420282 momoa-0.2.3/tests/test_data/schema.json
+-rw-r--r--   0        0        0      304 2024-04-15 23:20:38.420282 momoa-0.2.3/tests/test_data/valid.json
+-rw-r--r--   0        0        0     4167 2024-04-15 23:20:38.420282 momoa-0.2.3/tests/test_deserialization.py
+-rw-r--r--   0        0        0     2240 2024-04-15 23:20:38.420282 momoa-0.2.3/tests/test_format.py
+-rw-r--r--   0        0        0     3476 2024-04-15 23:20:38.420282 momoa-0.2.3/tests/test_model.py
+-rw-r--r--   0        0        0     1653 2024-04-15 23:20:38.420282 momoa-0.2.3/tests/test_schema.py
+-rw-r--r--   0        0        0     3687 2024-04-15 23:20:38.420282 momoa-0.2.3/tests/test_serialization.py
+-rw-r--r--   0        0        0     2420 1970-01-01 00:00:00.000000 momoa-0.2.3/PKG-INFO
```

### Comparing `momoa-0.2.1/README.md` & `momoa-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `momoa-0.2.1/momoa/__init__.py` & `momoa-0.2.3/momoa/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Basic class to parse a schema and prepare the model class."""
+
 from __future__ import annotations
 
 import json
 from copy import deepcopy
 from functools import cached_property
 from pathlib import Path
 from typing import Any, Dict, Mapping, Sequence, Type, Union
```

### Comparing `momoa-0.2.1/momoa/format.py` & `momoa-0.2.3/momoa/format.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 """Helper utilities for formatting serialized data."""
+
 from datetime import date, datetime
 from ipaddress import ip_address
 from typing import Any, Callable, cast, Mapping
 from uuid import UUID
 
 from dateutil.parser import isoparse
```

### Comparing `momoa-0.2.1/momoa/model.py` & `momoa-0.2.3/momoa/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 """Base wrapper class for building JSONSchema based models."""
+
 from __future__ import annotations
 
 from typing import Any, Callable, cast, Type
 
+from humps import pascalize
 from statham.schema.constants import NotPassed
 from statham.schema.elements import meta, String
 from statham.schema.exceptions import ValidationError
-from stringcase import pascalcase
 
 from .exceptions import DataValidationError
 from .format import StringFormat
 
 # Sentinel for unset values.
 UNDEFINED = NotPassed()
 
@@ -87,15 +88,15 @@
         Args:
             schema_class: Class derived from the JSONSchema.
             string_formatter: Class used to format strings.
 
         Returns:
             Subclass of the Model class.
         """
-        name = pascalcase(schema_class.__name__) + "Model"
+        name = pascalize(schema_class.__name__) + "Model"
         return cast(
             Type[Model],
             type(
                 name, (Model,), {"_schema_class": schema_class, "_formatter": string_formatter}
             ),
         )
```

### Comparing `momoa-0.2.1/pyproject.toml` & `momoa-0.2.3/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,79 +1,46 @@
 [project]
 name = "momoa"
-version = "0.2.1"
+version = "0.2.3"
 description = "A library for definition, validation and serialisation of Python objects based on JSONSchema specifications."
 readme = "README.md"
 authors = [
     { name = "Berislav Lopac", email = "berislav@lopac.net" },
 ]
+classifiers = [
+    "Development Status :: 4 - Beta",
+    "License :: OSI Approved :: MIT License",
+    "Operating System :: OS Independent",
+    "Programming Language :: Python :: 3.8",
+    "Programming Language :: Python :: 3.9",
+    "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
+    "Topic :: File Formats :: JSON :: JSON Schema",
+]
 requires-python = ">=3.8,<4.0"
 dependencies = [
     "statham-schema>=0.13.5",
-    "stringcase>=1.2.0",
     "python-dateutil>=2.8.2",
+    "pyhumps>=3.8.0",
 ]
 
 [project.license]
 text = "MIT"
 
-[project.urls]
-homepage = "https://momoa.readthedocs.io"
-repository = "https://github.com/berislavlopac/momoa"
-
-[tool.pdm.build]
-includes = [
-    "momoa/",
-]
-
-[tool.pdm.dev-dependencies]
+[project.optional-dependencies]
 docs = [
-    "mkdocs>=1.4.2",
-    "mkdocs-material>=9.0.9",
     "mkapi>=1.0.14",
-    "jinja2>=3.1.2",
-]
-test = [
-    "pytest>=7.2.1",
-    "pytest-cov>=4.0.0",
-    "pytest-spec>=3.2.0",
-    "mypy>=0.991",
-    "mutmut>=2.4.3",
-    "tox>=3.28.0",
-    "tox-pdm>=0.6.1",
-]
-checks = [
-    "black>=22.12.0",
-    "isort>=5.12.0",
-    "pydocstyle>=6.3.0",
-    "toml>=0.10.2",
-    "ruff>=0.0.238",
-]
-
-[tool.pdm.scripts.tests]
-cmd = "pytest --spec --cov"
-
-[tool.pdm.scripts.check-lint]
-shell = "    ruff .\n    black --check .\n    isort --check .\n"
-
-[tool.pdm.scripts.check-typing]
-cmd = "mypy --install-types --non-interactive momoa/"
-
-[tool.pdm.scripts.check-docs]
-cmd = "pydocstyle momoa/"
-
-[tool.pdm.scripts.checks]
-composite = [
-    "check-lint",
-    "check-typing",
-    "check-docs",
+    "mkdocs>=1.5.3",
+    "mkdocs-material>=9.5.17",
+    "jinja2>=3.1.3",
 ]
 
-[tool.pdm.scripts.new-commits]
-shell = "git log $(git describe --tags --abbrev=0)..HEAD --oneline --no-decorate"
+[project.urls]
+homepage = "https://momoa.readthedocs.io"
+repository = "https://github.com/berislavlopac/momoa"
 
 [tool.black]
 line-length = 96
 target-version = [
     "py38",
     "py39",
     "py310",
@@ -104,49 +71,115 @@
 exclude_lines = [
     "pragma: no cover",
     "@abstract",
 ]
 
 [tool.mypy]
 mypy_path = "momoa/"
+files = [
+    "momoa/",
+]
 ignore_missing_imports = true
 
 [tool.pydocstyle]
 add-ignore = "D105, D107, D212, D401"
 convention = "google"
 match-dir = "(?!tests).*"
 
 [tool.ruff]
+line-length = 96
+target-version = "py311"
+output-format = "grouped"
+
+[tool.ruff.lint]
 select = [
-    "E",
-    "F",
+    "E4",
+    "E7",
+    "E9",
     "W",
+    "F",
     "D",
-    "PL",
-    "ERA",
-    "N",
 ]
 ignore = [
     "D105",
     "D107",
     "D203",
     "D212",
     "D401",
     "D406",
     "D407",
+    "D413",
 ]
-line-length = 96
-target-version = "py38"
-format = "grouped"
 
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint.per-file-ignores]
 "tests/*" = [
     "D",
     "N",
     "PLR",
 ]
 
+[tool.pdm.build]
+includes = [
+    "momoa/",
+]
+
+[tool.pdm.dev-dependencies]
+test = [
+    "pytest>=7.2.1",
+    "pytest-cov>=4.0.0",
+    "pytest-spec>=3.2.0",
+    "tox>=3.28.0",
+    "tox-pdm>=0.6.1",
+]
+checks = [
+    "isort>=5.12.0",
+    "ruff>=0.0.238",
+]
+
+[tool.pdm.scripts.tests]
+cmd = "pytest --spec --cov"
+help = "Run unit tests and coverage."
+
+[tool.pdm.scripts.tests-quick]
+cmd = "pytest -m 'not api_request'"
+help = "Run unit tests without coverage and API request tests."
+
+[tool.pdm.scripts.check-lint]
+shell = "    ruff format --check .\n    isort --check .\n    ruff check .\n"
+help = "Run linting and formating checks."
+
+[tool.pdm.scripts.check-typing]
+cmd = "mypy --install-types --non-interactive"
+help = "Run static typing analysis."
+
+[tool.pdm.scripts.checks]
+composite = [
+    "check-lint",
+    "check-typing",
+]
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
+
+[tool.pdm.scripts.new-commits]
+shell = "git log $(git describe --tags --abbrev=0)..HEAD --oneline --no-decorate"
+help = "List all commits since the last tag."
+
 [build-system]
 requires = [
-    "pdm-pep517>=1.0.0",
+    "pdm-backend",
 ]
-build-backend = "pdm.pep517.api"
+build-backend = "pdm.backend"
```

### Comparing `momoa-0.2.1/tests/test_data/action_description.json` & `momoa-0.2.3/tests/test_data/action_description.json`

 * *Files identical despite different names*

### Comparing `momoa-0.2.1/tests/test_data/schema.json` & `momoa-0.2.3/tests/test_data/schema.json`

 * *Files identical despite different names*

### Comparing `momoa-0.2.1/tests/test_deserialization.py` & `momoa-0.2.3/tests/test_deserialization.py`

 * *Files identical despite different names*

### Comparing `momoa-0.2.1/tests/test_format.py` & `momoa-0.2.3/tests/test_format.py`

 * *Files identical despite different names*

### Comparing `momoa-0.2.1/tests/test_model.py` & `momoa-0.2.3/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `momoa-0.2.1/tests/test_schema.py` & `momoa-0.2.3/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `momoa-0.2.1/tests/test_serialization.py` & `momoa-0.2.3/tests/test_serialization.py`

 * *Files identical despite different names*

