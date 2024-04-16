# Comparing `tmp/pdm_download-0.1.1.tar.gz` & `tmp/pdm_download-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdm_download-0.1.1.tar", last modified: Thu Feb 22 05:05:07 2024, max compression
+gzip compressed data, was "pdm_download-0.1.2.tar", last modified: Tue Apr 16 10:27:58 2024, max compression
```

## Comparing `pdm_download-0.1.1.tar` & `pdm_download-0.1.2.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0     1067 2024-02-22 05:04:55.677606 pdm_download-0.1.1/LICENSE
--rw-r--r--   0        0        0     1074 2024-02-22 05:04:55.677606 pdm_download-0.1.1/README.md
--rw-r--r--   0        0        0      943 2024-02-22 05:05:07.565659 pdm_download-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      233 2024-02-22 05:04:55.677606 pdm_download-0.1.1/src/pdm_download/__init__.py
--rw-r--r--   0        0        0     6319 2024-02-22 05:04:55.677606 pdm_download-0.1.1/src/pdm_download/command.py
--rw-r--r--   0        0        0        0 2024-02-22 05:04:55.677606 pdm_download-0.1.1/tests/__init__.py
--rw-r--r--   0        0        0   162530 2024-02-22 05:04:55.677606 pdm_download-0.1.1/tests/packages/certifi-2023.11.17-py3-none-any.whl
--rw-r--r--   0        0        0   163637 2024-02-22 05:04:55.677606 pdm_download-0.1.1/tests/packages/certifi-2023.11.17.tar.gz
--rw-r--r--   0        0        0   133356 2024-02-22 05:04:55.681606 pdm_download-0.1.1/tests/packages/chardet-3.0.4-py2.py3-none-any.whl
--rw-r--r--   0        0        0  1868453 2024-02-22 05:04:55.681606 pdm_download-0.1.1/tests/packages/chardet-3.0.4.tar.gz
--rw-r--r--   0        0        0    58811 2024-02-22 05:04:55.681606 pdm_download-0.1.1/tests/packages/idna-2.10-py2.py3-none-any.whl
--rw-r--r--   0        0        0   175616 2024-02-22 05:04:55.685606 pdm_download-0.1.1/tests/packages/idna-2.10.tar.gz
--rw-r--r--   0        0        0    61826 2024-02-22 05:04:55.685606 pdm_download-0.1.1/tests/packages/requests-2.24.0-py2.py3-none-any.whl
--rw-r--r--   0        0        0   115071 2024-02-22 05:04:55.685606 pdm_download-0.1.1/tests/packages/requests-2.24.0.tar.gz
--rw-r--r--   0        0        0   127978 2024-02-22 05:04:55.685606 pdm_download-0.1.1/tests/packages/urllib3-1.25.11-py2.py3-none-any.whl
--rw-r--r--   0        0        0   260300 2024-02-22 05:04:55.685606 pdm_download-0.1.1/tests/packages/urllib3-1.25.11.tar.gz
--rw-r--r--   0        0        0     2496 2024-02-22 05:04:55.685606 pdm_download-0.1.1/tests/project/pdm.lock
--rw-r--r--   0        0        0     2721 2024-02-22 05:04:55.685606 pdm_download-0.1.1/tests/project/pdm.static.lock
--rw-r--r--   0        0        0      154 2024-02-22 05:04:55.685606 pdm_download-0.1.1/tests/project/pyproject.toml
--rw-r--r--   0        0        0     1098 2024-02-22 05:04:55.685606 pdm_download-0.1.1/tests/test_download.py
--rw-r--r--   0        0        0     1731 1970-01-01 00:00:00.000000 pdm_download-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1067 2024-04-16 10:27:48.605636 pdm_download-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1074 2024-04-16 10:27:48.605636 pdm_download-0.1.2/README.md
+-rw-r--r--   0        0        0      943 2024-04-16 10:27:58.425716 pdm_download-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      233 2024-04-16 10:27:48.605636 pdm_download-0.1.2/src/pdm_download/__init__.py
+-rw-r--r--   0        0        0     6484 2024-04-16 10:27:48.605636 pdm_download-0.1.2/src/pdm_download/command.py
+-rw-r--r--   0        0        0        0 2024-04-16 10:27:48.605636 pdm_download-0.1.2/tests/__init__.py
+-rw-r--r--   0        0        0   162530 2024-04-16 10:27:48.605636 pdm_download-0.1.2/tests/packages/certifi-2023.11.17-py3-none-any.whl
+-rw-r--r--   0        0        0   163637 2024-04-16 10:27:48.605636 pdm_download-0.1.2/tests/packages/certifi-2023.11.17.tar.gz
+-rw-r--r--   0        0        0   133356 2024-04-16 10:27:48.605636 pdm_download-0.1.2/tests/packages/chardet-3.0.4-py2.py3-none-any.whl
+-rw-r--r--   0        0        0  1868453 2024-04-16 10:27:48.609636 pdm_download-0.1.2/tests/packages/chardet-3.0.4.tar.gz
+-rw-r--r--   0        0        0    58811 2024-04-16 10:27:48.609636 pdm_download-0.1.2/tests/packages/idna-2.10-py2.py3-none-any.whl
+-rw-r--r--   0        0        0   175616 2024-04-16 10:27:48.609636 pdm_download-0.1.2/tests/packages/idna-2.10.tar.gz
+-rw-r--r--   0        0        0    61826 2024-04-16 10:27:48.609636 pdm_download-0.1.2/tests/packages/requests-2.24.0-py2.py3-none-any.whl
+-rw-r--r--   0        0        0   115071 2024-04-16 10:27:48.609636 pdm_download-0.1.2/tests/packages/requests-2.24.0.tar.gz
+-rw-r--r--   0        0        0   127978 2024-04-16 10:27:48.613636 pdm_download-0.1.2/tests/packages/urllib3-1.25.11-py2.py3-none-any.whl
+-rw-r--r--   0        0        0   260300 2024-04-16 10:27:48.613636 pdm_download-0.1.2/tests/packages/urllib3-1.25.11.tar.gz
+-rw-r--r--   0        0        0     2496 2024-04-16 10:27:48.613636 pdm_download-0.1.2/tests/project/pdm.lock
+-rw-r--r--   0        0        0     2721 2024-04-16 10:27:48.613636 pdm_download-0.1.2/tests/project/pdm.static.lock
+-rw-r--r--   0        0        0      154 2024-04-16 10:27:48.613636 pdm_download-0.1.2/tests/project/pyproject.toml
+-rw-r--r--   0        0        0     1098 2024-04-16 10:27:48.613636 pdm_download-0.1.2/tests/test_download.py
+-rw-r--r--   0        0        0     1731 1970-01-01 00:00:00.000000 pdm_download-0.1.2/PKG-INFO
```

### Comparing `pdm_download-0.1.1/LICENSE` & `pdm_download-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pdm_download-0.1.1/README.md` & `pdm_download-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `pdm_download-0.1.1/pyproject.toml` & `pdm_download-0.1.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     "Programming Language :: Python :: 3 :: Only",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
 ]
-version = "0.1.1"
+version = "0.1.2"
 
 [project.license]
 text = "MIT"
 
 [project.urls]
 Repository = "https://github.com/pdm-project/pdm-download"
```

### Comparing `pdm_download-0.1.1/src/pdm_download/command.py` & `pdm_download-0.1.2/src/pdm_download/command.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 from __future__ import annotations
 
 import argparse
 import hashlib
 from collections import defaultdict
 from concurrent.futures import Future, ThreadPoolExecutor
 from pathlib import Path
-from typing import TYPE_CHECKING, Iterable, Sequence, cast
+from typing import TYPE_CHECKING, Any, Iterable, Iterator, Sequence, cast
 
-from pdm import termui
 from pdm.cli.commands.base import BaseCommand
 from pdm.cli.options import lockfile_option
 from pdm.exceptions import PdmUsageError
 from rich.progress import (
     BarColumn,
     MofNCompleteColumn,
     Progress,
@@ -28,26 +27,32 @@
 
     class FileHash(TypedDict):
         url: str
         hash: str
         file: str
 
 
+def _iter_content_compat(resp: Any, chunk_size: int) -> Iterator[bytes]:
+    if hasattr(resp, "iter_content"):
+        return resp.iter_content(chunk_size)
+    return resp.iter_bytes(chunk_size)
+
+
 def _download_package(project: Project, package: FileHash, dest: Path) -> None:
     from unearth import Link
 
     hash_name, hash_value = package["hash"].split(":")
     hasher = hashlib.new(hash_name)
     with project.environment.get_finder() as finder:
         session = finder.session
         with session.get(package["url"], stream=True) as resp, dest.joinpath(
             package.get("file", Link(package["url"]).filename)
         ).open("wb") as fp:
             resp.raise_for_status()
-            for chunk in resp.iter_content(chunk_size=8192):
+            for chunk in _iter_content_compat(resp, chunk_size=8192):
                 hasher.update(chunk)
                 fp.write(chunk)
     if hasher.hexdigest() != hash_value:
         raise RuntimeError(
             f"Hash value of {package['file']} doesn't match. "
             f"Expected: {hash_value}, got: {hasher.hexdigest()}"
         )
@@ -66,15 +71,14 @@
         "•",
         MofNCompleteColumn(),
         "•",
         TimeRemainingColumn(),
         "•",
         TaskProgressColumn(),
         transient=True,
-        console=termui._console,
     ) as progress:
         task = progress.add_task("Downloading", total=len(packages))
         success_count = 0
 
         def progress_callback(future: Future) -> None:
             nonlocal success_count
             if future.exception():
```

### Comparing `pdm_download-0.1.1/tests/packages/certifi-2023.11.17-py3-none-any.whl` & `pdm_download-0.1.2/tests/packages/certifi-2023.11.17-py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm_download-0.1.1/tests/packages/certifi-2023.11.17.tar.gz` & `pdm_download-0.1.2/tests/packages/certifi-2023.11.17.tar.gz`

 * *Files identical despite different names*

### Comparing `pdm_download-0.1.1/tests/packages/chardet-3.0.4-py2.py3-none-any.whl` & `pdm_download-0.1.2/tests/packages/chardet-3.0.4-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm_download-0.1.1/tests/packages/chardet-3.0.4.tar.gz` & `pdm_download-0.1.2/tests/packages/chardet-3.0.4.tar.gz`

 * *Files identical despite different names*

### Comparing `pdm_download-0.1.1/tests/packages/idna-2.10-py2.py3-none-any.whl` & `pdm_download-0.1.2/tests/packages/idna-2.10-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm_download-0.1.1/tests/packages/idna-2.10.tar.gz` & `pdm_download-0.1.2/tests/packages/idna-2.10.tar.gz`

 * *Files identical despite different names*

### Comparing `pdm_download-0.1.1/tests/packages/requests-2.24.0-py2.py3-none-any.whl` & `pdm_download-0.1.2/tests/packages/requests-2.24.0-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm_download-0.1.1/tests/packages/requests-2.24.0.tar.gz` & `pdm_download-0.1.2/tests/packages/requests-2.24.0.tar.gz`

 * *Files identical despite different names*

### Comparing `pdm_download-0.1.1/tests/packages/urllib3-1.25.11-py2.py3-none-any.whl` & `pdm_download-0.1.2/tests/packages/urllib3-1.25.11-py2.py3-none-any.whl`

 * *Files identical despite different names*

### Comparing `pdm_download-0.1.1/tests/packages/urllib3-1.25.11.tar.gz` & `pdm_download-0.1.2/tests/packages/urllib3-1.25.11.tar.gz`

 * *Files identical despite different names*

### Comparing `pdm_download-0.1.1/tests/project/pdm.lock` & `pdm_download-0.1.2/tests/project/pdm.lock`

 * *Files identical despite different names*

### Comparing `pdm_download-0.1.1/tests/project/pdm.static.lock` & `pdm_download-0.1.2/tests/project/pdm.static.lock`

 * *Files identical despite different names*

### Comparing `pdm_download-0.1.1/tests/test_download.py` & `pdm_download-0.1.2/tests/test_download.py`

 * *Files identical despite different names*

### Comparing `pdm_download-0.1.1/PKG-INFO` & `pdm_download-0.1.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdm-download
-Version: 0.1.1
+Version: 0.1.2
 Summary: A PDM plugin to download all packages in a lockfile for offline use.
 Author-Email: Frost Ming <me@frostming.com>
 License: MIT
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

