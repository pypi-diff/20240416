# Comparing `tmp/dagster-airbyte-0.23.1.tar.gz` & `tmp/dagster-airbyte-0.23.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-airbyte-0.23.1.tar", last modified: Thu Apr 11 18:16:06 2024, max compression
+gzip compressed data, was "dagster-airbyte-0.23.2rc1.tar", last modified: Tue Apr 16 17:55:55 2024, max compression
```

## Comparing `dagster-airbyte-0.23.1.tar` & `dagster-airbyte-0.23.2rc1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:16:06.686781 dagster-airbyte-0.23.1/
--rw-r--r--   0 root         (0) root         (0)    11349 2024-04-11 18:04:20.000000 dagster-airbyte-0.23.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       67 2024-04-11 18:04:20.000000 dagster-airbyte-0.23.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      753 2024-04-11 18:16:06.686781 dagster-airbyte-0.23.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      131 2024-04-11 18:04:20.000000 dagster-airbyte-0.23.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:16:06.674781 dagster-airbyte-0.23.1/dagster_airbyte/
--rw-r--r--   0 root         (0) root         (0)     1215 2024-04-11 18:04:20.000000 dagster-airbyte-0.23.1/dagster_airbyte/__init__.py
--rw-r--r--   0 root         (0) root         (0)    47799 2024-04-11 18:04:20.000000 dagster-airbyte-0.23.1/dagster_airbyte/asset_defs.py
--rw-r--r--   0 root         (0) root         (0)      425 2024-04-11 18:04:20.000000 dagster-airbyte-0.23.1/dagster_airbyte/cli.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:16:06.678781 dagster-airbyte-0.23.1/dagster_airbyte/managed/
--rw-r--r--   0 root         (0) root         (0)      423 2024-04-11 18:04:20.000000 dagster-airbyte-0.23.1/dagster_airbyte/managed/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:16:06.682781 dagster-airbyte-0.23.1/dagster_airbyte/managed/generated/
--rw-r--r--   0 root         (0) root         (0)       76 2024-04-11 18:04:20.000000 dagster-airbyte-0.23.1/dagster_airbyte/managed/generated/__init__.py
--rw-r--r--   0 root         (0) root         (0)   119751 2024-04-11 18:04:20.000000 dagster-airbyte-0.23.1/dagster_airbyte/managed/generated/destinations.py
--rw-r--r--   0 root         (0) root         (0)   282784 2024-04-11 18:04:20.000000 dagster-airbyte-0.23.1/dagster_airbyte/managed/generated/sources.py
--rw-r--r--   0 root         (0) root         (0)    34862 2024-04-11 18:04:20.000000 dagster-airbyte-0.23.1/dagster_airbyte/managed/reconciliation.py
--rw-r--r--   0 root         (0) root         (0)    14588 2024-04-11 18:04:20.000000 dagster-airbyte-0.23.1/dagster_airbyte/managed/types.py
--rw-r--r--   0 root         (0) root         (0)     4128 2024-04-11 18:04:20.000000 dagster-airbyte-0.23.1/dagster_airbyte/ops.py
--rw-r--r--   0 root         (0) root         (0)        8 2024-04-11 18:04:20.000000 dagster-airbyte-0.23.1/dagster_airbyte/py.typed
--rw-r--r--   0 root         (0) root         (0)    27040 2024-04-11 18:04:20.000000 dagster-airbyte-0.23.1/dagster_airbyte/resources.py
--rw-r--r--   0 root         (0) root         (0)     1425 2024-04-11 18:04:20.000000 dagster-airbyte-0.23.1/dagster_airbyte/types.py
--rw-r--r--   0 root         (0) root         (0)     2823 2024-04-11 18:04:20.000000 dagster-airbyte-0.23.1/dagster_airbyte/utils.py
--rw-r--r--   0 root         (0) root         (0)       23 2024-04-11 18:04:20.000000 dagster-airbyte-0.23.1/dagster_airbyte/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:16:06.674781 dagster-airbyte-0.23.1/dagster_airbyte.egg-info/
--rw-r--r--   0 root         (0) root         (0)      753 2024-04-11 18:16:06.000000 dagster-airbyte-0.23.1/dagster_airbyte.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      809 2024-04-11 18:16:06.000000 dagster-airbyte-0.23.1/dagster_airbyte.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-11 18:16:06.000000 dagster-airbyte-0.23.1/dagster_airbyte.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       61 2024-04-11 18:16:06.000000 dagster-airbyte-0.23.1/dagster_airbyte.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-11 18:16:06.000000 dagster-airbyte-0.23.1/dagster_airbyte.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       90 2024-04-11 18:16:06.000000 dagster-airbyte-0.23.1/dagster_airbyte.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       16 2024-04-11 18:16:06.000000 dagster-airbyte-0.23.1/dagster_airbyte.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      162 2024-04-11 18:16:06.690781 dagster-airbyte-0.23.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1636 2024-04-11 18:04:20.000000 dagster-airbyte-0.23.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:55:55.551754 dagster-airbyte-0.23.2rc1/
+-rw-r--r--   0 root         (0) root         (0)    11349 2024-04-16 17:50:34.000000 dagster-airbyte-0.23.2rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       67 2024-04-16 17:50:34.000000 dagster-airbyte-0.23.2rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      756 2024-04-16 17:55:55.551754 dagster-airbyte-0.23.2rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      131 2024-04-16 17:50:34.000000 dagster-airbyte-0.23.2rc1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:55:55.543754 dagster-airbyte-0.23.2rc1/dagster_airbyte/
+-rw-r--r--   0 root         (0) root         (0)     1215 2024-04-16 17:50:34.000000 dagster-airbyte-0.23.2rc1/dagster_airbyte/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    48304 2024-04-16 17:50:34.000000 dagster-airbyte-0.23.2rc1/dagster_airbyte/asset_defs.py
+-rw-r--r--   0 root         (0) root         (0)      425 2024-04-16 17:50:34.000000 dagster-airbyte-0.23.2rc1/dagster_airbyte/cli.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:55:55.547754 dagster-airbyte-0.23.2rc1/dagster_airbyte/managed/
+-rw-r--r--   0 root         (0) root         (0)      423 2024-04-16 17:50:34.000000 dagster-airbyte-0.23.2rc1/dagster_airbyte/managed/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:55:55.547754 dagster-airbyte-0.23.2rc1/dagster_airbyte/managed/generated/
+-rw-r--r--   0 root         (0) root         (0)       76 2024-04-16 17:50:34.000000 dagster-airbyte-0.23.2rc1/dagster_airbyte/managed/generated/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   119751 2024-04-16 17:50:34.000000 dagster-airbyte-0.23.2rc1/dagster_airbyte/managed/generated/destinations.py
+-rw-r--r--   0 root         (0) root         (0)   282784 2024-04-16 17:50:34.000000 dagster-airbyte-0.23.2rc1/dagster_airbyte/managed/generated/sources.py
+-rw-r--r--   0 root         (0) root         (0)    34862 2024-04-16 17:50:34.000000 dagster-airbyte-0.23.2rc1/dagster_airbyte/managed/reconciliation.py
+-rw-r--r--   0 root         (0) root         (0)    14588 2024-04-16 17:50:34.000000 dagster-airbyte-0.23.2rc1/dagster_airbyte/managed/types.py
+-rw-r--r--   0 root         (0) root         (0)     4128 2024-04-16 17:50:34.000000 dagster-airbyte-0.23.2rc1/dagster_airbyte/ops.py
+-rw-r--r--   0 root         (0) root         (0)        8 2024-04-16 17:50:34.000000 dagster-airbyte-0.23.2rc1/dagster_airbyte/py.typed
+-rw-r--r--   0 root         (0) root         (0)    27040 2024-04-16 17:50:34.000000 dagster-airbyte-0.23.2rc1/dagster_airbyte/resources.py
+-rw-r--r--   0 root         (0) root         (0)     1425 2024-04-16 17:50:34.000000 dagster-airbyte-0.23.2rc1/dagster_airbyte/types.py
+-rw-r--r--   0 root         (0) root         (0)     2823 2024-04-16 17:50:34.000000 dagster-airbyte-0.23.2rc1/dagster_airbyte/utils.py
+-rw-r--r--   0 root         (0) root         (0)       26 2024-04-16 17:50:34.000000 dagster-airbyte-0.23.2rc1/dagster_airbyte/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:55:55.543754 dagster-airbyte-0.23.2rc1/dagster_airbyte.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      756 2024-04-16 17:55:55.000000 dagster-airbyte-0.23.2rc1/dagster_airbyte.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      809 2024-04-16 17:55:55.000000 dagster-airbyte-0.23.2rc1/dagster_airbyte.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-16 17:55:55.000000 dagster-airbyte-0.23.2rc1/dagster_airbyte.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       61 2024-04-16 17:55:55.000000 dagster-airbyte-0.23.2rc1/dagster_airbyte.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-16 17:55:55.000000 dagster-airbyte-0.23.2rc1/dagster_airbyte.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       96 2024-04-16 17:55:55.000000 dagster-airbyte-0.23.2rc1/dagster_airbyte.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       16 2024-04-16 17:55:55.000000 dagster-airbyte-0.23.2rc1/dagster_airbyte.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      162 2024-04-16 17:55:55.551754 dagster-airbyte-0.23.2rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1642 2024-04-16 17:50:34.000000 dagster-airbyte-0.23.2rc1/setup.py
```

### Comparing `dagster-airbyte-0.23.1/LICENSE` & `dagster-airbyte-0.23.2rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-airbyte-0.23.1/PKG-INFO` & `dagster-airbyte-0.23.2rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-airbyte
-Version: 0.23.1
+Version: 0.23.2rc1
 Summary: Package for integrating Airbyte with Dagster.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-airbyte
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-airbyte-0.23.1/dagster_airbyte/__init__.py` & `dagster-airbyte-0.23.2rc1/dagster_airbyte/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-airbyte-0.23.1/dagster_airbyte/asset_defs.py` & `dagster-airbyte-0.23.2rc1/dagster_airbyte/asset_defs.py`

 * *Files 1% similar despite different names*

```diff
@@ -176,14 +176,19 @@
                 io_manager_key=io_manager_key,
                 freshness_policy=(
                     assets_defn_meta.freshness_policies_by_output_name.get(k)
                     if assets_defn_meta.freshness_policies_by_output_name
                     else None
                 ),
                 dagster_type=Nothing,
+                auto_materialize_policy=assets_defn_meta.auto_materialize_policies_by_output_name.get(
+                    k, None
+                )
+                if assets_defn_meta.auto_materialize_policies_by_output_name
+                else None,
             )
             for k, v in (assets_defn_meta.keys_by_output_name or {}).items()
         },
         internal_asset_deps={
             k: set(v) for k, v in (assets_defn_meta.internal_asset_deps or {}).items()
         },
         compute_kind="airbyte",
@@ -223,14 +228,15 @@
     group_name: Optional[str] = None,
     normalization_tables: Optional[Mapping[str, Set[str]]] = None,
     deps: Optional[Iterable[Union[CoercibleToAssetKey, AssetsDefinition, SourceAsset]]] = None,
     upstream_assets: Optional[Set[AssetKey]] = None,
     schema_by_table_name: Optional[Mapping[str, TableSchema]] = None,
     freshness_policy: Optional[FreshnessPolicy] = None,
     stream_to_asset_map: Optional[Mapping[str, str]] = None,
+    auto_materialize_policy: Optional[AutoMaterializePolicy] = None,
 ) -> Sequence[AssetsDefinition]:
     """Builds a set of assets representing the tables created by an Airbyte sync operation.
 
     Args:
         connection_id (str): The Airbyte Connection ID that this op will sync. You can retrieve this
             value from the "Connections" tab of a given connector in the Airbyte UI.
         destination_tables (List[str]): The names of the tables that you want to be represented
@@ -243,14 +249,15 @@
             If left blank, assets will have a key of `AssetKey([table_name])`.
         deps (Optional[Sequence[Union[AssetsDefinition, SourceAsset, str, AssetKey]]]):
             A list of assets to add as sources.
         upstream_assets (Optional[Set[AssetKey]]): Deprecated, use deps instead. A list of assets to add as sources.
         freshness_policy (Optional[FreshnessPolicy]): A freshness policy to apply to the assets
         stream_to_asset_map (Optional[Mapping[str, str]]): A mapping of an Airbyte stream name to a Dagster asset.
             This allows the use of the "prefix" setting in Airbyte with special characters that aren't valid asset names.
+        auto_materialize_policy (Optional[AutoMaterializePolicy]): An auto materialization policy to apply to the assets.
     """
     if upstream_assets is not None and deps is not None:
         raise DagsterInvalidDefinitionError(
             "Cannot specify both deps and upstream_assets to build_airbyte_assets. Use only deps"
             " instead."
         )
 
@@ -266,14 +273,15 @@
             key=AssetKey([*asset_key_prefix, table]),
             metadata=(
                 {"table_schema": MetadataValue.table_schema(schema_by_table_name[table])}
                 if schema_by_table_name
                 else None
             ),
             freshness_policy=freshness_policy,
+            auto_materialize_policy=auto_materialize_policy,
         )
         for table in tables
     }
 
     internal_deps = {}
 
     # If normalization tables are specified, we need to add a dependency from the destination table
```

### Comparing `dagster-airbyte-0.23.1/dagster_airbyte/managed/generated/destinations.py` & `dagster-airbyte-0.23.2rc1/dagster_airbyte/managed/generated/destinations.py`

 * *Files identical despite different names*

### Comparing `dagster-airbyte-0.23.1/dagster_airbyte/managed/generated/sources.py` & `dagster-airbyte-0.23.2rc1/dagster_airbyte/managed/generated/sources.py`

 * *Files identical despite different names*

### Comparing `dagster-airbyte-0.23.1/dagster_airbyte/managed/reconciliation.py` & `dagster-airbyte-0.23.2rc1/dagster_airbyte/managed/reconciliation.py`

 * *Files identical despite different names*

### Comparing `dagster-airbyte-0.23.1/dagster_airbyte/managed/types.py` & `dagster-airbyte-0.23.2rc1/dagster_airbyte/managed/types.py`

 * *Files identical despite different names*

### Comparing `dagster-airbyte-0.23.1/dagster_airbyte/ops.py` & `dagster-airbyte-0.23.2rc1/dagster_airbyte/ops.py`

 * *Files identical despite different names*

### Comparing `dagster-airbyte-0.23.1/dagster_airbyte/resources.py` & `dagster-airbyte-0.23.2rc1/dagster_airbyte/resources.py`

 * *Files identical despite different names*

### Comparing `dagster-airbyte-0.23.1/dagster_airbyte/types.py` & `dagster-airbyte-0.23.2rc1/dagster_airbyte/types.py`

 * *Files identical despite different names*

### Comparing `dagster-airbyte-0.23.1/dagster_airbyte/utils.py` & `dagster-airbyte-0.23.2rc1/dagster_airbyte/utils.py`

 * *Files identical despite different names*

### Comparing `dagster-airbyte-0.23.1/dagster_airbyte.egg-info/PKG-INFO` & `dagster-airbyte-0.23.2rc1/dagster_airbyte.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-airbyte
-Version: 0.23.1
+Version: 0.23.2rc1
 Summary: Package for integrating Airbyte with Dagster.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-airbyte
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-airbyte-0.23.1/dagster_airbyte.egg-info/SOURCES.txt` & `dagster-airbyte-0.23.2rc1/dagster_airbyte.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dagster-airbyte-0.23.1/setup.py` & `dagster-airbyte-0.23.2rc1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,25 +33,25 @@
         "Programming Language :: Python :: 3.12",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_airbyte_tests*"]),
     python_requires=">=3.8,<3.13",
     install_requires=[
-        "dagster==1.7.1",
+        "dagster==1.7.2rc1",
         "requests",
     ],
     zip_safe=False,
     entry_points={
         "console_scripts": [
             "dagster-airbyte = dagster_airbyte.cli:main",
         ]
     },
     extras_require={
         "test": [
             "requests-mock",
         ],
         "managed": [
-            "dagster-managed-elements==0.23.1",
+            "dagster-managed-elements==0.23.2rc1",
         ],
     },
 )
```

