# Comparing `tmp/oem2orm-0.3.3.tar.gz` & `tmp/oem2orm-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oem2orm-0.3.3.tar", last modified: Mon Apr 15 14:58:24 2024, max compression
+gzip compressed data, was "oem2orm-0.4.0.tar", last modified: Tue Apr 16 16:43:41 2024, max compression
```

## Comparing `oem2orm-0.3.3.tar` & `oem2orm-0.4.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:58:24.193353 oem2orm-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-15 14:58:20.000000 oem2orm-0.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     4100 2024-04-15 14:58:24.193353 oem2orm-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3144 2024-04-15 14:58:20.000000 oem2orm-0.3.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:58:24.193353 oem2orm-0.3.3/oem2orm/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-15 14:58:20.000000 oem2orm-0.3.3/oem2orm/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      836 2024-04-15 14:58:20.000000 oem2orm-0.3.3/oem2orm/main.py
--rw-r--r--   0 runner    (1001) docker     (127)     6607 2024-04-15 14:58:20.000000 oem2orm-0.3.3/oem2orm/oep_compliance.py
--rw-r--r--   0 runner    (1001) docker     (127)    14437 2024-04-15 14:58:20.000000 oem2orm-0.3.3/oem2orm/oep_oedialect_oem2orm.py
--rw-r--r--   0 runner    (1001) docker     (127)     1580 2024-04-15 14:58:20.000000 oem2orm-0.3.3/oem2orm/postgresql_types.py
--rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-15 14:58:20.000000 oem2orm-0.3.3/oem2orm/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-15 14:58:24.193353 oem2orm-0.3.3/oem2orm.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     4100 2024-04-15 14:58:24.000000 oem2orm-0.3.3/oem2orm.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-15 14:58:24.000000 oem2orm-0.3.3/oem2orm.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-15 14:58:24.000000 oem2orm-0.3.3/oem2orm.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-15 14:58:24.000000 oem2orm-0.3.3/oem2orm.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)       62 2024-04-15 14:58:24.000000 oem2orm-0.3.3/oem2orm.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-15 14:58:24.000000 oem2orm-0.3.3/oem2orm.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-15 14:58:24.193353 oem2orm-0.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     1481 2024-04-15 14:58:20.000000 oem2orm-0.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:43:41.759929 oem2orm-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (127)    35149 2024-04-16 16:43:37.000000 oem2orm-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     4987 2024-04-16 16:43:41.759929 oem2orm-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     4029 2024-04-16 16:43:37.000000 oem2orm-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:43:41.759929 oem2orm-0.4.0/oem2orm/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-16 16:43:37.000000 oem2orm-0.4.0/oem2orm/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1030 2024-04-16 16:43:37.000000 oem2orm-0.4.0/oem2orm/main.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6638 2024-04-16 16:43:37.000000 oem2orm-0.4.0/oem2orm/oep_compliance.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14615 2024-04-16 16:43:37.000000 oem2orm-0.4.0/oem2orm/oep_oedialect_oem2orm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1564 2024-04-16 16:43:37.000000 oem2orm-0.4.0/oem2orm/postgresql_types.py
+-rw-r--r--   0 runner    (1001) docker     (127)       92 2024-04-16 16:43:37.000000 oem2orm-0.4.0/oem2orm/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-16 16:43:41.759929 oem2orm-0.4.0/oem2orm.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     4987 2024-04-16 16:43:41.000000 oem2orm-0.4.0/oem2orm.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      357 2024-04-16 16:43:41.000000 oem2orm-0.4.0/oem2orm.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-16 16:43:41.000000 oem2orm-0.4.0/oem2orm.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-16 16:43:41.000000 oem2orm-0.4.0/oem2orm.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       64 2024-04-16 16:43:41.000000 oem2orm-0.4.0/oem2orm.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        8 2024-04-16 16:43:41.000000 oem2orm-0.4.0/oem2orm.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-16 16:43:41.759929 oem2orm-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     1483 2024-04-16 16:43:37.000000 oem2orm-0.4.0/setup.py
```

### Comparing `oem2orm-0.3.3/LICENSE` & `oem2orm-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `oem2orm-0.3.3/PKG-INFO` & `oem2orm-0.4.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,132 +1,116 @@
 Metadata-Version: 2.1
 Name: oem2orm
-Version: 0.3.3
+Version: 0.4.0
 Summary: SQLAlchemy module to generate ORM, read from data model (oedatamodel) in open-energy-metadata JSON format
 Home-page: https://github.com/OpenEnergyPlatform/oem2orm
 Author: henhuy, jh-RLI
 Author-email: Hendrik.Huyskens@rl-institut.de
 Project-URL: Bug Reports, https://github.com/OpenEnergyPlatform/oem2orm/issues
 Project-URL: Source, https://github.com/OpenEnergyPlatform/oem2orm/tree/develop/oem2orm
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: sqlalchemy==1.3.14
-Requires-Dist: oedialect==1.1
+Requires-Dist: sqlalchemy==1.3.16
+Requires-Dist: oedialect==0.1.1
 Requires-Dist: requests
 Requires-Dist: jmespath
 Requires-Dist: omi
 Requires-Dist: click
 
-# OEM to ORM
+# oem 2 orm
 
-Create database tables (and schema) from oemetadata json file(s)
+Create database tables (and schema) from oemetadata json file(s). This tool is part of the open-energy-metadata (OEM) integration into the [OEP](https://openenergyplatform.org/).
 
-## Installation:
+## Installation
 
 You can install pacakge using standard python installation:
 `
 pip install oem2orm
 `
 
 or if you interested in CLI-version only you can install it using pipx (pipx must be installed):
 `
 pipx install oem2orm
 `
 see [Pipx-Documentation](https://pypa.github.io/pipx/) for further information.
 
+## Usage
 
-## Usage:
+Read the Restrictions section and have a look at our [tutorial](./tutorial/USAGE.md) section to get more information about the usage of oem2orm either as code module or CLI tool. The tutorials also provide information how to validate your oemetadata files.
 
-This tool is part of the open-energy-metadata (OEM) integration into the [OEP](https://openenergyplatform.org/).
-To use this tool with the OEP API you need to be signed up to the OEP since
-you need to provide an API-Token. 
+### Restrictions
 
-If you want to upload OEM that was officially reviewed you must clone the
-OEP data-preprocessing repository on [GitHub](https://github.com/OpenEnergyPlatform/data-preprocessing).
-The data-review folder contains all of the successfully reviewed OEM files.
+To use this tool with the OEP API you need to be signed up to the OEP since
+you need to provide an API-Token.
 
-For security reasons, tables can only be created in existing 
+For security reasons, tables can only be created in existing
 schemas and just in the schemas "model_draft" and "sandbox".
 
-Keep in mind the current state is not fully tested. The code is
-still quit error prone f.e. the postgres types (column datatype) are not fully 
+Keep in mind that f.e. the postgres types (column datatype) are not fully
 supported by the [oedialct](https://pypi.org/project/oedialect/) - work in progress.
 
-### Terminal/CLI-Application
-Step-by-Step: 
-0. pip and python have to be installed and setup on your machine
-1. Create env from requirements.txt, and activate
-2. Put the metadata file in the folder metadata or put your own folder in this 
-    directory
-3. execute the following in a terminal:
-```
-pipx install oem2orm
-oem2orm
-Enter metadata folder name:
-...
-```
-4. Provide credentials and folder name in prompt
-5. The table will be created 
-
-### Import as Module
-
-You can simply import this module in your Python script.py like this:
-
-```python
-from oem2orm import oep_oedialect_oem2orm as oem2orm
-```
-
-Now just call the functions provided in oem2orm like this:
-
-Recommended execution order:
-- Setup the logger
-```python
-oem2orm.setup_logger()
-```
-
-- Setup the Database API connection as Namedtuple storing the SQLAlchemy engine and metadata:
-```python
-db = oem2orm.setup_db_connection()
-```
-
-- Provide the oem files in a folder (in the current directory).
-- Pass the folder name to the function:
-```python
-metadata_folder = oem2orm.select_oem_dir(oem_folder_name="folder_name")
-```
-
-- Setup a SQLAlchemy ORM including all data-model in the provided oem files:
-```python
-orm = oem2orm.collect_ordered_tables_from_oem(db, metadata_folder)
-```
-
-- Create the tables on the Database:
-```python
-oem2orm.create_tables(db, orm)
-```
-
-- Delete all tables that have been created (all tables available in sa.metadata)
-```python
-oem2orm.delete_tables(db, orm)
-```
-
-## Docs:
+## Docs
 
 ### Database connection
+
 We use a global namedtuple called "DB" To store the sqlalchemy connection objects engine and metadata.
 The namedtuple is available wen import oem2orm in a script. To establish the namedtuple use the function
-setup_db_connection(). Now you can use DB.engine or DB.metadata.
+setup_db_connection(). Now you can use DB.engine or DB.metadata. In the background the connection is established
+using oedialect and the http API of the oeplatform website.
 
 ### oem2orm generator
 
-#### Supported datatypes
+The table objects (ORM) are generated on the fly from an oemetadata.json file. [oemetadata](https://github.com/OpenEnergyPlatform/oemetadata) is a metadata specification of the Open Energy Family. It includes about 50 fields that can be used to provide metadata for tabular data resources.
+A subset of these fields are grouped in the key "resources" ([see out example](https://github.com/OpenEnergyPlatform/oemetadata/blob/develop/metadata/v160/example.json#L237-L388)) in the metadata. These fields describe the schema of
+the data table (like table name, columns,  data types & table relations).
+
+The method oem2orm provides to create data tables on the OEP. It is especially useful if you attempt to automate the table creation and already use python or already have a oemetadata file available. The alternatives are:
+
+1. [manually describing](https://openenergyplatform.github.io/academy/tutorials/01_api/02_api_upload/#create-table) the table object in JSON and then use the oep HTTP API directly to create a table.  
+2. Use the [User Interface of the oeplatform website](https://openenergyplatform.org/dataedit/wizard/) to create a table and upload data.
+
+### Oemetadata format
+
+[Specification for the oemetadata](https://github.com/OpenEnergyPlatform/oemetadata)
+
+#### Oemetadata validation
+
+The oemetadata specification is integrated into the open energy platform using a tool called [omi (metadata integration)](https://github.com/OpenEnergyPlatform/omi). OMI provides functionality to run validation checks on the metadata up to the oemetadata version 1.6.0. oem2orm also provides a minimal oep compliance check that mocks the checks that are run on the oep website once the metadata is uploaded to a table.
+
+#### Supported column data types
+
+Currently oem2orm supports
+
+        "bigint"
+        "int":
+        "integer"
+        "varchar"
+        "json"
+        "text"
+        "timestamp"
+        "interval"
+        "string"
+        "float"
+        "boolean"
+        "date"
+        "hstore"
+        "decimal"
+        "numeric"
+        "double precision"
 
 #### Spatial Types
-We create columns with spatial datatypes using Geoalchemy2. 
+
+    "geometry point": Geometry("POINT",  spatial_index=False),
+    "geom": Geometry("GEOMETRY",  spatial_index=False),
+    "geometry": Geometry("GEOMETRY",  spatial_index=False),
+
+We create columns with spatial datatypes using Geoalchemy2.
 
 ## Database support
+
+We only tested this tool with PostgreSQL & sqlalchemy version 1.3
```

### Comparing `oem2orm-0.3.3/oem2orm/main.py` & `oem2orm-0.4.0/oem2orm/main.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,32 +1,35 @@
-
 import click
 import pathlib
 
 from oem2orm import oep_oedialect_oem2orm
 
 
 @click.group()
 def cli():
     pass
 
 
 @cli.command()
-@click.argument('metadata-folder', type=click.Path(exists=True))
+@click.argument("metadata-folder", type=click.Path(exists=True))
 def create_tables(metadata_folder):
     db = oep_oedialect_oem2orm.setup_db_connection()
     folder = pathlib.Path.cwd() / metadata_folder
     tables = oep_oedialect_oem2orm.collect_tables_from_oem(db, folder)
     oep_oedialect_oem2orm.create_tables(db, tables)
+    if len(tables) == 1:
+        # Upload metadata for single table
+        metadata = oep_oedialect_oem2orm.mdToDict(metadata_folder)
+        oep_oedialect_oem2orm.api_updateMdOnTable(metadata)
 
 
 @cli.command()
-@click.argument('metadata-folder', type=click.Path(exists=True))
+@click.argument("metadata-folder", type=click.Path(exists=True))
 def delete_tables(metadata_folder):
     db = oep_oedialect_oem2orm.setup_db_connection()
     folder = pathlib.Path.cwd() / metadata_folder
     tables = oep_oedialect_oem2orm.collect_tables_from_oem(db, folder)
     oep_oedialect_oem2orm.delete_tables(db, tables)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     cli()
```

### Comparing `oem2orm-0.3.3/oem2orm/oep_compliance.py` & `oem2orm-0.4.0/oem2orm/oep_compliance.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 Module for all functionality regarding the compliance of the integrated standards and 
 requirments from other oefamily software modules like omi.
 
 - check if the metadata will pass oep's metadata check that is performed before the saves the metadata.
 
 
 """
+
 import logging
 import pathlib
 import json
 
 from omi.dialects.oep.parser import ParserException
 from omi.structure import Compilable
 
@@ -20,14 +21,15 @@
 
 # instances of metadata parsers / compilers, order of priority
 METADATA_PARSERS = [OEP_V_1_5_Dialect(), OEP_V_1_4_Dialect()]
 METADATA_COMPILERS = [OEP_V_1_5_Dialect(), OEP_V_1_4_Dialect(), JSONCompiler()]
 
 logger = logging.getLogger()
 
+
 def read_input_json(file_path: pathlib.Path = "tests/data/metadata_v15.json"):
     with open(file_path, "r", encoding="utf-8") as f:
         jsn = json.load(f)
 
     return jsn
 
 
@@ -119,15 +121,17 @@
 # ----------- USE Cecks and Validation ------
 # Make use of omis validation to mock the
 # oemetadata check that is performed on the
 # OEP for ech metadata upload
 # -------------------------------------------
 
 
-def run_metadata_checks(oemetadata: dict = None, oemetadata_path: str = None,  check_jsonschema: bool = False):
+def run_metadata_checks(
+    oemetadata: dict = None, oemetadata_path: str = None, check_jsonschema: bool = False
+):
     """
     Runs metadata checks includes:
         - basic oep compliant check - tested by using omi's parsing and compiling
 
         Optional - included:
         - jsonschema valdiation
 
@@ -161,27 +165,31 @@
 
     if check_jsonschema:
         logger.info("Check if metadata is valid against the jsonschema.")
         parser_validation = JSONParser()
         schema = parser_validation.get_schema_by_metadata_version(metadata=metadata)
         result = parser_validation.is_valid(inp=metadata, schema=schema)
         if result is False:
-            result = result, parser_validation.validate(metadata=metadata, save_report=True)
-        
+            result = result, parser_validation.validate(
+                metadata=metadata, save_report=True
+            )
+
         return result
-            
+
 
 if __name__ == "__main__":
     correct_v15_test_data = "tests/data/metadata_v15.json"
     false_v15_test_data = "tests/data/bad_metadata_v15.json"
     v14_test_data = "tests/data/metadata_v14.json"
 
     meta = read_input_json(file_path=correct_v15_test_data)
     print("Check v15 metadata from file!")
-    result = run_metadata_checks(oemetadata_path=correct_v15_test_data, check_jsonschema=True)
+    result = run_metadata_checks(
+        oemetadata_path=correct_v15_test_data, check_jsonschema=True
+    )
     print("Check v15 metadata from object!")
     run_metadata_checks(oemetadata=meta)
 
     print("Check v14 metadata!")
     meta = read_input_json(file_path=correct_v15_test_data)
 
     # print("test expected error case: false usage")
```

### Comparing `oem2orm-0.3.3/oem2orm/oep_oedialect_oem2orm.py` & `oem2orm-0.4.0/oem2orm/oep_oedialect_oem2orm.py`

 * *Files 2% similar despite different names*

```diff
@@ -105,25 +105,29 @@
     :param db: API
     :param tables: SQLAlchemy ORM objects (automatically retrieved from OEM json strings)
     :return: none
     """
     for table in tables:
         logging.info(f"Working on table: {table}")
         if not db.engine.dialect.has_schema(db.engine, table.schema):
-            error_msg = f'The provided database schema: "{table.schema}" does not exist. Please use an existing ' \
-                        f'schema from the `name` column from: {OEP_URL}/dataedit/schemas'
+            error_msg = (
+                f'The provided database schema: "{table.schema}" does not exist. Please use an existing '
+                f"schema from the `name` column from: {OEP_URL}/dataedit/schemas"
+            )
             logging.info(error_msg)
             raise DatabaseError(error_msg)
         else:
             if not db.engine.dialect.has_table(db.engine, table.name, table.schema):
                 try:
                     table.create(checkfirst=True)
                     logging.info(f"Created table {table.name}")
                 except oedialect.engine.ConnectionException as ce:
-                    error_msg = f'Error when uploading table "{table.name}". Reason: {ce}.'
+                    error_msg = (
+                        f'Error when uploading table "{table.name}". Reason: {ce}.'
+                    )
                     logging.error(error_msg)
                     raise DatabaseError(error_msg) from ce
                 except sa.exc.ProgrammingError as pe:
                     error_msg = f'Table "{table.name}" already exists.'
                     logging.error(error_msg)
                     raise DatabaseError(error_msg) from pe
 
@@ -221,15 +225,16 @@
                     primary_key=field["name"] in primary_keys,
                     comment=field["description"],
                 )
             else:
                 column = sa.Column(
                     field["name"],
                     column_type,
-                    primary_key=field["name"] in primary_keys,
+                    primary_key=field["name"]
+                    in primary_keys,  # TODO: Should be fixed, see https://github.com/OpenEnergyPlatform/oedialect/issues/43
                     comment=field["description"],
                 )
             columns.append(column)
 
         if check_oep_api_schema_whitelist(schema):
             tables.append(
                 sa.Table(
```

### Comparing `oem2orm-0.3.3/oem2orm/postgresql_types.py` & `oem2orm-0.4.0/oem2orm/postgresql_types.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __copyright__ = "Reiner Lemoine Institut"
-__license__   = "GNU Affero General Public License Version 3 (AGPL-3.0)"
-__url__       = "https://github.com/openego/data_processing/blob/master/LICENSE"
-__author__    = "henhuy"
+__license__ = "GNU Affero General Public License Version 3 (AGPL-3.0)"
+__url__ = "https://github.com/openego/data_processing/blob/master/LICENSE"
+__author__ = "henhuy"
 
 import sqlalchemy as sa
 import sqlalchemy.dialects.postgresql as psql
 from geoalchemy2 import Geometry
 from sqlalchemy.dialects.postgresql import DOUBLE_PRECISION, HSTORE
 
 
@@ -23,24 +23,21 @@
         "string": sa.String,
         "float": sa.FLOAT,
         "boolean": sa.Boolean,
         "date": sa.Date,
         "hstore": HSTORE,
         "decimal": sa.DECIMAL,
         "numeric": sa.NUMERIC,
-
         # Spatial types
-        "geometry point": Geometry("POINT",  spatial_index=False),
-        "geom": Geometry("GEOMETRY",  spatial_index=False),
-        "geometry": Geometry("GEOMETRY",  spatial_index=False),
-
+        "geometry point": Geometry("POINT", spatial_index=False),
+        "geom": Geometry("GEOMETRY", spatial_index=False),
+        "geometry": Geometry("GEOMETRY", spatial_index=False),
         # not support with oedialect
-        "double precision": psql.DOUBLE_PRECISION
+        "double precision": psql.DOUBLE_PRECISION,
         # "double precision array": sa.ARRAY("DOUBLE_PRECISION"),
-
     }
 
     def __getitem__(self, item):
         if item is None:
             raise ValueError("Field type is 'None'.")
         if item.split(" ")[-1] == "array":
             db_type = self.types[item[:-6]]
```

### Comparing `oem2orm-0.3.3/oem2orm.egg-info/PKG-INFO` & `oem2orm-0.4.0/oem2orm.egg-info/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,132 +1,116 @@
 Metadata-Version: 2.1
 Name: oem2orm
-Version: 0.3.3
+Version: 0.4.0
 Summary: SQLAlchemy module to generate ORM, read from data model (oedatamodel) in open-energy-metadata JSON format
 Home-page: https://github.com/OpenEnergyPlatform/oem2orm
 Author: henhuy, jh-RLI
 Author-email: Hendrik.Huyskens@rl-institut.de
 Project-URL: Bug Reports, https://github.com/OpenEnergyPlatform/oem2orm/issues
 Project-URL: Source, https://github.com/OpenEnergyPlatform/oem2orm/tree/develop/oem2orm
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
-Requires-Dist: sqlalchemy==1.3.14
-Requires-Dist: oedialect==1.1
+Requires-Dist: sqlalchemy==1.3.16
+Requires-Dist: oedialect==0.1.1
 Requires-Dist: requests
 Requires-Dist: jmespath
 Requires-Dist: omi
 Requires-Dist: click
 
-# OEM to ORM
+# oem 2 orm
 
-Create database tables (and schema) from oemetadata json file(s)
+Create database tables (and schema) from oemetadata json file(s). This tool is part of the open-energy-metadata (OEM) integration into the [OEP](https://openenergyplatform.org/).
 
-## Installation:
+## Installation
 
 You can install pacakge using standard python installation:
 `
 pip install oem2orm
 `
 
 or if you interested in CLI-version only you can install it using pipx (pipx must be installed):
 `
 pipx install oem2orm
 `
 see [Pipx-Documentation](https://pypa.github.io/pipx/) for further information.
 
+## Usage
 
-## Usage:
+Read the Restrictions section and have a look at our [tutorial](./tutorial/USAGE.md) section to get more information about the usage of oem2orm either as code module or CLI tool. The tutorials also provide information how to validate your oemetadata files.
 
-This tool is part of the open-energy-metadata (OEM) integration into the [OEP](https://openenergyplatform.org/).
-To use this tool with the OEP API you need to be signed up to the OEP since
-you need to provide an API-Token. 
+### Restrictions
 
-If you want to upload OEM that was officially reviewed you must clone the
-OEP data-preprocessing repository on [GitHub](https://github.com/OpenEnergyPlatform/data-preprocessing).
-The data-review folder contains all of the successfully reviewed OEM files.
+To use this tool with the OEP API you need to be signed up to the OEP since
+you need to provide an API-Token.
 
-For security reasons, tables can only be created in existing 
+For security reasons, tables can only be created in existing
 schemas and just in the schemas "model_draft" and "sandbox".
 
-Keep in mind the current state is not fully tested. The code is
-still quit error prone f.e. the postgres types (column datatype) are not fully 
+Keep in mind that f.e. the postgres types (column datatype) are not fully
 supported by the [oedialct](https://pypi.org/project/oedialect/) - work in progress.
 
-### Terminal/CLI-Application
-Step-by-Step: 
-0. pip and python have to be installed and setup on your machine
-1. Create env from requirements.txt, and activate
-2. Put the metadata file in the folder metadata or put your own folder in this 
-    directory
-3. execute the following in a terminal:
-```
-pipx install oem2orm
-oem2orm
-Enter metadata folder name:
-...
-```
-4. Provide credentials and folder name in prompt
-5. The table will be created 
-
-### Import as Module
-
-You can simply import this module in your Python script.py like this:
-
-```python
-from oem2orm import oep_oedialect_oem2orm as oem2orm
-```
-
-Now just call the functions provided in oem2orm like this:
-
-Recommended execution order:
-- Setup the logger
-```python
-oem2orm.setup_logger()
-```
-
-- Setup the Database API connection as Namedtuple storing the SQLAlchemy engine and metadata:
-```python
-db = oem2orm.setup_db_connection()
-```
-
-- Provide the oem files in a folder (in the current directory).
-- Pass the folder name to the function:
-```python
-metadata_folder = oem2orm.select_oem_dir(oem_folder_name="folder_name")
-```
-
-- Setup a SQLAlchemy ORM including all data-model in the provided oem files:
-```python
-orm = oem2orm.collect_ordered_tables_from_oem(db, metadata_folder)
-```
-
-- Create the tables on the Database:
-```python
-oem2orm.create_tables(db, orm)
-```
-
-- Delete all tables that have been created (all tables available in sa.metadata)
-```python
-oem2orm.delete_tables(db, orm)
-```
-
-## Docs:
+## Docs
 
 ### Database connection
+
 We use a global namedtuple called "DB" To store the sqlalchemy connection objects engine and metadata.
 The namedtuple is available wen import oem2orm in a script. To establish the namedtuple use the function
-setup_db_connection(). Now you can use DB.engine or DB.metadata.
+setup_db_connection(). Now you can use DB.engine or DB.metadata. In the background the connection is established
+using oedialect and the http API of the oeplatform website.
 
 ### oem2orm generator
 
-#### Supported datatypes
+The table objects (ORM) are generated on the fly from an oemetadata.json file. [oemetadata](https://github.com/OpenEnergyPlatform/oemetadata) is a metadata specification of the Open Energy Family. It includes about 50 fields that can be used to provide metadata for tabular data resources.
+A subset of these fields are grouped in the key "resources" ([see out example](https://github.com/OpenEnergyPlatform/oemetadata/blob/develop/metadata/v160/example.json#L237-L388)) in the metadata. These fields describe the schema of
+the data table (like table name, columns,  data types & table relations).
+
+The method oem2orm provides to create data tables on the OEP. It is especially useful if you attempt to automate the table creation and already use python or already have a oemetadata file available. The alternatives are:
+
+1. [manually describing](https://openenergyplatform.github.io/academy/tutorials/01_api/02_api_upload/#create-table) the table object in JSON and then use the oep HTTP API directly to create a table.  
+2. Use the [User Interface of the oeplatform website](https://openenergyplatform.org/dataedit/wizard/) to create a table and upload data.
+
+### Oemetadata format
+
+[Specification for the oemetadata](https://github.com/OpenEnergyPlatform/oemetadata)
+
+#### Oemetadata validation
+
+The oemetadata specification is integrated into the open energy platform using a tool called [omi (metadata integration)](https://github.com/OpenEnergyPlatform/omi). OMI provides functionality to run validation checks on the metadata up to the oemetadata version 1.6.0. oem2orm also provides a minimal oep compliance check that mocks the checks that are run on the oep website once the metadata is uploaded to a table.
+
+#### Supported column data types
+
+Currently oem2orm supports
+
+        "bigint"
+        "int":
+        "integer"
+        "varchar"
+        "json"
+        "text"
+        "timestamp"
+        "interval"
+        "string"
+        "float"
+        "boolean"
+        "date"
+        "hstore"
+        "decimal"
+        "numeric"
+        "double precision"
 
 #### Spatial Types
-We create columns with spatial datatypes using Geoalchemy2. 
+
+    "geometry point": Geometry("POINT",  spatial_index=False),
+    "geom": Geometry("GEOMETRY",  spatial_index=False),
+    "geometry": Geometry("GEOMETRY",  spatial_index=False),
+
+We create columns with spatial datatypes using Geoalchemy2.
 
 ## Database support
+
+We only tested this tool with PostgreSQL & sqlalchemy version 1.3
```

### Comparing `oem2orm-0.3.3/setup.py` & `oem2orm-0.4.0/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 here = path.abspath(path.dirname(__file__))
 
 with open(path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="oem2orm",
-    version="0.3.3",
+    version="0.4.0",
     author="henhuy, jh-RLI",
     author_email="Hendrik.Huyskens@rl-institut.de",
     description="SQLAlchemy module to generate ORM, read from data model (oedatamodel) in open-energy-metadata JSON format",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/OpenEnergyPlatform/oem2orm",
     packages=setuptools.find_packages(),
@@ -24,15 +24,15 @@
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: GNU Affero General Public License v3",
         "Operating System :: OS Independent",
     ],
     python_requires='>=3.6',
-    install_requires=['sqlalchemy==1.3.14', 'oedialect==1.1', 'requests', 'jmespath', 'omi', 'click'],  # Optional
+    install_requires=['sqlalchemy==1.3.16', 'oedialect==0.1.1', 'requests', 'jmespath', 'omi', 'click'],  # Optional
     project_urls={  # Optional
         'Bug Reports': 'https://github.com/OpenEnergyPlatform/oem2orm/issues',
         'Source': 'https://github.com/OpenEnergyPlatform/oem2orm/tree/develop/oem2orm',
     },
     entry_points={
         'console_scripts': ['oem2orm=oem2orm.main:cli'],
     }
```

