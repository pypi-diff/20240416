# Comparing `tmp/kagglehub-0.2.2.tar.gz` & `tmp/kagglehub-0.2.3.tar.gz`

## Comparing `kagglehub-0.2.2.tar` & `kagglehub-0.2.3.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0     4110 2020-02-02 00:00:00.000000 kagglehub-0.2.2/CHANGELOG.md
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 kagglehub-0.2.2/Dockerfile
--rwxr-xr-x   0        0        0     1683 2020-02-02 00:00:00.000000 kagglehub-0.2.2/docker-hatch
--rw-r--r--   0        0        0     3340 2020-02-02 00:00:00.000000 kagglehub-0.2.2/integration_tests/test_model_download.py
--rw-r--r--   0        0        0     5346 2020-02-02 00:00:00.000000 kagglehub-0.2.2/integration_tests/test_model_upload.py
--rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 kagglehub-0.2.2/src/kagglehub/__init__.py
--rw-r--r--   0        0        0     4996 2020-02-02 00:00:00.000000 kagglehub-0.2.2/src/kagglehub/auth.py
--rw-r--r--   0        0        0     4716 2020-02-02 00:00:00.000000 kagglehub-0.2.2/src/kagglehub/cache.py
--rw-r--r--   0        0        0    11513 2020-02-02 00:00:00.000000 kagglehub-0.2.2/src/kagglehub/clients.py
--rw-r--r--   0        0        0     3067 2020-02-02 00:00:00.000000 kagglehub-0.2.2/src/kagglehub/colab_cache_resolver.py
--rw-r--r--   0        0        0     4960 2020-02-02 00:00:00.000000 kagglehub-0.2.2/src/kagglehub/config.py
--rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 kagglehub-0.2.2/src/kagglehub/env.py
--rw-r--r--   0        0        0     3625 2020-02-02 00:00:00.000000 kagglehub-0.2.2/src/kagglehub/exceptions.py
--rw-r--r--   0        0        0     6797 2020-02-02 00:00:00.000000 kagglehub-0.2.2/src/kagglehub/gcs_upload.py
--rw-r--r--   0        0        0     2958 2020-02-02 00:00:00.000000 kagglehub-0.2.2/src/kagglehub/handle.py
--rw-r--r--   0        0        0     3130 2020-02-02 00:00:00.000000 kagglehub-0.2.2/src/kagglehub/http_resolver.py
--rw-r--r--   0        0        0     1464 2020-02-02 00:00:00.000000 kagglehub-0.2.2/src/kagglehub/integrity.py
--rw-r--r--   0        0        0     2964 2020-02-02 00:00:00.000000 kagglehub-0.2.2/src/kagglehub/kaggle_cache_resolver.py
--rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 kagglehub-0.2.2/src/kagglehub/logging.py
--rw-r--r--   0        0        0     1852 2020-02-02 00:00:00.000000 kagglehub-0.2.2/src/kagglehub/models.py
--rw-r--r--   0        0        0     3630 2020-02-02 00:00:00.000000 kagglehub-0.2.2/src/kagglehub/models_helpers.py
--rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 kagglehub-0.2.2/src/kagglehub/registry.py
--rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 kagglehub-0.2.2/src/kagglehub/resolver.py
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 kagglehub-0.2.2/tests/__init__.py
--rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 kagglehub-0.2.2/tests/fixtures.py
--rw-r--r--   0        0        0     4925 2020-02-02 00:00:00.000000 kagglehub-0.2.2/tests/test_auth.py
--rw-r--r--   0        0        0     8114 2020-02-02 00:00:00.000000 kagglehub-0.2.2/tests/test_cache.py
--rw-r--r--   0        0        0     5644 2020-02-02 00:00:00.000000 kagglehub-0.2.2/tests/test_colab_cache_model_download.py
--rw-r--r--   0        0        0     7071 2020-02-02 00:00:00.000000 kagglehub-0.2.2/tests/test_config.py
--rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 kagglehub-0.2.2/tests/test_handle.py
--rw-r--r--   0        0        0    12013 2020-02-02 00:00:00.000000 kagglehub-0.2.2/tests/test_http_model_download.py
--rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 kagglehub-0.2.2/tests/test_integrity.py
--rw-r--r--   0        0        0     5361 2020-02-02 00:00:00.000000 kagglehub-0.2.2/tests/test_kaggle_api_client.py
--rw-r--r--   0        0        0     6145 2020-02-02 00:00:00.000000 kagglehub-0.2.2/tests/test_kaggle_cache_model_download.py
--rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 kagglehub-0.2.2/tests/test_kagglehub_version.py
--rw-r--r--   0        0        0    12928 2020-02-02 00:00:00.000000 kagglehub-0.2.2/tests/test_model_upload.py
--rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 kagglehub-0.2.2/tests/test_registry.py
--rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 kagglehub-0.2.2/tests/test_utils.py
--rw-r--r--   0        0        0     4314 2020-02-02 00:00:00.000000 kagglehub-0.2.2/tests/utils.py
--rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 kagglehub-0.2.2/tests/data/archive.tar.gz
--rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 kagglehub-0.2.2/tests/data/config.json
--rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 kagglehub-0.2.2/tests/data/foo.txt
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 kagglehub-0.2.2/tools/cicd/Dockerfile
--rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 kagglehub-0.2.2/tools/cicd/cloudbuild.yaml
--rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 kagglehub-0.2.2/tools/cicd/integration-tests.yaml
--rw-r--r--   0        0        0     3184 2020-02-02 00:00:00.000000 kagglehub-0.2.2/tools/release/cloudbuild.yaml
--rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 kagglehub-0.2.2/.gitignore
--rw-r--r--   0        0        0    11541 2020-02-02 00:00:00.000000 kagglehub-0.2.2/LICENSE
--rw-r--r--   0        0        0     4590 2020-02-02 00:00:00.000000 kagglehub-0.2.2/README.md
--rw-r--r--   0        0        0     3130 2020-02-02 00:00:00.000000 kagglehub-0.2.2/pyproject.toml
--rw-r--r--   0        0        0    18113 2020-02-02 00:00:00.000000 kagglehub-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0     4219 2020-02-02 00:00:00.000000 kagglehub-0.2.3/CHANGELOG.md
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 kagglehub-0.2.3/Dockerfile
+-rwxr-xr-x   0        0        0     1683 2020-02-02 00:00:00.000000 kagglehub-0.2.3/docker-hatch
+-rw-r--r--   0        0        0     3340 2020-02-02 00:00:00.000000 kagglehub-0.2.3/integration_tests/test_model_download.py
+-rw-r--r--   0        0        0     5347 2020-02-02 00:00:00.000000 kagglehub-0.2.3/integration_tests/test_model_upload.py
+-rw-r--r--   0        0        0      581 2020-02-02 00:00:00.000000 kagglehub-0.2.3/src/kagglehub/__init__.py
+-rw-r--r--   0        0        0     4996 2020-02-02 00:00:00.000000 kagglehub-0.2.3/src/kagglehub/auth.py
+-rw-r--r--   0        0        0     4716 2020-02-02 00:00:00.000000 kagglehub-0.2.3/src/kagglehub/cache.py
+-rw-r--r--   0        0        0    11513 2020-02-02 00:00:00.000000 kagglehub-0.2.3/src/kagglehub/clients.py
+-rw-r--r--   0        0        0     3067 2020-02-02 00:00:00.000000 kagglehub-0.2.3/src/kagglehub/colab_cache_resolver.py
+-rw-r--r--   0        0        0     4960 2020-02-02 00:00:00.000000 kagglehub-0.2.3/src/kagglehub/config.py
+-rw-r--r--   0        0        0     1065 2020-02-02 00:00:00.000000 kagglehub-0.2.3/src/kagglehub/env.py
+-rw-r--r--   0        0        0     3625 2020-02-02 00:00:00.000000 kagglehub-0.2.3/src/kagglehub/exceptions.py
+-rw-r--r--   0        0        0     7564 2020-02-02 00:00:00.000000 kagglehub-0.2.3/src/kagglehub/gcs_upload.py
+-rw-r--r--   0        0        0     2905 2020-02-02 00:00:00.000000 kagglehub-0.2.3/src/kagglehub/handle.py
+-rw-r--r--   0        0        0     3130 2020-02-02 00:00:00.000000 kagglehub-0.2.3/src/kagglehub/http_resolver.py
+-rw-r--r--   0        0        0     1464 2020-02-02 00:00:00.000000 kagglehub-0.2.3/src/kagglehub/integrity.py
+-rw-r--r--   0        0        0     2964 2020-02-02 00:00:00.000000 kagglehub-0.2.3/src/kagglehub/kaggle_cache_resolver.py
+-rw-r--r--   0        0        0      527 2020-02-02 00:00:00.000000 kagglehub-0.2.3/src/kagglehub/logging.py
+-rw-r--r--   0        0        0     1852 2020-02-02 00:00:00.000000 kagglehub-0.2.3/src/kagglehub/models.py
+-rw-r--r--   0        0        0     3630 2020-02-02 00:00:00.000000 kagglehub-0.2.3/src/kagglehub/models_helpers.py
+-rw-r--r--   0        0        0     1174 2020-02-02 00:00:00.000000 kagglehub-0.2.3/src/kagglehub/registry.py
+-rw-r--r--   0        0        0      932 2020-02-02 00:00:00.000000 kagglehub-0.2.3/src/kagglehub/resolver.py
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 kagglehub-0.2.3/tests/__init__.py
+-rw-r--r--   0        0        0      349 2020-02-02 00:00:00.000000 kagglehub-0.2.3/tests/fixtures.py
+-rw-r--r--   0        0        0     4925 2020-02-02 00:00:00.000000 kagglehub-0.2.3/tests/test_auth.py
+-rw-r--r--   0        0        0     8114 2020-02-02 00:00:00.000000 kagglehub-0.2.3/tests/test_cache.py
+-rw-r--r--   0        0        0     5644 2020-02-02 00:00:00.000000 kagglehub-0.2.3/tests/test_colab_cache_model_download.py
+-rw-r--r--   0        0        0     7071 2020-02-02 00:00:00.000000 kagglehub-0.2.3/tests/test_config.py
+-rw-r--r--   0        0        0     1436 2020-02-02 00:00:00.000000 kagglehub-0.2.3/tests/test_handle.py
+-rw-r--r--   0        0        0    12013 2020-02-02 00:00:00.000000 kagglehub-0.2.3/tests/test_http_model_download.py
+-rw-r--r--   0        0        0     1090 2020-02-02 00:00:00.000000 kagglehub-0.2.3/tests/test_integrity.py
+-rw-r--r--   0        0        0     5361 2020-02-02 00:00:00.000000 kagglehub-0.2.3/tests/test_kaggle_api_client.py
+-rw-r--r--   0        0        0     6145 2020-02-02 00:00:00.000000 kagglehub-0.2.3/tests/test_kaggle_cache_model_download.py
+-rw-r--r--   0        0        0      196 2020-02-02 00:00:00.000000 kagglehub-0.2.3/tests/test_kagglehub_version.py
+-rw-r--r--   0        0        0    12928 2020-02-02 00:00:00.000000 kagglehub-0.2.3/tests/test_model_upload.py
+-rw-r--r--   0        0        0     1607 2020-02-02 00:00:00.000000 kagglehub-0.2.3/tests/test_registry.py
+-rw-r--r--   0        0        0     1873 2020-02-02 00:00:00.000000 kagglehub-0.2.3/tests/test_utils.py
+-rw-r--r--   0        0        0     4314 2020-02-02 00:00:00.000000 kagglehub-0.2.3/tests/utils.py
+-rw-r--r--   0        0        0      184 2020-02-02 00:00:00.000000 kagglehub-0.2.3/tests/data/archive.tar.gz
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 kagglehub-0.2.3/tests/data/config.json
+-rw-r--r--   0        0        0        3 2020-02-02 00:00:00.000000 kagglehub-0.2.3/tests/data/foo.txt
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 kagglehub-0.2.3/tools/cicd/Dockerfile
+-rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 kagglehub-0.2.3/tools/cicd/cloudbuild.yaml
+-rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 kagglehub-0.2.3/tools/cicd/integration-tests.yaml
+-rw-r--r--   0        0        0     3184 2020-02-02 00:00:00.000000 kagglehub-0.2.3/tools/release/cloudbuild.yaml
+-rw-r--r--   0        0        0     3077 2020-02-02 00:00:00.000000 kagglehub-0.2.3/.gitignore
+-rw-r--r--   0        0        0    11541 2020-02-02 00:00:00.000000 kagglehub-0.2.3/LICENSE
+-rw-r--r--   0        0        0     4546 2020-02-02 00:00:00.000000 kagglehub-0.2.3/README.md
+-rw-r--r--   0        0        0     3130 2020-02-02 00:00:00.000000 kagglehub-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0    18069 2020-02-02 00:00:00.000000 kagglehub-0.2.3/PKG-INFO
```

### Comparing `kagglehub-0.2.2/CHANGELOG.md` & `kagglehub-0.2.3/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 # Changelog
 
 ## Next (Unreleased)
 
+## v0.2.3 (April 16th, 2024)
+
+* Improve upload speed ([#100](https://github.com/Kaggle/kagglehub/pull/100))
+
 ## v0.2.2 (March 27th, 2024)
 
 * Add support for single file upload ([#97](https://github.com/Kaggle/kagglehub/pull/97))
 
 ## v0.2.1 (March 21th, 2024)
 
 * Add support for directory upload ([#82](https://github.com/Kaggle/kagglehub/pull/93))
```

### Comparing `kagglehub-0.2.2/docker-hatch` & `kagglehub-0.2.3/docker-hatch`

 * *Files identical despite different names*

### Comparing `kagglehub-0.2.2/integration_tests/test_model_download.py` & `kagglehub-0.2.3/integration_tests/test_model_download.py`

 * *Files identical despite different names*

### Comparing `kagglehub-0.2.2/integration_tests/test_model_upload.py` & `kagglehub-0.2.3/integration_tests/test_model_upload.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,15 +42,15 @@
             raise RuntimeError(runtime_error_message)
 
         return wrapper
 
     return decorator
 
 
-@retry(times=5, delay_seconds=5, exception_to_check=BackendError)
+@retry(times=5, delay_seconds=10, exception_to_check=BackendError)
 def upload_with_retries(handle: str, temp_dir: str, license_name: str) -> None:
     """
     Uploads a model with retries on BackendError indicating the instance slug is already in use.
 
     Args:
         handle: The model handle.
         temp_dir: Temporary directory where the model is stored.
```

### Comparing `kagglehub-0.2.2/src/kagglehub/__init__.py` & `kagglehub-0.2.3/src/kagglehub/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.2.2"
+__version__ = "0.2.3"
 
 import kagglehub.logging  # configures the library logger.
 from kagglehub import colab_cache_resolver, http_resolver, kaggle_cache_resolver, registry
 from kagglehub.auth import login
 from kagglehub.models import model_download, model_upload
 
 registry.model_resolver.add_implementation(http_resolver.ModelHttpResolver())
```

### Comparing `kagglehub-0.2.2/src/kagglehub/auth.py` & `kagglehub-0.2.3/src/kagglehub/auth.py`

 * *Files identical despite different names*

### Comparing `kagglehub-0.2.2/src/kagglehub/cache.py` & `kagglehub-0.2.3/src/kagglehub/cache.py`

 * *Files identical despite different names*

### Comparing `kagglehub-0.2.2/src/kagglehub/clients.py` & `kagglehub-0.2.3/src/kagglehub/clients.py`

 * *Files identical despite different names*

### Comparing `kagglehub-0.2.2/src/kagglehub/colab_cache_resolver.py` & `kagglehub-0.2.3/src/kagglehub/colab_cache_resolver.py`

 * *Files identical despite different names*

### Comparing `kagglehub-0.2.2/src/kagglehub/config.py` & `kagglehub-0.2.3/src/kagglehub/config.py`

 * *Files identical despite different names*

### Comparing `kagglehub-0.2.2/src/kagglehub/env.py` & `kagglehub-0.2.3/src/kagglehub/env.py`

 * *Files identical despite different names*

### Comparing `kagglehub-0.2.2/src/kagglehub/exceptions.py` & `kagglehub-0.2.3/src/kagglehub/exceptions.py`

 * *Files identical despite different names*

### Comparing `kagglehub-0.2.2/src/kagglehub/gcs_upload.py` & `kagglehub-0.2.3/src/kagglehub/gcs_upload.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import logging
 import os
+import shutil
 import time
 import zipfile
 from datetime import datetime
+from multiprocessing import Pool
 from pathlib import Path
 from tempfile import TemporaryDirectory
-from typing import List, Union
+from typing import List, Tuple, Union
 
 import requests
 from requests.exceptions import ConnectionError, Timeout
 from tqdm import tqdm
 from tqdm.utils import CallbackIOWrapper
 
 from kagglehub.clients import KaggleApiV1Client
@@ -132,36 +134,55 @@
                 retry_count += 1
                 uploaded_bytes = _check_uploaded_size(session_uri, file_size)
                 pbar.n = uploaded_bytes  # Update progress bar to reflect actual uploaded bytes
 
     return response["token"]
 
 
+def zip_file(args: Tuple[Path, Path, Path]) -> int:
+    file_path, zip_path, source_path_obj = args
+    arcname = file_path.relative_to(source_path_obj)
+    size = file_path.stat().st_size
+    with zipfile.ZipFile(zip_path, "a", zipfile.ZIP_STORED, allowZip64=True) as zipf:
+        zipf.write(file_path, arcname)
+    return size
+
+
+def zip_files(source_path_obj: Path, zip_path: Path) -> List[int]:
+    files = [file for file in source_path_obj.rglob("*") if file.is_file()]
+    args = [(file, zip_path, source_path_obj) for file in files]
+
+    with Pool() as pool:
+        sizes = pool.map(zip_file, args)
+    return sizes
+
+
 def upload_files(source_path: str, model_type: str) -> List[str]:
-    """Zip and Upload directory or a single file.
-    Parameters
-    ==========
-    source_path: the source path to upload from (can be a directory or a file)
-    model_type: Type of the model that is being uploaded.
-    """
     source_path_obj = Path(source_path)
-
     with TemporaryDirectory() as temp_dir:
         temp_dir_path = Path(temp_dir)
+        total_size = 0
 
         if source_path_obj.is_dir():
-            zip_path = temp_dir_path / TEMP_ARCHIVE_FILE
-            with zipfile.ZipFile(zip_path, "w", zipfile.ZIP_DEFLATED) as zipf:
-                for file_path in source_path_obj.rglob("*"):
-                    if file_path.is_file():
-                        arcname = file_path.relative_to(source_path_obj)
-                        zipf.write(file_path, arcname)
-            upload_path = str(zip_path)
+            for file_path in source_path_obj.rglob("*"):
+                if file_path.is_file():
+                    total_size += file_path.stat().st_size
         elif source_path_obj.is_file():
-            temp_file_path = temp_dir_path / source_path_obj.name
-            temp_file_path.write_bytes(source_path_obj.read_bytes())
-            upload_path = str(temp_file_path)
+            total_size = source_path_obj.stat().st_size
         else:
             path_error_message = "The source path does not point to a valid file or directory."
             raise ValueError(path_error_message)
 
+        with tqdm(total=total_size, desc="Zipping", unit="B", unit_scale=True, unit_divisor=1024) as pbar:
+            if source_path_obj.is_dir():
+                zip_path = temp_dir_path / "archive.zip"
+                sizes = zip_files(source_path_obj, zip_path)
+                for size in sizes:
+                    pbar.update(size)
+                upload_path = str(zip_path)
+            elif source_path_obj.is_file():
+                temp_file_path = temp_dir_path / source_path_obj.name
+                shutil.copy(source_path_obj, temp_file_path)
+                pbar.update(temp_file_path.stat().st_size)
+                upload_path = str(temp_file_path)
+
         return [token for token in [_upload_blob(upload_path, model_type)] if token]
```

### Comparing `kagglehub-0.2.2/src/kagglehub/handle.py` & `kagglehub-0.2.3/src/kagglehub/handle.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,17 +34,17 @@
         handle_str = f"{self.owner}/{self.model}/{self.framework}/{self.variation}"
         if self.is_versioned():
             return f"{handle_str}/{self.version}"
         return handle_str
 
     def to_url(self) -> str:
         if self.is_versioned():
-            return f"https://www.kaggle.com/models/{self.owner}/{self.model}/frameworks/{self.framework}/variations/{self.variation}/versions/{self.version}"
+            return f"https://www.kaggle.com/models/{self.owner}/{self.model}/{self.framework}/{self.variation}/{self.version}"
         else:
-            return f"https://www.kaggle.com/models/{self.owner}/{self.model}/frameworks/{self.framework}/variations/{self.variation}"
+            return f"https://www.kaggle.com/models/{self.owner}/{self.model}/{self.framework}/{self.variation}"
 
 
 @dataclass
 class DatasetHandle:
     owner: str
     dataset_name: str
     version: Optional[int] = None
```

### Comparing `kagglehub-0.2.2/src/kagglehub/http_resolver.py` & `kagglehub-0.2.3/src/kagglehub/http_resolver.py`

 * *Files identical despite different names*

### Comparing `kagglehub-0.2.2/src/kagglehub/integrity.py` & `kagglehub-0.2.3/src/kagglehub/integrity.py`

 * *Files identical despite different names*

### Comparing `kagglehub-0.2.2/src/kagglehub/kaggle_cache_resolver.py` & `kagglehub-0.2.3/src/kagglehub/kaggle_cache_resolver.py`

 * *Files identical despite different names*

### Comparing `kagglehub-0.2.2/src/kagglehub/logging.py` & `kagglehub-0.2.3/src/kagglehub/logging.py`

 * *Files identical despite different names*

### Comparing `kagglehub-0.2.2/src/kagglehub/models.py` & `kagglehub-0.2.3/src/kagglehub/models.py`

 * *Files identical despite different names*

### Comparing `kagglehub-0.2.2/src/kagglehub/models_helpers.py` & `kagglehub-0.2.3/src/kagglehub/models_helpers.py`

 * *Files identical despite different names*

### Comparing `kagglehub-0.2.2/src/kagglehub/registry.py` & `kagglehub-0.2.3/src/kagglehub/registry.py`

 * *Files identical despite different names*

### Comparing `kagglehub-0.2.2/src/kagglehub/resolver.py` & `kagglehub-0.2.3/src/kagglehub/resolver.py`

 * *Files identical despite different names*

### Comparing `kagglehub-0.2.2/tests/test_auth.py` & `kagglehub-0.2.3/tests/test_auth.py`

 * *Files identical despite different names*

### Comparing `kagglehub-0.2.2/tests/test_cache.py` & `kagglehub-0.2.3/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `kagglehub-0.2.2/tests/test_colab_cache_model_download.py` & `kagglehub-0.2.3/tests/test_colab_cache_model_download.py`

 * *Files identical despite different names*

### Comparing `kagglehub-0.2.2/tests/test_config.py` & `kagglehub-0.2.3/tests/test_config.py`

 * *Files identical despite different names*

### Comparing `kagglehub-0.2.2/tests/test_handle.py` & `kagglehub-0.2.3/tests/test_handle.py`

 * *Files identical despite different names*

### Comparing `kagglehub-0.2.2/tests/test_http_model_download.py` & `kagglehub-0.2.3/tests/test_http_model_download.py`

 * *Files identical despite different names*

### Comparing `kagglehub-0.2.2/tests/test_integrity.py` & `kagglehub-0.2.3/tests/test_integrity.py`

 * *Files identical despite different names*

### Comparing `kagglehub-0.2.2/tests/test_kaggle_api_client.py` & `kagglehub-0.2.3/tests/test_kaggle_api_client.py`

 * *Files identical despite different names*

### Comparing `kagglehub-0.2.2/tests/test_kaggle_cache_model_download.py` & `kagglehub-0.2.3/tests/test_kaggle_cache_model_download.py`

 * *Files identical despite different names*

### Comparing `kagglehub-0.2.2/tests/test_model_upload.py` & `kagglehub-0.2.3/tests/test_model_upload.py`

 * *Files identical despite different names*

### Comparing `kagglehub-0.2.2/tests/test_registry.py` & `kagglehub-0.2.3/tests/test_registry.py`

 * *Files identical despite different names*

### Comparing `kagglehub-0.2.2/tests/test_utils.py` & `kagglehub-0.2.3/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `kagglehub-0.2.2/tests/utils.py` & `kagglehub-0.2.3/tests/utils.py`

 * *Files identical despite different names*

### Comparing `kagglehub-0.2.2/tools/cicd/cloudbuild.yaml` & `kagglehub-0.2.3/tools/cicd/cloudbuild.yaml`

 * *Files identical despite different names*

### Comparing `kagglehub-0.2.2/tools/cicd/integration-tests.yaml` & `kagglehub-0.2.3/tools/cicd/integration-tests.yaml`

 * *Files identical despite different names*

### Comparing `kagglehub-0.2.2/tools/release/cloudbuild.yaml` & `kagglehub-0.2.3/tools/release/cloudbuild.yaml`

 * *Files identical despite different names*

### Comparing `kagglehub-0.2.2/.gitignore` & `kagglehub-0.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `kagglehub-0.2.2/LICENSE` & `kagglehub-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `kagglehub-0.2.2/README.md` & `kagglehub-0.2.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,15 @@
 
 Alternatively, you can set the `KAGGLE_CONFIG_DIR` environment variable to change this location to `$KAGGLE_CONFIG_DIR/kaggle.json`.
 
 Note for Windows users: The default directory is `%HOMEPATH%/kaggle.json`.
 
 ### Download Model
 
-The following examples download the `answer-equivalence-bem` variation of this Kaggle model: https://www.kaggle.com/models/google/bert/frameworks/tensorFlow2/variations/answer-equivalence-bem
+The following examples download the `answer-equivalence-bem` variation of this Kaggle model: https://www.kaggle.com/models/google/bert/tensorFlow2/answer-equivalence-bem
 
 ```python
 import kagglehub
 
 # Download the latest version.
 kagglehub.model_download('google/bert/tensorFlow2/answer-equivalence-bem')
 
@@ -70,15 +70,15 @@
 ### Upload Model
 Uploads a new variation (or a new variation's version if it already exists).
 
 ```python
 import kagglehub
 
 # For example, to upload a new variation to this model:
-# - https://www.kaggle.com/models/google/bert/frameworks/tensorFlow2/variations/answer-equivalence-bem
+# - https://www.kaggle.com/models/google/bert/tensorFlow2/answer-equivalence-bem
 # 
 # You would use the following handle: `google/bert/tensorFlow2/answer-equivalence-bem`
 handle = '<KAGGLE_USERNAME>/<MODEL>/<FRAMEWORK>/<VARIATION>'
 local_model_dir = 'path/to/local/model/dir'
 
 kagglehub.model_upload(handle, local_model_dir)
```

### Comparing `kagglehub-0.2.2/pyproject.toml` & `kagglehub-0.2.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `kagglehub-0.2.2/PKG-INFO` & `kagglehub-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: kagglehub
-Version: 0.2.2
+Version: 0.2.3
 Summary: Access Kaggle resources anywhere
 Project-URL: Homepage, https://github.com/Kaggle/kagglehub
 Project-URL: Bug Tracker, https://github.com/Kaggle/kagglehub/issues
 Author-email: Kaggle <support@kaggle.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
@@ -263,15 +263,15 @@
 
 Alternatively, you can set the `KAGGLE_CONFIG_DIR` environment variable to change this location to `$KAGGLE_CONFIG_DIR/kaggle.json`.
 
 Note for Windows users: The default directory is `%HOMEPATH%/kaggle.json`.
 
 ### Download Model
 
-The following examples download the `answer-equivalence-bem` variation of this Kaggle model: https://www.kaggle.com/models/google/bert/frameworks/tensorFlow2/variations/answer-equivalence-bem
+The following examples download the `answer-equivalence-bem` variation of this Kaggle model: https://www.kaggle.com/models/google/bert/tensorFlow2/answer-equivalence-bem
 
 ```python
 import kagglehub
 
 # Download the latest version.
 kagglehub.model_download('google/bert/tensorFlow2/answer-equivalence-bem')
 
@@ -288,15 +288,15 @@
 ### Upload Model
 Uploads a new variation (or a new variation's version if it already exists).
 
 ```python
 import kagglehub
 
 # For example, to upload a new variation to this model:
-# - https://www.kaggle.com/models/google/bert/frameworks/tensorFlow2/variations/answer-equivalence-bem
+# - https://www.kaggle.com/models/google/bert/tensorFlow2/answer-equivalence-bem
 # 
 # You would use the following handle: `google/bert/tensorFlow2/answer-equivalence-bem`
 handle = '<KAGGLE_USERNAME>/<MODEL>/<FRAMEWORK>/<VARIATION>'
 local_model_dir = 'path/to/local/model/dir'
 
 kagglehub.model_upload(handle, local_model_dir)
```

