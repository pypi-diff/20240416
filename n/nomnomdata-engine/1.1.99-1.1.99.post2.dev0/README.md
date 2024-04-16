# Comparing `tmp/nomnomdata_engine-1.1.99.tar.gz` & `tmp/nomnomdata_engine-1.1.99.post2.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nomnomdata_engine-1.1.99.tar", max compression
+gzip compressed data, was "nomnomdata_engine-1.1.99.post2.dev0.tar", max compression
```

## Comparing `nomnomdata_engine-1.1.99.tar` & `nomnomdata_engine-1.1.99.post2.dev0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      702 2024-01-18 17:02:14.081686 nomnomdata_engine-1.1.99/LICENSE
--rw-r--r--   0        0        0       37 2024-01-18 17:02:14.081686 nomnomdata_engine-1.1.99/README.md
--rw-r--r--   0        0        0      432 2024-01-18 17:02:14.081686 nomnomdata_engine-1.1.99/nomnomdata/engine/__init__.py
--rw-r--r--   0        0        0    10061 2024-01-18 17:02:14.081686 nomnomdata_engine-1.1.99/nomnomdata/engine/components.py
--rw-r--r--   0        0        0    84349 2024-01-18 17:02:14.081686 nomnomdata_engine-1.1.99/nomnomdata/engine/connections.py
--rw-r--r--   0        0        0     5598 2024-01-18 17:02:14.081686 nomnomdata_engine-1.1.99/nomnomdata/engine/encoders.py
--rw-r--r--   0        0        0    14368 2024-01-18 17:02:14.081686 nomnomdata_engine-1.1.99/nomnomdata/engine/engine.py
--rw-r--r--   0        0        0      516 2024-01-18 17:02:14.081686 nomnomdata_engine-1.1.99/nomnomdata/engine/errors.py
--rw-r--r--   0        0        0      290 2024-01-18 17:02:14.082686 nomnomdata_engine-1.1.99/nomnomdata/engine/globals.py
--rw-r--r--   0        0        0     2448 2024-01-18 17:02:14.082686 nomnomdata_engine-1.1.99/nomnomdata/engine/logging.py
--rw-r--r--   0        0        0    11023 2024-01-18 17:02:14.082686 nomnomdata_engine-1.1.99/nomnomdata/engine/nominode.py
--rw-r--r--   0        0        0     9574 2024-01-18 17:02:14.082686 nomnomdata_engine-1.1.99/nomnomdata/engine/parameters.py
--rw-r--r--   0        0        0    35388 2024-01-18 17:02:14.082686 nomnomdata_engine-1.1.99/nomnomdata/engine/shared_configs.py
--rw-r--r--   0        0        0     4357 2024-01-18 17:02:14.082686 nomnomdata_engine-1.1.99/nomnomdata/engine/testing.py
--rw-r--r--   0        0        0      162 2024-01-18 17:02:14.082686 nomnomdata_engine-1.1.99/nomnomdata/engine/util.py
--rw-r--r--   0        0        0     1291 2024-01-18 17:02:27.961661 nomnomdata_engine-1.1.99/pyproject.toml
--rw-r--r--   0        0        0     1131 1970-01-01 00:00:00.000000 nomnomdata_engine-1.1.99/PKG-INFO
+-rw-r--r--   0        0        0      702 2024-01-29 16:56:42.880492 nomnomdata_engine-1.1.99.post2.dev0/LICENSE
+-rw-r--r--   0        0        0       37 2024-01-29 16:56:42.880492 nomnomdata_engine-1.1.99.post2.dev0/README.md
+-rw-r--r--   0        0        0      432 2024-01-29 16:56:42.880492 nomnomdata_engine-1.1.99.post2.dev0/nomnomdata/engine/__init__.py
+-rw-r--r--   0        0        0    10061 2024-01-29 16:56:42.880492 nomnomdata_engine-1.1.99.post2.dev0/nomnomdata/engine/components.py
+-rw-r--r--   0        0        0    84349 2024-01-29 16:56:42.881492 nomnomdata_engine-1.1.99.post2.dev0/nomnomdata/engine/connections.py
+-rw-r--r--   0        0        0     5598 2024-01-29 16:56:42.881492 nomnomdata_engine-1.1.99.post2.dev0/nomnomdata/engine/encoders.py
+-rw-r--r--   0        0        0    14368 2024-01-29 16:56:42.881492 nomnomdata_engine-1.1.99.post2.dev0/nomnomdata/engine/engine.py
+-rw-r--r--   0        0        0      516 2024-01-29 16:56:42.881492 nomnomdata_engine-1.1.99.post2.dev0/nomnomdata/engine/errors.py
+-rw-r--r--   0        0        0      290 2024-01-29 16:56:42.881492 nomnomdata_engine-1.1.99.post2.dev0/nomnomdata/engine/globals.py
+-rw-r--r--   0        0        0     2448 2024-01-29 16:56:42.881492 nomnomdata_engine-1.1.99.post2.dev0/nomnomdata/engine/logging.py
+-rw-r--r--   0        0        0    11023 2024-01-29 16:56:42.881492 nomnomdata_engine-1.1.99.post2.dev0/nomnomdata/engine/nominode.py
+-rw-r--r--   0        0        0     9574 2024-01-29 16:56:42.881492 nomnomdata_engine-1.1.99.post2.dev0/nomnomdata/engine/parameters.py
+-rw-r--r--   0        0        0    38444 2024-01-29 16:56:42.881492 nomnomdata_engine-1.1.99.post2.dev0/nomnomdata/engine/shared_configs.py
+-rw-r--r--   0        0        0     4357 2024-01-29 16:56:42.882492 nomnomdata_engine-1.1.99.post2.dev0/nomnomdata/engine/testing.py
+-rw-r--r--   0        0        0      162 2024-01-29 16:56:42.882492 nomnomdata_engine-1.1.99.post2.dev0/nomnomdata/engine/util.py
+-rw-r--r--   0        0        0     1302 2024-01-29 16:56:56.671311 nomnomdata_engine-1.1.99.post2.dev0/pyproject.toml
+-rw-r--r--   0        0        0     1142 1970-01-01 00:00:00.000000 nomnomdata_engine-1.1.99.post2.dev0/PKG-INFO
```

### Comparing `nomnomdata_engine-1.1.99/LICENSE` & `nomnomdata_engine-1.1.99.post2.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `nomnomdata_engine-1.1.99/nomnomdata/engine/components.py` & `nomnomdata_engine-1.1.99.post2.dev0/nomnomdata/engine/components.py`

 * *Files identical despite different names*

### Comparing `nomnomdata_engine-1.1.99/nomnomdata/engine/connections.py` & `nomnomdata_engine-1.1.99.post2.dev0/nomnomdata/engine/connections.py`

 * *Files identical despite different names*

### Comparing `nomnomdata_engine-1.1.99/nomnomdata/engine/encoders.py` & `nomnomdata_engine-1.1.99.post2.dev0/nomnomdata/engine/encoders.py`

 * *Files identical despite different names*

### Comparing `nomnomdata_engine-1.1.99/nomnomdata/engine/engine.py` & `nomnomdata_engine-1.1.99.post2.dev0/nomnomdata/engine/engine.py`

 * *Files identical despite different names*

### Comparing `nomnomdata_engine-1.1.99/nomnomdata/engine/errors.py` & `nomnomdata_engine-1.1.99.post2.dev0/nomnomdata/engine/errors.py`

 * *Files identical despite different names*

### Comparing `nomnomdata_engine-1.1.99/nomnomdata/engine/logging.py` & `nomnomdata_engine-1.1.99.post2.dev0/nomnomdata/engine/logging.py`

 * *Files identical despite different names*

### Comparing `nomnomdata_engine-1.1.99/nomnomdata/engine/nominode.py` & `nomnomdata_engine-1.1.99.post2.dev0/nomnomdata/engine/nominode.py`

 * *Files identical despite different names*

### Comparing `nomnomdata_engine-1.1.99/nomnomdata/engine/parameters.py` & `nomnomdata_engine-1.1.99.post2.dev0/nomnomdata/engine/parameters.py`

 * *Files identical despite different names*

### Comparing `nomnomdata_engine-1.1.99/nomnomdata/engine/shared_configs.py` & `nomnomdata_engine-1.1.99.post2.dev0/nomnomdata/engine/shared_configs.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,87 @@
 from nomnomdata.engine.components import Parameter, ParameterGroup, SharedConfig
 from nomnomdata.engine.parameters import Boolean, Code, Enum, Int, Nested, String
 
+ApiToBigQueryParameters = SharedConfig(
+    shared_config_type_uuid="APIRS-BIGQRY",
+    alias="API Response to BigQuery Load Options",
+    description="Information needed when loading data from an API response into a BigQuery table.",
+    categories=["Google", "BigQuery", "API"],
+    parameter_groups=[
+        ParameterGroup(
+            Parameter(
+                name="fields_mapping_autodetect",
+                display_name="Autodetect Column Mappings",
+                description="Automatically create the BigQuery table description.",
+                type=Boolean(),
+                required=False,
+                default=True,
+                help_header_id="Autodetect Column Mappings",
+            ),
+            Parameter(
+                name="add_default_fields",
+                display_name="Add Nom Nom Columns",
+                description="Add the nnd_updated and nnd_created columns to the BigQuery table.",
+                type=Boolean(),
+                required=False,
+                default=True,
+                help_header_id="Add Nom Nom Columns",
+            ),
+            Parameter(
+                name="column_parameters",
+                display_name="Column Parameters",
+                description="Details about each column within the tables.",
+                required=False,
+                many=True,
+                type=Nested(
+                    Parameter(
+                        name="api_field_path",
+                        display_name="API Property",
+                        description="Specify the API property name or JSON path.",
+                        type=String(),
+                        required=True,
+                    ),
+                    Parameter(
+                        name="bigquery_row",
+                        display_name="BigQuery Column Name",
+                        description="Specify the name of the column.",
+                        type=String(max=128),
+                        required=True,
+                    ),
+                    Parameter(
+                        name="bigquery_row_type",
+                        display_name="BigQuery Column Type",
+                        description="Specify the type of the column.",
+                        type=Enum(
+                            choices=[
+                                "STRING",
+                                "BIGNUMERIC",
+                                "BOOL",
+                                "BYTES",
+                                "DATE",
+                                "DATETIME",
+                                "FLOAT64",
+                                "GEOGRAPHY",
+                                "INT64",
+                                "JSON",
+                                "NUMERIC",
+                                "STRING",
+                                "TIME",
+                                "TIMESTAMP",
+                            ]
+                        ),
+                        required=True,
+                    ),
+                ),
+            ),
+        ),
+    ],
+)
+
+
 AzureBlobFileToDatabase = SharedConfig(
     shared_config_type_uuid="AZRBL-DBSHR",
     alias="Azure Blob Storage to Relational Database Load Options",
     description="Information needed when loading data from files stored on Azure Blob Storage into a relational database.",
     categories=[
         "Azure",
         "Blob Storage",
```

### Comparing `nomnomdata_engine-1.1.99/nomnomdata/engine/testing.py` & `nomnomdata_engine-1.1.99.post2.dev0/nomnomdata/engine/testing.py`

 * *Files identical despite different names*

### Comparing `nomnomdata_engine-1.1.99/pyproject.toml` & `nomnomdata_engine-1.1.99.post2.dev0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 license = "LGPL-3.0-only"
 name = "nomnomdata-engine"
 packages = [
   {include = "nomnomdata"},
 ]
 readme = "README.md"
 repository = "https://gitlab.com/nomnomdata/tools/nomnomdata-engine"
-version = "1.1.99"
+version = "1.1.99.post2.dev0"
 
 [tool.poetry.dependencies]
 dunamai = "^1.1.0"
 httmock = "^1.3.0"
 nomnomdata-cli = "^0.1.7"
 python = "^3.7"
 pyyaml = "^5.3.1"
```

### Comparing `nomnomdata_engine-1.1.99/PKG-INFO` & `nomnomdata_engine-1.1.99.post2.dev0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nomnomdata-engine
-Version: 1.1.99
+Version: 1.1.99.post2.dev0
 Summary: Package containing tooling for developing nominode engines
 Home-page: https://gitlab.com/nomnomdata/tools/nomnomdata-engine
 License: LGPL-3.0-only
 Author: Nom Nom Data Inc
 Author-email: info@nomnomdata.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: GNU Lesser General Public License v3 (LGPLv3)
```

