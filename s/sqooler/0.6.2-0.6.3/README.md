# Comparing `tmp/sqooler-0.6.2.tar.gz` & `tmp/sqooler-0.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqooler-0.6.2.tar", max compression
+gzip compressed data, was "sqooler-0.6.3.tar", max compression
```

## Comparing `sqooler-0.6.2.tar` & `sqooler-0.6.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1211 2024-03-18 17:38:21.370303 sqooler-0.6.2/LICENSE
--rw-r--r--   0        0        0     3928 2024-03-21 16:38:07.651464 sqooler-0.6.2/README.md
--rw-r--r--   0        0        0     1057 2024-04-14 17:29:05.618373 sqooler-0.6.2/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-18 17:38:21.374962 sqooler-0.6.2/src/sqooler/__init__.py
--rw-r--r--   0        0        0    12140 2024-04-03 16:25:44.628605 sqooler-0.6.2/src/sqooler/schemes.py
--rw-r--r--   0        0        0     8775 2024-03-29 14:08:39.014572 sqooler-0.6.2/src/sqooler/security.py
--rw-r--r--   0        0        0    27199 2024-04-14 14:39:47.120255 sqooler-0.6.2/src/sqooler/spoolers.py
--rw-r--r--   0        0        0        0 2024-03-21 16:38:07.659018 sqooler-0.6.2/src/sqooler/storage_providers/__init__.py
--rw-r--r--   0        0        0    21846 2024-04-07 17:16:12.295483 sqooler-0.6.2/src/sqooler/storage_providers/base.py
--rw-r--r--   0        0        0    26455 2024-04-05 16:52:36.004035 sqooler-0.6.2/src/sqooler/storage_providers/dropbox.py
--rw-r--r--   0        0        0    22693 2024-04-14 14:40:25.633341 sqooler-0.6.2/src/sqooler/storage_providers/local.py
--rw-r--r--   0        0        0    27299 2024-04-07 17:16:05.334587 sqooler-0.6.2/src/sqooler/storage_providers/mongodb.py
--rw-r--r--   0        0        0     6472 2024-04-14 14:40:46.943889 sqooler-0.6.2/src/sqooler/utils.py
--rw-r--r--   0        0        0     4927 1970-01-01 00:00:00.000000 sqooler-0.6.2/PKG-INFO
+-rw-r--r--   0        0        0     1211 2024-03-18 17:38:21.370303 sqooler-0.6.3/LICENSE
+-rw-r--r--   0        0        0     3928 2024-03-21 16:38:07.651464 sqooler-0.6.3/README.md
+-rw-r--r--   0        0        0     1057 2024-04-16 20:23:10.386599 sqooler-0.6.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-03-18 17:38:21.374962 sqooler-0.6.3/src/sqooler/__init__.py
+-rw-r--r--   0        0        0    12140 2024-04-03 16:25:44.628605 sqooler-0.6.3/src/sqooler/schemes.py
+-rw-r--r--   0        0        0     8775 2024-03-29 14:08:39.014572 sqooler-0.6.3/src/sqooler/security.py
+-rw-r--r--   0        0        0    27245 2024-04-16 20:23:01.954085 sqooler-0.6.3/src/sqooler/spoolers.py
+-rw-r--r--   0        0        0        0 2024-03-21 16:38:07.659018 sqooler-0.6.3/src/sqooler/storage_providers/__init__.py
+-rw-r--r--   0        0        0    22085 2024-04-16 20:11:29.601741 sqooler-0.6.3/src/sqooler/storage_providers/base.py
+-rw-r--r--   0        0        0    25716 2024-04-16 20:11:29.602180 sqooler-0.6.3/src/sqooler/storage_providers/dropbox.py
+-rw-r--r--   0        0        0    21513 2024-04-16 20:11:29.602485 sqooler-0.6.3/src/sqooler/storage_providers/local.py
+-rw-r--r--   0        0        0    26090 2024-04-16 20:11:29.602903 sqooler-0.6.3/src/sqooler/storage_providers/mongodb.py
+-rw-r--r--   0        0        0     6472 2024-04-14 14:40:46.943889 sqooler-0.6.3/src/sqooler/utils.py
+-rw-r--r--   0        0        0     4927 1970-01-01 00:00:00.000000 sqooler-0.6.3/PKG-INFO
```

### Comparing `sqooler-0.6.2/LICENSE` & `sqooler-0.6.3/LICENSE`

 * *Files identical despite different names*

### Comparing `sqooler-0.6.2/README.md` & `sqooler-0.6.3/README.md`

 * *Files identical despite different names*

### Comparing `sqooler-0.6.2/pyproject.toml` & `sqooler-0.6.3/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "sqooler"
-version = "0.6.2"
+version = "0.6.3"
 description = "Code that enables validated cloud access to quantum hardware (simulators)"
 authors = ["fretchen <fred.jendrzejewski@gmail.com>"]
 repository = "https://github.com/Alqor-UG/sqooler"
 documentation = "https://alqor-ug.github.io/sqooler"
 license = "Unlicense"
 readme = "README.md"
 packages = [{include = "sqooler", from = "src"}]
```

### Comparing `sqooler-0.6.2/src/sqooler/schemes.py` & `sqooler-0.6.3/src/sqooler/schemes.py`

 * *Files identical despite different names*

### Comparing `sqooler-0.6.2/src/sqooler/security.py` & `sqooler-0.6.3/src/sqooler/security.py`

 * *Files identical despite different names*

### Comparing `sqooler-0.6.2/src/sqooler/spoolers.py` & `sqooler-0.6.3/src/sqooler/spoolers.py`

 * *Files 1% similar despite different names*

```diff
@@ -457,14 +457,15 @@
         n_max_shots: int = 1000,
         version: str = "0.0.1",
         cold_atom_type: ColdAtomStr = "spin",
         n_max_experiments: int = 15,
         wire_order: WireOrderStr = "interleaved",
         num_species: int = 1,
         operational: bool = True,
+        sign: bool = False,
     ):
         """
         The constructor of the class. The  arguments are the same as for the Spooler
         class with two additions.
 
 
         """
@@ -476,14 +477,15 @@
             n_max_shots,
             version,
             cold_atom_type,
             n_max_experiments,
             wire_order,
             num_species,
             operational,
+            sign,
         )
         self.remote_client = remote_client
         self.labscript_params = labscript_params
         self.run = run
 
     def add_job(
         self, json_dict: dict[str, dict], job_id: str
```

### Comparing `sqooler-0.6.2/src/sqooler/storage_providers/base.py` & `sqooler-0.6.3/src/sqooler/storage_providers/base.py`

 * *Files 0% similar despite different names*

```diff
@@ -116,27 +116,32 @@
         Raises:
             FileNotFoundError: If the backend does not exist
         """
         backend_config_info = self.get_config(display_name)
         qiskit_backend_dict = self.backend_dict_to_qiskit(backend_config_info)
         return qiskit_backend_dict
 
-    @abstractmethod
     def get_backend_status(
         self, display_name: DisplayNameStr
     ) -> BackendStatusSchemaOut:
         """
         Get the status of the backend. This follows the qiskit logic.
 
         Args:
             display_name: The name of the backend
 
         Returns:
             The status dict of the backend
+
+        Raises:
+            FileNotFoundError: If the backend does not exist
         """
+        backend_config_info = self.get_config(display_name)
+        qiskit_backend_dict = self.backend_dict_to_qiskit_status(backend_config_info)
+        return qiskit_backend_dict
 
     @abstractmethod
     def upload_job(
         self, job_dict: dict, display_name: DisplayNameStr, username: str
     ) -> str:
         """
         Upload the job to the storage provider.
```

### Comparing `sqooler-0.6.2/src/sqooler/storage_providers/dropbox.py` & `sqooler-0.6.3/src/sqooler/storage_providers/dropbox.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,14 @@
 from dropbox.files import WriteMode
 from dropbox.exceptions import ApiError, AuthError
 
 from ..schemes import (
     ResultDict,
     StatusMsgDict,
     DropboxLoginInformation,
-    BackendStatusSchemaOut,
     BackendConfigSchemaIn,
     NextJobSchema,
     DisplayNameStr,
 )
 from ..security import JWK, sign_payload
 from .base import StorageProvider, validate_active, datetime_handler
 
@@ -501,34 +500,14 @@
         backend_json_path = f"Backend_files/Config/{display_name}"
         backend_config_dict = self.get_file_content(
             storage_path=backend_json_path, job_id="config"
         )
         typed_config = self._adapt_get_config(backend_config_dict)
         return typed_config
 
-    def get_backend_status(
-        self, display_name: DisplayNameStr
-    ) -> BackendStatusSchemaOut:
-        """
-        Get the status of the backend. This follows the qiskit logic.
-
-        Args:
-            display_name: The name of the backend
-
-        Returns:
-            The status dict of the backend
-        """
-        backend_json_path = f"Backend_files/Config/{display_name}"
-        backend_config_dict = self.get_file_content(
-            storage_path=backend_json_path, job_id="config"
-        )
-        backend_config_info = BackendConfigSchemaIn(**backend_config_dict)
-        qiskit_backend_dict = self.backend_dict_to_qiskit_status(backend_config_info)
-        return qiskit_backend_dict
-
     def upload_job(
         self, job_dict: dict, display_name: DisplayNameStr, username: str
     ) -> str:
         """
         This function uploads a job to the backend and creates the job_id.
 
         Args:
```

### Comparing `sqooler-0.6.2/src/sqooler/storage_providers/local.py` & `sqooler-0.6.3/src/sqooler/storage_providers/local.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 import shutil
 import os
 
 from ..schemes import (
     ResultDict,
     StatusMsgDict,
     LocalLoginInformation,
-    BackendStatusSchemaOut,
     BackendConfigSchemaIn,
     NextJobSchema,
     DisplayNameStr,
 )
 
 from .base import StorageProvider, validate_active, datetime_handler
 from ..security import JWK, sign_payload
@@ -194,46 +193,14 @@
         # Filter out only the JSON files
         json_files = [item for item in all_items if item.endswith(".json")]
 
         # Get the backend names
         backend_names = [os.path.splitext(file_name)[0] for file_name in json_files]
         return backend_names
 
-    def get_backend_status(
-        self, display_name: DisplayNameStr
-    ) -> BackendStatusSchemaOut:
-        """
-        Get the status of the backend. This follows the qiskit logic.
-
-        Args:
-            display_name: The name of the backend
-
-        Returns:
-            The status dict of the backend
-
-        Raises:
-            FileNotFoundError: If the backend does not exist
-        """
-        # path of the configs
-        file_name = display_name + ".json"
-        config_path = self.base_path + "/backends/configs"
-        full_json_path = os.path.join(config_path, file_name)
-        secure_path = os.path.normpath(full_json_path)
-        with open(secure_path, "r", encoding="utf-8") as json_file:
-            backend_config_dict = json.load(json_file)
-
-        if not backend_config_dict:
-            raise FileNotFoundError(
-                f"The backend {display_name} does not exist for the given storageprovider."
-            )
-
-        backend_config_info = BackendConfigSchemaIn(**backend_config_dict)
-        qiskit_backend_dict = self.backend_dict_to_qiskit_status(backend_config_info)
-        return qiskit_backend_dict
-
     def upload_job(
         self, job_dict: dict, display_name: DisplayNameStr, username: str
     ) -> str:
         """
         Upload the job to the storage provider.
 
         Args:
```

### Comparing `sqooler-0.6.2/src/sqooler/storage_providers/mongodb.py` & `sqooler-0.6.3/src/sqooler/storage_providers/mongodb.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 from bson.errors import InvalidId
 from bson.codec_options import CodecOptions
 
 from ..schemes import (
     ResultDict,
     StatusMsgDict,
     MongodbLoginInformation,
-    BackendStatusSchemaOut,
     BackendConfigSchemaIn,
     NextJobSchema,
     DisplayNameStr,
 )
 
 from .base import StorageProvider, validate_active
 from ..security import JWK, sign_payload
@@ -244,47 +243,14 @@
             expected_keys_for_jws = {"header", "payload", "signature"}
             if set(config_dict.keys()) == expected_keys_for_jws:
                 backend_names.append(config_dict["payload"]["display_name"])
             else:
                 backend_names.append(config_dict["display_name"])
         return backend_names
 
-    def get_backend_status(
-        self, display_name: DisplayNameStr
-    ) -> BackendStatusSchemaOut:
-        """
-        Get the status of the backend. This follows the qiskit logic.
-
-        Args:
-            display_name: The name of the backend
-
-        Returns:
-            The status dict of the backend
-
-        Raises:
-            FileNotFoundError: If the backend does not exist
-        """
-        # get the database on which we work
-        database = self.client["backends"]
-        config_collection = database["configs"]
-
-        # create the filter for the document with display_name that is equal to display_name
-        document_to_find = {"display_name": display_name}
-        backend_config_dict = config_collection.find_one(document_to_find)
-
-        if not backend_config_dict:
-            raise FileNotFoundError(
-                f"The backend {display_name} does not exist for the given storageprovider."
-            )
-
-        backend_config_dict.pop("_id")
-        backend_config_info = BackendConfigSchemaIn(**backend_config_dict)
-        qiskit_backend_dict = self.backend_dict_to_qiskit_status(backend_config_info)
-        return qiskit_backend_dict
-
     def upload_config(
         self,
         config_dict: BackendConfigSchemaIn,
         display_name: DisplayNameStr,
         private_jwk: Optional[JWK] = None,
     ) -> None:
         """
```

### Comparing `sqooler-0.6.2/src/sqooler/utils.py` & `sqooler-0.6.3/src/sqooler/utils.py`

 * *Files identical despite different names*

### Comparing `sqooler-0.6.2/PKG-INFO` & `sqooler-0.6.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqooler
-Version: 0.6.2
+Version: 0.6.3
 Summary: Code that enables validated cloud access to quantum hardware (simulators)
 Home-page: https://github.com/Alqor-UG/sqooler
 License: Unlicense
 Keywords: pydantic,quantum-hardware,sdk-python
 Author: fretchen
 Author-email: fred.jendrzejewski@gmail.com
 Requires-Python: >=3.10,<4.0
```

