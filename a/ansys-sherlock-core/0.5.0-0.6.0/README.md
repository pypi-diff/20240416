# Comparing `tmp/ansys_sherlock_core-0.5.0.tar.gz` & `tmp/ansys_sherlock_core-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansys_sherlock_core-0.5.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "ansys_sherlock_core-0.6.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ansys_sherlock_core-0.5.0.tar` & `ansys_sherlock_core-0.6.0.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1089 2024-03-07 15:07:43.022562 ansys_sherlock_core-0.5.0/LICENSE
--rw-r--r--   0        0        0     4003 2024-03-07 15:07:43.022562 ansys_sherlock_core-0.5.0/README.rst
--rw-r--r--   0        0        0     2088 2024-03-07 15:07:43.022562 ansys_sherlock_core-0.5.0/pyproject.toml
--rw-r--r--   0        0        0      645 2024-03-07 15:07:43.022562 ansys_sherlock_core-0.5.0/src/ansys/sherlock/core/__init__.py
--rw-r--r--   0        0        0    74913 2024-03-07 15:07:43.022562 ansys_sherlock_core-0.5.0/src/ansys/sherlock/core/analysis.py
--rw-r--r--   0        0        0     4385 2024-03-07 15:07:43.022562 ansys_sherlock_core-0.5.0/src/ansys/sherlock/core/common.py
--rw-r--r--   0        0        0    31813 2024-03-07 15:07:43.022562 ansys_sherlock_core-0.5.0/src/ansys/sherlock/core/errors.py
--rw-r--r--   0        0        0      796 2024-03-07 15:07:43.022562 ansys_sherlock_core-0.5.0/src/ansys/sherlock/core/grpc_stub.py
--rw-r--r--   0        0        0     4987 2024-03-07 15:07:43.022562 ansys_sherlock_core-0.5.0/src/ansys/sherlock/core/launcher.py
--rw-r--r--   0        0        0    11825 2024-03-07 15:07:43.026562 ansys_sherlock_core-0.5.0/src/ansys/sherlock/core/layer.py
--rw-r--r--   0        0        0    76155 2024-03-07 15:07:43.026562 ansys_sherlock_core-0.5.0/src/ansys/sherlock/core/lifecycle.py
--rw-r--r--   0        0        0     2038 2024-03-07 15:07:43.026562 ansys_sherlock_core-0.5.0/src/ansys/sherlock/core/logging.py
--rw-r--r--   0        0        0    14694 2024-03-07 15:07:43.026562 ansys_sherlock_core-0.5.0/src/ansys/sherlock/core/model.py
--rw-r--r--   0        0        0    34541 2024-03-07 15:07:43.026562 ansys_sherlock_core-0.5.0/src/ansys/sherlock/core/parts.py
--rw-r--r--   0        0        0    66395 2024-03-07 15:07:43.026562 ansys_sherlock_core-0.5.0/src/ansys/sherlock/core/project.py
--rw-r--r--   0        0        0      929 2024-03-07 15:07:43.026562 ansys_sherlock_core-0.5.0/src/ansys/sherlock/core/sherlock.py
--rw-r--r--   0        0        0    33711 2024-03-07 15:07:43.026562 ansys_sherlock_core-0.5.0/src/ansys/sherlock/core/stackup.py
--rw-r--r--   0        0        0      108 2024-03-07 15:07:43.026562 ansys_sherlock_core-0.5.0/src/ansys/sherlock/core/types/__init__.py
--rw-r--r--   0        0        0     3053 2024-03-07 15:07:43.026562 ansys_sherlock_core-0.5.0/src/ansys/sherlock/core/types/analysis_types.py
--rw-r--r--   0        0        0     2505 2024-03-07 15:07:43.026562 ansys_sherlock_core-0.5.0/src/ansys/sherlock/core/types/common_types.py
--rw-r--r--   0        0        0     2261 2024-03-07 15:07:43.026562 ansys_sherlock_core-0.5.0/src/ansys/sherlock/core/types/layer_types.py
--rw-r--r--   0        0        0     2444 2024-03-07 15:07:43.026562 ansys_sherlock_core-0.5.0/src/ansys/sherlock/core/types/parts_types.py
--rw-r--r--   0        0        0     4669 2024-03-07 15:07:43.026562 ansys_sherlock_core-0.5.0/src/ansys/sherlock/core/types/project_types.py
--rw-r--r--   0        0        0      614 2024-03-07 15:07:43.026562 ansys_sherlock_core-0.5.0/src/ansys/sherlock/core/types/stackup_types.py
--rw-r--r--   0        0        0     5715 1970-01-01 00:00:00.000000 ansys_sherlock_core-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0     1089 2024-04-16 16:03:33.022837 ansys_sherlock_core-0.6.0/LICENSE
+-rw-r--r--   0        0        0     4003 2024-04-16 16:03:33.022837 ansys_sherlock_core-0.6.0/README.rst
+-rw-r--r--   0        0        0     2088 2024-04-16 16:03:33.026837 ansys_sherlock_core-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0      645 2024-04-16 16:03:33.026837 ansys_sherlock_core-0.6.0/src/ansys/sherlock/core/__init__.py
+-rw-r--r--   0        0        0    74913 2024-04-16 16:03:33.026837 ansys_sherlock_core-0.6.0/src/ansys/sherlock/core/analysis.py
+-rw-r--r--   0        0        0     4385 2024-04-16 16:03:33.026837 ansys_sherlock_core-0.6.0/src/ansys/sherlock/core/common.py
+-rw-r--r--   0        0        0    32504 2024-04-16 16:03:33.026837 ansys_sherlock_core-0.6.0/src/ansys/sherlock/core/errors.py
+-rw-r--r--   0        0        0      796 2024-04-16 16:03:33.026837 ansys_sherlock_core-0.6.0/src/ansys/sherlock/core/grpc_stub.py
+-rw-r--r--   0        0        0     4987 2024-04-16 16:03:33.026837 ansys_sherlock_core-0.6.0/src/ansys/sherlock/core/launcher.py
+-rw-r--r--   0        0        0    11825 2024-04-16 16:03:33.026837 ansys_sherlock_core-0.6.0/src/ansys/sherlock/core/layer.py
+-rw-r--r--   0        0        0    76155 2024-04-16 16:03:33.026837 ansys_sherlock_core-0.6.0/src/ansys/sherlock/core/lifecycle.py
+-rw-r--r--   0        0        0     2038 2024-04-16 16:03:33.026837 ansys_sherlock_core-0.6.0/src/ansys/sherlock/core/logging.py
+-rw-r--r--   0        0        0    28292 2024-04-16 16:03:33.026837 ansys_sherlock_core-0.6.0/src/ansys/sherlock/core/model.py
+-rw-r--r--   0        0        0    37537 2024-04-16 16:03:33.026837 ansys_sherlock_core-0.6.0/src/ansys/sherlock/core/parts.py
+-rw-r--r--   0        0        0    73410 2024-04-16 16:03:33.026837 ansys_sherlock_core-0.6.0/src/ansys/sherlock/core/project.py
+-rw-r--r--   0        0        0      929 2024-04-16 16:03:33.026837 ansys_sherlock_core-0.6.0/src/ansys/sherlock/core/sherlock.py
+-rw-r--r--   0        0        0    33711 2024-04-16 16:03:33.026837 ansys_sherlock_core-0.6.0/src/ansys/sherlock/core/stackup.py
+-rw-r--r--   0        0        0      108 2024-04-16 16:03:33.026837 ansys_sherlock_core-0.6.0/src/ansys/sherlock/core/types/__init__.py
+-rw-r--r--   0        0        0     3053 2024-04-16 16:03:33.026837 ansys_sherlock_core-0.6.0/src/ansys/sherlock/core/types/analysis_types.py
+-rw-r--r--   0        0        0     3349 2024-04-16 16:03:33.026837 ansys_sherlock_core-0.6.0/src/ansys/sherlock/core/types/common_types.py
+-rw-r--r--   0        0        0     2261 2024-04-16 16:03:33.026837 ansys_sherlock_core-0.6.0/src/ansys/sherlock/core/types/layer_types.py
+-rw-r--r--   0        0        0     2444 2024-04-16 16:03:33.030837 ansys_sherlock_core-0.6.0/src/ansys/sherlock/core/types/parts_types.py
+-rw-r--r--   0        0        0     5329 2024-04-16 16:03:33.030837 ansys_sherlock_core-0.6.0/src/ansys/sherlock/core/types/project_types.py
+-rw-r--r--   0        0        0      614 2024-04-16 16:03:33.030837 ansys_sherlock_core-0.6.0/src/ansys/sherlock/core/types/stackup_types.py
+-rw-r--r--   0        0        0     5715 1970-01-01 00:00:00.000000 ansys_sherlock_core-0.6.0/PKG-INFO
```

### Comparing `ansys_sherlock_core-0.5.0/LICENSE` & `ansys_sherlock_core-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ansys_sherlock_core-0.5.0/README.rst` & `ansys_sherlock_core-0.6.0/README.rst`

 * *Files identical despite different names*

### Comparing `ansys_sherlock_core-0.5.0/pyproject.toml` & `ansys_sherlock_core-0.6.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "ansys-sherlock-core"
-version = "0.5.0"
+version = "0.6.0"
 description = "A python wrapper for Ansys Sherlock"
 readme = "README.rst"
 requires-python = ">=3.8,<4"
 license = {file = "LICENSE"}
 authors = [{name = "ANSYS, Inc.", email = "pyansys.core@ansys.com"}]
 maintainers = [{name = "ANSYS, Inc.", email = "pyansys.core@ansys.com"}]
 classifiers = [
@@ -20,30 +20,30 @@
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 
 dependencies = [
-    "ansys-api-sherlock==0.1.24",
+    "ansys-api-sherlock==0.1.27",
     "grpcio>=1.17",
     "importlib-metadata>=4.0,<5; python_version<='3.8'",
     "protobuf~=3.20",
 ]
 
 [project.optional-dependencies]
 tests = [
-    "grpcio==1.62.0",
+    "grpcio==1.62.1",
     "protobuf==3.20.3",
-    "pytest==8.1.0",
-    "pytest-cov==4.1.0",
+    "pytest==8.1.1",
+    "pytest-cov==5.0.0",
 ]
 doc = [
-    "ansys-sphinx-theme==0.14.0",
-    "numpydoc==1.6.0",
+    "ansys-sphinx-theme==0.15.2",
+    "numpydoc==1.7.0",
     "Sphinx==6.2.1", # BLOCKED BY sphinx-design - Cannot upgrade to Sphinx 7 for now
     "sphinx-copybutton==0.5.2",
     "sphinx_design==0.5.0",
     "sphinx-gallery==0.15.0",
 ]
 
 [project.urls]
```

### Comparing `ansys_sherlock_core-0.5.0/src/ansys/sherlock/core/__init__.py` & `ansys_sherlock_core-0.6.0/src/ansys/sherlock/core/__init__.py`

 * *Files identical despite different names*

### Comparing `ansys_sherlock_core-0.5.0/src/ansys/sherlock/core/analysis.py` & `ansys_sherlock_core-0.6.0/src/ansys/sherlock/core/analysis.py`

 * *Files identical despite different names*

### Comparing `ansys_sherlock_core-0.5.0/src/ansys/sherlock/core/common.py` & `ansys_sherlock_core-0.6.0/src/ansys/sherlock/core/common.py`

 * *Files identical despite different names*

### Comparing `ansys_sherlock_core-0.5.0/src/ansys/sherlock/core/errors.py` & `ansys_sherlock_core-0.6.0/src/ansys/sherlock/core/errors.py`

 * *Files 0% similar despite different names*

```diff
@@ -633,14 +633,26 @@
         self.message = message
 
     def __str__(self):
         """Format error message."""
         return f"Model service error: {self.message}"
 
 
+class SherlockExportAEDBError(Exception):
+    """Contains the error raised when an Electronics Desktop model cannot be exported."""
+
+    def __init__(self, message):
+        """Initialize error message."""
+        self.message = message
+
+    def __str__(self):
+        """Format error message."""
+        return f"Export AEDB error: {self.message}"
+
+
 class SherlockInvalidLoadDirectionError(Exception):
     """Contains the error raised when the load direction string is invalid."""
 
     def __init__(self, message):
         """Initialize error message."""
         self.message = message
 
@@ -997,7 +1009,19 @@
     def str_itr(self):
         """Format error message."""
         if self.message is None:
             return [f"Update parts list properties error: {error}" for error in self.error_array]
 
         assert self.error_array is None
         return [f"Update parts list properties error: {self.message}"]
+
+
+class SherlockExportNetListError(Exception):
+    """Contains the error raised when a net list cannot be exported."""
+
+    def __init__(self, message):
+        """Initialize error message."""
+        self.message = message
+
+    def __str__(self):
+        """Format error message."""
+        return f"Export net list error: {self.message}"
```

### Comparing `ansys_sherlock_core-0.5.0/src/ansys/sherlock/core/grpc_stub.py` & `ansys_sherlock_core-0.6.0/src/ansys/sherlock/core/grpc_stub.py`

 * *Files identical despite different names*

### Comparing `ansys_sherlock_core-0.5.0/src/ansys/sherlock/core/launcher.py` & `ansys_sherlock_core-0.6.0/src/ansys/sherlock/core/launcher.py`

 * *Files identical despite different names*

### Comparing `ansys_sherlock_core-0.5.0/src/ansys/sherlock/core/layer.py` & `ansys_sherlock_core-0.6.0/src/ansys/sherlock/core/layer.py`

 * *Files identical despite different names*

### Comparing `ansys_sherlock_core-0.5.0/src/ansys/sherlock/core/lifecycle.py` & `ansys_sherlock_core-0.6.0/src/ansys/sherlock/core/lifecycle.py`

 * *Files identical despite different names*

### Comparing `ansys_sherlock_core-0.5.0/src/ansys/sherlock/core/logging.py` & `ansys_sherlock_core-0.6.0/src/ansys/sherlock/core/logging.py`

 * *Files identical despite different names*

### Comparing `ansys_sherlock_core-0.5.0/src/ansys/sherlock/core/parts.py` & `ansys_sherlock_core-0.6.0/src/ansys/sherlock/core/parts.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,31 +1,33 @@
-# © 2023 ANSYS, Inc. All rights reserved
+# © 2024 ANSYS, Inc. All rights reserved
 
 """Module containing all parts management capabilities."""
 
 try:
     import SherlockPartsService_pb2
     import SherlockPartsService_pb2_grpc
 except ModuleNotFoundError:
     from ansys.api.sherlock.v0 import SherlockPartsService_pb2
     from ansys.api.sherlock.v0 import SherlockPartsService_pb2_grpc
 
 from ansys.sherlock.core import LOG
 from ansys.sherlock.core.errors import (
     SherlockEnableLeadModelingError,
+    SherlockExportNetListError,
     SherlockExportPartsListError,
     SherlockGetPartLocationError,
     SherlockImportPartsListError,
     SherlockUpdatePartsFromAVLError,
     SherlockUpdatePartsListError,
     SherlockUpdatePartsListPropertiesError,
     SherlockUpdatePartsLocationsByFileError,
     SherlockUpdatePartsLocationsError,
 )
 from ansys.sherlock.core.grpc_stub import GrpcStub
+from ansys.sherlock.core.types.common_types import TableDelimiter
 from ansys.sherlock.core.types.parts_types import (
     AVLDescription,
     AVLPartNum,
     PartLocation,
     PartsListSearchDuplicationMode,
     PartsListSearchMatchingMode,
 )
@@ -925,7 +927,93 @@
 
             return return_code.value
 
         except SherlockUpdatePartsListPropertiesError as e:
             for error in e.str_itr():
                 LOG.error(error)
             raise e
+
+    def export_net_list(
+        self,
+        project,
+        cca_name,
+        output_file,
+        col_delimiter=TableDelimiter.COMMA,
+        overwrite_existing=False,
+        utf8_enabled=False,
+    ):
+        """Export a net list to a delimited output file.
+
+        Parameters
+        ----------
+        project : str
+            Name of the Sherlock project.
+        cca_name : str
+            Name of the CCA.
+        output_file : str
+            Full path for the output file where the net list will be written.
+        col_delimiter : TableDelimiter, optional
+            The delimiter character to be used. Defaults to TableDelimiter.COMMA.
+        overwrite_existing : bool, optional
+            Flag to determine if existing .CSV files should be overwritten
+            if they match the output_file. Defaults to False.
+        utf8_enabled : bool, optional
+            Flag that specifies if UTF-8 will be used for .CSV files. Defaults to False.
+
+        Returns
+        -------
+        int
+            Status code of the response. 0 for success.
+
+        Examples
+        --------
+        >>> from ansys.sherlock.core.launcher import launch_sherlock
+        >>> sherlock = launch_sherlock()
+        >>> sherlock.project.import_odb_archive(
+            "ODB++ Tutorial.tgz",
+            True,
+            True,
+            True,
+            True,
+            project="Test",
+            cca_name="Card",
+        )
+        >>> sherlock.parts.export_net_list(
+            "Test",
+            "Card",
+            "Net List.csv",
+            col_delimiter=TableDelimiter.TAB,
+            overwrite_existing=True,
+            utf8_enabled=True
+        )
+        """
+        try:
+            if project == "":
+                raise SherlockExportNetListError(message="Project name is invalid.")
+            if cca_name == "":
+                raise SherlockExportNetListError(message="CCA name is invalid.")
+            if output_file == "":
+                raise SherlockExportNetListError(message="Output file path is required.")
+
+            if not self._is_connection_up():
+                LOG.error("There is no connection to a gRPC service.")
+                return
+
+            request = SherlockPartsService_pb2.ExportNetListRequest(
+                project=project,
+                ccaName=cca_name,
+                outputFilePath=output_file,
+                overwriteExisting=overwrite_existing,
+                colDelimiter=col_delimiter,
+                utf8Enabled=utf8_enabled,
+            )
+
+            response = self.stub.exportNetList(request)
+
+            if response.value == -1:
+                raise SherlockExportNetListError(response.message)
+
+        except SherlockExportNetListError as e:
+            LOG.error(str(e))
+            raise e
+
+        return response.value
```

### Comparing `ansys_sherlock_core-0.5.0/src/ansys/sherlock/core/project.py` & `ansys_sherlock_core-0.6.0/src/ansys/sherlock/core/project.py`

 * *Files 10% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 from ansys.sherlock.core.types.project_types import (
     BoardBounds,
     CsvExcelFile,
     IcepakFile,
     ImageBounds,
     ImageFile,
     LegendBounds,
+    StrainMapsFileType,
 )
 
 
 class Project(GrpcStub):
     """Contains all project management capabilities."""
 
     def __init__(self, channel):
@@ -539,128 +540,268 @@
                 LOG.info(response.message)
                 return response.value
         except SherlockAddCCAError as e:
             LOG.error(str(e))
             raise e
 
     def add_strain_maps(self, project, strain_maps):
-        """Add a CSV file with strain maps to the CCAs.
+        """Add strain map files to CCAs in a Sherlock project.
 
         Parameters
         ----------
         project: str
             Name of the Sherlock project to add strain maps to.
         strain_maps : list
             List of strain maps consisting of these properties:
 
             - strain_map_file : str
                 Full path to the CSV file with the strain maps.
             - file_comment : str
                 Comment to associate with the file.
+            - file_type : StrainMapsFileType
+                Strain maps file type. Options are CSV, Excel, and Image.
             - header_row_count : int
                 Number of rows before the file's column header.
             - reference_id_column : str
                 Name of the column in the file with reference IDs.
             - strain_column : str
                 Name of the column in the file with strain values.
             - strain_units : str
                 Strain units. Options are ``µε`` and ``ε``.
+            - image_file : StrainMapImageFile, optional
+                The properties of the strain map file to add.
             - ccas : list, optional
                 List of CCA names to assign the file to. When no list is
                 specified, the file is assigned to all CCAs in the project.
 
         Returns
         -------
         int
             Status code of the response. 0 for success.
 
         Examples
         --------
         >>> from ansys.sherlock.core.launcher import launch_sherlock
+        >>> from ansys.sherlock.core.types.project_types import (
+            BoardBounds,
+            ImageBounds,
+            ImageFile,
+            LegendBounds,
+            LegendOrientation,
+            StrainMapsFileType,
+            StrainMapLegendOrientation,
+        )
         >>> sherlock = launch_sherlock()
-        >>> sherlock.project.add_strain_maps("Tutorial Project",
-            [("StrainMap.csv",
-            "This is the strain map file for the project",
-            0,
-            "refDes",
-            "strain",
-            "µε"
-            ["Main Board"])
-            )],
+        >>> sherlock.project.add_strain_maps(
+            "Tutorial Project",
+                [
+                    (
+                        "StrainMap.csv",
+                        "This is the strain map file for the project",
+                        StrainMapsFileType.CSV,
+                        0,
+                        "refDes",
+                        "strain",
+                        "µε",
+                        ["Main Board"]
+                    )
+                ]
+            )
+        >>> strain_map_image_properties = (
+                BoardBounds([
+                    (1.0, 2.0),
+                    (3.0, 4.0),
+                    (1.0, 2.0),
+                    (1.0, 2.0)
+                ]),
+                "in",
+                ImageBounds(0.0, 0.0, 10.0, 8.0),
+                LegendBounds(1.0, 2.0, 4.0, 2.0),
+                StrainMapLegendOrientation.VERTICAL,
+                20.0,
+                50.0,
+                "µε"
+            )
+        >>> sherlock.project.add_strain_maps(
+            "Tutorial Project",
+                [
+                    (
+                        "StrainMap.jpg",
+                        "This is the strain map image for the project",
+                        StrainMapsFileType.IMAGE,
+                        strain_map_image_properties,
+                        ["Main Board"]
+                    )
+                ]
+            )
         """
         try:
             if project == "":
                 raise SherlockAddStrainMapsError(message="Project name is invalid.")
 
             if len(strain_maps) == 0:
                 raise SherlockAddStrainMapsError(message="Strain maps are missing.")
 
             # Validate first
             for i, strain_map in enumerate(strain_maps):
-                if len(strain_map) < 6 or len(strain_map) > 7:
-                    raise SherlockAddStrainMapsError(
-                        f"Number of elements ({str(len(strain_maps))}) is wrong for strain map {i}."  # noqa: E501
-                    )
-                elif not isinstance(strain_map[0], str) or strain_map[0] == "":
-                    raise SherlockAddStrainMapsError(f"Path is required for strain map {i}.")
-                elif not isinstance(strain_map[2], int) or strain_map[2] == "":
-                    raise SherlockAddStrainMapsError(
-                        f"Header row count is required for strain map {i}."
-                    )
-                elif strain_map[2] < 0:
-                    raise SherlockAddStrainMapsError(
-                        f"Header row count must be greater than or equal to 0 for strain map {i}."
-                    )
-                elif not isinstance(strain_map[3], str) or strain_map[3] == "":
-                    raise SherlockAddStrainMapsError(
-                        f"Reference ID column is required for strain map {i}."
-                    )
-                elif not isinstance(strain_map[4], str) or strain_map[4] == "":
-                    raise SherlockAddStrainMapsError(
-                        f"Strain column is required for strain map {i}."
-                    )
-                elif not isinstance(strain_map[5], str) or strain_map[5] == "":
-                    raise SherlockAddStrainMapsError(
-                        f"Strain units are required for strain map {i}."
-                    )
-                elif strain_map[5] != "µε" and strain_map[5] != "ε":
-                    raise SherlockAddStrainMapsError(
-                        f'Strain units "{strain_map[5]}" are invalid for strain map {i}.'
-                    )
-                elif (
-                    len(strain_map) == 7
-                    and strain_map[6] is not None
-                    and type(strain_map[6]) is not list
+                if (
+                    strain_map[2] == StrainMapsFileType.CSV
+                    or strain_map[2] == StrainMapsFileType.EXCEL
                 ):
-                    raise SherlockAddStrainMapsError(
-                        message=f"cca_names is not a list for strain map {i}."
-                    )
+                    if len(strain_map) < 7 or len(strain_map) > 8:
+                        raise SherlockAddStrainMapsError(
+                            f"Number of elements ({str(len(strain_maps))}) is wrong for strain map {i}."  # noqa: E501
+                        )
+                    elif not isinstance(strain_map[0], str) or strain_map[0] == "":
+                        raise SherlockAddStrainMapsError(f"Path is required for strain map {i}.")
+                    elif not isinstance(strain_map[3], int) or strain_map[3] == "":
+                        raise SherlockAddStrainMapsError(
+                            f"Header row count is required for strain map {i}."
+                        )
+                    elif strain_map[3] < 0:
+                        raise SherlockAddStrainMapsError(
+                            f"Header row count must be greater than or "
+                            f"equal to 0 for strain map {i}."
+                        )
+                    elif not isinstance(strain_map[4], str) or strain_map[4] == "":
+                        raise SherlockAddStrainMapsError(
+                            f"Reference ID column is required for strain map {i}."
+                        )
+                    elif not isinstance(strain_map[5], str) or strain_map[5] == "":
+                        raise SherlockAddStrainMapsError(
+                            f"Strain column is required for strain map {i}."
+                        )
+                    elif not isinstance(strain_map[6], str) or strain_map[6] == "":
+                        raise SherlockAddStrainMapsError(
+                            f"Strain units are required for strain map {i}."
+                        )
+                    elif strain_map[6] != "µε" and strain_map[6] != "ε":
+                        raise SherlockAddStrainMapsError(
+                            f'Strain units "{strain_map[6]}" are invalid for strain map {i}.'
+                        )
+                    elif (
+                        len(strain_map) == 8
+                        and strain_map[7] is not None
+                        and type(strain_map[7]) is not list
+                    ):
+                        raise SherlockAddStrainMapsError(
+                            message=f"cca_names is not a list " f"for strain map {i}."
+                        )
+
+                elif strain_map[2] == StrainMapsFileType.IMAGE:
+                    if len(strain_map) < 4 or len(strain_map) > 5:
+                        raise SherlockAddStrainMapsError(
+                            f"Number of elements ({str(len(strain_maps))}) "
+                            f"is wrong for strain map {i}."
+                        )
+                    elif not isinstance(strain_map[0], str) or strain_map[0] == "":
+                        raise SherlockAddStrainMapsError(f"Path is required for strain map {i}.")
+                    elif not isinstance(strain_map[3], tuple) or strain_map[3] == "":
+                        raise SherlockAddStrainMapsError(
+                            f"image_file is not a list for strain map {i}."
+                        )
+
+                    image_file_properties = strain_map[3]
+
+                    if not isinstance(image_file_properties[0], BoardBounds):
+                        raise SherlockAddStrainMapsError(
+                            f"Invalid board bounds for " f"strain map {i}."
+                        )
+
+                    if not isinstance(image_file_properties[1], (str, type(None))):
+                        raise SherlockAddStrainMapsError(
+                            f"Invalid coordinate units for " f"strain map {i}."
+                        )
+
+                    if not isinstance(image_file_properties[2], ImageBounds):
+                        raise SherlockAddStrainMapsError(
+                            f"Invalid image bounds for " f"strain map {i}."
+                        )
+
+                    if not isinstance(image_file_properties[3], LegendBounds):
+                        raise SherlockAddStrainMapsError(
+                            f"Invalid legend bounds for " f"strain map {i}."
+                        )
+
+                    if not isinstance(image_file_properties[4], int):
+                        raise SherlockAddStrainMapsError(
+                            f"Invalid legend orientation for " f"strain map {i}."
+                        )
+
+                    if not isinstance(image_file_properties[5], float):
+                        raise SherlockAddStrainMapsError(
+                            f"Invalid minimum strain for " f"strain map {i}."
+                        )
+
+                    if not isinstance(image_file_properties[6], float):
+                        raise SherlockAddStrainMapsError(
+                            f"Invalid maximum strain for " f"strain map {i}."
+                        )
+
+                    if not isinstance(image_file_properties[7], str):
+                        raise SherlockAddStrainMapsError(
+                            f"Invalid strain units for " f"strain map {i}."
+                        )
 
             if not self._is_connection_up():
                 LOG.error("There is no connection to a gRPC service.")
                 return
 
             request = SherlockProjectService_pb2.AddStrainMapRequest(project=project)
 
             # Add the strain maps to the request
             for s in strain_maps:
                 strain_map = request.strainMapFiles.add()
                 strain_map.strainMapFile = s[0]
                 strain_map.fileComment = s[1]
-                strain_map.headerRowCount = s[2]
-                strain_map.referenceIDColumn = s[3]
-                strain_map.strainColumn = s[4]
-                strain_map.strainUnits = s[5]
-
-                """Add the CCA names to the request."""
-                if len(s) == 7:
-                    cca_names = s[6]
-                    if cca_names is not None:
-                        for cca_name in cca_names:
-                            strain_map.cca.append(cca_name)
+                strain_map.fileType = s[2]
+
+                if s[2] == StrainMapsFileType.CSV or s[2] == StrainMapsFileType.EXCEL:
+                    strain_map.headerRowCount = s[3]
+                    strain_map.referenceIDColumn = s[4]
+                    strain_map.strainColumn = s[5]
+                    strain_map.strainUnits = s[6]
+
+                    """Add the CCA names to the request."""
+                    if len(s) == 8:
+                        cca_names = s[7]
+                        if cca_names is not None:
+                            for cca_name in cca_names:
+                                strain_map.cca.append(cca_name)
+
+                elif s[2] == StrainMapsFileType.IMAGE:
+                    strain_map_image_properties = s[3]
+                    image_file_properties = strain_map.imageFile
+                    image_properties = strain_map_image_properties
+
+                    for vertex in image_properties[0].bounds:
+                        node_coordinate = strain_map.imageFile.boardBounds.add()
+                        node_coordinate.vertexX = vertex[0]
+                        node_coordinate.vertexY = vertex[1]
+
+                    image_file_properties.coordinateUnits = image_properties[1]
+                    image_file_properties.imageBounds.imageX = image_properties[2].image_x
+                    image_file_properties.imageBounds.imageY = image_properties[2].image_y
+                    image_file_properties.imageBounds.imageH = image_properties[2].height
+                    image_file_properties.imageBounds.imageW = image_properties[2].width
+                    image_file_properties.legendBounds.legendX = image_properties[3].legend_x
+                    image_file_properties.legendBounds.legendY = image_properties[3].legend_y
+                    image_file_properties.legendBounds.legendH = image_properties[3].height
+                    image_file_properties.legendBounds.legendW = image_properties[3].width
+                    image_file_properties.legendOrientation = image_properties[4]
+                    image_file_properties.minStrain = image_properties[5]
+                    image_file_properties.maxStrain = image_properties[6]
+                    image_file_properties.strainUnits = image_properties[7]
+
+                    """Add the CCA names to the request."""
+                    if len(s) == 5:
+                        cca_names = s[4]
+                        if cca_names is not None:
+                            for cca_name in cca_names:
+                                strain_map.cca.append(cca_name)
 
             response = self.stub.addStrainMap(request)
 
             return_code = response.returnCode
 
             if return_code.value == -1:
                 if return_code.message == "":
```

### Comparing `ansys_sherlock_core-0.5.0/src/ansys/sherlock/core/sherlock.py` & `ansys_sherlock_core-0.6.0/src/ansys/sherlock/core/sherlock.py`

 * *Files identical despite different names*

### Comparing `ansys_sherlock_core-0.5.0/src/ansys/sherlock/core/stackup.py` & `ansys_sherlock_core-0.6.0/src/ansys/sherlock/core/stackup.py`

 * *Files identical despite different names*

### Comparing `ansys_sherlock_core-0.5.0/src/ansys/sherlock/core/types/analysis_types.py` & `ansys_sherlock_core-0.6.0/src/ansys/sherlock/core/types/analysis_types.py`

 * *Files identical despite different names*

### Comparing `ansys_sherlock_core-0.5.0/src/ansys/sherlock/core/types/layer_types.py` & `ansys_sherlock_core-0.6.0/src/ansys/sherlock/core/types/layer_types.py`

 * *Files identical despite different names*

### Comparing `ansys_sherlock_core-0.5.0/src/ansys/sherlock/core/types/parts_types.py` & `ansys_sherlock_core-0.6.0/src/ansys/sherlock/core/types/parts_types.py`

 * *Files identical despite different names*

### Comparing `ansys_sherlock_core-0.5.0/src/ansys/sherlock/core/types/project_types.py` & `ansys_sherlock_core-0.6.0/src/ansys/sherlock/core/types/project_types.py`

 * *Files 6% similar despite different names*

```diff
@@ -143,7 +143,31 @@
     "CSV"
     EXCEL = __file_type.Excel
     "Excel"
     IMAGE = __file_type.Image
     "Image"
     TMAP = __file_type.TMAP
     "Icepak Thermal Map (.TMAP)"
+
+
+class StrainMapsFileType:
+    """Constants for File Type in the Add Strain Maps request."""
+
+    __file_type = project_service.AddStrainMapRequest.StrainMapFile.FileType
+    CSV = __file_type.CSV
+    "CSV"
+    EXCEL = __file_type.Excel
+    "Excel"
+    IMAGE = __file_type.Image
+    "Image"
+
+
+class StrainMapLegendOrientation:
+    """Constants for legend orientation in the add strain maps request."""
+
+    __legend_orientation = (
+        project_service.AddStrainMapRequest.StrainMapFile.StrainMapImageFile.LegendOrientation
+    )
+    HORIZONTAL = __legend_orientation.Horizontal
+    "Horizontal"
+    VERTICAL = __legend_orientation.Vertical
+    "Vertical"
```

### Comparing `ansys_sherlock_core-0.5.0/src/ansys/sherlock/core/types/stackup_types.py` & `ansys_sherlock_core-0.6.0/src/ansys/sherlock/core/types/stackup_types.py`

 * *Files identical despite different names*

### Comparing `ansys_sherlock_core-0.5.0/PKG-INFO` & `ansys_sherlock_core-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 Metadata-Version: 2.1
 Name: ansys-sherlock-core
-Version: 0.5.0
+Version: 0.6.0
 Summary: A python wrapper for Ansys Sherlock
 Author-email: "ANSYS, Inc." <pyansys.core@ansys.com>
 Maintainer-email: "ANSYS, Inc." <pyansys.core@ansys.com>
 Requires-Python: >=3.8,<4
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Science/Research
 Classifier: Topic :: Scientific/Engineering :: Information Analysis
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: ansys-api-sherlock==0.1.24
+Requires-Dist: ansys-api-sherlock==0.1.27
 Requires-Dist: grpcio>=1.17
 Requires-Dist: importlib-metadata>=4.0,<5; python_version<='3.8'
 Requires-Dist: protobuf~=3.20
-Requires-Dist: ansys-sphinx-theme==0.14.0 ; extra == "doc"
-Requires-Dist: numpydoc==1.6.0 ; extra == "doc"
+Requires-Dist: ansys-sphinx-theme==0.15.2 ; extra == "doc"
+Requires-Dist: numpydoc==1.7.0 ; extra == "doc"
 Requires-Dist: Sphinx==6.2.1 ; extra == "doc"
 Requires-Dist: sphinx-copybutton==0.5.2 ; extra == "doc"
 Requires-Dist: sphinx_design==0.5.0 ; extra == "doc"
 Requires-Dist: sphinx-gallery==0.15.0 ; extra == "doc"
-Requires-Dist: grpcio==1.62.0 ; extra == "tests"
+Requires-Dist: grpcio==1.62.1 ; extra == "tests"
 Requires-Dist: protobuf==3.20.3 ; extra == "tests"
-Requires-Dist: pytest==8.1.0 ; extra == "tests"
-Requires-Dist: pytest-cov==4.1.0 ; extra == "tests"
+Requires-Dist: pytest==8.1.1 ; extra == "tests"
+Requires-Dist: pytest-cov==5.0.0 ; extra == "tests"
 Project-URL: Documentation, https://sherlock.docs.pyansys.com
 Project-URL: Homepage, https://github.com/ansys/pysherlock
 Project-URL: Source, https://github.com/ansys/pysherlock
 Project-URL: Tracker, https://github.com/ansys/pysherlock/issues
 Provides-Extra: doc
 Provides-Extra: tests
```

