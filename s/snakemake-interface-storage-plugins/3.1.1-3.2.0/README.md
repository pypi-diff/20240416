# Comparing `tmp/snakemake_interface_storage_plugins-3.1.1.tar.gz` & `tmp/snakemake_interface_storage_plugins-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snakemake_interface_storage_plugins-3.1.1.tar", max compression
+gzip compressed data, was "snakemake_interface_storage_plugins-3.2.0.tar", max compression
```

## Comparing `snakemake_interface_storage_plugins-3.1.1.tar` & `snakemake_interface_storage_plugins-3.2.0.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1076 2024-03-07 10:09:22.541468 snakemake_interface_storage_plugins-3.1.1/LICENSE
--rw-r--r--   0        0        0     8633 2024-03-07 10:09:22.541468 snakemake_interface_storage_plugins-3.1.1/README.md
--rw-r--r--   0        0        0      911 2024-03-07 10:09:22.541468 snakemake_interface_storage_plugins-3.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-07 10:09:22.541468 snakemake_interface_storage_plugins-3.1.1/snakemake_interface_storage_plugins/__init__.py
--rw-r--r--   0        0        0      525 2024-03-07 10:09:22.541468 snakemake_interface_storage_plugins-3.1.1/snakemake_interface_storage_plugins/common.py
--rw-r--r--   0        0        0     2858 2024-03-07 10:09:22.541468 snakemake_interface_storage_plugins-3.1.1/snakemake_interface_storage_plugins/io.py
--rw-r--r--   0        0        0     2041 2024-03-07 10:09:22.541468 snakemake_interface_storage_plugins-3.1.1/snakemake_interface_storage_plugins/registry/__init__.py
--rw-r--r--   0        0        0     1315 2024-03-07 10:09:22.541468 snakemake_interface_storage_plugins-3.1.1/snakemake_interface_storage_plugins/registry/plugin.py
--rw-r--r--   0        0        0      898 2024-03-07 10:09:22.541468 snakemake_interface_storage_plugins-3.1.1/snakemake_interface_storage_plugins/settings.py
--rw-r--r--   0        0        0     7389 2024-03-07 10:09:22.541468 snakemake_interface_storage_plugins-3.1.1/snakemake_interface_storage_plugins/storage_object.py
--rw-r--r--   0        0        0     5155 2024-03-07 10:09:22.541468 snakemake_interface_storage_plugins-3.1.1/snakemake_interface_storage_plugins/storage_provider.py
--rw-r--r--   0        0        0     3519 2024-03-07 10:09:22.541468 snakemake_interface_storage_plugins-3.1.1/snakemake_interface_storage_plugins/tests.py
--rw-r--r--   0        0        0     9369 1970-01-01 00:00:00.000000 snakemake_interface_storage_plugins-3.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1076 2024-04-15 08:35:34.470394 snakemake_interface_storage_plugins-3.2.0/LICENSE
+-rw-r--r--   0        0        0     8633 2024-04-15 08:35:34.470394 snakemake_interface_storage_plugins-3.2.0/README.md
+-rw-r--r--   0        0        0      911 2024-04-15 08:35:34.470394 snakemake_interface_storage_plugins-3.2.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-15 08:35:34.470394 snakemake_interface_storage_plugins-3.2.0/snakemake_interface_storage_plugins/__init__.py
+-rw-r--r--   0        0        0      525 2024-04-15 08:35:34.470394 snakemake_interface_storage_plugins-3.2.0/snakemake_interface_storage_plugins/common.py
+-rw-r--r--   0        0        0     2858 2024-04-15 08:35:34.470394 snakemake_interface_storage_plugins-3.2.0/snakemake_interface_storage_plugins/io.py
+-rw-r--r--   0        0        0     2041 2024-04-15 08:35:34.470394 snakemake_interface_storage_plugins-3.2.0/snakemake_interface_storage_plugins/registry/__init__.py
+-rw-r--r--   0        0        0     1315 2024-04-15 08:35:34.470394 snakemake_interface_storage_plugins-3.2.0/snakemake_interface_storage_plugins/registry/plugin.py
+-rw-r--r--   0        0        0      898 2024-04-15 08:35:34.470394 snakemake_interface_storage_plugins-3.2.0/snakemake_interface_storage_plugins/settings.py
+-rw-r--r--   0        0        0     7389 2024-04-15 08:35:34.470394 snakemake_interface_storage_plugins-3.2.0/snakemake_interface_storage_plugins/storage_object.py
+-rw-r--r--   0        0        0     5155 2024-04-15 08:35:34.470394 snakemake_interface_storage_plugins-3.2.0/snakemake_interface_storage_plugins/storage_provider.py
+-rw-r--r--   0        0        0     4118 2024-04-15 08:35:34.470394 snakemake_interface_storage_plugins-3.2.0/snakemake_interface_storage_plugins/tests.py
+-rw-r--r--   0        0        0     9369 1970-01-01 00:00:00.000000 snakemake_interface_storage_plugins-3.2.0/PKG-INFO
```

### Comparing `snakemake_interface_storage_plugins-3.1.1/LICENSE` & `snakemake_interface_storage_plugins-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `snakemake_interface_storage_plugins-3.1.1/README.md` & `snakemake_interface_storage_plugins-3.2.0/README.md`

 * *Files identical despite different names*

### Comparing `snakemake_interface_storage_plugins-3.1.1/pyproject.toml` & `snakemake_interface_storage_plugins-3.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "snakemake-interface-storage-plugins"
-version = "3.1.1"
+version = "3.2.0"
 description = "This package provides a stable interface for interactions between Snakemake and its storage plugins."
 authors = ["Johannes Koester <johannes.koester@uni-due.de>"]
 readme = "README.md"
 homepage = "https://github.com/snakemake/snakemake-interface-storage-plugins"
 
 [tool.poetry.dependencies]
 python = "^3.11"
```

### Comparing `snakemake_interface_storage_plugins-3.1.1/snakemake_interface_storage_plugins/common.py` & `snakemake_interface_storage_plugins-3.2.0/snakemake_interface_storage_plugins/common.py`

 * *Files identical despite different names*

### Comparing `snakemake_interface_storage_plugins-3.1.1/snakemake_interface_storage_plugins/io.py` & `snakemake_interface_storage_plugins-3.2.0/snakemake_interface_storage_plugins/io.py`

 * *Files identical despite different names*

### Comparing `snakemake_interface_storage_plugins-3.1.1/snakemake_interface_storage_plugins/registry/__init__.py` & `snakemake_interface_storage_plugins-3.2.0/snakemake_interface_storage_plugins/registry/__init__.py`

 * *Files identical despite different names*

### Comparing `snakemake_interface_storage_plugins-3.1.1/snakemake_interface_storage_plugins/registry/plugin.py` & `snakemake_interface_storage_plugins-3.2.0/snakemake_interface_storage_plugins/registry/plugin.py`

 * *Files identical despite different names*

### Comparing `snakemake_interface_storage_plugins-3.1.1/snakemake_interface_storage_plugins/settings.py` & `snakemake_interface_storage_plugins-3.2.0/snakemake_interface_storage_plugins/settings.py`

 * *Files identical despite different names*

### Comparing `snakemake_interface_storage_plugins-3.1.1/snakemake_interface_storage_plugins/storage_object.py` & `snakemake_interface_storage_plugins-3.2.0/snakemake_interface_storage_plugins/storage_object.py`

 * *Files identical despite different names*

### Comparing `snakemake_interface_storage_plugins-3.1.1/snakemake_interface_storage_plugins/storage_provider.py` & `snakemake_interface_storage_plugins-3.2.0/snakemake_interface_storage_plugins/storage_provider.py`

 * *Files identical despite different names*

### Comparing `snakemake_interface_storage_plugins-3.1.1/snakemake_interface_storage_plugins/tests.py` & `snakemake_interface_storage_plugins-3.2.0/snakemake_interface_storage_plugins/tests.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 __copyright__ = "Copyright 2023, Christopher Tomkins-Tinch, Johannes Köster"
 __email__ = "johannes.koester@uni-due.de"
 __license__ = "MIT"
 
 from abc import ABC, abstractmethod
 import asyncio
 from pathlib import Path
+import sys
 from typing import Optional, Type
 
 from snakemake_interface_storage_plugins.storage_provider import (
     StorageProviderBase,
     StorageQueryValidationResult,
 )
 from snakemake_interface_storage_plugins.settings import (
@@ -20,14 +21,15 @@
 
 class TestStorageBase(ABC):
     __test__ = False
     retrieve_only = False
     store_only = False
     delete = True
     touch = False
+    files_only = True
 
     @abstractmethod
     def get_storage_provider_cls(self) -> Type[StorageProviderBase]:
         ...
 
     def get_storage_provider_settings(self) -> Optional[StorageProviderSettingsBase]:
         return None
@@ -42,25 +44,41 @@
 
     def _get_obj(self, tmp_path, query):
         provider = self._get_provider(tmp_path)
 
         return provider.object(query)
 
     def test_storage(self, tmp_path):
+        self._test_storage(tmp_path, directory=False)
+        if not self.files_only:
+            self._test_storage(tmp_path, directory=True)
+
+    def _test_storage(self, tmp_path, directory=False):
+        print(
+            f"Testing storage of {'files' if not directory else 'directories'}.",
+            file=sys.stderr,
+        )
+
         assert not (
             self.store_only and self.retrieve_only
         ), "store_only and retrieve_only may not be True at the same time"
 
         obj = self._get_obj(tmp_path, self.get_query(tmp_path))
 
         stored = False
         try:
             if not self.retrieve_only:
-                obj.local_path().parent.mkdir(parents=True, exist_ok=True)
-                with open(obj.local_path(), "w") as f:
+                if directory:
+                    dirpath = obj.local_path()
+                    filepath = dirpath / "test.txt"
+                else:
+                    dirpath = obj.local_path().parent
+                    filepath = obj.local_path()
+                dirpath.mkdir(parents=True, exist_ok=True)
+                with open(filepath, "w") as f:
                     f.write("test")
                     f.flush()
                 obj.store_object()
                 stored = True
                 obj.local_path().unlink()
 
             assert obj.exists()
```

### Comparing `snakemake_interface_storage_plugins-3.1.1/PKG-INFO` & `snakemake_interface_storage_plugins-3.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snakemake-interface-storage-plugins
-Version: 3.1.1
+Version: 3.2.0
 Summary: This package provides a stable interface for interactions between Snakemake and its storage plugins.
 Home-page: https://github.com/snakemake/snakemake-interface-storage-plugins
 Author: Johannes Koester
 Author-email: johannes.koester@uni-due.de
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
```

