# Comparing `tmp/dagster-embedded-elt-0.23.1.tar.gz` & `tmp/dagster-embedded-elt-0.23.2rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dagster-embedded-elt-0.23.1.tar", last modified: Thu Apr 11 18:15:27 2024, max compression
+gzip compressed data, was "dagster-embedded-elt-0.23.2rc1.tar", last modified: Tue Apr 16 17:58:50 2024, max compression
```

## Comparing `dagster-embedded-elt-0.23.1.tar` & `dagster-embedded-elt-0.23.2rc1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:15:27.058513 dagster-embedded-elt-0.23.1/
--rw-r--r--   0 root         (0) root         (0)    11349 2024-04-11 18:04:20.000000 dagster-embedded-elt-0.23.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)       97 2024-04-11 18:04:20.000000 dagster-embedded-elt-0.23.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      744 2024-04-11 18:15:27.058513 dagster-embedded-elt-0.23.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      146 2024-04-11 18:04:20.000000 dagster-embedded-elt-0.23.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:15:27.034513 dagster-embedded-elt-0.23.1/dagster_embedded_elt/
--rw-r--r--   0 root         (0) root         (0)      163 2024-04-11 18:04:20.000000 dagster-embedded-elt-0.23.1/dagster_embedded_elt/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:15:27.038513 dagster-embedded-elt-0.23.1/dagster_embedded_elt/dlt/
--rw-r--r--   0 root         (0) root         (0)      270 2024-04-11 18:04:20.000000 dagster-embedded-elt-0.23.1/dagster_embedded_elt/dlt/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3768 2024-04-11 18:04:20.000000 dagster-embedded-elt-0.23.1/dagster_embedded_elt/dlt/asset_decorator.py
--rw-r--r--   0 root         (0) root         (0)      129 2024-04-11 18:04:20.000000 dagster-embedded-elt-0.23.1/dagster_embedded_elt/dlt/constants.py
--rw-r--r--   0 root         (0) root         (0)     5629 2024-04-11 18:04:20.000000 dagster-embedded-elt-0.23.1/dagster_embedded_elt/dlt/resource.py
--rw-r--r--   0 root         (0) root         (0)     1563 2024-04-11 18:04:20.000000 dagster-embedded-elt-0.23.1/dagster_embedded_elt/dlt/translator.py
--rw-r--r--   0 root         (0) root         (0)        8 2024-04-11 18:04:20.000000 dagster-embedded-elt-0.23.1/dagster_embedded_elt/py.typed
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:15:27.054513 dagster-embedded-elt-0.23.1/dagster_embedded_elt/sling/
--rw-r--r--   0 root         (0) root         (0)      718 2024-04-11 18:04:20.000000 dagster-embedded-elt-0.23.1/dagster_embedded_elt/sling/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4931 2024-04-11 18:04:20.000000 dagster-embedded-elt-0.23.1/dagster_embedded_elt/sling/asset_decorator.py
--rw-r--r--   0 root         (0) root         (0)     4162 2024-04-11 18:04:20.000000 dagster-embedded-elt-0.23.1/dagster_embedded_elt/sling/asset_defs.py
--rw-r--r--   0 root         (0) root         (0)     8087 2024-04-11 18:04:20.000000 dagster-embedded-elt-0.23.1/dagster_embedded_elt/sling/dagster_sling_translator.py
--rw-r--r--   0 root         (0) root         (0)    17477 2024-04-11 18:04:20.000000 dagster-embedded-elt-0.23.1/dagster_embedded_elt/sling/resources.py
--rw-r--r--   0 root         (0) root         (0)     1106 2024-04-11 18:04:20.000000 dagster-embedded-elt-0.23.1/dagster_embedded_elt/sling/sling_replication.py
--rw-r--r--   0 root         (0) root         (0)       23 2024-04-11 18:04:20.000000 dagster-embedded-elt-0.23.1/dagster_embedded_elt/version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-11 18:15:27.034513 dagster-embedded-elt-0.23.1/dagster_embedded_elt.egg-info/
--rw-r--r--   0 root         (0) root         (0)      744 2024-04-11 18:15:26.000000 dagster-embedded-elt-0.23.1/dagster_embedded_elt.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      886 2024-04-11 18:15:26.000000 dagster-embedded-elt-0.23.1/dagster_embedded_elt.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-11 18:15:26.000000 dagster-embedded-elt-0.23.1/dagster_embedded_elt.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-11 18:15:26.000000 dagster-embedded-elt-0.23.1/dagster_embedded_elt.egg-info/not-zip-safe
--rw-r--r--   0 root         (0) root         (0)       52 2024-04-11 18:15:26.000000 dagster-embedded-elt-0.23.1/dagster_embedded_elt.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       21 2024-04-11 18:15:26.000000 dagster-embedded-elt-0.23.1/dagster_embedded_elt.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)      124 2024-04-11 18:04:20.000000 dagster-embedded-elt-0.23.1/integration.yaml
--rw-r--r--   0 root         (0) root         (0)      167 2024-04-11 18:15:27.062513 dagster-embedded-elt-0.23.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1427 2024-04-11 18:04:20.000000 dagster-embedded-elt-0.23.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:58:50.968118 dagster-embedded-elt-0.23.2rc1/
+-rw-r--r--   0 root         (0) root         (0)    11349 2024-04-16 17:50:34.000000 dagster-embedded-elt-0.23.2rc1/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       97 2024-04-16 17:50:34.000000 dagster-embedded-elt-0.23.2rc1/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      747 2024-04-16 17:58:50.968118 dagster-embedded-elt-0.23.2rc1/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      146 2024-04-16 17:50:34.000000 dagster-embedded-elt-0.23.2rc1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:58:50.964118 dagster-embedded-elt-0.23.2rc1/dagster_embedded_elt/
+-rw-r--r--   0 root         (0) root         (0)      163 2024-04-16 17:50:34.000000 dagster-embedded-elt-0.23.2rc1/dagster_embedded_elt/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:58:50.968118 dagster-embedded-elt-0.23.2rc1/dagster_embedded_elt/dlt/
+-rw-r--r--   0 root         (0) root         (0)      270 2024-04-16 17:50:34.000000 dagster-embedded-elt-0.23.2rc1/dagster_embedded_elt/dlt/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3681 2024-04-16 17:50:34.000000 dagster-embedded-elt-0.23.2rc1/dagster_embedded_elt/dlt/asset_decorator.py
+-rw-r--r--   0 root         (0) root         (0)      129 2024-04-16 17:50:34.000000 dagster-embedded-elt-0.23.2rc1/dagster_embedded_elt/dlt/constants.py
+-rw-r--r--   0 root         (0) root         (0)     7024 2024-04-16 17:50:34.000000 dagster-embedded-elt-0.23.2rc1/dagster_embedded_elt/dlt/resource.py
+-rw-r--r--   0 root         (0) root         (0)     1563 2024-04-16 17:50:34.000000 dagster-embedded-elt-0.23.2rc1/dagster_embedded_elt/dlt/translator.py
+-rw-r--r--   0 root         (0) root         (0)        8 2024-04-16 17:50:34.000000 dagster-embedded-elt-0.23.2rc1/dagster_embedded_elt/py.typed
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:58:50.968118 dagster-embedded-elt-0.23.2rc1/dagster_embedded_elt/sling/
+-rw-r--r--   0 root         (0) root         (0)      718 2024-04-16 17:50:34.000000 dagster-embedded-elt-0.23.2rc1/dagster_embedded_elt/sling/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4738 2024-04-16 17:50:34.000000 dagster-embedded-elt-0.23.2rc1/dagster_embedded_elt/sling/asset_decorator.py
+-rw-r--r--   0 root         (0) root         (0)     4162 2024-04-16 17:50:34.000000 dagster-embedded-elt-0.23.2rc1/dagster_embedded_elt/sling/asset_defs.py
+-rw-r--r--   0 root         (0) root         (0)     8087 2024-04-16 17:50:34.000000 dagster-embedded-elt-0.23.2rc1/dagster_embedded_elt/sling/dagster_sling_translator.py
+-rw-r--r--   0 root         (0) root         (0)    17560 2024-04-16 17:50:34.000000 dagster-embedded-elt-0.23.2rc1/dagster_embedded_elt/sling/resources.py
+-rw-r--r--   0 root         (0) root         (0)     1106 2024-04-16 17:50:34.000000 dagster-embedded-elt-0.23.2rc1/dagster_embedded_elt/sling/sling_replication.py
+-rw-r--r--   0 root         (0) root         (0)       26 2024-04-16 17:50:34.000000 dagster-embedded-elt-0.23.2rc1/dagster_embedded_elt/version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-16 17:58:50.964118 dagster-embedded-elt-0.23.2rc1/dagster_embedded_elt.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      747 2024-04-16 17:58:50.000000 dagster-embedded-elt-0.23.2rc1/dagster_embedded_elt.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      886 2024-04-16 17:58:50.000000 dagster-embedded-elt-0.23.2rc1/dagster_embedded_elt.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-16 17:58:50.000000 dagster-embedded-elt-0.23.2rc1/dagster_embedded_elt.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-16 17:58:50.000000 dagster-embedded-elt-0.23.2rc1/dagster_embedded_elt.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)       55 2024-04-16 17:58:50.000000 dagster-embedded-elt-0.23.2rc1/dagster_embedded_elt.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       21 2024-04-16 17:58:50.000000 dagster-embedded-elt-0.23.2rc1/dagster_embedded_elt.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)      124 2024-04-16 17:50:34.000000 dagster-embedded-elt-0.23.2rc1/integration.yaml
+-rw-r--r--   0 root         (0) root         (0)      167 2024-04-16 17:58:50.972118 dagster-embedded-elt-0.23.2rc1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1430 2024-04-16 17:50:34.000000 dagster-embedded-elt-0.23.2rc1/setup.py
```

### Comparing `dagster-embedded-elt-0.23.1/LICENSE` & `dagster-embedded-elt-0.23.2rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `dagster-embedded-elt-0.23.1/PKG-INFO` & `dagster-embedded-elt-0.23.2rc1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-embedded-elt
-Version: 0.23.1
+Version: 0.23.2rc1
 Summary: Package for performing ETL/ELT tasks with Dagster.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-embedded-elt
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-embedded-elt-0.23.1/dagster_embedded_elt/dlt/asset_decorator.py` & `dagster-embedded-elt-0.23.2rc1/dagster_embedded_elt/dlt/asset_decorator.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Callable, Optional
+from typing import Any, Callable, Optional
 
 from dagster import (
     AssetsDefinition,
     AssetSpec,
     multi_asset,
 )
 from dlt.extract.source import DltSource
@@ -15,15 +15,15 @@
 def dlt_assets(
     *,
     dlt_source: DltSource,
     dlt_pipeline: Pipeline,
     name: Optional[str] = None,
     group_name: Optional[str] = None,
     dlt_dagster_translator: DagsterDltTranslator = DagsterDltTranslator(),
-) -> Callable[..., AssetsDefinition]:
+) -> Callable[[Callable[..., Any]], AssetsDefinition]:
     """Asset Factory for using data load tool (dlt).
 
     Args:
         dlt_source (DltSource): The DltSource to be ingested.
         dlt_pipeline (Pipeline): The dlt Pipeline defining the destination parameters.
         name (Optional[str], optional): The name of the op.
         group_name (Optional[str], optional): The name of the asset group.
@@ -72,30 +72,28 @@
                 name="github",
                 group_name="github",
             )
             def github_reactions_dagster_assets(context: AssetExecutionContext, dlt: DltDagsterResource):
                 yield from dlt.run(context=context)
 
     """
-
-    def inner(fn) -> AssetsDefinition:
-        specs = [
+    return multi_asset(
+        name=name,
+        group_name=group_name,
+        compute_kind="dlt",
+        can_subset=True,
+        specs=[
             AssetSpec(
                 key=dlt_dagster_translator.get_asset_key(dlt_source_resource),
                 deps=dlt_dagster_translator.get_deps_asset_keys(dlt_source_resource),
                 auto_materialize_policy=dlt_dagster_translator.get_auto_materialize_policy(
                     dlt_source_resource
                 ),
                 metadata={
                     META_KEY_SOURCE: dlt_source,
                     META_KEY_PIPELINE: dlt_pipeline,
                     META_KEY_TRANSLATOR: dlt_dagster_translator,
                 },
             )
             for dlt_source_resource in dlt_source.resources.values()
-        ]
-        assets_definition = multi_asset(
-            specs=specs, name=name, group_name=group_name, compute_kind="dlt", can_subset=True
-        )(fn)
-        return assets_definition
-
-    return inner
+        ],
+    )
```

### Comparing `dagster-embedded-elt-0.23.1/dagster_embedded_elt/dlt/resource.py` & `dagster-embedded-elt-0.23.2rc1/dagster_embedded_elt/dlt/resource.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import Any, Iterator, Mapping, Union
+from typing import Any, Iterator, Mapping, Optional, Union
 
 from dagster import (
     AssetExecutionContext,
     AssetMaterialization,
     ConfigurableResource,
     MaterializeResult,
     OpExecutionContext,
@@ -16,14 +16,18 @@
 
 from .constants import META_KEY_PIPELINE, META_KEY_SOURCE, META_KEY_TRANSLATOR
 from .translator import DagsterDltTranslator
 
 
 @experimental
 class DagsterDltResource(ConfigurableResource):
+    @classmethod
+    def _is_dagster_maintained(cls) -> bool:
+        return True
+
     def _cast_load_info_metadata(self, mapping: Mapping[Any, Any]) -> Mapping[Any, Any]:
         """Converts pendulum DateTime and Timezone values in a mapping to strings.
 
         Workaround for dagster._core.errors.DagsterInvalidMetadata: Could not resolve the metadata
         value for "jobs" to a known type. Value is not JSON serializable.
 
         Args:
@@ -91,35 +95,55 @@
 
         return base_metadata
 
     @public
     def run(
         self,
         context: Union[OpExecutionContext, AssetExecutionContext],
+        dlt_source: Optional[DltSource] = None,
+        dlt_pipeline: Optional[Pipeline] = None,
+        dagster_dlt_translator: Optional[DagsterDltTranslator] = None,
         **kwargs,
-    ) -> Iterator[Union[AssetMaterialization, MaterializeResult]]:
+    ) -> Iterator[Union[MaterializeResult, AssetMaterialization]]:
         """Runs the dlt pipeline with subset support.
 
         Args:
             context (Union[OpExecutionContext, AssetExecutionContext]): Asset or op execution context
+            dlt_source (Optional[DltSource]): optional dlt source if resource is used from an `@op`
+            dlt_pipeline (Optional[Pipeline]): optional dlt pipeline if resource is used from an `@op`
+            dagster_dlt_translator (Optional[DagsterDltTranslator]): optional dlt translator if resource is used from an `@op`
             **kwargs (dict[str, Any]): Keyword args passed to pipeline `run` method
 
         Returns:
-            Iterator[Union[AssetMaterialization, MaterializeResult]]: A generator of AssetMaterialization or MaterializeResult
+            Iterator[Union[MaterializeResult, AssetMaterialization]]: An iterator of MaterializeResult or AssetMaterialization
 
         """
-        metadata_by_key = context.assets_def.metadata_by_key
-        first_asset_metadata = next(iter(metadata_by_key.values()))
+        # This resource can be used in both `asset` and `op` definitions. In the context of an asset
+        # execution, we retrieve the dlt source, pipeline, and translator from the asset metadata.
+        # This allows us to provide the parameter _only_ in the `dlt_assets` decorator.
+        if isinstance(context, AssetExecutionContext):
+            metadata_by_key = context.assets_def.metadata_by_key
+            first_asset_metadata = next(iter(metadata_by_key.values()))
+
+            dlt_source = check.inst(first_asset_metadata.get(META_KEY_SOURCE), DltSource)
+            dlt_pipeline = check.inst(first_asset_metadata.get(META_KEY_PIPELINE), Pipeline)
+            dagster_dlt_translator = check.inst(
+                first_asset_metadata.get(META_KEY_TRANSLATOR), DagsterDltTranslator
+            )
 
-        dlt_source = check.inst(first_asset_metadata.get(META_KEY_SOURCE), DltSource)
-        dlt_pipeline = check.inst(first_asset_metadata.get(META_KEY_PIPELINE), Pipeline)
-        dagster_dlt_translator = check.inst(
-            first_asset_metadata.get(META_KEY_TRANSLATOR), DagsterDltTranslator
+        dlt_source = check.not_none(
+            dlt_source, "dlt_source is a required parameter in an op context"
+        )
+        dlt_pipeline = check.not_none(
+            dlt_pipeline, "dlt_pipeline is a required parameter in an op context"
         )
 
+        # Default to base translator if undefined
+        dagster_dlt_translator = dagster_dlt_translator or DagsterDltTranslator()
+
         asset_key_dlt_source_resource_mapping = {
             dagster_dlt_translator.get_asset_key(dlt_source_resource): dlt_source_resource
             for dlt_source_resource in dlt_source.resources.values()
         }
 
         # Filter sources by asset key sub-selection
         if context.is_subset:
@@ -137,14 +161,16 @@
                     for dlt_source_resource in asset_key_dlt_source_resource_mapping.values()
                     if dlt_source_resource
                 ]
             )
 
         load_info = dlt_pipeline.run(dlt_source, **kwargs)
 
+        has_asset_def: bool = bool(context and context.has_assets_def)
+
         for asset_key, dlt_source_resource in asset_key_dlt_source_resource_mapping.items():
             metadata = self.extract_resource_metadata(dlt_source_resource, load_info)
-            if isinstance(context, AssetExecutionContext):
+            if has_asset_def:
                 yield MaterializeResult(asset_key=asset_key, metadata=metadata)
 
             else:
                 yield AssetMaterialization(asset_key=asset_key, metadata=metadata)
```

### Comparing `dagster-embedded-elt-0.23.1/dagster_embedded_elt/dlt/translator.py` & `dagster-embedded-elt-0.23.2rc1/dagster_embedded_elt/dlt/translator.py`

 * *Files identical despite different names*

### Comparing `dagster-embedded-elt-0.23.1/dagster_embedded_elt/sling/__init__.py` & `dagster-embedded-elt-0.23.2rc1/dagster_embedded_elt/sling/__init__.py`

 * *Files identical despite different names*

### Comparing `dagster-embedded-elt-0.23.1/dagster_embedded_elt/sling/asset_decorator.py` & `dagster-embedded-elt-0.23.2rc1/dagster_embedded_elt/sling/asset_decorator.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,15 +30,15 @@
     *,
     replication_config: SlingReplicationParam,
     dagster_sling_translator: DagsterSlingTranslator = DagsterSlingTranslator(),
     name: Optional[str] = None,
     partitions_def: Optional[PartitionsDefinition] = None,
     backfill_policy: Optional[BackfillPolicy] = None,
     op_tags: Optional[Mapping[str, Any]] = None,
-) -> Callable[..., AssetsDefinition]:
+) -> Callable[[Callable[..., Any]], AssetsDefinition]:
     """Create a definition for how to materialize a set of Sling replication streams as Dagster assets, as
     described by a Sling replication config. This will create on Asset for every Sling target stream.
 
     A Sling Replication config is a configuration that maps sources to destinations. For the full
     spec and descriptions, see `Sling's Documentation <https://docs.slingdata.io/sling-cli/run/configuration>`_.
 
     Args:
@@ -76,42 +76,34 @@
             def my_assets(context, sling: SlingResource):
                 yield from sling.replicate(context=context)
     """
     replication_config = validate_replication(replication_config)
     streams = get_streams_from_replication(replication_config)
     code_version = non_secure_md5_hash_str(str(replication_config).encode())
 
-    specs: list[AssetSpec] = []
-    for stream in streams:
-        specs.append(
+    return multi_asset(
+        name=name,
+        compute_kind="sling",
+        partitions_def=partitions_def,
+        can_subset=False,
+        op_tags=op_tags,
+        backfill_policy=backfill_policy,
+        specs=[
             AssetSpec(
                 key=dagster_sling_translator.get_asset_key(stream),
                 deps=dagster_sling_translator.get_deps_asset_key(stream),
                 description=dagster_sling_translator.get_description(stream),
-                metadata={  # type: ignore
+                metadata={
                     **dagster_sling_translator.get_metadata(stream),
                     METADATA_KEY_TRANSLATOR: dagster_sling_translator,
                     METADATA_KEY_REPLICATION_CONFIG: replication_config,
                 },
                 group_name=dagster_sling_translator.get_group_name(stream),
                 freshness_policy=dagster_sling_translator.get_freshness_policy(stream),
                 auto_materialize_policy=dagster_sling_translator.get_auto_materialize_policy(
                     stream
                 ),
                 code_version=code_version,
             )
-        )
-
-    def inner(fn) -> AssetsDefinition:
-        asset_definition = multi_asset(
-            name=name,
-            compute_kind="sling",
-            partitions_def=partitions_def,
-            can_subset=False,
-            op_tags=op_tags,
-            backfill_policy=backfill_policy,
-            specs=specs,
-        )(fn)
-
-        return asset_definition
-
-    return inner
+            for stream in streams
+        ],
+    )
```

### Comparing `dagster-embedded-elt-0.23.1/dagster_embedded_elt/sling/asset_defs.py` & `dagster-embedded-elt-0.23.2rc1/dagster_embedded_elt/sling/asset_defs.py`

 * *Files identical despite different names*

### Comparing `dagster-embedded-elt-0.23.1/dagster_embedded_elt/sling/dagster_sling_translator.py` & `dagster-embedded-elt-0.23.2rc1/dagster_embedded_elt/sling/dagster_sling_translator.py`

 * *Files identical despite different names*

### Comparing `dagster-embedded-elt-0.23.1/dagster_embedded_elt/sling/resources.py` & `dagster-embedded-elt-0.23.2rc1/dagster_embedded_elt/sling/resources.py`

 * *Files 1% similar despite different names*

```diff
@@ -224,14 +224,18 @@
     """
 
     source_connection: Optional[SlingSourceConnection] = None
     target_connection: Optional[SlingTargetConnection] = None
     connections: List[SlingConnectionResource] = []
     _stdout: List[str] = []
 
+    @classmethod
+    def _is_dagster_maintained(cls) -> bool:
+        return True
+
     def _clean_connection_dict(self, d: Dict[str, Any]) -> Dict[str, Any]:
         d = _process_env_vars(d)
         if d["connection_string"]:
             d["url"] = d["connection_string"]
         if "connection_string" in d:
             del d["connection_string"]
         return d
```

### Comparing `dagster-embedded-elt-0.23.1/dagster_embedded_elt/sling/sling_replication.py` & `dagster-embedded-elt-0.23.2rc1/dagster_embedded_elt/sling/sling_replication.py`

 * *Files identical despite different names*

### Comparing `dagster-embedded-elt-0.23.1/dagster_embedded_elt.egg-info/PKG-INFO` & `dagster-embedded-elt-0.23.2rc1/dagster_embedded_elt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dagster-embedded-elt
-Version: 0.23.1
+Version: 0.23.2rc1
 Summary: Package for performing ETL/ELT tasks with Dagster.
 Home-page: https://github.com/dagster-io/dagster/tree/master/python_modules/libraries/dagster-embedded-elt
 Author: Dagster Labs
 Author-email: hello@dagsterlabs.com
 License: Apache-2.0
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

### Comparing `dagster-embedded-elt-0.23.1/dagster_embedded_elt.egg-info/SOURCES.txt` & `dagster-embedded-elt-0.23.2rc1/dagster_embedded_elt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dagster-embedded-elt-0.23.1/setup.py` & `dagster-embedded-elt-0.23.2rc1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,15 +30,15 @@
         "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3.12",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: OS Independent",
     ],
     packages=find_packages(exclude=["dagster_embedded_elt_tests*"]),
     python_requires=">=3.8,<3.13",
-    install_requires=["dagster==1.7.1", "sling>=1.1.5", "dlt>=0.4"],
+    install_requires=["dagster==1.7.2rc1", "sling>=1.1.5", "dlt>=0.4"],
     zip_safe=False,
     extras_require={
         "test": [
             "duckdb",
         ]
     },
 )
```

