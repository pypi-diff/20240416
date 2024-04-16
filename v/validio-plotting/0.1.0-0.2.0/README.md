# Comparing `tmp/validio_plotting-0.1.0.tar.gz` & `tmp/validio_plotting-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "validio_plotting-0.1.0.tar", max compression
+gzip compressed data, was "validio_plotting-0.2.0.tar", max compression
```

## Comparing `validio_plotting-0.1.0.tar` & `validio_plotting-0.2.0.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0      305 2024-01-08 13:33:36.726746 validio_plotting-0.1.0/README.md
--rw-r--r--   0        0        0     1918 2024-01-08 13:33:36.727442 validio_plotting-0.1.0/pyproject.toml
--rw-r--r--   0        0        0    10937 2024-01-08 13:33:36.727746 validio_plotting-0.1.0/validio_plotting/main.py
--rw-r--r--   0        0        0      984 1970-01-01 00:00:00.000000 validio_plotting-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      305 2024-01-15 08:43:33.692614 validio_plotting-0.2.0/README.md
+-rw-r--r--   0        0        0     1870 2024-04-16 09:40:37.872851 validio_plotting-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0    10986 2024-01-15 08:43:33.693916 validio_plotting-0.2.0/validio_plotting/main.py
+-rw-r--r--   0        0        0     1019 1970-01-01 00:00:00.000000 validio_plotting-0.2.0/PKG-INFO
```

### Comparing `validio_plotting-0.1.0/pyproject.toml` & `validio_plotting-0.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,28 @@
 [tool.poetry]
 name = "validio-plotting"
-version = "0.1.0"
+version = "0.2.0"
 description = "App to graph  metrics from Validio SDK"
 authors = ["Validio <support@validio.io>"]
 license = "Apache-2.0"
-packages = [{include = "validio_plotting"}]
+packages = [{ include = "validio_plotting" }]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
-validio-sdk = "^0.13.1"
 typer = "^0.7.0"
 prompt-toolkit = "^3.0.43"
-validio-cli = "^0.13.1"
+validio-cli = "0.17.0"
+validio-sdk = "0.17.0"
 plotext = "^5.2.8"
 
 
 [tool.poetry.group.dev.dependencies]
 ruff = "^0.1.11"
 pytest = "^7.4.4"
-black = "^23.12.1"
 mypy = "^1.8.0"
 licensecheck = "^2023.1.1"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
@@ -66,17 +65,14 @@
 ]
 
 "*/tests/*.py" = ["D"]
 
 [tool.ruff.pydocstyle]
 convention = "google"
 
-[tool.black]
-preview = true
-
 [tool.mypy]
 ignore_missing_imports = true
 disallow_untyped_calls = true
 disallow_untyped_defs = true
 disallow_incomplete_defs = true
 check_untyped_defs = true
 disallow_untyped_decorators = false
```

### Comparing `validio_plotting-0.1.0/validio_plotting/main.py` & `validio_plotting-0.2.0/validio_plotting/main.py`

 * *Files 1% similar despite different names*

```diff
@@ -184,17 +184,20 @@
                 pass
 
         if events.done.is_set():
             break
 
         if events.graph.is_set():
             events.graph.clear()
-            source_id, validator_id, segment_id, start_idx = (
-                await _get_validator_and_segment(vc, start_idx=start_idx)
-            )
+            (
+                source_id,
+                validator_id,
+                segment_id,
+                start_idx,
+            ) = await _get_validator_and_segment(vc, start_idx=start_idx)
 
         if events.history.is_set():
             events.history.clear()
             while True:
                 with contextlib.suppress(ValueError):
                     print()
                     historical_minutes = int(input("Historical minutes: "))
```

### Comparing `validio_plotting-0.1.0/PKG-INFO` & `validio_plotting-0.2.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: validio-plotting
-Version: 0.1.0
+Version: 0.2.0
 Summary: App to graph  metrics from Validio SDK
 License: Apache-2.0
 Author: Validio
 Author-email: support@validio.io
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: plotext (>=5.2.8,<6.0.0)
 Requires-Dist: prompt-toolkit (>=3.0.43,<4.0.0)
 Requires-Dist: typer (>=0.7.0,<0.8.0)
-Requires-Dist: validio-cli (>=0.13.1,<0.14.0)
-Requires-Dist: validio-sdk (>=0.13.1,<0.14.0)
+Requires-Dist: validio-cli (==0.17.0)
+Requires-Dist: validio-sdk (==0.17.0)
 Description-Content-Type: text/markdown
 
 # validio-plotting
 
 This is a tool that uses the [`validio-sdk`] to fetch metrics and plot them in
 the terminal.
```

