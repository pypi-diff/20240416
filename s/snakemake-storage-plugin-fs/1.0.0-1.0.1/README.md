# Comparing `tmp/snakemake_storage_plugin_fs-1.0.0.tar.gz` & `tmp/snakemake_storage_plugin_fs-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snakemake_storage_plugin_fs-1.0.0.tar", max compression
+gzip compressed data, was "snakemake_storage_plugin_fs-1.0.1.tar", max compression
```

## Comparing `snakemake_storage_plugin_fs-1.0.0.tar` & `snakemake_storage_plugin_fs-1.0.1.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0     1066 2024-02-28 06:58:29.817946 snakemake_storage_plugin_fs-1.0.0/LICENSE
--rw-r--r--   0        0        0      139 2024-02-28 06:58:29.817946 snakemake_storage_plugin_fs-1.0.0/README.md
--rw-r--r--   0        0        0      948 2024-02-28 06:58:29.817946 snakemake_storage_plugin_fs-1.0.0/pyproject.toml
--rw-r--r--   0        0        0     8924 2024-02-28 06:58:29.817946 snakemake_storage_plugin_fs-1.0.0/snakemake_storage_plugin_fs/__init__.py
--rw-r--r--   0        0        0     1185 1970-01-01 00:00:00.000000 snakemake_storage_plugin_fs-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1066 2024-04-16 14:58:15.716772 snakemake_storage_plugin_fs-1.0.1/LICENSE
+-rw-r--r--   0        0        0      139 2024-04-16 14:58:15.716772 snakemake_storage_plugin_fs-1.0.1/README.md
+-rw-r--r--   0        0        0      948 2024-04-16 14:58:15.716772 snakemake_storage_plugin_fs-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0     9268 2024-04-16 14:58:15.716772 snakemake_storage_plugin_fs-1.0.1/snakemake_storage_plugin_fs/__init__.py
+-rw-r--r--   0        0        0     1185 1970-01-01 00:00:00.000000 snakemake_storage_plugin_fs-1.0.1/PKG-INFO
```

### Comparing `snakemake_storage_plugin_fs-1.0.0/LICENSE` & `snakemake_storage_plugin_fs-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `snakemake_storage_plugin_fs-1.0.0/pyproject.toml` & `snakemake_storage_plugin_fs-1.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "snakemake-storage-plugin-fs"
-version = "1.0.0"
+version = "1.0.1"
 description = " A Snakemake storage plugin that reads and writes from a locally mounted filesystem using rsync"
 authors = ["Johannes Koester <johannes.koester@uni-due.de>"]
 readme = "README.md"
 license = "MIT"
 repository = "https://github.com/snakemake/snakemake-storage-plugin-fs"
 documentation = "https://snakemake.github.io/snakemake-plugin-catalog/plugins/storage/fs.html"
 keywords = ["snakemake", "plugin", "storage", "filesystem", "rsync"]
```

### Comparing `snakemake_storage_plugin_fs-1.0.0/snakemake_storage_plugin_fs/__init__.py` & `snakemake_storage_plugin_fs-1.0.1/snakemake_storage_plugin_fs/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os
 from pathlib import Path
 import shutil
 import subprocess
 from typing import Any, Iterable, List, Optional
+from urllib.parse import urlparse
 
 import sysrsync
 
 from snakemake_interface_common.exceptions import WorkflowError
 from snakemake_interface_storage_plugins.storage_provider import (
     StorageProviderBase,
     ExampleQuery,
@@ -75,14 +76,24 @@
 
     @classmethod
     def is_valid_query(cls, query: str) -> StorageQueryValidationResult:
         """Return whether the given query is valid for this storage provider."""
         # Ensure that also queries containing wildcards (e.g. {sample}) are accepted
         # and considered valid. The wildcards will be resolved before the storage
         # object is actually used.
+
+        # disallow queries that are URL like
+        parsed = urlparse(query)
+        if parsed.scheme:
+            return StorageQueryValidationResult(
+                query=query,
+                valid=False,
+                message="Query is URL-like, but should be a system path instead.",
+            )
+
         try:
             Path(query)
         except Exception:
             return StorageQueryValidationResult(
                 query=query,
                 valid=False,
                 message="Query is not a valid path.",
```

### Comparing `snakemake_storage_plugin_fs-1.0.0/PKG-INFO` & `snakemake_storage_plugin_fs-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: snakemake-storage-plugin-fs
-Version: 1.0.0
+Version: 1.0.1
 Summary:  A Snakemake storage plugin that reads and writes from a locally mounted filesystem using rsync
 Home-page: https://github.com/snakemake/snakemake-storage-plugin-fs
 License: MIT
 Keywords: snakemake,plugin,storage,filesystem,rsync
 Author: Johannes Koester
 Author-email: johannes.koester@uni-due.de
 Requires-Python: >=3.11,<4.0
```

