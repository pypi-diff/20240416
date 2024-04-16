# Comparing `tmp/pydantic_async_validation-0.1.2.tar.gz` & `tmp/pydantic_async_validation-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pydantic_async_validation-0.1.2.tar", max compression
+gzip compressed data, was "pydantic_async_validation-0.1.3.tar", max compression
```

## Comparing `pydantic_async_validation-0.1.2.tar` & `pydantic_async_validation-0.1.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1077 2024-01-04 20:53:26.037105 pydantic_async_validation-0.1.2/LICENSE
--rw-r--r--   0        0        0     9023 2024-01-04 20:53:26.037105 pydantic_async_validation-0.1.2/README.md
--rw-r--r--   0        0        0      181 2024-01-04 20:53:26.037105 pydantic_async_validation-0.1.2/pydantic_async_validation/__init__.py
--rw-r--r--   0        0        0      445 2024-01-04 20:53:26.037105 pydantic_async_validation-0.1.2/pydantic_async_validation/constants.py
--rw-r--r--   0        0        0      950 2024-01-04 20:53:26.037105 pydantic_async_validation-0.1.2/pydantic_async_validation/fastapi.py
--rw-r--r--   0        0        0     2491 2024-01-04 20:53:26.037105 pydantic_async_validation-0.1.2/pydantic_async_validation/metaclasses.py
--rw-r--r--   0        0        0     4998 2024-01-04 20:53:26.037105 pydantic_async_validation-0.1.2/pydantic_async_validation/mixins.py
--rw-r--r--   0        0        0     6307 2024-01-04 20:53:26.037105 pydantic_async_validation-0.1.2/pydantic_async_validation/utils.py
--rw-r--r--   0        0        0     2857 2024-01-04 20:53:26.037105 pydantic_async_validation-0.1.2/pydantic_async_validation/validators.py
--rw-r--r--   0        0        0     1142 2024-01-04 20:53:26.037105 pydantic_async_validation-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     9785 1970-01-01 00:00:00.000000 pydantic_async_validation-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1077 2024-04-16 09:12:39.894928 pydantic_async_validation-0.1.3/LICENSE
+-rw-r--r--   0        0        0     9023 2024-04-16 09:12:39.894928 pydantic_async_validation-0.1.3/README.md
+-rw-r--r--   0        0        0      181 2024-04-16 09:12:39.894928 pydantic_async_validation-0.1.3/pydantic_async_validation/__init__.py
+-rw-r--r--   0        0        0      445 2024-04-16 09:12:39.894928 pydantic_async_validation-0.1.3/pydantic_async_validation/constants.py
+-rw-r--r--   0        0        0      950 2024-04-16 09:12:39.894928 pydantic_async_validation-0.1.3/pydantic_async_validation/fastapi.py
+-rw-r--r--   0        0        0     2491 2024-04-16 09:12:39.894928 pydantic_async_validation-0.1.3/pydantic_async_validation/metaclasses.py
+-rw-r--r--   0        0        0     4998 2024-04-16 09:12:39.894928 pydantic_async_validation-0.1.3/pydantic_async_validation/mixins.py
+-rw-r--r--   0        0        0     6347 2024-04-16 09:12:39.894928 pydantic_async_validation-0.1.3/pydantic_async_validation/utils.py
+-rw-r--r--   0        0        0     2857 2024-04-16 09:12:39.894928 pydantic_async_validation-0.1.3/pydantic_async_validation/validators.py
+-rw-r--r--   0        0        0     1172 2024-04-16 09:12:39.894928 pydantic_async_validation-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     9781 1970-01-01 00:00:00.000000 pydantic_async_validation-0.1.3/PKG-INFO
```

### Comparing `pydantic_async_validation-0.1.2/LICENSE` & `pydantic_async_validation-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pydantic_async_validation-0.1.2/README.md` & `pydantic_async_validation-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `pydantic_async_validation-0.1.2/pydantic_async_validation/fastapi.py` & `pydantic_async_validation-0.1.3/pydantic_async_validation/fastapi.py`

 * *Files identical despite different names*

### Comparing `pydantic_async_validation-0.1.2/pydantic_async_validation/metaclasses.py` & `pydantic_async_validation-0.1.3/pydantic_async_validation/metaclasses.py`

 * *Files identical despite different names*

### Comparing `pydantic_async_validation-0.1.2/pydantic_async_validation/mixins.py` & `pydantic_async_validation-0.1.3/pydantic_async_validation/mixins.py`

 * *Files identical despite different names*

### Comparing `pydantic_async_validation-0.1.2/pydantic_async_validation/utils.py` & `pydantic_async_validation-0.1.3/pydantic_async_validation/utils.py`

 * *Files 5% similar despite different names*

```diff
@@ -178,28 +178,28 @@
             InitErrorDetails,
             {
                 # Original data is ErrorDetails, we need to convert it back to
                 # InitErrorDetails
                 **error,
                 'type': (
                     PydanticCustomError(
-                        error['type'],
-                        cast(ErrorDetails, error)['msg'],
+                        error['type'],  # type: ignore
+                        cast(ErrorDetails, error)['msg'],  # type: ignore
                     )
                     if isinstance(error['type'], str)
                     else error['type']
                 ),
                 'loc': (*prefix, *error['loc']),
             },
         )
         if "msg" in error
         else cast(
             InitErrorDetails,
             {
                 # Original data is InitErrorDetails, all fine
                 **error,
-                'loc': (*prefix, *error['loc']),
+                'loc': (*prefix, *error.get('loc', [])),
             },
         )
         for error
         in errors
     ]
```

### Comparing `pydantic_async_validation-0.1.2/pydantic_async_validation/validators.py` & `pydantic_async_validation-0.1.3/pydantic_async_validation/validators.py`

 * *Files identical despite different names*

### Comparing `pydantic_async_validation-0.1.2/pyproject.toml` & `pydantic_async_validation-0.1.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,42 +1,44 @@
 [tool.poetry]
 name = "pydantic-async-validation"
-version = "0.1.2"
+version = "0.1.3"
 description = "Add async validation to pydantic"
 authors = ["TEAM23 GmbH <info@team23.de>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "pydantic_async_validation"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 pydantic = ">=2.0.0,<3.0.0"
 fastapi = {version = ">=0.100.0,<1.0.0", optional = true}
-pytest = "^7.4.0"
+pytest = ">=7.4,<9.0"
 
 [tool.poetry.extras]
 fastapi = ["fastapi"]
 
 [tool.poetry.group.dev.dependencies]
-pytest = ">=7.1.2,<8.0.0"
-pytest-cov = ">=3,<5"
+pytest = ">=7.1.2,<9.0.0"
+pytest-cov = ">=3,<6"
 pytest-asyncio = ">=0.21.1,<0.24.0"
-mypy = ">=0.971,<2.0"
 tox = ">=3.26,<5.0"
-httpx = ">=0.24.1,<0.27.0"
-ruff = ">=0.0.284,<0.2.0"
+httpx = ">=0.24.1,<0.28.0"
+ruff = ">=0.2.0,<0.4.0"
+pyright = ">=1.1.350,<1.2"
 
 [tool.ruff]
-select = ["F","E","W","C","I","N","UP","ANN","S","B","A","COM","C4","T20","PT","ARG","TD","RUF"]
 line-length = 115
 target-version = "py38"
-ignore = ["A001","A002","A003","ANN101","ANN102","ANN401","C901","N8","B008","F405","F821"]
 output-format = "grouped"
 
-[tool.ruff.per-file-ignores]
+[tool.ruff.lint]
+select = ["F","E","W","C","I","N","UP","ANN","S","B","A","COM","C4","T20","PT","ARG","TD","RUF"]
+ignore = ["A001","A002","A003","ANN101","ANN102","ANN401","C901","N8","B008","F405","F821"]
+
+[tool.ruff.lint.per-file-ignores]
 "__init__.py" = ["F401"]
 "conftest.py" = ["S101","ANN","F401"]
 "test_*.py" = ["S101","ANN","F401"]
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pydantic_async_validation-0.1.2/PKG-INFO` & `pydantic_async_validation-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pydantic-async-validation
-Version: 0.1.2
+Version: 0.1.3
 Summary: Add async validation to pydantic
 License: MIT
 Author: TEAM23 GmbH
 Author-email: info@team23.de
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
@@ -12,15 +12,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Provides-Extra: fastapi
 Requires-Dist: fastapi (>=0.100.0,<1.0.0) ; extra == "fastapi"
 Requires-Dist: pydantic (>=2.0.0,<3.0.0)
-Requires-Dist: pytest (>=7.4.0,<8.0.0)
+Requires-Dist: pytest (>=7.4,<9.0)
 Description-Content-Type: text/markdown
 
 # `pydantic-async-validation`
 
 Add async validation to your pydantic models 🥳. This allows you to add validation that actually checks the database
 or makes an API call or just use any code you did write async.
```

