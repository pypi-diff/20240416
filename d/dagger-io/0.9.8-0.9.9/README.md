# Comparing `tmp/dagger_io-0.9.8.tar.gz` & `tmp/dagger_io-0.9.9.tar.gz`

## Comparing `dagger_io-0.9.8.tar` & `dagger_io-0.9.9.tar`

### file list

```diff
@@ -1,63 +1,63 @@
--rw-r--r--   0        0        0    13965 2020-02-02 00:00:00.000000 dagger_io-0.9.8/CHANGELOG.md
--rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 dagger_io-0.9.8/docs/client.rst
--rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 dagger_io-0.9.8/docs/conf.py
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 dagger_io-0.9.8/docs/connection.rst
--rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 dagger_io-0.9.8/docs/exceptions.rst
--rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 dagger_io-0.9.8/docs/index.rst
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 dagger_io-0.9.8/docs/module.rst
--rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 dagger_io-0.9.8/docs/_ext/dagger_ext.py
--rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 dagger_io-0.9.8/src/dagger/__init__.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 dagger_io-0.9.8/src/dagger/__main__.py
--rw-r--r--   0        0        0     3204 2020-02-02 00:00:00.000000 dagger_io-0.9.8/src/dagger/_config.py
--rw-r--r--   0        0        0     3277 2020-02-02 00:00:00.000000 dagger_io-0.9.8/src/dagger/_connection.py
--rw-r--r--   0        0        0     5349 2020-02-02 00:00:00.000000 dagger_io-0.9.8/src/dagger/_exceptions.py
--rw-r--r--   0        0        0     1449 2020-02-02 00:00:00.000000 dagger_io-0.9.8/src/dagger/_managers.py
--rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 dagger_io-0.9.8/src/dagger/log.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dagger_io-0.9.8/src/dagger/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dagger_io-0.9.8/src/dagger/_codegen/__init__.py
--rw-r--r--   0        0        0     1764 2020-02-02 00:00:00.000000 dagger_io-0.9.8/src/dagger/_codegen/cli.py
--rw-r--r--   0        0        0    27506 2020-02-02 00:00:00.000000 dagger_io-0.9.8/src/dagger/_codegen/generator.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dagger_io-0.9.8/src/dagger/_engine/__init__.py
--rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 dagger_io-0.9.8/src/dagger/_engine/_version.py
--rw-r--r--   0        0        0     4821 2020-02-02 00:00:00.000000 dagger_io-0.9.8/src/dagger/_engine/conn.py
--rw-r--r--   0        0        0     8912 2020-02-02 00:00:00.000000 dagger_io-0.9.8/src/dagger/_engine/download.py
--rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 dagger_io-0.9.8/src/dagger/_engine/progress.py
--rw-r--r--   0        0        0     3822 2020-02-02 00:00:00.000000 dagger_io-0.9.8/src/dagger/_engine/session.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dagger_io-0.9.8/src/dagger/client/__init__.py
--rw-r--r--   0        0        0     8592 2020-02-02 00:00:00.000000 dagger_io-0.9.8/src/dagger/client/_core.py
--rw-r--r--   0        0        0     3694 2020-02-02 00:00:00.000000 dagger_io-0.9.8/src/dagger/client/_guards.py
--rw-r--r--   0        0        0     7551 2020-02-02 00:00:00.000000 dagger_io-0.9.8/src/dagger/client/_session.py
--rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 dagger_io-0.9.8/src/dagger/client/base.py
--rw-r--r--   0        0        0   184794 2020-02-02 00:00:00.000000 dagger_io-0.9.8/src/dagger/client/gen.py
--rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 dagger_io-0.9.8/src/dagger/mod/__init__.py
--rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 dagger_io-0.9.8/src/dagger/mod/_arguments.py
--rw-r--r--   0        0        0     3487 2020-02-02 00:00:00.000000 dagger_io-0.9.8/src/dagger/mod/_converter.py
--rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 dagger_io-0.9.8/src/dagger/mod/_exceptions.py
--rw-r--r--   0        0        0    17334 2020-02-02 00:00:00.000000 dagger_io-0.9.8/src/dagger/mod/_module.py
--rw-r--r--   0        0        0    12362 2020-02-02 00:00:00.000000 dagger_io-0.9.8/src/dagger/mod/_resolver.py
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 dagger_io-0.9.8/src/dagger/mod/_types.py
--rw-r--r--   0        0        0     4696 2020-02-02 00:00:00.000000 dagger_io-0.9.8/src/dagger/mod/_utils.py
--rw-r--r--   0        0        0     2395 2020-02-02 00:00:00.000000 dagger_io-0.9.8/src/dagger/mod/cli.py
--rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 dagger_io-0.9.8/tests/conftest.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dagger_io-0.9.8/tests/client/__init__.py
--rw-r--r--   0        0        0     8224 2020-02-02 00:00:00.000000 dagger_io-0.9.8/tests/client/test_codegen.py
--rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 dagger_io-0.9.8/tests/client/test_config.py
--rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 dagger_io-0.9.8/tests/client/test_connection_errors.py
--rw-r--r--   0        0        0     3378 2020-02-02 00:00:00.000000 dagger_io-0.9.8/tests/client/test_default_client.py
--rw-r--r--   0        0        0     3827 2020-02-02 00:00:00.000000 dagger_io-0.9.8/tests/client/test_execute_errors.py
--rw-r--r--   0        0        0     4145 2020-02-02 00:00:00.000000 dagger_io-0.9.8/tests/client/test_inputs.py
--rw-r--r--   0        0        0     6502 2020-02-02 00:00:00.000000 dagger_io-0.9.8/tests/client/test_integration.py
--rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 dagger_io-0.9.8/tests/client/test_integration_connection.py
--rw-r--r--   0        0        0     1423 2020-02-02 00:00:00.000000 dagger_io-0.9.8/tests/client/test_response.py
--rw-r--r--   0        0        0     2145 2020-02-02 00:00:00.000000 dagger_io-0.9.8/tests/engine/test_cli.py
--rw-r--r--   0        0        0     5128 2020-02-02 00:00:00.000000 dagger_io-0.9.8/tests/engine/test_download.py
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 dagger_io-0.9.8/tests/modules/test_forward_reference.py
--rw-r--r--   0        0        0     2453 2020-02-02 00:00:00.000000 dagger_io-0.9.8/tests/modules/test_registration.py
--rw-r--r--   0        0        0    11705 2020-02-02 00:00:00.000000 dagger_io-0.9.8/tests/modules/test_results.py
--rw-r--r--   0        0        0     2415 2020-02-02 00:00:00.000000 dagger_io-0.9.8/tests/modules/test_utils.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 dagger_io-0.9.8/.gitignore
--rw-r--r--   0        0        0    10758 2020-02-02 00:00:00.000000 dagger_io-0.9.8/LICENSE
--rw-r--r--   0        0        0     4223 2020-02-02 00:00:00.000000 dagger_io-0.9.8/README.md
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 dagger_io-0.9.8/hatch.toml
--rw-r--r--   0        0        0     4991 2020-02-02 00:00:00.000000 dagger_io-0.9.8/pyproject.toml
--rw-r--r--   0        0        0     5744 2020-02-02 00:00:00.000000 dagger_io-0.9.8/PKG-INFO
+-rw-r--r--   0        0        0    14562 2020-02-02 00:00:00.000000 dagger_io-0.9.9/CHANGELOG.md
+-rw-r--r--   0        0        0      119 2020-02-02 00:00:00.000000 dagger_io-0.9.9/docs/client.rst
+-rw-r--r--   0        0        0      886 2020-02-02 00:00:00.000000 dagger_io-0.9.9/docs/conf.py
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 dagger_io-0.9.9/docs/connection.rst
+-rw-r--r--   0        0        0      694 2020-02-02 00:00:00.000000 dagger_io-0.9.9/docs/exceptions.rst
+-rw-r--r--   0        0        0      838 2020-02-02 00:00:00.000000 dagger_io-0.9.9/docs/index.rst
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 dagger_io-0.9.9/docs/module.rst
+-rw-r--r--   0        0        0     1236 2020-02-02 00:00:00.000000 dagger_io-0.9.9/docs/_ext/dagger_ext.py
+-rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 dagger_io-0.9.9/src/dagger/__init__.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 dagger_io-0.9.9/src/dagger/__main__.py
+-rw-r--r--   0        0        0     3204 2020-02-02 00:00:00.000000 dagger_io-0.9.9/src/dagger/_config.py
+-rw-r--r--   0        0        0     3277 2020-02-02 00:00:00.000000 dagger_io-0.9.9/src/dagger/_connection.py
+-rw-r--r--   0        0        0     5349 2020-02-02 00:00:00.000000 dagger_io-0.9.9/src/dagger/_exceptions.py
+-rw-r--r--   0        0        0     1449 2020-02-02 00:00:00.000000 dagger_io-0.9.9/src/dagger/_managers.py
+-rw-r--r--   0        0        0      999 2020-02-02 00:00:00.000000 dagger_io-0.9.9/src/dagger/log.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dagger_io-0.9.9/src/dagger/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dagger_io-0.9.9/src/dagger/_codegen/__init__.py
+-rw-r--r--   0        0        0     1764 2020-02-02 00:00:00.000000 dagger_io-0.9.9/src/dagger/_codegen/cli.py
+-rw-r--r--   0        0        0    27506 2020-02-02 00:00:00.000000 dagger_io-0.9.9/src/dagger/_codegen/generator.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dagger_io-0.9.9/src/dagger/_engine/__init__.py
+-rw-r--r--   0        0        0       64 2020-02-02 00:00:00.000000 dagger_io-0.9.9/src/dagger/_engine/_version.py
+-rw-r--r--   0        0        0     4821 2020-02-02 00:00:00.000000 dagger_io-0.9.9/src/dagger/_engine/conn.py
+-rw-r--r--   0        0        0     8912 2020-02-02 00:00:00.000000 dagger_io-0.9.9/src/dagger/_engine/download.py
+-rw-r--r--   0        0        0     1040 2020-02-02 00:00:00.000000 dagger_io-0.9.9/src/dagger/_engine/progress.py
+-rw-r--r--   0        0        0     3822 2020-02-02 00:00:00.000000 dagger_io-0.9.9/src/dagger/_engine/session.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dagger_io-0.9.9/src/dagger/client/__init__.py
+-rw-r--r--   0        0        0     8592 2020-02-02 00:00:00.000000 dagger_io-0.9.9/src/dagger/client/_core.py
+-rw-r--r--   0        0        0     3694 2020-02-02 00:00:00.000000 dagger_io-0.9.9/src/dagger/client/_guards.py
+-rw-r--r--   0        0        0     7551 2020-02-02 00:00:00.000000 dagger_io-0.9.9/src/dagger/client/_session.py
+-rw-r--r--   0        0        0      991 2020-02-02 00:00:00.000000 dagger_io-0.9.9/src/dagger/client/base.py
+-rw-r--r--   0        0        0   195351 2020-02-02 00:00:00.000000 dagger_io-0.9.9/src/dagger/client/gen.py
+-rw-r--r--   0        0        0      489 2020-02-02 00:00:00.000000 dagger_io-0.9.9/src/dagger/mod/__init__.py
+-rw-r--r--   0        0        0      745 2020-02-02 00:00:00.000000 dagger_io-0.9.9/src/dagger/mod/_arguments.py
+-rw-r--r--   0        0        0     3803 2020-02-02 00:00:00.000000 dagger_io-0.9.9/src/dagger/mod/_converter.py
+-rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 dagger_io-0.9.9/src/dagger/mod/_exceptions.py
+-rw-r--r--   0        0        0    17360 2020-02-02 00:00:00.000000 dagger_io-0.9.9/src/dagger/mod/_module.py
+-rw-r--r--   0        0        0    12510 2020-02-02 00:00:00.000000 dagger_io-0.9.9/src/dagger/mod/_resolver.py
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 dagger_io-0.9.9/src/dagger/mod/_types.py
+-rw-r--r--   0        0        0     4691 2020-02-02 00:00:00.000000 dagger_io-0.9.9/src/dagger/mod/_utils.py
+-rw-r--r--   0        0        0     2395 2020-02-02 00:00:00.000000 dagger_io-0.9.9/src/dagger/mod/cli.py
+-rw-r--r--   0        0        0      186 2020-02-02 00:00:00.000000 dagger_io-0.9.9/tests/conftest.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 dagger_io-0.9.9/tests/client/__init__.py
+-rw-r--r--   0        0        0     8224 2020-02-02 00:00:00.000000 dagger_io-0.9.9/tests/client/test_codegen.py
+-rw-r--r--   0        0        0      946 2020-02-02 00:00:00.000000 dagger_io-0.9.9/tests/client/test_config.py
+-rw-r--r--   0        0        0     1581 2020-02-02 00:00:00.000000 dagger_io-0.9.9/tests/client/test_connection_errors.py
+-rw-r--r--   0        0        0     3378 2020-02-02 00:00:00.000000 dagger_io-0.9.9/tests/client/test_default_client.py
+-rw-r--r--   0        0        0     3827 2020-02-02 00:00:00.000000 dagger_io-0.9.9/tests/client/test_execute_errors.py
+-rw-r--r--   0        0        0     4145 2020-02-02 00:00:00.000000 dagger_io-0.9.9/tests/client/test_inputs.py
+-rw-r--r--   0        0        0     6502 2020-02-02 00:00:00.000000 dagger_io-0.9.9/tests/client/test_integration.py
+-rw-r--r--   0        0        0      811 2020-02-02 00:00:00.000000 dagger_io-0.9.9/tests/client/test_integration_connection.py
+-rw-r--r--   0        0        0     1423 2020-02-02 00:00:00.000000 dagger_io-0.9.9/tests/client/test_response.py
+-rw-r--r--   0        0        0     2145 2020-02-02 00:00:00.000000 dagger_io-0.9.9/tests/engine/test_cli.py
+-rw-r--r--   0        0        0     5128 2020-02-02 00:00:00.000000 dagger_io-0.9.9/tests/engine/test_download.py
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 dagger_io-0.9.9/tests/modules/test_forward_reference.py
+-rw-r--r--   0        0        0     2873 2020-02-02 00:00:00.000000 dagger_io-0.9.9/tests/modules/test_registration.py
+-rw-r--r--   0        0        0    12355 2020-02-02 00:00:00.000000 dagger_io-0.9.9/tests/modules/test_results.py
+-rw-r--r--   0        0        0     2586 2020-02-02 00:00:00.000000 dagger_io-0.9.9/tests/modules/test_utils.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 dagger_io-0.9.9/.gitignore
+-rw-r--r--   0        0        0    10758 2020-02-02 00:00:00.000000 dagger_io-0.9.9/LICENSE
+-rw-r--r--   0        0        0     4223 2020-02-02 00:00:00.000000 dagger_io-0.9.9/README.md
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 dagger_io-0.9.9/hatch.toml
+-rw-r--r--   0        0        0     4991 2020-02-02 00:00:00.000000 dagger_io-0.9.9/pyproject.toml
+-rw-r--r--   0        0        0     5744 2020-02-02 00:00:00.000000 dagger_io-0.9.9/PKG-INFO
```

### Comparing `dagger_io-0.9.8/CHANGELOG.md` & `dagger_io-0.9.9/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -3,14 +3,32 @@
 
 The format is based on [Keep a Changelog](https://keepachangelog.com/en/1.0.0/),
 adheres to [Semantic Versioning](https://semver.org/spec/v2.0.0.html),
 and is generated by [Changie](https://github.com/miniscruff/changie).
 
 
 
+## sdk/python/v0.9.9 - 2024-02-09
+
+This SDK uses 🚙 Engine + 🚗 CLI version `v0.9.9`. [See what changed in that release](https://github.com/dagger/dagger/releases/tag/v0.9.9).
+
+🐍 https://pypi.org/project/dagger-io/v0.9.9/
+📖 https://dagger-io.readthedocs.io/en/sdk-python-v0.9.9/
+
+
+### Dependencies
+- Bump Engine to v0.9.9 by @github-actions in https://github.com/dagger/dagger/pull/6636
+
+### What to do next
+- Read the [documentation](https://docs.dagger.io/sdk/python)
+- Join our [Discord server](https://discord.gg/dagger-io)
+- Follow us on [Twitter](https://twitter.com/dagger_io)
+
+
+
 ## sdk/python/v0.9.8 - 2024-02-01
 
 This SDK uses 🚙 Engine + 🚗 CLI version `v0.9.8`. [See what changed in that release](https://github.com/dagger/dagger/releases/tag/v0.9.8).
 
 🐍 https://pypi.org/project/dagger-io/v0.9.8/
 📖 https://dagger-io.readthedocs.io/en/sdk-python-v0.9.8/
```

### Comparing `dagger_io-0.9.8/docs/conf.py` & `dagger_io-0.9.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.9.8/docs/exceptions.rst` & `dagger_io-0.9.9/docs/exceptions.rst`

 * *Files identical despite different names*

### Comparing `dagger_io-0.9.8/docs/index.rst` & `dagger_io-0.9.9/docs/index.rst`

 * *Files identical despite different names*

### Comparing `dagger_io-0.9.8/docs/_ext/dagger_ext.py` & `dagger_io-0.9.9/docs/_ext/dagger_ext.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.9.8/src/dagger/__init__.py` & `dagger_io-0.9.9/src/dagger/__init__.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.9.8/src/dagger/_config.py` & `dagger_io-0.9.9/src/dagger/_config.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.9.8/src/dagger/_connection.py` & `dagger_io-0.9.9/src/dagger/_connection.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.9.8/src/dagger/_exceptions.py` & `dagger_io-0.9.9/src/dagger/_exceptions.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.9.8/src/dagger/_managers.py` & `dagger_io-0.9.9/src/dagger/_managers.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.9.8/src/dagger/log.py` & `dagger_io-0.9.9/src/dagger/log.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.9.8/src/dagger/_codegen/cli.py` & `dagger_io-0.9.9/src/dagger/_codegen/cli.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.9.8/src/dagger/_codegen/generator.py` & `dagger_io-0.9.9/src/dagger/_codegen/generator.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.9.8/src/dagger/_engine/conn.py` & `dagger_io-0.9.9/src/dagger/_engine/conn.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.9.8/src/dagger/_engine/download.py` & `dagger_io-0.9.9/src/dagger/_engine/download.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.9.8/src/dagger/_engine/progress.py` & `dagger_io-0.9.9/src/dagger/_engine/progress.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.9.8/src/dagger/_engine/session.py` & `dagger_io-0.9.9/src/dagger/_engine/session.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.9.8/src/dagger/client/_core.py` & `dagger_io-0.9.9/src/dagger/client/_core.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.9.8/src/dagger/client/_guards.py` & `dagger_io-0.9.9/src/dagger/client/_guards.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.9.8/src/dagger/client/_session.py` & `dagger_io-0.9.9/src/dagger/client/_session.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.9.8/src/dagger/client/base.py` & `dagger_io-0.9.9/src/dagger/client/base.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.9.8/src/dagger/client/gen.py` & `dagger_io-0.9.9/src/dagger/client/gen.py`

 * *Files 3% similar despite different names*

```diff
@@ -917,35 +917,14 @@
     def rootfs(self) -> "Directory":
         """Retrieves this container's root filesystem. Mounts are not included."""
         _args: list[Arg] = []
         _ctx = self._select("rootfs", _args)
         return Directory(_ctx)
 
     @typecheck
-    def shell(
-        self,
-        *,
-        args: Sequence[str] | None = None,
-    ) -> "Terminal":
-        """Return an interactive terminal for this container using its configured
-        shell if not overridden by args (or sh as a fallback default).
-
-        Parameters
-        ----------
-        args:
-            If set, override the container's default shell and invoke these
-            arguments instead.
-        """
-        _args = [
-            Arg("args", args, None),
-        ]
-        _ctx = self._select("shell", _args)
-        return Terminal(_ctx)
-
-    @typecheck
     async def stderr(self) -> str:
         """The error stream of the last executed command.
 
         Will execute default command if none is set, or error if there's no
         default.
 
         Returns
@@ -1012,14 +991,36 @@
         )
         return Container(_ctx)
 
     def __await__(self):
         return self.sync().__await__()
 
     @typecheck
+    def terminal(
+        self,
+        *,
+        cmd: Sequence[str] | None = None,
+    ) -> "Terminal":
+        """Return an interactive terminal for this container using its configured
+        default terminal command if not overridden by args (or sh as a
+        fallback default).
+
+        Parameters
+        ----------
+        cmd:
+            If set, override the container's default terminal command and
+            invoke these command arguments instead.
+        """
+        _args = [
+            Arg("cmd", cmd, None),
+        ]
+        _ctx = self._select("terminal", _args)
+        return Terminal(_ctx)
+
+    @typecheck
     async def user(self) -> str:
         """Retrieves the user to be set for all commands.
 
         Returns
         -------
         str
             The `String` scalar type represents textual data, represented as
@@ -1050,26 +1051,26 @@
         _args = [
             Arg("args", args),
         ]
         _ctx = self._select("withDefaultArgs", _args)
         return Container(_ctx)
 
     @typecheck
-    def with_default_shell(self, args: Sequence[str]) -> "Container":
-        """Set the default command to invoke for the "shell" API.
+    def with_default_terminal_cmd(self, args: Sequence[str]) -> "Container":
+        """Set the default command to invoke for the container's terminal API.
 
         Parameters
         ----------
         args:
-            The args of the command to set the default shell to.
+            The args of the command.
         """
         _args = [
             Arg("args", args),
         ]
-        _ctx = self._select("withDefaultShell", _args)
+        _ctx = self._select("withDefaultTerminalCmd", _args)
         return Container(_ctx)
 
     @typecheck
     def with_directory(
         self,
         path: str,
         directory: "Directory",
@@ -1964,32 +1965,32 @@
 class Directory(Type):
     """A directory."""
 
     @typecheck
     def as_module(
         self,
         *,
-        source_subpath: str | None = "/",
+        source_root_path: str | None = ".",
     ) -> "Module":
         """Load the directory as a Dagger module
 
         Parameters
         ----------
-        source_subpath:
+        source_root_path:
             An optional subpath of the directory which contains the module's
-            source code.
+            configuration file.
             This is needed when the module code is in a subdirectory but
             requires parent directories to be loaded in order to execute. For
             example, the module source code may need a go.mod, project.toml,
             package.json, etc. file from a parent directory.
             If not set, the module source code is loaded from the root of the
             directory.
         """
         _args = [
-            Arg("sourceSubpath", source_subpath, "/"),
+            Arg("sourceRootPath", source_root_path, "."),
         ]
         _ctx = self._select("asModule", _args)
         return Module(_ctx)
 
     @typecheck
     def diff(self, other: "Directory") -> "Directory":
         """Gets the difference between this directory and an another directory.
@@ -2431,15 +2432,17 @@
         """
         _args: list[Arg] = []
         _ctx = self._select("id", _args)
         return await _ctx.execute(EnvVariableID)
 
     @typecheck
     async def name(self) -> str:
-        """Returns
+        """The environment variable name.
+
+        Returns
         -------
         str
             The `String` scalar type represents textual data, represented as
             UTF-8 character sequences. The String type is most often used by
             GraphQL to represent free-form human-readable text.
 
         Raises
@@ -2453,15 +2456,17 @@
             return self._name
         _args: list[Arg] = []
         _ctx = self._select("name", _args)
         return await _ctx.execute(str)
 
     @typecheck
     async def value(self) -> str:
-        """Returns
+        """The environment variable value.
+
+        Returns
         -------
         str
             The `String` scalar type represents textual data, represented as
             UTF-8 character sequences. The String type is most often used by
             GraphQL to represent free-form human-readable text.
 
         Raises
@@ -2490,15 +2495,17 @@
     )
 
     _description: str | None
     _name: str | None
 
     @typecheck
     async def description(self) -> str:
-        """Returns
+        """A doc string for the field, if any.
+
+        Returns
         -------
         str
             The `String` scalar type represents textual data, represented as
             UTF-8 character sequences. The String type is most often used by
             GraphQL to represent free-form human-readable text.
 
         Raises
@@ -2537,15 +2544,17 @@
         """
         _args: list[Arg] = []
         _ctx = self._select("id", _args)
         return await _ctx.execute(FieldTypeDefID)
 
     @typecheck
     async def name(self) -> str:
-        """Returns
+        """The name of the field in lowerCamelCase format.
+
+        Returns
         -------
         str
             The `String` scalar type represents textual data, represented as
             UTF-8 character sequences. The String type is most often used by
             GraphQL to represent free-form human-readable text.
 
         Raises
@@ -2559,14 +2568,15 @@
             return self._name
         _args: list[Arg] = []
         _ctx = self._select("name", _args)
         return await _ctx.execute(str)
 
     @typecheck
     def type_def(self) -> "TypeDef":
+        """The type of the field."""
         _args: list[Arg] = []
         _ctx = self._select("typeDef", _args)
         return TypeDef(_ctx)
 
 
 class File(Type):
     """A file."""
@@ -2755,26 +2765,29 @@
     )
 
     _description: str | None
     _name: str | None
 
     @typecheck
     async def args(self) -> list["FunctionArg"]:
+        """Arguments accepted by the function, if any."""
         _args: list[Arg] = []
         _ctx = self._select("args", _args)
         _ctx = FunctionArg(_ctx)._select_multiple(
             _default_value="defaultValue",
             _description="description",
             _name="name",
         )
         return await _ctx.execute(list[FunctionArg])
 
     @typecheck
     async def description(self) -> str:
-        """Returns
+        """A doc string for the function, if any.
+
+        Returns
         -------
         str
             The `String` scalar type represents textual data, represented as
             UTF-8 character sequences. The String type is most often used by
             GraphQL to represent free-form human-readable text.
 
         Raises
@@ -2813,15 +2826,17 @@
         """
         _args: list[Arg] = []
         _ctx = self._select("id", _args)
         return await _ctx.execute(FunctionID)
 
     @typecheck
     async def name(self) -> str:
-        """Returns
+        """The name of the function.
+
+        Returns
         -------
         str
             The `String` scalar type represents textual data, represented as
             UTF-8 character sequences. The String type is most often used by
             GraphQL to represent free-form human-readable text.
 
         Raises
@@ -2835,14 +2850,15 @@
             return self._name
         _args: list[Arg] = []
         _ctx = self._select("name", _args)
         return await _ctx.execute(str)
 
     @typecheck
     def return_type(self) -> "TypeDef":
+        """The type returned by the function."""
         _args: list[Arg] = []
         _ctx = self._select("returnType", _args)
         return TypeDef(_ctx)
 
     @typecheck
     def with_arg(
         self,
@@ -2911,15 +2927,18 @@
 
     _default_value: JSON | None
     _description: str | None
     _name: str | None
 
     @typecheck
     async def default_value(self) -> JSON:
-        """Returns
+        """A default value to use for this argument when not explicitly set by
+        the caller, if any.
+
+        Returns
         -------
         JSON
             An arbitrary JSON-encoded value.
 
         Raises
         ------
         ExecuteTimeoutError
@@ -2931,15 +2950,17 @@
             return self._default_value
         _args: list[Arg] = []
         _ctx = self._select("defaultValue", _args)
         return await _ctx.execute(JSON)
 
     @typecheck
     async def description(self) -> str:
-        """Returns
+        """A doc string for the argument, if any.
+
+        Returns
         -------
         str
             The `String` scalar type represents textual data, represented as
             UTF-8 character sequences. The String type is most often used by
             GraphQL to represent free-form human-readable text.
 
         Raises
@@ -2978,15 +2999,17 @@
         """
         _args: list[Arg] = []
         _ctx = self._select("id", _args)
         return await _ctx.execute(FunctionArgID)
 
     @typecheck
     async def name(self) -> str:
-        """Returns
+        """The name of the argument in lowerCamelCase format.
+
+        Returns
         -------
         str
             The `String` scalar type represents textual data, represented as
             UTF-8 character sequences. The String type is most often used by
             GraphQL to represent free-form human-readable text.
 
         Raises
@@ -3000,14 +3023,15 @@
             return self._name
         _args: list[Arg] = []
         _ctx = self._select("name", _args)
         return await _ctx.execute(str)
 
     @typecheck
     def type_def(self) -> "TypeDef":
+        """The type of the argument."""
         _args: list[Arg] = []
         _ctx = self._select("typeDef", _args)
         return TypeDef(_ctx)
 
 
 class FunctionCall(Type):
     """An active function call."""
@@ -3035,25 +3059,28 @@
         """
         _args: list[Arg] = []
         _ctx = self._select("id", _args)
         return await _ctx.execute(FunctionCallID)
 
     @typecheck
     async def input_args(self) -> list["FunctionCallArgValue"]:
+        """The argument values the function is being invoked with."""
         _args: list[Arg] = []
         _ctx = self._select("inputArgs", _args)
         _ctx = FunctionCallArgValue(_ctx)._select_multiple(
             _name="name",
             _value="value",
         )
         return await _ctx.execute(list[FunctionCallArgValue])
 
     @typecheck
     async def name(self) -> str:
-        """Returns
+        """The name of the function being called.
+
+        Returns
         -------
         str
             The `String` scalar type represents textual data, represented as
             UTF-8 character sequences. The String type is most often used by
             GraphQL to represent free-form human-readable text.
 
         Raises
@@ -3065,15 +3092,18 @@
         """
         _args: list[Arg] = []
         _ctx = self._select("name", _args)
         return await _ctx.execute(str)
 
     @typecheck
     async def parent(self) -> JSON:
-        """Returns
+        """The value of the parent object of the function being called. If the
+        function is top-level to the module, this is always an empty object.
+
+        Returns
         -------
         JSON
             An arbitrary JSON-encoded value.
 
         Raises
         ------
         ExecuteTimeoutError
@@ -3083,15 +3113,18 @@
         """
         _args: list[Arg] = []
         _ctx = self._select("parent", _args)
         return await _ctx.execute(JSON)
 
     @typecheck
     async def parent_name(self) -> str:
-        """Returns
+        """The name of the parent object of the function being called. If the
+        function is top-level to the module, this is the name of the module.
+
+        Returns
         -------
         str
             The `String` scalar type represents textual data, represented as
             UTF-8 character sequences. The String type is most often used by
             GraphQL to represent free-form human-readable text.
 
         Raises
@@ -3168,15 +3201,17 @@
         """
         _args: list[Arg] = []
         _ctx = self._select("id", _args)
         return await _ctx.execute(FunctionCallArgValueID)
 
     @typecheck
     async def name(self) -> str:
-        """Returns
+        """The name of the argument.
+
+        Returns
         -------
         str
             The `String` scalar type represents textual data, represented as
             UTF-8 character sequences. The String type is most often used by
             GraphQL to represent free-form human-readable text.
 
         Raises
@@ -3190,15 +3225,17 @@
             return self._name
         _args: list[Arg] = []
         _ctx = self._select("name", _args)
         return await _ctx.execute(str)
 
     @typecheck
     async def value(self) -> JSON:
-        """Returns
+        """The value of the argument represented as a JSON serialized string.
+
+        Returns
         -------
         JSON
             An arbitrary JSON-encoded value.
 
         Raises
         ------
         ExecuteTimeoutError
@@ -3214,14 +3251,15 @@
 
 
 class GeneratedCode(Type):
     """The result of running an SDK's codegen."""
 
     @typecheck
     def code(self) -> Directory:
+        """The directory containing the generated code."""
         _args: list[Arg] = []
         _ctx = self._select("code", _args)
         return Directory(_ctx)
 
     @typecheck
     async def id(self) -> GeneratedCodeID:
         """A unique identifier for this GeneratedCode.
@@ -3245,15 +3283,18 @@
         """
         _args: list[Arg] = []
         _ctx = self._select("id", _args)
         return await _ctx.execute(GeneratedCodeID)
 
     @typecheck
     async def vcs_generated_paths(self) -> list[str]:
-        """Returns
+        """List of paths to mark generated in version control (i.e.
+        .gitattributes).
+
+        Returns
         -------
         list[str]
             The `String` scalar type represents textual data, represented as
             UTF-8 character sequences. The String type is most often used by
             GraphQL to represent free-form human-readable text.
 
         Raises
@@ -3265,15 +3306,17 @@
         """
         _args: list[Arg] = []
         _ctx = self._select("vcsGeneratedPaths", _args)
         return await _ctx.execute(list[str])
 
     @typecheck
     async def vcs_ignored_paths(self) -> list[str]:
-        """Returns
+        """List of paths to ignore in version control (i.e. .gitignore).
+
+        Returns
         -------
         list[str]
             The `String` scalar type represents textual data, represented as
             UTF-8 character sequences. The String type is most often used by
             GraphQL to represent free-form human-readable text.
 
         Raises
@@ -3338,15 +3381,17 @@
         """
         _args: list[Arg] = []
         _ctx = self._select("cloneURL", _args)
         return await _ctx.execute(str)
 
     @typecheck
     async def commit(self) -> str:
-        """Returns
+        """The resolved commit of the git repo this source points to.
+
+        Returns
         -------
         str
             The `String` scalar type represents textual data, represented as
             UTF-8 character sequences. The String type is most often used by
             GraphQL to represent free-form human-readable text.
 
         Raises
@@ -3357,14 +3402,23 @@
             If the API returns an error.
         """
         _args: list[Arg] = []
         _ctx = self._select("commit", _args)
         return await _ctx.execute(str)
 
     @typecheck
+    def context_directory(self) -> Directory:
+        """The directory containing everything needed to load load and use the
+        module.
+        """
+        _args: list[Arg] = []
+        _ctx = self._select("contextDirectory", _args)
+        return Directory(_ctx)
+
+    @typecheck
     async def html_url(self) -> str:
         """The URL to the source's git repo in a web browser
 
         Returns
         -------
         str
             The `String` scalar type represents textual data, represented as
@@ -3404,36 +3458,42 @@
             If the API returns an error.
         """
         _args: list[Arg] = []
         _ctx = self._select("id", _args)
         return await _ctx.execute(GitModuleSourceID)
 
     @typecheck
-    async def source_subpath(self) -> str:
-        """Returns
+    async def root_subpath(self) -> str:
+        """The path to the root of the module source under the context directory.
+        This directory contains its configuration file. It also contains its
+        source code (possibly as a subdirectory).
+
+        Returns
         -------
         str
             The `String` scalar type represents textual data, represented as
             UTF-8 character sequences. The String type is most often used by
             GraphQL to represent free-form human-readable text.
 
         Raises
         ------
         ExecuteTimeoutError
             If the time to execute the query exceeds the configured timeout.
         QueryError
             If the API returns an error.
         """
         _args: list[Arg] = []
-        _ctx = self._select("sourceSubpath", _args)
+        _ctx = self._select("rootSubpath", _args)
         return await _ctx.execute(str)
 
     @typecheck
     async def version(self) -> str:
-        """Returns
+        """The specified version of the git repo this source points to.
+
+        Returns
         -------
         str
             The `String` scalar type represents textual data, represented as
             UTF-8 character sequences. The String type is most often used by
             GraphQL to represent free-form human-readable text.
 
         Raises
@@ -3578,14 +3638,30 @@
             If the API returns an error.
         """
         _args: list[Arg] = []
         _ctx = self._select("id", _args)
         return await _ctx.execute(GitRepositoryID)
 
     @typecheck
+    def ref(self, name: str) -> GitRef:
+        """Returns details of a ref.
+
+        Parameters
+        ----------
+        name:
+            Ref's name (can be a commit identifier, a tag name, a branch name,
+            or a fully-qualified ref).
+        """
+        _args = [
+            Arg("name", name),
+        ]
+        _ctx = self._select("ref", _args)
+        return GitRef(_ctx)
+
+    @typecheck
     def tag(self, name: str) -> GitRef:
         """Returns details of a tag.
 
         Parameters
         ----------
         name:
             Tag's name (e.g., "v0.3.9").
@@ -3775,14 +3851,15 @@
     args. This is currently only used to represent pre-existing usage of
     graphql input types in the core API. It is not used by user modules
     and shouldn't ever be as user module accept input objects via their id
     rather than graphql input types."""
 
     @typecheck
     async def fields(self) -> list[FieldTypeDef]:
+        """Static fields defined on this input object, if any."""
         _args: list[Arg] = []
         _ctx = self._select("fields", _args)
         _ctx = FieldTypeDef(_ctx)._select_multiple(
             _description="description",
             _name="name",
         )
         return await _ctx.execute(list[FieldTypeDef])
@@ -3810,15 +3887,17 @@
         """
         _args: list[Arg] = []
         _ctx = self._select("id", _args)
         return await _ctx.execute(InputTypeDefID)
 
     @typecheck
     async def name(self) -> str:
-        """Returns
+        """The name of the input object.
+
+        Returns
         -------
         str
             The `String` scalar type represents textual data, represented as
             UTF-8 character sequences. The String type is most often used by
             GraphQL to represent free-form human-readable text.
 
         Raises
@@ -3834,15 +3913,17 @@
 
 
 class InterfaceTypeDef(Type):
     """A definition of a custom interface defined in a Module."""
 
     @typecheck
     async def description(self) -> str:
-        """Returns
+        """The doc string for the interface, if any.
+
+        Returns
         -------
         str
             The `String` scalar type represents textual data, represented as
             UTF-8 character sequences. The String type is most often used by
             GraphQL to represent free-form human-readable text.
 
         Raises
@@ -3854,14 +3935,15 @@
         """
         _args: list[Arg] = []
         _ctx = self._select("description", _args)
         return await _ctx.execute(str)
 
     @typecheck
     async def functions(self) -> list[Function]:
+        """Functions defined on this interface, if any."""
         _args: list[Arg] = []
         _ctx = self._select("functions", _args)
         _ctx = Function(_ctx)._select_multiple(
             _description="description",
             _name="name",
         )
         return await _ctx.execute(list[Function])
@@ -3889,15 +3971,17 @@
         """
         _args: list[Arg] = []
         _ctx = self._select("id", _args)
         return await _ctx.execute(InterfaceTypeDefID)
 
     @typecheck
     async def name(self) -> str:
-        """Returns
+        """The name of the interface.
+
+        Returns
         -------
         str
             The `String` scalar type represents textual data, represented as
             UTF-8 character sequences. The String type is most often used by
             GraphQL to represent free-form human-readable text.
 
         Raises
@@ -3909,15 +3993,18 @@
         """
         _args: list[Arg] = []
         _ctx = self._select("name", _args)
         return await _ctx.execute(str)
 
     @typecheck
     async def source_module_name(self) -> str:
-        """Returns
+        """If this InterfaceTypeDef is associated with a Module, the name of the
+        module. Unset otherwise.
+
+        Returns
         -------
         str
             The `String` scalar type represents textual data, represented as
             UTF-8 character sequences. The String type is most often used by
             GraphQL to represent free-form human-readable text.
 
         Raises
@@ -3966,15 +4053,17 @@
         """
         _args: list[Arg] = []
         _ctx = self._select("id", _args)
         return await _ctx.execute(LabelID)
 
     @typecheck
     async def name(self) -> str:
-        """Returns
+        """The label name.
+
+        Returns
         -------
         str
             The `String` scalar type represents textual data, represented as
             UTF-8 character sequences. The String type is most often used by
             GraphQL to represent free-form human-readable text.
 
         Raises
@@ -3988,15 +4077,17 @@
             return self._name
         _args: list[Arg] = []
         _ctx = self._select("name", _args)
         return await _ctx.execute(str)
 
     @typecheck
     async def value(self) -> str:
-        """Returns
+        """The label value.
+
+        Returns
         -------
         str
             The `String` scalar type represents textual data, represented as
             UTF-8 character sequences. The String type is most often used by
             GraphQL to represent free-form human-readable text.
 
         Raises
@@ -4014,14 +4105,15 @@
 
 
 class ListTypeDef(Type):
     """A definition of a list type in a Module."""
 
     @typecheck
     def element_type_def(self) -> "TypeDef":
+        """The type of the elements in the list."""
         _args: list[Arg] = []
         _ctx = self._select("elementTypeDef", _args)
         return TypeDef(_ctx)
 
     @typecheck
     async def id(self) -> ListTypeDefID:
         """A unique identifier for this ListTypeDef.
@@ -4049,14 +4141,23 @@
 
 
 class LocalModuleSource(Type):
     """Module source that that originates from a path locally relative to
     an arbitrary directory."""
 
     @typecheck
+    def context_directory(self) -> Directory:
+        """The directory containing everything needed to load load and use the
+        module.
+        """
+        _args: list[Arg] = []
+        _ctx = self._select("contextDirectory", _args)
+        return Directory(_ctx)
+
+    @typecheck
     async def id(self) -> LocalModuleSourceID:
         """A unique identifier for this LocalModuleSource.
 
         Note
         ----
         This is lazily evaluated, no operation is actually run.
 
@@ -4074,31 +4175,35 @@
             If the API returns an error.
         """
         _args: list[Arg] = []
         _ctx = self._select("id", _args)
         return await _ctx.execute(LocalModuleSourceID)
 
     @typecheck
-    async def source_subpath(self) -> str:
-        """Returns
+    async def root_subpath(self) -> str:
+        """The path to the root of the module source under the context directory.
+        This directory contains its configuration file. It also contains its
+        source code (possibly as a subdirectory).
+
+        Returns
         -------
         str
             The `String` scalar type represents textual data, represented as
             UTF-8 character sequences. The String type is most often used by
             GraphQL to represent free-form human-readable text.
 
         Raises
         ------
         ExecuteTimeoutError
             If the time to execute the query exceeds the configured timeout.
         QueryError
             If the API returns an error.
         """
         _args: list[Arg] = []
-        _ctx = self._select("sourceSubpath", _args)
+        _ctx = self._select("rootSubpath", _args)
         return await _ctx.execute(str)
 
 
 class Module(Type):
     """A Dagger module."""
 
     __slots__ = (
@@ -4111,36 +4216,40 @@
     _description: str | None
     _name: str | None
     _sdk: str | None
     _serve: Void | None
 
     @typecheck
     async def dependencies(self) -> list["Module"]:
+        """Modules used by this module."""
         _args: list[Arg] = []
         _ctx = self._select("dependencies", _args)
         _ctx = Module(_ctx)._select_multiple(
             _description="description",
             _name="name",
             _sdk="sdk",
             _serve="serve",
         )
         return await _ctx.execute(list[Module])
 
     @typecheck
     async def dependency_config(self) -> list["ModuleDependency"]:
+        """The dependencies as configured by the module."""
         _args: list[Arg] = []
         _ctx = self._select("dependencyConfig", _args)
         _ctx = ModuleDependency(_ctx)._select_multiple(
             _name="name",
         )
         return await _ctx.execute(list[ModuleDependency])
 
     @typecheck
     async def description(self) -> str:
-        """Returns
+        """The doc string of the module, if any
+
+        Returns
         -------
         str
             The `String` scalar type represents textual data, represented as
             UTF-8 character sequences. The String type is most often used by
             GraphQL to represent free-form human-readable text.
 
         Raises
@@ -4153,22 +4262,29 @@
         if hasattr(self, "_description"):
             return self._description
         _args: list[Arg] = []
         _ctx = self._select("description", _args)
         return await _ctx.execute(str)
 
     @typecheck
-    def generated_source_root_directory(self) -> Directory:
-        """The module's root directory containing the config file for it and its
-        source (possibly as a subdir). It includes any generated code or
-        updated config files created after initial load, but not any
-        files/directories that were unchanged after sdk codegen was run.
+    def generated_context_diff(self) -> Directory:
+        """The generated files and directories made on top of the module source's
+        context directory.
         """
         _args: list[Arg] = []
-        _ctx = self._select("generatedSourceRootDirectory", _args)
+        _ctx = self._select("generatedContextDiff", _args)
+        return Directory(_ctx)
+
+    @typecheck
+    def generated_context_directory(self) -> Directory:
+        """The module source's context plus any configuration and source files
+        created by codegen.
+        """
+        _args: list[Arg] = []
+        _ctx = self._select("generatedContextDirectory", _args)
         return Directory(_ctx)
 
     @typecheck
     async def id(self) -> ModuleID:
         """A unique identifier for this Module.
 
         Note
@@ -4197,25 +4313,28 @@
         """Retrieves the module with the objects loaded via its SDK."""
         _args: list[Arg] = []
         _ctx = self._select("initialize", _args)
         return Module(_ctx)
 
     @typecheck
     async def interfaces(self) -> list["TypeDef"]:
+        """Interfaces served by this module."""
         _args: list[Arg] = []
         _ctx = self._select("interfaces", _args)
         _ctx = TypeDef(_ctx)._select_multiple(
             _kind="kind",
             _optional="optional",
         )
         return await _ctx.execute(list[TypeDef])
 
     @typecheck
     async def name(self) -> str:
-        """Returns
+        """The name of the module
+
+        Returns
         -------
         str
             The `String` scalar type represents textual data, represented as
             UTF-8 character sequences. The String type is most often used by
             GraphQL to represent free-form human-readable text.
 
         Raises
@@ -4229,31 +4348,38 @@
             return self._name
         _args: list[Arg] = []
         _ctx = self._select("name", _args)
         return await _ctx.execute(str)
 
     @typecheck
     async def objects(self) -> list["TypeDef"]:
+        """Objects served by this module."""
         _args: list[Arg] = []
         _ctx = self._select("objects", _args)
         _ctx = TypeDef(_ctx)._select_multiple(
             _kind="kind",
             _optional="optional",
         )
         return await _ctx.execute(list[TypeDef])
 
     @typecheck
     def runtime(self) -> Container:
+        """The container that runs the module's entrypoint. It will fail to
+        execute if the module doesn't compile.
+        """
         _args: list[Arg] = []
         _ctx = self._select("runtime", _args)
         return Container(_ctx)
 
     @typecheck
     async def sdk(self) -> str:
-        """Returns
+        """The SDK used by this module. Either a name of a builtin SDK or a
+        module source ref string pointing to the SDK's implementation.
+
+        Returns
         -------
         str
             The `String` scalar type represents textual data, represented as
             UTF-8 character sequences. The String type is most often used by
             GraphQL to represent free-form human-readable text.
 
         Raises
@@ -4293,37 +4419,20 @@
             return self._serve
         _args: list[Arg] = []
         _ctx = self._select("serve", _args)
         return await _ctx.execute(Void | None)
 
     @typecheck
     def source(self) -> "ModuleSource":
+        """The source for the module."""
         _args: list[Arg] = []
         _ctx = self._select("source", _args)
         return ModuleSource(_ctx)
 
     @typecheck
-    def with_dependencies(
-        self,
-        dependencies: Sequence["ModuleDependency"],
-    ) -> "Module":
-        """Update the module configuration to use the given dependencies.
-
-        Parameters
-        ----------
-        dependencies:
-            The dependency modules to install.
-        """
-        _args = [
-            Arg("dependencies", dependencies),
-        ]
-        _ctx = self._select("withDependencies", _args)
-        return Module(_ctx)
-
-    @typecheck
     def with_description(self, description: str) -> "Module":
         """Retrieves the module with the given description
 
         Parameters
         ----------
         description:
             The description to set
@@ -4340,53 +4449,23 @@
         _args = [
             Arg("iface", iface),
         ]
         _ctx = self._select("withInterface", _args)
         return Module(_ctx)
 
     @typecheck
-    def with_name(self, name: str) -> "Module":
-        """Update the module configuration to use the given name.
-
-        Parameters
-        ----------
-        name:
-            The name to use.
-        """
-        _args = [
-            Arg("name", name),
-        ]
-        _ctx = self._select("withName", _args)
-        return Module(_ctx)
-
-    @typecheck
     def with_object(self, object: "TypeDef") -> "Module":
         """This module plus the given Object type and associated functions."""
         _args = [
             Arg("object", object),
         ]
         _ctx = self._select("withObject", _args)
         return Module(_ctx)
 
     @typecheck
-    def with_sdk(self, sdk: str) -> "Module":
-        """Update the module configuration to use the given SDK.
-
-        Parameters
-        ----------
-        sdk:
-            The SDK to use.
-        """
-        _args = [
-            Arg("sdk", sdk),
-        ]
-        _ctx = self._select("withSDK", _args)
-        return Module(_ctx)
-
-    @typecheck
     def with_source(self, source: "ModuleSource") -> "Module":
         """Retrieves the module with basic configuration loaded if present.
 
         Parameters
         ----------
         source:
             The module source to initialize from.
@@ -4435,15 +4514,17 @@
         """
         _args: list[Arg] = []
         _ctx = self._select("id", _args)
         return await _ctx.execute(ModuleDependencyID)
 
     @typecheck
     async def name(self) -> str:
-        """Returns
+        """The name of the dependency module.
+
+        Returns
         -------
         str
             The `String` scalar type represents textual data, represented as
             UTF-8 character sequences. The String type is most often used by
             GraphQL to represent free-form human-readable text.
 
         Raises
@@ -4457,31 +4538,34 @@
             return self._name
         _args: list[Arg] = []
         _ctx = self._select("name", _args)
         return await _ctx.execute(str)
 
     @typecheck
     def source(self) -> "ModuleSource":
+        """The source for the dependency module."""
         _args: list[Arg] = []
         _ctx = self._select("source", _args)
         return ModuleSource(_ctx)
 
 
 class ModuleSource(Type):
     """The source needed to load and run a module, along with any metadata
     about the source such as versions/urls/etc."""
 
     @typecheck
     def as_git_source(self) -> GitModuleSource:
+        """If the source is a of kind git, the git source representation of it."""
         _args: list[Arg] = []
         _ctx = self._select("asGitSource", _args)
         return GitModuleSource(_ctx)
 
     @typecheck
     def as_local_source(self) -> LocalModuleSource:
+        """If the source is of kind local, the local source representation of it."""
         _args: list[Arg] = []
         _ctx = self._select("asLocalSource", _args)
         return LocalModuleSource(_ctx)
 
     @typecheck
     def as_module(self) -> Module:
         """Load the source as a module. If this is a local source, the parent
@@ -4510,17 +4594,58 @@
             If the API returns an error.
         """
         _args: list[Arg] = []
         _ctx = self._select("asString", _args)
         return await _ctx.execute(str)
 
     @typecheck
+    async def config_exists(self) -> bool:
+        """Returns whether the module source has a configuration file.
+
+        Returns
+        -------
+        bool
+            The `Boolean` scalar type represents `true` or `false`.
+
+        Raises
+        ------
+        ExecuteTimeoutError
+            If the time to execute the query exceeds the configured timeout.
+        QueryError
+            If the API returns an error.
+        """
+        _args: list[Arg] = []
+        _ctx = self._select("configExists", _args)
+        return await _ctx.execute(bool)
+
+    @typecheck
+    def context_directory(self) -> Directory:
+        """The directory containing everything needed to load load and use the
+        module.
+        """
+        _args: list[Arg] = []
+        _ctx = self._select("contextDirectory", _args)
+        return Directory(_ctx)
+
+    @typecheck
+    async def dependencies(self) -> list[ModuleDependency]:
+        """The dependencies of the module source. Includes dependencies from the
+        configuration and any extras from withDependencies calls.
+        """
+        _args: list[Arg] = []
+        _ctx = self._select("dependencies", _args)
+        _ctx = ModuleDependency(_ctx)._select_multiple(
+            _name="name",
+        )
+        return await _ctx.execute(list[ModuleDependency])
+
+    @typecheck
     def directory(self, path: str) -> Directory:
-        """The directory containing the actual module's source code, as
-        determined from the root directory and subpath.
+        """The directory containing the module configuration and source code
+        (source code may be in a subdir).
 
         Parameters
         ----------
         path:
             The path from the source directory to select.
         """
         _args = [
@@ -4552,15 +4677,17 @@
         """
         _args: list[Arg] = []
         _ctx = self._select("id", _args)
         return await _ctx.execute(ModuleSourceID)
 
     @typecheck
     async def kind(self) -> ModuleSourceKind:
-        """Returns
+        """The kind of source (e.g. local, git, etc.)
+
+        Returns
         -------
         ModuleSourceKind
             The kind of module source.
 
         Raises
         ------
         ExecuteTimeoutError
@@ -4570,15 +4697,16 @@
         """
         _args: list[Arg] = []
         _ctx = self._select("kind", _args)
         return await _ctx.execute(ModuleSourceKind)
 
     @typecheck
     async def module_name(self) -> str:
-        """If set, the name of the module this source references
+        """If set, the name of the module this source references, including any
+        overrides at runtime by callers.
 
         Returns
         -------
         str
             The `String` scalar type represents textual data, represented as
             UTF-8 character sequences. The String type is most often used by
             GraphQL to represent free-form human-readable text.
@@ -4591,14 +4719,60 @@
             If the API returns an error.
         """
         _args: list[Arg] = []
         _ctx = self._select("moduleName", _args)
         return await _ctx.execute(str)
 
     @typecheck
+    async def module_original_name(self) -> str:
+        """The original name of the module this source references, as defined in
+        the module configuration.
+
+        Returns
+        -------
+        str
+            The `String` scalar type represents textual data, represented as
+            UTF-8 character sequences. The String type is most often used by
+            GraphQL to represent free-form human-readable text.
+
+        Raises
+        ------
+        ExecuteTimeoutError
+            If the time to execute the query exceeds the configured timeout.
+        QueryError
+            If the API returns an error.
+        """
+        _args: list[Arg] = []
+        _ctx = self._select("moduleOriginalName", _args)
+        return await _ctx.execute(str)
+
+    @typecheck
+    async def resolve_context_path_from_caller(self) -> str:
+        """The path to the module source's context directory on the caller's
+        filesystem. Only valid for local sources.
+
+        Returns
+        -------
+        str
+            The `String` scalar type represents textual data, represented as
+            UTF-8 character sequences. The String type is most often used by
+            GraphQL to represent free-form human-readable text.
+
+        Raises
+        ------
+        ExecuteTimeoutError
+            If the time to execute the query exceeds the configured timeout.
+        QueryError
+            If the API returns an error.
+        """
+        _args: list[Arg] = []
+        _ctx = self._select("resolveContextPathFromCaller", _args)
+        return await _ctx.execute(str)
+
+    @typecheck
     def resolve_dependency(self, dep: "ModuleSource") -> "ModuleSource":
         """Resolve the provided module source arg as a dependency relative to
         this module source.
 
         Parameters
         ----------
         dep:
@@ -4607,23 +4781,50 @@
         _args = [
             Arg("dep", dep),
         ]
         _ctx = self._select("resolveDependency", _args)
         return ModuleSource(_ctx)
 
     @typecheck
-    def root_directory(self) -> Directory:
+    def resolve_from_caller(self) -> "ModuleSource":
+        """Load the source from its path on the caller's filesystem, including
+        only needed+configured files and directories. Only valid for local
+        sources.
+        """
         _args: list[Arg] = []
-        _ctx = self._select("rootDirectory", _args)
-        return Directory(_ctx)
+        _ctx = self._select("resolveFromCaller", _args)
+        return ModuleSource(_ctx)
+
+    @typecheck
+    async def source_root_subpath(self) -> str:
+        """The path relative to context of the root of the module source, which
+        contains dagger.json. It also contains the module implementation
+        source code, but that may or may not being a subdir of this root.
+
+        Returns
+        -------
+        str
+            The `String` scalar type represents textual data, represented as
+            UTF-8 character sequences. The String type is most often used by
+            GraphQL to represent free-form human-readable text.
+
+        Raises
+        ------
+        ExecuteTimeoutError
+            If the time to execute the query exceeds the configured timeout.
+        QueryError
+            If the API returns an error.
+        """
+        _args: list[Arg] = []
+        _ctx = self._select("sourceRootSubpath", _args)
+        return await _ctx.execute(str)
 
     @typecheck
-    async def subpath(self) -> str:
-        """The path to the module subdirectory containing the actual module's
-        source code.
+    async def source_subpath(self) -> str:
+        """The path relative to context of the module implementation source code.
 
         Returns
         -------
         str
             The `String` scalar type represents textual data, represented as
             UTF-8 character sequences. The String type is most often used by
             GraphQL to represent free-form human-readable text.
@@ -4632,37 +4833,120 @@
         ------
         ExecuteTimeoutError
             If the time to execute the query exceeds the configured timeout.
         QueryError
             If the API returns an error.
         """
         _args: list[Arg] = []
-        _ctx = self._select("subpath", _args)
+        _ctx = self._select("sourceSubpath", _args)
         return await _ctx.execute(str)
 
+    @typecheck
+    def with_context_directory(self, dir: Directory) -> "ModuleSource":
+        """Update the module source with a new context directory. Only valid for
+        local sources.
+
+        Parameters
+        ----------
+        dir:
+            The directory to set as the context directory.
+        """
+        _args = [
+            Arg("dir", dir),
+        ]
+        _ctx = self._select("withContextDirectory", _args)
+        return ModuleSource(_ctx)
+
+    @typecheck
+    def with_dependencies(
+        self,
+        dependencies: Sequence[ModuleDependency],
+    ) -> "ModuleSource":
+        """Append the provided dependencies to the module source's dependency
+        list.
+
+        Parameters
+        ----------
+        dependencies:
+            The dependencies to append.
+        """
+        _args = [
+            Arg("dependencies", dependencies),
+        ]
+        _ctx = self._select("withDependencies", _args)
+        return ModuleSource(_ctx)
+
+    @typecheck
+    def with_name(self, name: str) -> "ModuleSource":
+        """Update the module source with a new name.
+
+        Parameters
+        ----------
+        name:
+            The name to set.
+        """
+        _args = [
+            Arg("name", name),
+        ]
+        _ctx = self._select("withName", _args)
+        return ModuleSource(_ctx)
+
+    @typecheck
+    def with_sdk(self, sdk: str) -> "ModuleSource":
+        """Update the module source with a new SDK.
+
+        Parameters
+        ----------
+        sdk:
+            The SDK to set.
+        """
+        _args = [
+            Arg("sdk", sdk),
+        ]
+        _ctx = self._select("withSDK", _args)
+        return ModuleSource(_ctx)
+
+    @typecheck
+    def with_source_subpath(self, path: str) -> "ModuleSource":
+        """Update the module source with a new source subpath.
+
+        Parameters
+        ----------
+        path:
+            The path to set as the source subpath.
+        """
+        _args = [
+            Arg("path", path),
+        ]
+        _ctx = self._select("withSourceSubpath", _args)
+        return ModuleSource(_ctx)
+
     def with_(self, cb: Callable[["ModuleSource"], "ModuleSource"]) -> "ModuleSource":
         """Call the provided callable with current ModuleSource.
 
         This is useful for reusability and readability by not breaking the calling chain.
         """
         return cb(self)
 
 
 class ObjectTypeDef(Type):
     """A definition of a custom object defined in a Module."""
 
     @typecheck
     def constructor(self) -> Function:
+        """The function used to construct new instances of this object, if any"""
         _args: list[Arg] = []
         _ctx = self._select("constructor", _args)
         return Function(_ctx)
 
     @typecheck
     async def description(self) -> str:
-        """Returns
+        """The doc string for the object, if any.
+
+        Returns
         -------
         str
             The `String` scalar type represents textual data, represented as
             UTF-8 character sequences. The String type is most often used by
             GraphQL to represent free-form human-readable text.
 
         Raises
@@ -4674,24 +4958,26 @@
         """
         _args: list[Arg] = []
         _ctx = self._select("description", _args)
         return await _ctx.execute(str)
 
     @typecheck
     async def fields(self) -> list[FieldTypeDef]:
+        """Static fields defined on this object, if any."""
         _args: list[Arg] = []
         _ctx = self._select("fields", _args)
         _ctx = FieldTypeDef(_ctx)._select_multiple(
             _description="description",
             _name="name",
         )
         return await _ctx.execute(list[FieldTypeDef])
 
     @typecheck
     async def functions(self) -> list[Function]:
+        """Functions defined on this object, if any."""
         _args: list[Arg] = []
         _ctx = self._select("functions", _args)
         _ctx = Function(_ctx)._select_multiple(
             _description="description",
             _name="name",
         )
         return await _ctx.execute(list[Function])
@@ -4719,15 +5005,17 @@
         """
         _args: list[Arg] = []
         _ctx = self._select("id", _args)
         return await _ctx.execute(ObjectTypeDefID)
 
     @typecheck
     async def name(self) -> str:
-        """Returns
+        """The name of the object.
+
+        Returns
         -------
         str
             The `String` scalar type represents textual data, represented as
             UTF-8 character sequences. The String type is most often used by
             GraphQL to represent free-form human-readable text.
 
         Raises
@@ -4739,15 +5027,18 @@
         """
         _args: list[Arg] = []
         _ctx = self._select("name", _args)
         return await _ctx.execute(str)
 
     @typecheck
     async def source_module_name(self) -> str:
-        """Returns
+        """If this ObjectTypeDef is associated with a Module, the name of the
+        module. Unset otherwise.
+
+        Returns
         -------
         str
             The `String` scalar type represents textual data, represented as
             UTF-8 character sequences. The String type is most often used by
             GraphQL to represent free-form human-readable text.
 
         Raises
@@ -4775,15 +5066,17 @@
     _description: str | None
     _experimental_skip_healthcheck: bool | None
     _port: int | None
     _protocol: NetworkProtocol | None
 
     @typecheck
     async def description(self) -> str | None:
-        """Returns
+        """The port description.
+
+        Returns
         -------
         str | None
             The `String` scalar type represents textual data, represented as
             UTF-8 character sequences. The String type is most often used by
             GraphQL to represent free-form human-readable text.
 
         Raises
@@ -4797,15 +5090,17 @@
             return self._description
         _args: list[Arg] = []
         _ctx = self._select("description", _args)
         return await _ctx.execute(str | None)
 
     @typecheck
     async def experimental_skip_healthcheck(self) -> bool:
-        """Returns
+        """Skip the health check when run as a service.
+
+        Returns
         -------
         bool
             The `Boolean` scalar type represents `true` or `false`.
 
         Raises
         ------
         ExecuteTimeoutError
@@ -4842,15 +5137,17 @@
         """
         _args: list[Arg] = []
         _ctx = self._select("id", _args)
         return await _ctx.execute(PortID)
 
     @typecheck
     async def port(self) -> int:
-        """Returns
+        """The port number.
+
+        Returns
         -------
         int
             The `Int` scalar type represents non-fractional signed whole
             numeric values. Int can represent values between -(2^31) and 2^31
             - 1.
 
         Raises
@@ -4864,15 +5161,17 @@
             return self._port
         _args: list[Arg] = []
         _ctx = self._select("port", _args)
         return await _ctx.execute(int)
 
     @typecheck
     async def protocol(self) -> NetworkProtocol:
-        """Returns
+        """The transport layer protocol.
+
+        Returns
         -------
         NetworkProtocol
             Transport layer network protocol associated to a port.
 
         Raises
         ------
         ExecuteTimeoutError
@@ -5495,34 +5794,28 @@
         return ModuleDependency(_ctx)
 
     @typecheck
     def module_source(
         self,
         ref_string: str,
         *,
-        root_directory: Directory | None = None,
         stable: bool | None = False,
     ) -> ModuleSource:
         """Create a new module source instance from a source ref string.
 
         Parameters
         ----------
         ref_string:
             The string ref representation of the module source
-        root_directory:
-            An explicitly set root directory for the module source. This is
-            required to load local sources as modules; other source types
-            implicitly encode the root directory and do not require this.
         stable:
             If true, enforce that the source is a stable version for source
             kinds that support versioning.
         """
         _args = [
             Arg("refString", ref_string),
-            Arg("rootDirectory", root_directory, None),
             Arg("stable", stable, False),
         ]
         _ctx = self._select("moduleSource", _args)
         return ModuleSource(_ctx)
 
     @typecheck
     def pipeline(
@@ -5817,19 +6110,28 @@
         return Service(_ctx)
 
     @typecheck
     async def up(
         self,
         *,
         ports: Sequence[PortForward] | None = [],
-        native: bool | None = False,
+        random: bool | None = False,
     ) -> Void | None:
         """Creates a tunnel that forwards traffic from the caller's network to
         this service.
 
+        Parameters
+        ----------
+        ports:
+            List of frontend/backend port mappings to forward.
+            Frontend is the port accepting traffic on the host, backend is the
+            service port.
+        random:
+            Bind each tunnel port to a random port on the host.
+
         Returns
         -------
         Void | None
             The absence of a value.  A Null Void is used as a placeholder for
             resolvers that do not return anything.
 
         Raises
@@ -5837,15 +6139,15 @@
         ExecuteTimeoutError
             If the time to execute the query exceeds the configured timeout.
         QueryError
             If the API returns an error.
         """
         _args = [
             Arg("ports", ports, []),
-            Arg("native", native, False),
+            Arg("random", random, False),
         ]
         _ctx = self._select("up", _args)
         return await _ctx.execute(Void | None)
 
 
 class Socket(Type):
     """A Unix or TCP/IP socket that can be mounted into a container."""
@@ -5937,32 +6239,44 @@
     )
 
     _kind: TypeDefKind | None
     _optional: bool | None
 
     @typecheck
     def as_input(self) -> InputTypeDef:
+        """If kind is INPUT, the input-specific type definition. If kind is not
+        INPUT, this will be null.
+        """
         _args: list[Arg] = []
         _ctx = self._select("asInput", _args)
         return InputTypeDef(_ctx)
 
     @typecheck
     def as_interface(self) -> InterfaceTypeDef:
+        """If kind is INTERFACE, the interface-specific type definition. If kind
+        is not INTERFACE, this will be null.
+        """
         _args: list[Arg] = []
         _ctx = self._select("asInterface", _args)
         return InterfaceTypeDef(_ctx)
 
     @typecheck
     def as_list(self) -> ListTypeDef:
+        """If kind is LIST, the list-specific type definition. If kind is not
+        LIST, this will be null.
+        """
         _args: list[Arg] = []
         _ctx = self._select("asList", _args)
         return ListTypeDef(_ctx)
 
     @typecheck
     def as_object(self) -> ObjectTypeDef:
+        """If kind is OBJECT, the object-specific type definition. If kind is not
+        OBJECT, this will be null.
+        """
         _args: list[Arg] = []
         _ctx = self._select("asObject", _args)
         return ObjectTypeDef(_ctx)
 
     @typecheck
     async def id(self) -> TypeDefID:
         """A unique identifier for this TypeDef.
@@ -5986,15 +6300,17 @@
         """
         _args: list[Arg] = []
         _ctx = self._select("id", _args)
         return await _ctx.execute(TypeDefID)
 
     @typecheck
     async def kind(self) -> TypeDefKind:
-        """Returns
+        """The kind of type this is (e.g. primitive, list, object).
+
+        Returns
         -------
         TypeDefKind
             Distinguishes the different kinds of TypeDefs.
 
         Raises
         ------
         ExecuteTimeoutError
@@ -6006,15 +6322,17 @@
             return self._kind
         _args: list[Arg] = []
         _ctx = self._select("kind", _args)
         return await _ctx.execute(TypeDefKind)
 
     @typecheck
     async def optional(self) -> bool:
-        """Returns
+        """Whether this type can be set to null. Defaults to false.
+
+        Returns
         -------
         bool
             The `Boolean` scalar type represents `true` or `false`.
 
         Raises
         ------
         ExecuteTimeoutError
```

### Comparing `dagger_io-0.9.8/src/dagger/mod/_arguments.py` & `dagger_io-0.9.9/src/dagger/mod/_arguments.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.9.8/src/dagger/mod/_converter.py` & `dagger_io-0.9.9/src/dagger/mod/_converter.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 import dataclasses
 import functools
 import inspect
 import logging
 import typing
-from collections.abc import Sequence
+from collections.abc import Collection
 
 from beartype.door import TypeHint
 from cattrs.preconf.json import make_converter as make_json_converter
 
 from ._types import ObjectDefinition
 from ._utils import (
     get_doc,
     is_annotated,
-    is_optional,
+    is_nullable,
     is_union,
-    non_optional,
+    non_null,
     strip_annotations,
     syncify,
 )
 
 logger = logging.getLogger(__name__)
 
 if typing.TYPE_CHECKING:
@@ -63,15 +63,18 @@
         dagger_type_unstructure,
     )
 
     return conv
 
 
 @functools.cache
-def to_typedef(annotation: type) -> "TypeDef":  # noqa: C901
+def to_typedef(  # noqa: C901
+    annotation: type,
+    has_default: bool | None = None,
+) -> "TypeDef":
     """Convert Python object to API type."""
     assert not is_annotated(
         annotation
     ), "Annotated types should be handled by the caller."
 
     import dagger
     from dagger import dag
@@ -80,18 +83,22 @@
     td = dag.type_def()
 
     if isinstance(annotation, dataclasses.InitVar):
         annotation = annotation.type
 
     typ = TypeHint(annotation)
 
-    if is_optional(typ):
+    if is_nullable(typ) and has_default is False:
+        msg = f"Nullable type must have a default value: {typ.hint!r}"
+        raise TypeError(msg)
+
+    if is_nullable(typ) or has_default is True:
         td = td.with_optional(True)
 
-    typ = non_optional(typ)
+    typ = non_null(typ)
 
     if typ is TypeHint(type(None)):
         return td.with_kind(dagger.TypeDefKind.VOID_KIND)
 
     builtins = {
         str: dagger.TypeDefKind.STRING_KIND,
         int: dagger.TypeDefKind.INTEGER_KIND,
@@ -102,23 +109,24 @@
         return td.with_kind(builtins[typ.hint])
 
     # Can't represent unions in the API.
     if is_union(typ):
         msg = f"Unsupported union type: {typ.hint}"
         raise TypeError(msg)
 
-    if typ.is_subhint(TypeHint(Sequence)):
-        if len(typ) != 1:
+    # NB: str is a Collection, but we've handled it above.
+    if typ.is_subhint(TypeHint(Collection)):
+        try:
+            return td.with_list_of(to_typedef(typ.args[0]))
+        except IndexError:
             msg = (
-                "Expected sequence type to be subscripted "
-                f"with 1 subtype, got {len(typ)}"
+                "Expected collection type to be subscripted "
+                f"with 1 subtype, got {len(typ)}: {typ.hint!r}"
             )
-            raise TypeError(msg)
-
-        return td.with_list_of(to_typedef(typ.args[0]))
+            raise TypeError(msg) from None
 
     if inspect.isclass(cls := typ.hint):
         custom_obj: ObjectDefinition | None = getattr(cls, "__dagger_type__", None)
 
         if custom_obj is not None:
             return td.with_object(
                 custom_obj.name,
```

### Comparing `dagger_io-0.9.8/src/dagger/mod/_exceptions.py` & `dagger_io-0.9.9/src/dagger/mod/_exceptions.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.9.8/src/dagger/mod/_module.py` & `dagger_io-0.9.9/src/dagger/mod/_module.py`

 * *Files 1% similar despite different names*

```diff
@@ -215,15 +215,16 @@
     async def _register(self, resolvers: Resolvers, mod_name: str) -> dagger.ModuleID:
         # Resolvers are collected at import time, but only actually
         # registered during "serve".
         mod = self._mod
 
         for obj, obj_resolvers in resolvers.items():
             if obj.name == "":
-                raise InternalError("Unexpected empty object name")
+                msg = "Unexpected empty object name"
+                raise InternalError(msg)
 
             typedef = dag.type_def().with_object(
                 obj.name,
                 description=obj.doc,
             )
             for r in obj_resolvers.values():
                 if r.name == "" and obj.name != mod_name:
```

### Comparing `dagger_io-0.9.8/src/dagger/mod/_resolver.py` & `dagger_io-0.9.9/src/dagger/mod/_resolver.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,15 +78,15 @@
     type_annotation: type
     is_optional: bool
 
     @override
     def register(self, typedef: dagger.TypeDef) -> dagger.TypeDef:
         return typedef.with_field(
             self.name,
-            to_typedef(self.type_annotation).with_optional(self.is_optional),
+            to_typedef(self.type_annotation, self.is_optional),
             description=self.doc or None,
         )
 
     @override
     async def get_result(
         self,
         _: cattrs.Converter,
@@ -121,21 +121,21 @@
         return repr(self.sig_func)
 
     @override
     def register(self, typedef: dagger.TypeDef) -> dagger.TypeDef:
         """Add a new object to current module."""
         fn = dag.function(self.name, to_typedef(self.return_type))
 
-        if self.doc:
-            fn = fn.with_description(self.doc)
+        if self.func_doc is not None:
+            fn = fn.with_description(self.func_doc)
 
         for param in self.parameters.values():
             fn = fn.with_arg(
                 param.name,
-                to_typedef(param.resolved_type).with_optional(param.is_optional),
+                to_typedef(param.resolved_type, param.is_optional),
                 description=param.doc,
                 default_value=self._get_default_value(param),
             )
 
         return typedef.with_function(fn) if self.name else typedef.with_constructor(fn)
 
     def _get_default_value(self, param: Parameter) -> dagger.JSON | None:
@@ -200,14 +200,19 @@
         """Return the callable to invoke."""
         # It should be the same as `wrapped_func` except for the alternative
         # constructor which is different than `wrapped_func`.
         # It's simpler not to execute `__init__` directly since it's unbound.
         return get_alt_constructor(self.wrapped_func) or self.wrapped_func
 
     @property
+    def func_doc(self):
+        """Return the description for the callable to invoke."""
+        return self.doc if self.doc is not None else get_doc(self.func)
+
+    @property
     def sig_func(self):
         """Return the callable to inspect."""
         # For more accurate inspection, as it can be different
         # than the callable to invoke.
         if inspect.isclass(cls := self.wrapped_func):
             return get_alt_constructor(cls) or cls.__init__
         return self.wrapped_func
@@ -351,15 +356,15 @@
             elif self.name == "":
                 origin = self.func
 
         self.resolver = FunctionResolver(
             original_name=original_name,
             name=name,
             wrapped_func=self.func,
-            doc=self.doc or get_doc(self.func),
+            doc=self.doc,
             origin=origin,
         )
 
     def __set_name__(self, owner: type, name: str):
         if self.name is None:
             self.name = name
             self.resolver.name = name
```

### Comparing `dagger_io-0.9.8/src/dagger/mod/_utils.py` & `dagger_io-0.9.9/src/dagger/mod/_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,15 +76,15 @@
                 arg.documentation
                 for arg in reversed(typing.get_args(obj))
                 if isinstance(arg, typing_extensions.Doc)
             ),
             None,
         )
     if inspect.getmodule(obj) != builtins and (
-        inspect.isclass(obj) or inspect.isfunction(obj)
+        inspect.isclass(obj) or inspect.isroutine(obj)
     ):
         doc = inspect.getdoc(obj)
         # By default, a dataclass's __doc__ will be the signature of the class,
         # not None.
         if (
             doc
             and dataclasses.is_dataclass(obj)
@@ -111,24 +111,24 @@
 
 
 def is_union(th: TypeHint) -> bool:
     """Returns True if the unsubscripted part of a type is a Union."""
     return isinstance(th, UnionTypeHint)
 
 
-def is_optional(th: TypeHint) -> bool:
+def is_nullable(th: TypeHint) -> bool:
     """Returns True if the annotation is SomeType | None.
 
     Does not support Annotated types. Use only on types that have been
     resolved with get_type_hints.
     """
     return th.is_bearable(None)
 
 
-def non_optional(th: TypeHint) -> TypeHint:
+def non_null(th: TypeHint) -> TypeHint:
     """Removes None from a union.
 
     Does not support Annotated types. Use only on types that have been
     resolved with get_type_hints.
     """
     if TypeHint(None) not in th:
         return th
```

### Comparing `dagger_io-0.9.8/src/dagger/mod/cli.py` & `dagger_io-0.9.9/src/dagger/mod/cli.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.9.8/tests/client/test_codegen.py` & `dagger_io-0.9.9/tests/client/test_codegen.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.9.8/tests/client/test_config.py` & `dagger_io-0.9.9/tests/client/test_config.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.9.8/tests/client/test_connection_errors.py` & `dagger_io-0.9.9/tests/client/test_connection_errors.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.9.8/tests/client/test_default_client.py` & `dagger_io-0.9.9/tests/client/test_default_client.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.9.8/tests/client/test_execute_errors.py` & `dagger_io-0.9.9/tests/client/test_execute_errors.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.9.8/tests/client/test_inputs.py` & `dagger_io-0.9.9/tests/client/test_inputs.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.9.8/tests/client/test_integration.py` & `dagger_io-0.9.9/tests/client/test_integration.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.9.8/tests/client/test_integration_connection.py` & `dagger_io-0.9.9/tests/client/test_integration_connection.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.9.8/tests/client/test_response.py` & `dagger_io-0.9.9/tests/client/test_response.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.9.8/tests/engine/test_cli.py` & `dagger_io-0.9.9/tests/engine/test_cli.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.9.8/tests/engine/test_download.py` & `dagger_io-0.9.9/tests/engine/test_download.py`

 * *Files identical despite different names*

### Comparing `dagger_io-0.9.8/tests/modules/test_registration.py` & `dagger_io-0.9.9/tests/modules/test_registration.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,14 @@
+from typing import cast
+
 import pytest
 
 from dagger.mod import Module
 from dagger.mod._exceptions import NameConflictError, UserError
+from dagger.mod._resolver import FunctionResolver
 
 
 def get_resolver(mod: Module, parent_name: str, resolver_name: str):
     return mod.get_resolver(
         mod.get_resolvers("foo"),
         parent_name,
         resolver_name,
@@ -117,8 +120,20 @@
 
     @mod.function
     def fn_with_doc():
         """Foo."""
 
     r = get_resolver(mod, "Foo", "fn_with_doc")
 
-    assert r.doc == "Foo."
+    assert cast(FunctionResolver, r).func_doc == "Foo."
+
+
+@pytest.mark.anyio()
+async def test_nullable_no_default():
+    mod = Module()
+
+    @mod.function
+    def echo(msg: str | None) -> str:
+        return "hello" if msg is None else msg
+
+    with pytest.raises(TypeError, match="must have a default value"):
+        await mod._register(mod.get_resolvers("foo"), "foo")
```

### Comparing `dagger_io-0.9.8/tests/modules/test_results.py` & `dagger_io-0.9.9/tests/modules/test_results.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import json
 from dataclasses import InitVar
-from typing import Annotated
+from typing import Annotated, cast
 
 import pytest
 from typing_extensions import Self
 
 import dagger
 from dagger import Arg, Doc, dag
 from dagger.mod import Module
 from dagger.mod._exceptions import FatalError
+from dagger.mod._resolver import FunctionResolver
 
 pytestmark = [
     pytest.mark.anyio,
 ]
 
 
 def get_resolver(mod: Module, parent_name: str, resolver_name: str):
@@ -171,14 +172,41 @@
 
     assert Foo().foo == "oof"
     assert Foo.create().foo == "bar"
     assert await get_result(mod, "Foo", {}, "", {}) == {"foo": "bar"}
     assert await get_result(mod, "Foo", {}, "", {"bar": "baz"}) == {"foo": "baz"}
 
 
+async def test_constructor_doc():
+    mod = Module()
+
+    @mod.object_type
+    class Foo:
+        """Object doc."""
+
+    constructor = cast(FunctionResolver, get_resolver(mod, "Foo", ""))
+    assert constructor.func_doc == "Object doc."
+
+
+async def test_alt_constructor_doc():
+    mod = Module()
+
+    @mod.object_type
+    class Foo:
+        """Object doc."""
+
+        @classmethod
+        def create(cls):
+            """Constructor doc."""
+            return cls()
+
+    constructor = cast(FunctionResolver, get_resolver(mod, "Foo", ""))
+    assert constructor.func_doc == "Constructor doc."
+
+
 async def test_alt_async_constructor():
     # The alternative constructor also allows running async code.
     mod = Module()
 
     async def default_value():
         return "bar"
```

### Comparing `dagger_io-0.9.8/tests/modules/test_utils.py` & `dagger_io-0.9.9/tests/modules/test_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,48 +1,53 @@
 from typing import Annotated, Optional
 
 import pytest
 from beartype.door import TypeHint
-from typing_extensions import Doc
+from typing_extensions import Doc, Self
 
 from dagger import Arg, field
 from dagger.mod import Module
-from dagger.mod._utils import get_arg_name, get_doc, is_optional, non_optional
+from dagger.mod._utils import get_arg_name, get_doc, is_nullable, non_null
 
 
 @pytest.mark.parametrize(
     ("typ", "expected"),
     [
         (str, False),
         (str | int, False),
         (str | None, True),
         (Optional[str], True),
     ],
 )
-def test_is_optional(typ, expected):
-    assert is_optional(TypeHint(typ)) == expected
+def test_is_nullable(typ, expected):
+    assert is_nullable(TypeHint(typ)) == expected
 
 
 @pytest.mark.parametrize(
     ("typ", "expected"),
     [
         (str, str),
         (str | None, str),
         (Optional[str], str),
         (str | int | None, str | int),
         (str | int, str | int),
     ],
 )
 def test_non_optional(typ, expected):
-    assert non_optional(TypeHint(typ)) == TypeHint(expected)
+    assert non_null(TypeHint(typ)) == TypeHint(expected)
 
 
 class ClassWithDocstring:
     """Foo."""
 
+    @classmethod
+    def create(cls) -> Self:
+        """Bar."""
+        return cls()
+
 
 def func_with_docstring():
     """Foo."""
 
 
 async def async_func_with_docstring():
     """Foo."""
@@ -60,14 +65,18 @@
         Annotated[str, Doc("Bar."), Doc("Foo.")],
     ],
 )
 def test_get_doc(annotation):
     assert get_doc(annotation) == "Foo."
 
 
+def test_get_factory_doc():
+    assert get_doc(ClassWithDocstring.create) == "Bar."
+
+
 class ClassWithoutDocstring:
     ...
 
 
 def func_without_docstring():
     ...
```

### Comparing `dagger_io-0.9.8/LICENSE` & `dagger_io-0.9.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dagger_io-0.9.8/README.md` & `dagger_io-0.9.9/README.md`

 * *Files identical despite different names*

### Comparing `dagger_io-0.9.8/pyproject.toml` & `dagger_io-0.9.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `dagger_io-0.9.8/PKG-INFO` & `dagger_io-0.9.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagger-io
-Version: 0.9.8
+Version: 0.9.9
 Summary: A client package for running Dagger pipelines in Python.
 Project-URL: Homepage, https://dagger.io
 Project-URL: Documentation, https://docs.dagger.io/sdk/python
 Project-URL: Repository, https://github.com/dagger/dagger/tree/main/sdk/python
 Project-URL: Tracker, https://github.com/dagger/dagger/issues
 Project-URL: Release Notes, https://github.com/dagger/dagger/releases?q=tag%3Asdk%2Fpython%2Fv0
 Project-URL: Community, https://discord.gg/ufnyBtc8uY
```

