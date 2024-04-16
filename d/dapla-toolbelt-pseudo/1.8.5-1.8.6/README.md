# Comparing `tmp/dapla_toolbelt_pseudo-1.8.5.tar.gz` & `tmp/dapla_toolbelt_pseudo-1.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dapla_toolbelt_pseudo-1.8.5.tar", max compression
+gzip compressed data, was "dapla_toolbelt_pseudo-1.8.6.tar", max compression
```

## Comparing `dapla_toolbelt_pseudo-1.8.5.tar` & `dapla_toolbelt_pseudo-1.8.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1073 2024-04-15 06:30:14.054759 dapla_toolbelt_pseudo-1.8.5/LICENSE
--rw-r--r--   0        0        0    17053 2024-04-15 06:30:14.054759 dapla_toolbelt_pseudo-1.8.5/README.md
--rw-r--r--   0        0        0     4728 2024-04-15 06:30:27.778695 dapla_toolbelt_pseudo-1.8.5/pyproject.toml
--rw-r--r--   0        0        0     1493 2024-04-15 06:30:14.058759 dapla_toolbelt_pseudo-1.8.5/src/dapla_pseudo/__init__.py
--rw-r--r--   0        0        0     1763 2024-04-15 06:30:14.058759 dapla_toolbelt_pseudo-1.8.5/src/dapla_pseudo/constants.py
--rw-r--r--   0        0        0      994 2024-04-15 06:30:14.058759 dapla_toolbelt_pseudo-1.8.5/src/dapla_pseudo/exceptions.py
--rw-r--r--   0        0        0      847 2024-04-15 06:30:14.058759 dapla_toolbelt_pseudo-1.8.5/src/dapla_pseudo/models.py
--rw-r--r--   0        0        0        0 2024-04-15 06:30:14.058759 dapla_toolbelt_pseudo-1.8.5/src/dapla_pseudo/py.typed
--rw-r--r--   0        0        0      828 2024-04-15 06:30:14.058759 dapla_toolbelt_pseudo-1.8.5/src/dapla_pseudo/types.py
--rw-r--r--   0        0        0     2115 2024-04-15 06:30:14.058759 dapla_toolbelt_pseudo-1.8.5/src/dapla_pseudo/utils.py
--rw-r--r--   0        0        0      543 2024-04-15 06:30:14.058759 dapla_toolbelt_pseudo-1.8.5/src/dapla_pseudo/v1/__init__.py
--rw-r--r--   0        0        0    12531 2024-04-15 06:30:14.058759 dapla_toolbelt_pseudo-1.8.5/src/dapla_pseudo/v1/api_models.py
--rw-r--r--   0        0        0     2974 2024-04-15 06:30:14.058759 dapla_toolbelt_pseudo-1.8.5/src/dapla_pseudo/v1/baseclass.py
--rw-r--r--   0        0        0     6118 2024-04-15 06:30:14.058759 dapla_toolbelt_pseudo-1.8.5/src/dapla_pseudo/v1/client.py
--rw-r--r--   0        0        0    15341 2024-04-15 06:30:14.058759 dapla_toolbelt_pseudo-1.8.5/src/dapla_pseudo/v1/depseudo.py
--rw-r--r--   0        0        0    15621 2024-04-15 06:30:14.058759 dapla_toolbelt_pseudo-1.8.5/src/dapla_pseudo/v1/pseudo.py
--rw-r--r--   0        0        0     9346 2024-04-15 06:30:14.058759 dapla_toolbelt_pseudo-1.8.5/src/dapla_pseudo/v1/pseudo_commons.py
--rw-r--r--   0        0        0    19278 2024-04-15 06:30:14.058759 dapla_toolbelt_pseudo-1.8.5/src/dapla_pseudo/v1/repseudo.py
--rw-r--r--   0        0        0     8347 2024-04-15 06:30:14.058759 dapla_toolbelt_pseudo-1.8.5/src/dapla_pseudo/v1/result.py
--rw-r--r--   0        0        0     4188 2024-04-15 06:30:14.058759 dapla_toolbelt_pseudo-1.8.5/src/dapla_pseudo/v1/supported_file_format.py
--rw-r--r--   0        0        0     5611 2024-04-15 06:30:14.058759 dapla_toolbelt_pseudo-1.8.5/src/dapla_pseudo/v1/validation.py
--rw-r--r--   0        0        0    18503 1970-01-01 00:00:00.000000 dapla_toolbelt_pseudo-1.8.5/PKG-INFO
+-rw-r--r--   0        0        0     1073 2024-04-16 13:36:34.903602 dapla_toolbelt_pseudo-1.8.6/LICENSE
+-rw-r--r--   0        0        0    18202 2024-04-16 13:36:34.903602 dapla_toolbelt_pseudo-1.8.6/README.md
+-rw-r--r--   0        0        0     4728 2024-04-16 13:36:49.947715 dapla_toolbelt_pseudo-1.8.6/pyproject.toml
+-rw-r--r--   0        0        0     1493 2024-04-16 13:36:34.903602 dapla_toolbelt_pseudo-1.8.6/src/dapla_pseudo/__init__.py
+-rw-r--r--   0        0        0     1763 2024-04-16 13:36:34.903602 dapla_toolbelt_pseudo-1.8.6/src/dapla_pseudo/constants.py
+-rw-r--r--   0        0        0      994 2024-04-16 13:36:34.903602 dapla_toolbelt_pseudo-1.8.6/src/dapla_pseudo/exceptions.py
+-rw-r--r--   0        0        0      847 2024-04-16 13:36:34.903602 dapla_toolbelt_pseudo-1.8.6/src/dapla_pseudo/models.py
+-rw-r--r--   0        0        0        0 2024-04-16 13:36:34.903602 dapla_toolbelt_pseudo-1.8.6/src/dapla_pseudo/py.typed
+-rw-r--r--   0        0        0      853 2024-04-16 13:36:34.903602 dapla_toolbelt_pseudo-1.8.6/src/dapla_pseudo/types.py
+-rw-r--r--   0        0        0     2115 2024-04-16 13:36:34.903602 dapla_toolbelt_pseudo-1.8.6/src/dapla_pseudo/utils.py
+-rw-r--r--   0        0        0      543 2024-04-16 13:36:34.903602 dapla_toolbelt_pseudo-1.8.6/src/dapla_pseudo/v1/__init__.py
+-rw-r--r--   0        0        0    12559 2024-04-16 13:36:34.903602 dapla_toolbelt_pseudo-1.8.6/src/dapla_pseudo/v1/api_models.py
+-rw-r--r--   0        0        0     2974 2024-04-16 13:36:34.903602 dapla_toolbelt_pseudo-1.8.6/src/dapla_pseudo/v1/baseclass.py
+-rw-r--r--   0        0        0     6265 2024-04-16 13:36:34.903602 dapla_toolbelt_pseudo-1.8.6/src/dapla_pseudo/v1/client.py
+-rw-r--r--   0        0        0    15341 2024-04-16 13:36:34.903602 dapla_toolbelt_pseudo-1.8.6/src/dapla_pseudo/v1/depseudo.py
+-rw-r--r--   0        0        0    15660 2024-04-16 13:36:34.903602 dapla_toolbelt_pseudo-1.8.6/src/dapla_pseudo/v1/pseudo.py
+-rw-r--r--   0        0        0     9116 2024-04-16 13:36:34.903602 dapla_toolbelt_pseudo-1.8.6/src/dapla_pseudo/v1/pseudo_commons.py
+-rw-r--r--   0        0        0    19278 2024-04-16 13:36:34.903602 dapla_toolbelt_pseudo-1.8.6/src/dapla_pseudo/v1/repseudo.py
+-rw-r--r--   0        0        0     8347 2024-04-16 13:36:34.903602 dapla_toolbelt_pseudo-1.8.6/src/dapla_pseudo/v1/result.py
+-rw-r--r--   0        0        0     4451 2024-04-16 13:36:34.903602 dapla_toolbelt_pseudo-1.8.6/src/dapla_pseudo/v1/supported_file_format.py
+-rw-r--r--   0        0        0     5611 2024-04-16 13:36:34.903602 dapla_toolbelt_pseudo-1.8.6/src/dapla_pseudo/v1/validation.py
+-rw-r--r--   0        0        0    19652 1970-01-01 00:00:00.000000 dapla_toolbelt_pseudo-1.8.6/PKG-INFO
```

### Comparing `dapla_toolbelt_pseudo-1.8.5/LICENSE` & `dapla_toolbelt_pseudo-1.8.6/LICENSE`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-1.8.5/README.md` & `dapla_toolbelt_pseudo-1.8.6/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -200,15 +200,15 @@
     .to_polars(**options)                  # Get the result as a polars dataframe
 )
 ```
 
 #### Pseudonymize using custom keys/keysets
 
 ```python
-from dapla_pseudo import pseudonymize
+from dapla_pseudo import Pseudonymize, PseudoKeyset
 
 # Pseudonymize fields in a local file using the default key:
 df = (
     Pseudonymize.from_polars(df)                            # Specify what dataframe to use
     .on_fields("fornavn")                                   # Select the field to pseudonymize
     .with_default_encryption()                              # Select the pseudonymization algorithm to apply
     .run()                                         # Apply pseudonymization to the selected field
@@ -246,14 +246,57 @@
     Pseudonymize.from_polars(df)
     .on_fields("fornavn")
     .with_default_encryption(custom_key="1234567890") # Note that the custom key has to be the same as "primaryKeyId" in the custom keyset
     .run(custom_keyset=custom_keyset)
     .to_polars()
 )
 ```
+#### Pseudonymize using custom rules
+
+Instead of declaring the pseudonymization rules via the Pseudonymize functions, one can define the rules manually.
+This can be done via the `PseudoRule` class like this:
+
+```python
+from dapla_pseudo import Pseudonymize, PseudoRule
+
+rule_json = {
+    'name': 'my-fule',
+     'pattern': '**/identifiers/*',
+     'func': 'redact(placeholder=#)' # This is a shorthand representation of the redact function
+}
+
+rule = PseudoRule.from_json(rule_json)
+
+df = (
+    Pseudonymize.from_polars(df)
+    .add_rules(rule) # Add one or more pseudonymization rules
+    .run()
+    .to_polars()
+)
+```
+
+Pseudonymization rules can also be read from file. This is especially handy when there are several rules, or if you
+prefer to store and maintain pseudonymization rules externally. For example:
+
+```python
+from dapla_pseudo import PseudoRule
+import json
+
+with open("pseudo-rules.json", 'r') as rules_file:
+    rules_json = json.load(rules_file)
+
+pseudo_rules = [PseudoRule.from_json(rule) for rule in rules_json]
+
+df = (
+    Pseudonymize.from_polars(df)
+    .add_rules(pseudo_rules)
+    .run()
+    .to_polars()
+)
+```
 
 ### Depseudonymize
 
 The "Depseudonymize" functions are almost exactly the same as when pseudonymizing.
 User can map from Stable ID *back to* FNR.
 
 ```python
```

### Comparing `dapla_toolbelt_pseudo-1.8.5/pyproject.toml` & `dapla_toolbelt_pseudo-1.8.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dapla-toolbelt-pseudo"
-version = "1.8.5"
+version = "1.8.6"
 description = "Pseudonymization extensions for Dapla"
 authors = ["Dapla Developers <dapla-platform-developers@ssb.no>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/statisticsnorway/dapla-toolbelt-pseudo"
 repository = "https://github.com/statisticsnorway/dapla-toolbelt-pseudo"
 documentation = "https://statisticsnorway.github.io/dapla-toolbelt-pseudo"
```

### Comparing `dapla_toolbelt_pseudo-1.8.5/src/dapla_pseudo/__init__.py` & `dapla_toolbelt_pseudo-1.8.6/src/dapla_pseudo/__init__.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-1.8.5/src/dapla_pseudo/constants.py` & `dapla_toolbelt_pseudo-1.8.6/src/dapla_pseudo/constants.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-1.8.5/src/dapla_pseudo/exceptions.py` & `dapla_toolbelt_pseudo-1.8.6/src/dapla_pseudo/exceptions.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-1.8.5/src/dapla_pseudo/models.py` & `dapla_toolbelt_pseudo-1.8.6/src/dapla_pseudo/models.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-1.8.5/src/dapla_pseudo/types.py` & `dapla_toolbelt_pseudo-1.8.6/src/dapla_pseudo/types.py`

 * *Files 12% similar despite different names*

```diff
@@ -8,15 +8,18 @@
 import gcsfs
 import pandas as pd
 
 from dapla_pseudo.v1.api_models import Field
 
 FieldDecl: TypeAlias = str | dict[str, str] | Field
 BinaryFileDecl: TypeAlias = (
-    io.BufferedReader | fsspec.spec.AbstractBufferedFile | gcsfs.core.GCSFile
+    io.BufferedReader
+    | fsspec.spec.AbstractBufferedFile
+    | gcsfs.core.GCSFile
+    | io.BytesIO
 )
 
 DatasetDecl: TypeAlias = pd.DataFrame | BinaryFileDecl | str | Path
 FileLikeDatasetDecl: TypeAlias = BinaryFileDecl | str | Path
 FileSpecDecl: TypeAlias = tuple[str | None, BinaryFileDecl | str, str]
 # FileSpecDecl is derived from the "files" argument in multi-part requests from the "Requests"-library
 # The tuple semantically means: ('filename', fileobj, 'content_type')
```

### Comparing `dapla_toolbelt_pseudo-1.8.5/src/dapla_pseudo/utils.py` & `dapla_toolbelt_pseudo-1.8.6/src/dapla_pseudo/utils.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-1.8.5/src/dapla_pseudo/v1/__init__.py` & `dapla_toolbelt_pseudo-1.8.6/src/dapla_pseudo/v1/__init__.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-1.8.5/src/dapla_pseudo/v1/api_models.py` & `dapla_toolbelt_pseudo-1.8.6/src/dapla_pseudo/v1/api_models.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 class Mimetypes(str, Enum):
     """Mimetypes is an enum of supported mimetypes, for use in HTTP requests.
 
     As a proxy, this also defines the supported input file formats when reading from a file.
     """
 
     JSON = "application/json"
+    ZIP = "application/zip"
     CSV = "text/csv"
 
 
 class Field(APIModel):
     """Field represents a targeted piece of data within a dataset or record.
 
     Parameters:
```

### Comparing `dapla_toolbelt_pseudo-1.8.5/src/dapla_pseudo/v1/baseclass.py` & `dapla_toolbelt_pseudo-1.8.6/src/dapla_pseudo/v1/baseclass.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-1.8.5/src/dapla_pseudo/v1/client.py` & `dapla_toolbelt_pseudo-1.8.6/src/dapla_pseudo/v1/client.py`

 * *Files 16% similar despite different names*

```diff
@@ -158,14 +158,17 @@
     except AttributeError:
         # Fallback to default name
         name = "unknown"
 
     if not name.endswith(".json") and input_content_type is Mimetypes.JSON:
         name = f"{name}.json"  # Pseudo service expects a file extension
 
+    if not name.endswith(".zip") and input_content_type is Mimetypes.ZIP:
+        name = f"{name}.zip"  # Pseudo service expects a file extension
+
     if "/" in name:
         name = name.split("/")[-1]  # Pseudo service expects a file name, not a path
 
     return name
 
 
 def _client() -> PseudoClient:
```

### Comparing `dapla_toolbelt_pseudo-1.8.5/src/dapla_pseudo/v1/depseudo.py` & `dapla_toolbelt_pseudo-1.8.6/src/dapla_pseudo/v1/depseudo.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-1.8.5/src/dapla_pseudo/v1/pseudo.py` & `dapla_toolbelt_pseudo-1.8.6/src/dapla_pseudo/v1/pseudo.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,15 +24,14 @@
 from dapla_pseudo.v1.api_models import PseudoFieldRequest
 from dapla_pseudo.v1.api_models import PseudoFunction
 from dapla_pseudo.v1.api_models import PseudoKeyset
 from dapla_pseudo.v1.api_models import PseudonymizeFileRequest
 from dapla_pseudo.v1.api_models import PseudoRule
 from dapla_pseudo.v1.client import PseudoClient
 from dapla_pseudo.v1.pseudo_commons import File
-from dapla_pseudo.v1.pseudo_commons import HierarchicalDataFrame
 from dapla_pseudo.v1.pseudo_commons import PseudoFieldResponse
 from dapla_pseudo.v1.pseudo_commons import PseudoFileResponse
 from dapla_pseudo.v1.pseudo_commons import RawPseudoMetadata
 from dapla_pseudo.v1.pseudo_commons import get_file_data_from_dataset
 from dapla_pseudo.v1.pseudo_commons import pseudo_operation_dataset
 from dapla_pseudo.v1.pseudo_commons import pseudonymize_operation_field
 from dapla_pseudo.v1.result import Result
@@ -40,31 +39,35 @@
 
 class Pseudonymize:
     """Starting point for pseudonymization of datasets.
 
     This class should not be instantiated, only the static methods should be used.
     """
 
-    dataset: File | pl.DataFrame | HierarchicalDataFrame
+    dataset: File | pl.DataFrame
 
     @staticmethod
     def from_pandas(dataframe: pd.DataFrame) -> "Pseudonymize._Pseudonymizer":
         """Initialize a pseudonymization request from a pandas DataFrame."""
         dataset: pl.DataFrame = pl.from_pandas(dataframe)
         if pl.Struct in dataset.dtypes:
-            Pseudonymize.dataset = HierarchicalDataFrame(dataset)
+            # Hierachial dataset must be processed as a file
+            file_handle, content_type = get_file_data_from_dataset(dataframe)
+            Pseudonymize.dataset = File(file_handle, content_type)
         else:
             Pseudonymize.dataset = dataset
         return Pseudonymize._Pseudonymizer()
 
     @staticmethod
     def from_polars(dataframe: pl.DataFrame) -> "Pseudonymize._Pseudonymizer":
         """Initialize a pseudonymization request from a polars DataFrame."""
         if pl.Struct in dataframe.dtypes:
-            Pseudonymize.dataset = HierarchicalDataFrame(dataframe)
+            # Hierachial dataset must be processed as a file
+            file_handle, content_type = get_file_data_from_dataset(dataframe)
+            Pseudonymize.dataset = File(file_handle, content_type)
         else:
             Pseudonymize.dataset = dataframe
         return Pseudonymize._Pseudonymizer()
 
     @staticmethod
     def from_file(dataset: FileLikeDatasetDecl) -> "Pseudonymize._Pseudonymizer":
         """Initialize a pseudonymization request from a pandas dataframe read from file.
@@ -129,36 +132,34 @@
 
             Returns:
                 Result: The pseudonymized dataset and the associated metadata.
             """
             if Pseudonymize.dataset is None:
                 raise ValueError("No dataset has been provided.")
 
-            if self._rules == []:
+            if not self._rules:
                 raise ValueError(
                     "No fields have been provided. Use the 'on_fields' or the 'add_rules' method."
                 )
 
             if custom_keyset is not None:
                 self._pseudo_keyset = custom_keyset
 
             self._timeout = timeout
             match Pseudonymize.dataset:  # Differentiate between file and DataFrame
                 case File():
                     return self._pseudonymize_dataframe(Pseudonymize.dataset)
                 case pl.DataFrame():
                     return self._pseudonymize_field(Pseudonymize.dataset)
-                case HierarchicalDataFrame():
-                    return self._pseudonymize_dataframe(Pseudonymize.dataset.contents)
                 case _ as invalid_dataset:
                     raise ValueError(
                         f"Unsupported data type: {type(invalid_dataset)}. Should only be DataFrame or file-like type."
                     )
 
-        def _pseudonymize_dataframe(self, dataframe: File | pl.DataFrame) -> Result:
+        def _pseudonymize_dataframe(self, dataframe: File) -> Result:
             """Pseudonymize the entire dataframe."""
             pseudonymize_request = PseudonymizeFileRequest(
                 pseudo_config=PseudoConfig(
                     rules=self._rules,
                     keysets=KeyWrapper(self._pseudo_keyset).keyset_list(),
                 ),
                 target_content_type=Mimetypes.JSON,
```

### Comparing `dapla_toolbelt_pseudo-1.8.5/src/dapla_pseudo/v1/pseudo_commons.py` & `dapla_toolbelt_pseudo-1.8.6/src/dapla_pseudo/v1/pseudo_commons.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Common functions shared by all pseudo modules."""
 
 import io
 import json
 import os
 import typing as t
+import zipfile
 from dataclasses import dataclass
 from pathlib import Path
 
 import fsspec
 import polars as pl
 import requests
 from dapla import FileClient
@@ -38,15 +39,15 @@
     """'File' represents a file to be pseudonymized."""
 
     file_handle: BinaryFileDecl
     content_type: Mimetypes
 
 
 def get_file_data_from_dataset(
-    dataset: FileLikeDatasetDecl,
+    dataset: FileLikeDatasetDecl | pl.DataFrame,
 ) -> tuple[BinaryFileDecl, Mimetypes]:
     """Converts the given dataset to a file handle and content type.
 
     Args:
         dataset (FileLikeDatasetDecl): The provided dataset
 
     Raises:
@@ -74,14 +75,25 @@
                         "No Google Authentication found in environment"
                     ) from err
             else:
                 file_handle = open(dataset, "rb")
 
             file_handle.seek(0)
 
+        # Convert Polars dataframe to a zipped archive with json data
+        case pl.DataFrame() as df:
+            file_handle = io.BytesIO()
+            with zipfile.ZipFile(
+                file_handle, "a", compression=zipfile.ZIP_DEFLATED, compresslevel=9
+            ) as zip_file:
+                zip_file.writestr("data.json", json.dumps(df.to_dicts()))
+                zip_file.filename = "data.zip"
+            file_handle.seek(0)
+            return file_handle, Mimetypes.ZIP
+
         case io.BufferedReader():
             # File handle
             dataset.seek(0)
             file_handle = dataset
         case fsspec.spec.AbstractBufferedFile():
             # This is a file handle to a remote storage system such as GCS.
             # It provides random access for the underlying file-like data (without downloading the whole thing).
@@ -128,21 +140,14 @@
             f"The provided input format '{file_format}' is not supported from file."
         ) from None
 
     return content_type
 
 
 @dataclass
-class HierarchicalDataFrame:
-    """HierarchicalDataset holds a hierarchical dataframe."""
-
-    contents: pl.DataFrame
-
-
-@dataclass
 class RawPseudoMetadata:
     """RawPseudoMetadata holds the raw metadata obtained from Pseudo Service."""
 
     logs: list[str]
     metrics: list[str]
     datadoc: list[dict[str, t.Any]]
     field_name: str | None = None
@@ -164,67 +169,52 @@
     raw_metadata: RawPseudoMetadata
     content_type: Mimetypes
     file_name: str
     streamed: bool = True
 
 
 def pseudo_operation_dataset(
-    dataset_ref: File | pl.DataFrame,
+    dataset_ref: File,
     pseudo_operation_request: (
         PseudonymizeFileRequest | DepseudonymizeFileRequest | RepseudonymizeFileRequest
     ),
 ) -> PseudoFileResponse:
     """Calls pseudonymization API for an entire dataset (file handle or dataframe) and returns the pseudonymized data and metadata.
 
     Args:
-        dataset_ref: A file handle or a dataframe representing the data to be pseudonymized
+        dataset_ref: A file handle representing the data to be pseudonymized
         pseudo_operation_request: An object representing the data and how it should be pseudonymized
 
     Returns:
         PseudoFileResponse: An object representing the response from the Pseudo Service.
     """
     request_spec: FileSpecDecl = (
         None,
         pseudo_operation_request.to_json(),
         str(Mimetypes.JSON),
     )
     file_name: str
     data_spec: FileSpecDecl
 
-    if type(dataset_ref) is pl.DataFrame:
-        file_name = "data.json"
+    with dataset_ref.file_handle as file_handle:
+        file_name = _extract_name(
+            file_handle=file_handle, input_content_type=dataset_ref.content_type
+        )
         data_spec = (
             file_name,
-            json.dumps(dataset_ref.to_dicts()),
+            file_handle,
             str(pseudo_operation_request.target_content_type),
         )
+        # Post to file endpoint must be within the 'with' block to keep the file_handle open
         response = _client()._post_to_file_endpoint(
             path=PseudoClient.pseudo_op_to_endpoint[type(pseudo_operation_request)],
             request_spec=request_spec,
             data_spec=data_spec,
-            stream=False,
+            stream=True,
         )
-    else:
-        file = t.cast(File, dataset_ref)
-        with file.file_handle as file_handle:
-            file_name = _extract_name(
-                file_handle=file_handle, input_content_type=file.content_type
-            )
-            data_spec = (
-                file_name,
-                file_handle,
-                str(pseudo_operation_request.target_content_type),
-            )
-            # Post to file endpoint must be within the 'with' block to keep the file_handle open
-            response = _client()._post_to_file_endpoint(
-                path=PseudoClient.pseudo_op_to_endpoint[type(pseudo_operation_request)],
-                request_spec=request_spec,
-                data_spec=data_spec,
-                stream=True,
-            )
 
     payload = json.loads(response.content.decode("utf-8"))
     pseudo_data = payload["data"]
     metadata = RawPseudoMetadata(
         logs=payload["logs"],
         metrics=payload["metrics"],
         datadoc=payload["datadoc_metadata"]["pseudo_variables"],
```

### Comparing `dapla_toolbelt_pseudo-1.8.5/src/dapla_pseudo/v1/repseudo.py` & `dapla_toolbelt_pseudo-1.8.6/src/dapla_pseudo/v1/repseudo.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-1.8.5/src/dapla_pseudo/v1/result.py` & `dapla_toolbelt_pseudo-1.8.6/src/dapla_pseudo/v1/result.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-1.8.5/src/dapla_pseudo/v1/supported_file_format.py` & `dapla_toolbelt_pseudo-1.8.6/src/dapla_pseudo/v1/supported_file_format.py`

 * *Files 12% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
 class SupportedOutputFileFormat(Enum):
     """SupportedOutputFileFormat contains the supported file formats when outputting the result to a file.
 
     Note that this does NOT describe the valid file extensions of _input_ data when reading from a file.
     """
 
+    ZIP = "zip"
     CSV = "csv"
     JSON = "json"
     XML = "xml"
     PARQUET = "parquet"
 
     @classmethod
     def _missing_(cls, value: object) -> None:
@@ -32,14 +33,15 @@
             % (", ".join([repr(m.value) for m in cls]))
         )
 
 
 FORMAT_TO_MIMETYPE_FUNCTION = {
     SupportedOutputFileFormat.CSV: "text/csv",
     SupportedOutputFileFormat.JSON: "application/json",
+    SupportedOutputFileFormat.ZIP: "application/zip",
 }
 
 
 def read_to_pandas_df(
     supported_format: SupportedOutputFileFormat,
     df_dataset: BytesIO | Path,
     **kwargs: Any,
@@ -52,14 +54,18 @@
             )  # Pseudo Service CSV-separator is ';'
         case SupportedOutputFileFormat.JSON:
             return pd.DataFrame(pd.read_json(df_dataset, **kwargs))
         case SupportedOutputFileFormat.XML:
             return pd.read_xml(df_dataset, **kwargs)
         case SupportedOutputFileFormat.PARQUET:
             return pd.read_parquet(df_dataset, **kwargs)
+        case SupportedOutputFileFormat.ZIP:
+            raise ValueError(
+                f"Unsupported file format for Pandas: '{supported_format}'."
+            )
 
 
 def read_to_polars_df(
     supported_format: SupportedOutputFileFormat,
     df_dataset: BytesIO | Path,
     **kwargs: Any,
 ) -> pl.DataFrame:
@@ -69,17 +75,17 @@
             return pl.read_csv(
                 df_dataset, separator=";", **kwargs
             )  # Pseudo Service CSV-separator is ';'
         case SupportedOutputFileFormat.JSON:
             return pl.read_json(df_dataset, **kwargs)
         case SupportedOutputFileFormat.PARQUET:
             return pl.read_parquet(df_dataset, **kwargs)
-        case SupportedOutputFileFormat.XML:
+        case SupportedOutputFileFormat.XML | SupportedOutputFileFormat.ZIP:
             raise ValueError(
-                "Unsupported file format for Polars: 'XML'. Use Pandas instead."
+                f"Unsupported file format for Polars: '{supported_format}'."
             )
 
 
 def write_from_dicts(
     data: list[dict[str, t.Any]],
     supported_format: SupportedOutputFileFormat,
     file_like: BufferedWriter,
```

### Comparing `dapla_toolbelt_pseudo-1.8.5/src/dapla_pseudo/v1/validation.py` & `dapla_toolbelt_pseudo-1.8.6/src/dapla_pseudo/v1/validation.py`

 * *Files identical despite different names*

### Comparing `dapla_toolbelt_pseudo-1.8.5/PKG-INFO` & `dapla_toolbelt_pseudo-1.8.6/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dapla-toolbelt-pseudo
-Version: 1.8.5
+Version: 1.8.6
 Summary: Pseudonymization extensions for Dapla
 Home-page: https://github.com/statisticsnorway/dapla-toolbelt-pseudo
 License: MIT
 Author: Dapla Developers
 Author-email: dapla-platform-developers@ssb.no
 Requires-Python: >=3.10,<3.13
 Classifier: Development Status :: 4 - Beta
@@ -235,15 +235,15 @@
     .to_polars(**options)                  # Get the result as a polars dataframe
 )
 ```
 
 #### Pseudonymize using custom keys/keysets
 
 ```python
-from dapla_pseudo import pseudonymize
+from dapla_pseudo import Pseudonymize, PseudoKeyset
 
 # Pseudonymize fields in a local file using the default key:
 df = (
     Pseudonymize.from_polars(df)                            # Specify what dataframe to use
     .on_fields("fornavn")                                   # Select the field to pseudonymize
     .with_default_encryption()                              # Select the pseudonymization algorithm to apply
     .run()                                         # Apply pseudonymization to the selected field
@@ -281,14 +281,57 @@
     Pseudonymize.from_polars(df)
     .on_fields("fornavn")
     .with_default_encryption(custom_key="1234567890") # Note that the custom key has to be the same as "primaryKeyId" in the custom keyset
     .run(custom_keyset=custom_keyset)
     .to_polars()
 )
 ```
+#### Pseudonymize using custom rules
+
+Instead of declaring the pseudonymization rules via the Pseudonymize functions, one can define the rules manually.
+This can be done via the `PseudoRule` class like this:
+
+```python
+from dapla_pseudo import Pseudonymize, PseudoRule
+
+rule_json = {
+    'name': 'my-fule',
+     'pattern': '**/identifiers/*',
+     'func': 'redact(placeholder=#)' # This is a shorthand representation of the redact function
+}
+
+rule = PseudoRule.from_json(rule_json)
+
+df = (
+    Pseudonymize.from_polars(df)
+    .add_rules(rule) # Add one or more pseudonymization rules
+    .run()
+    .to_polars()
+)
+```
+
+Pseudonymization rules can also be read from file. This is especially handy when there are several rules, or if you
+prefer to store and maintain pseudonymization rules externally. For example:
+
+```python
+from dapla_pseudo import PseudoRule
+import json
+
+with open("pseudo-rules.json", 'r') as rules_file:
+    rules_json = json.load(rules_file)
+
+pseudo_rules = [PseudoRule.from_json(rule) for rule in rules_json]
+
+df = (
+    Pseudonymize.from_polars(df)
+    .add_rules(pseudo_rules)
+    .run()
+    .to_polars()
+)
+```
 
 ### Depseudonymize
 
 The "Depseudonymize" functions are almost exactly the same as when pseudonymizing.
 User can map from Stable ID *back to* FNR.
 
 ```python
```

