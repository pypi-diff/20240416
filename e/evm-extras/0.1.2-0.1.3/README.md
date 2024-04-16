# Comparing `tmp/evm_extras-0.1.2.tar.gz` & `tmp/evm_extras-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "evm_extras-0.1.2.tar", max compression
+gzip compressed data, was "evm_extras-0.1.3.tar", max compression
```

## Comparing `evm_extras-0.1.2.tar` & `evm_extras-0.1.3.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0     1063 2023-11-06 15:37:10.057780 evm_extras-0.1.2/LICENSE
--rw-r--r--   0        0        0      588 2024-01-25 00:50:29.319296 evm_extras-0.1.2/README.md
--rw-r--r--   0        0        0      381 2024-01-29 19:45:53.974213 evm_extras-0.1.2/evm_extras/__init__.py
--rw-r--r--   0        0        0     1748 2024-01-24 23:45:31.568855 evm_extras-0.1.2/evm_extras/abc.py
--rw-r--r--   0        0        0     1226 2024-01-24 17:38:10.961356 evm_extras-0.1.2/evm_extras/exceptions.py
--rw-r--r--   0        0        0      126 2024-01-24 17:42:50.305366 evm_extras-0.1.2/evm_extras/globals.py
--rw-r--r--   0        0        0     5849 2024-01-29 19:45:53.964485 evm_extras-0.1.2/evm_extras/tools.py
--rw-r--r--   0        0        0      140 2024-01-29 19:45:53.968633 evm_extras-0.1.2/evm_extras/types.py
--rw-r--r--   0        0        0     1112 2024-01-29 19:45:53.971776 evm_extras-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1599 1970-01-01 00:00:00.000000 evm_extras-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1063 2023-11-06 15:37:10.057780 evm_extras-0.1.3/LICENSE
+-rw-r--r--   0        0        0      588 2024-01-25 00:50:29.319296 evm_extras-0.1.3/README.md
+-rw-r--r--   0        0        0      381 2024-01-29 19:45:53.974213 evm_extras-0.1.3/evm_extras/__init__.py
+-rw-r--r--   0        0        0     1749 2024-04-16 20:09:23.891571 evm_extras-0.1.3/evm_extras/abc.py
+-rw-r--r--   0        0        0     2621 2024-04-16 20:09:23.885537 evm_extras-0.1.3/evm_extras/exceptions.py
+-rw-r--r--   0        0        0      126 2024-01-24 17:42:50.305366 evm_extras-0.1.3/evm_extras/globals.py
+-rw-r--r--   0        0        0     5849 2024-01-29 19:45:53.964485 evm_extras-0.1.3/evm_extras/tools.py
+-rw-r--r--   0        0        0      140 2024-01-29 19:45:53.968633 evm_extras-0.1.3/evm_extras/types.py
+-rw-r--r--   0        0        0     1112 2024-04-16 20:09:23.888719 evm_extras-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     1599 1970-01-01 00:00:00.000000 evm_extras-0.1.3/PKG-INFO
```

### Comparing `evm_extras-0.1.2/LICENSE` & `evm_extras-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `evm_extras-0.1.2/README.md` & `evm_extras-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `evm_extras-0.1.2/evm_extras/abc.py` & `evm_extras-0.1.3/evm_extras/abc.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     @property
     def provider(self) -> AsyncWeb3:
         """
         Get the AsyncWeb3 provider associated with the wallet instance.
 
         :return: An instance of AsyncWeb3.
         """
-        return self.provider
+        return self._provider
 
     @property
     def version(self) -> int | None:
         """
         Get the version number of the DeFi protocol.
 
         :return: Version number if available, otherwise None.
```

### Comparing `evm_extras-0.1.2/evm_extras/tools.py` & `evm_extras-0.1.3/evm_extras/tools.py`

 * *Files identical despite different names*

### Comparing `evm_extras-0.1.2/pyproject.toml` & `evm_extras-0.1.3/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = 'evm_extras'
-version = '0.1.2'
+version = '0.1.3'
 description = 'The package containing utilities to develop Web3-based projects'
 authors = ['Alexey <abelenkov2006@gmail.com>']
 license = 'MIT'
 readme = 'README.md'
 repository = 'https://github.com/blnkoff/evm-extras'
 homepage = 'https://github.com/blnkoff/evm-extras'
 classifiers = [
```

### Comparing `evm_extras-0.1.2/PKG-INFO` & `evm_extras-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: evm_extras
-Version: 0.1.2
+Version: 0.1.3
 Summary: The package containing utilities to develop Web3-based projects
 Home-page: https://github.com/blnkoff/evm-extras
 License: MIT
 Author: Alexey
 Author-email: abelenkov2006@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: Development Status :: 4 - Beta
```

