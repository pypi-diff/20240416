# Comparing `tmp/infrahub_sync-0.3.0.tar.gz` & `tmp/infrahub_sync-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "infrahub_sync-0.3.0.tar", max compression
+gzip compressed data, was "infrahub_sync-0.4.0.tar", max compression
```

## Comparing `infrahub_sync-0.3.0.tar` & `infrahub_sync-0.4.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0       35 2024-03-11 10:21:33.711524 infrahub_sync-0.3.0/README.md
--rw-r--r--   0        0        0     1633 2024-03-19 08:22:57.220489 infrahub_sync-0.3.0/infrahub-sync/infrahub_sync/__init__.py
--rw-r--r--   0        0        0     7119 2024-03-19 08:22:57.220628 infrahub_sync-0.3.0/infrahub-sync/infrahub_sync/adapters/infrahub.py
--rw-r--r--   0        0        0     5370 2024-03-19 08:22:57.220765 infrahub_sync-0.3.0/infrahub-sync/infrahub_sync/adapters/nautobot.py
--rw-r--r--   0        0        0     5040 2024-03-19 08:22:57.220890 infrahub_sync-0.3.0/infrahub-sync/infrahub_sync/adapters/netbox.py
--rw-r--r--   0        0        0     4572 2024-03-19 08:22:57.221015 infrahub_sync-0.3.0/infrahub-sync/infrahub_sync/cli.py
--rw-r--r--   0        0        0     4569 2024-03-19 10:14:03.026557 infrahub_sync-0.3.0/infrahub-sync/infrahub_sync/generator/__init__.py
--rw-r--r--   0        0        0      787 2024-03-19 08:22:57.222558 infrahub_sync-0.3.0/infrahub-sync/infrahub_sync/generator/templates/diffsync_adapter.j2
--rw-r--r--   0        0        0     1318 2024-03-19 08:22:57.222646 infrahub_sync-0.3.0/infrahub-sync/infrahub_sync/generator/templates/diffsync_models.j2
--rw-r--r--   0        0        0      430 2024-03-11 10:21:33.715397 infrahub_sync-0.3.0/infrahub-sync/infrahub_sync/generator/utils.py
--rw-r--r--   0        0        0     6143 2024-03-19 14:17:52.145501 infrahub_sync-0.3.0/infrahub-sync/infrahub_sync/utils.py
--rw-r--r--   0        0        0     2774 2024-03-19 08:22:57.224329 infrahub_sync-0.3.0/potenda/potenda/__init__.py
--rw-r--r--   0        0        0     5910 2024-03-19 13:15:21.700871 infrahub_sync-0.3.0/pyproject.toml
--rw-r--r--   0        0        0      904 1970-01-01 00:00:00.000000 infrahub_sync-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     3345 2024-04-08 18:55:47.929487 infrahub_sync-0.4.0/README.md
+-rw-r--r--   0        0        0     1976 2024-04-16 12:15:57.981671 infrahub_sync-0.4.0/infrahub-sync/infrahub_sync/__init__.py
+-rw-r--r--   0        0        0     7854 2024-04-16 12:27:48.410912 infrahub_sync-0.4.0/infrahub-sync/infrahub_sync/adapters/infrahub.py
+-rw-r--r--   0        0        0     5522 2024-04-16 12:27:48.413371 infrahub_sync-0.4.0/infrahub-sync/infrahub_sync/adapters/nautobot.py
+-rw-r--r--   0        0        0     5191 2024-04-16 12:27:48.412118 infrahub_sync-0.4.0/infrahub-sync/infrahub_sync/adapters/netbox.py
+-rw-r--r--   0        0        0     4588 2024-04-16 12:15:57.982607 infrahub_sync-0.4.0/infrahub-sync/infrahub_sync/cli.py
+-rw-r--r--   0        0        0     4776 2024-04-16 12:15:57.982827 infrahub_sync-0.4.0/infrahub-sync/infrahub_sync/generator/__init__.py
+-rw-r--r--   0        0        0      787 2024-03-27 08:24:41.653251 infrahub_sync-0.4.0/infrahub-sync/infrahub_sync/generator/templates/diffsync_adapter.j2
+-rw-r--r--   0        0        0     1343 2024-04-16 12:15:57.982957 infrahub_sync-0.4.0/infrahub-sync/infrahub_sync/generator/templates/diffsync_models.j2
+-rw-r--r--   0        0        0      430 2024-03-27 08:24:41.653393 infrahub_sync-0.4.0/infrahub-sync/infrahub_sync/generator/utils.py
+-rw-r--r--   0        0        0     6143 2024-04-16 12:27:48.408566 infrahub_sync-0.4.0/infrahub-sync/infrahub_sync/utils.py
+-rw-r--r--   0        0        0     2774 2024-03-27 08:24:41.654066 infrahub_sync-0.4.0/potenda/potenda/__init__.py
+-rw-r--r--   0        0        0     5941 2024-04-16 12:46:11.189487 infrahub_sync-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0     4162 1970-01-01 00:00:00.000000 infrahub_sync-0.4.0/PKG-INFO
```

### Comparing `infrahub_sync-0.3.0/infrahub-sync/infrahub_sync/__init__.py` & `infrahub_sync-0.4.0/infrahub-sync/infrahub_sync/__init__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,43 +1,46 @@
 from typing import Any, Dict, List, Optional
 
-from pydantic import BaseModel
+try:
+    from pydantic import v1 as pydantic  # type: ignore[attr-defined]
+except ImportError:
+    import pydantic  # type: ignore[no-redef]
 
 
-class SchemaMappingField(BaseModel):
+class SchemaMappingField(pydantic.BaseModel):
     name: str
-    mapping: Optional[str]
-    static: Optional[Any]
-    reference: Optional[str]
+    mapping: Optional[str] = pydantic.Field(default=None)
+    static: Optional[Any] = pydantic.Field(default=None)
+    reference: Optional[str] = pydantic.Field(default=None)
 
 
-class SchemaMappingModel(BaseModel):
+class SchemaMappingModel(pydantic.BaseModel):
     name: str
     mapping: str
-    identifiers: Optional[List[str]]
-    fields: List[SchemaMappingField]
+    identifiers: Optional[List[str]] = pydantic.Field(default=None)
+    fields: List[SchemaMappingField] = []
 
 
-class SyncAdapter(BaseModel):
+class SyncAdapter(pydantic.BaseModel):
     name: str
-    settings: Optional[Dict[str, Any]]
+    settings: Optional[Dict[str, Any]] = {}
 
 
-class SyncStore(BaseModel):
+class SyncStore(pydantic.BaseModel):
     type: str
-    settings: Optional[Dict[str, Any]]
+    settings: Optional[Dict[str, Any]] = {}
 
 
-class SyncConfig(BaseModel):
+class SyncConfig(pydantic.BaseModel):
     name: str
-    store: Optional[SyncStore]
+    store: Optional[SyncStore] = []
     source: SyncAdapter
     destination: SyncAdapter
-    order: List[str]
-    schema_mapping: List[SchemaMappingModel]
+    order: List[str] = pydantic.Field(default_factory=list)
+    schema_mapping: List[SchemaMappingModel] = []
 
 
 class SyncInstance(SyncConfig):
     directory: str
 
 
 class DiffSyncMixin:
```

### Comparing `infrahub_sync-0.3.0/infrahub-sync/infrahub_sync/adapters/infrahub.py` & `infrahub_sync-0.4.0/infrahub-sync/infrahub_sync/adapters/infrahub.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,24 +1,29 @@
 import copy
-from typing import Any, Dict, Mapping
+from typing import Any, Dict, Mapping, Optional
 
 from infrahub_sdk import (
     Config,
     InfrahubClientSync,
     InfrahubNodeSync,
     NodeSchema,
     NodeStoreSync,
 )
 from infrahub_sdk.exceptions import NodeNotFoundError
 from infrahub_sdk.utils import compare_lists
 
-from diffsync import DiffSync, DiffSyncModel
+from diffsync import DiffSyncModel
 from infrahub_sync import DiffSyncMixin, DiffSyncModelMixin, SyncAdapter, SyncConfig
 from infrahub_sync.generator import has_field
 
+try:
+    from diffsync import Adapter as DiffSyncAdapter  # type: ignore[attr-defined]
+except ImportError:
+    from diffsync import DiffSync as DiffSyncAdapter  # type: ignore[no-redef]
+
 
 def update_node(node: InfrahubNodeSync, attrs: dict):
     for attr_name, attr_value in attrs.items():
         if attr_name in node._schema.attribute_names:
             attr = getattr(node, attr_name)
             attr.value = attr_value
 
@@ -39,15 +44,15 @@
 
                     for new_id in new_only:
                         attr.add(new_id)
 
     return node
 
 
-class InfrahubAdapter(DiffSyncMixin, DiffSync):
+class InfrahubAdapter(DiffSyncMixin, DiffSyncAdapter):
     type = "Infrahub"
 
     def __init__(self, *args, target: str, adapter: SyncAdapter, config: SyncConfig, branch: str = None, **kwargs):
         super().__init__(*args, **kwargs)
         self.target = target
         self.config = config
         if branch:
@@ -143,29 +148,47 @@
                     data[key] = new_values
 
     return data
 
 
 class InfrahubModel(DiffSyncModelMixin, DiffSyncModel):
     @classmethod
-    def create(cls, diffsync, ids: Mapping[Any, Any], attrs: Mapping[Any, Any]):
-        schema = diffsync.client.schema.get(kind=cls.__name__)
+    def create(
+        cls,
+        ids: Mapping[Any, Any],
+        attrs: Mapping[Any, Any],
+        diffsync: Optional[DiffSyncAdapter] = None,
+        adapter: Optional[DiffSyncAdapter] = None,
+    ):
+        context = adapter if adapter is not None else diffsync
+
+        if context is None:
+            raise ValueError("Either 'diffsync' or 'adapter' must be provided.")
 
-        data = diffsync_to_infrahub(ids=ids, attrs=attrs, schema=schema, store=diffsync.client.store)
+        schema = context.client.schema.get(kind=cls.__name__)
+        data = diffsync_to_infrahub(ids=ids, attrs=attrs, schema=schema, store=context.client.store)
         unique_id = cls(**ids, **attrs).get_unique_id()
         source_id = None
-        if diffsync.account:
-            source_id = diffsync.account.id
-        create_data = diffsync.client.schema.generate_payload_create(
+        if context.account:
+            source_id = context.account.id
+        create_data = context.client.schema.generate_payload_create(
             schema=schema, data=data, source=source_id, is_protected=True
         )
-        node = diffsync.client.create(kind=cls.__name__, data=create_data)
+        node = context.client.create(kind=cls.__name__, data=create_data)
         node.save(allow_upsert=True)
-        diffsync.client.store.set(key=unique_id, node=node)
-        return super().create(diffsync, ids=ids, attrs=attrs)
+        context.client.store.set(key=unique_id, node=node)
+
+        if diffsync:
+            return super().create(diffsync, ids=ids, attrs=attrs)
+        if adapter:
+            return super().create(adapter, ids=ids, attrs=attrs)
+        if not (diffsync or adapter):
+            raise ValueError("Either 'diffsync' or 'adapter' must be provided.")
+
+        return None
 
     def update(self, attrs):
         node = self.diffsync.client.get(id=self.local_id, kind=self.__class__.__name__)
 
         node = update_node(node=node, attrs=attrs)
         node.save(allow_upsert=True)
```

### Comparing `infrahub_sync-0.3.0/infrahub-sync/infrahub_sync/adapters/nautobot.py` & `infrahub_sync-0.4.0/infrahub-sync/infrahub_sync/adapters/nautobot.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,23 +2,29 @@
 
 # pylint: disable=R0801
 import os
 from typing import TYPE_CHECKING, Any, Dict
 
 import pynautobot
 
-from diffsync import DiffSync, DiffSyncModel
+from diffsync import DiffSyncModel
 from infrahub_sync import (
     DiffSyncMixin,
     DiffSyncModelMixin,
     SchemaMappingModel,
     SyncAdapter,
     SyncConfig,
 )
 
+try:
+    from diffsync import Adapter as DiffSync  # type: ignore[attr-defined]
+except ImportError:
+    from diffsync import DiffSync  # type: ignore[no-redef]
+
+
 if TYPE_CHECKING:
     from pynautobot.core.response import Record as NautobotRecord
 
 
 def get_value(obj, name: str):
     """Query a value in dot notation recursively on a NautobotRecord"""
     if "." not in name:
```

### Comparing `infrahub_sync-0.3.0/infrahub-sync/infrahub_sync/adapters/netbox.py` & `infrahub_sync-0.4.0/infrahub-sync/infrahub_sync/adapters/netbox.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,23 +2,28 @@
 
 # pylint: disable=R0801
 import os
 from typing import TYPE_CHECKING, Any, Dict
 
 import pynetbox
 
-from diffsync import DiffSync, DiffSyncModel
+from diffsync import DiffSyncModel
 from infrahub_sync import (
     DiffSyncMixin,
     DiffSyncModelMixin,
     SchemaMappingModel,
     SyncAdapter,
     SyncConfig,
 )
 
+try:
+    from diffsync import Adapter as DiffSync  # type: ignore[attr-defined]
+except ImportError:
+    from diffsync import DiffSync  # type: ignore[no-redef]
+
 if TYPE_CHECKING:
     from pynetbox.core.response import Record as NetboxRecord
 
 
 def get_value(obj, name: str):
     """Query a value in dot notation recursively on a NetboxRecord"""
     if "." not in name:
```

### Comparing `infrahub_sync-0.3.0/infrahub-sync/infrahub_sync/cli.py` & `infrahub_sync-0.4.0/infrahub-sync/infrahub_sync/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 @app.command(name="sync")
 def sync_cmd(
     name: str = typer.Option(default=None, help="Name of the sync to use"),
     config_file: str = typer.Option(default=None, help="File path to the sync configuration YAML file"),
     directory: str = typer.Option(None, help="Base directory to search for sync configurations"),
     branch: str = typer.Option(default=None, help="Branch to use for the sync."),
     diff: bool = typer.Option(
-        default=True, help="Print the differences between the source and the destinatio before syncing"
+        default=True, help="Print the differences between the source and the destination before syncing"
     ),
     show_progress: bool = typer.Option(default=True, help="Show a progress bar during syncing"),
 ):
     """Synchronize the data between source and the destination systems for a given project or configuration file."""
     if sum([bool(name), bool(config_file)]) != 1:
         print_error_and_abort("Please specify exactly one of 'name' or 'config_file'.")
 
@@ -84,15 +84,15 @@
         ptd.sync(diff=mydiff)
         end_synctime = timer()
         console.print(f"Sync: Completed in {end_synctime - start_synctime} sec")
     else:
         console.print("No diffence found. Nothing to sync")
 
 
-@app.command()
+@app.command(name="generate")
 def generate(
     name: str = typer.Option(default=None, help="Name of the sync to use"),
     config_file: str = typer.Option(default=None, help="File path to the sync configuration YAML file"),
     directory: str = typer.Option(None, help="Base directory to search for sync configurations"),
 ):
     """Generate all the python files for a given sync based on the configuration."""
```

### Comparing `infrahub_sync-0.3.0/infrahub-sync/infrahub_sync/generator/__init__.py` & `infrahub_sync-0.4.0/infrahub-sync/infrahub_sync/generator/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -101,23 +101,30 @@
     return "{" + ", ".join(children_list) + "}"
 
 
 def get_kind(item: Union[RelationshipSchema, AttributeSchema]) -> str:
     kind = "str"
     if isinstance(item, AttributeSchema):
         kind = ATTRIBUTE_KIND_MAP.get(item.kind, "str")
-        if item.optional or item.default_value is not None:
+        if item.optional:
             kind = f"Optional[{kind}]"
+            if item.default_value is not None:
+                kind += f" = {item.default_value}"
+            else:
+                kind += " = None"
 
     elif isinstance(item, RelationshipSchema) and item.cardinality == "one":
         if item.optional:
-            kind = f"Optional[{kind}]"
+            kind = f"Optional[{kind}] = None"
 
     elif isinstance(item, RelationshipSchema) and item.cardinality == "many":
-        kind = "List[str] = []"
+        kind = "List[str]"
+        if item.optional:
+            kind = f"Optional[{kind}]"
+        kind += " = []"
 
     return kind
 
 
 def has_children(node: NodeSchema, config: SyncConfig) -> bool:
     if get_children(config=config, node=node):
         return True
```

### Comparing `infrahub_sync-0.3.0/infrahub-sync/infrahub_sync/generator/templates/diffsync_adapter.j2` & `infrahub_sync-0.4.0/infrahub-sync/infrahub_sync/generator/templates/diffsync_adapter.j2`

 * *Files identical despite different names*

### Comparing `infrahub_sync-0.3.0/infrahub-sync/infrahub_sync/generator/templates/diffsync_models.j2` & `infrahub_sync-0.4.0/infrahub-sync/infrahub_sync/generator/templates/diffsync_models.j2`

 * *Files 10% similar despite different names*

```diff
@@ -11,24 +11,24 @@
 {%-   if node | get_identifiers(config) and config | has_node(node.kind) %}
 
 class {{ nodekind }}({{ adapter.name.title() }}Model):
     _modelname = "{{ node.kind }}"
     _identifiers = {{ node | get_identifiers(config) | list_to_set }}
     _attributes = {{ node | get_attributes(config) | list_to_set }}
 {%- if node | has_children(config) %}
-    _children = {{ node | get_children(config) }}
+    _children: List[str] = {{ node | get_children(config) }}
 {%- endif -%}
 
 {%-    for attr in node.attributes -%}
 {%-      if config | has_field(node.kind, attr.name) %}
     {{ attr.name }}: {{ attr | get_kind }}
 {%-       endif -%}
 {%-    endfor %}
 {%-    for rel in node.relationships -%}
 {%-      if config | has_field(node.kind, rel.name) %}
     {{ rel.name }}: {{ rel | get_kind }}
 {%-       endif -%}
 {%-    endfor %}
-    local_id: Optional[str]
-    local_data: Optional[Any]
+    local_id: Optional[str] = None
+    local_data: Optional[Any] = None
 {%-   endif -%}
 {% endfor %}
```

### Comparing `infrahub_sync-0.3.0/infrahub-sync/infrahub_sync/utils.py` & `infrahub_sync-0.4.0/infrahub-sync/infrahub_sync/utils.py`

 * *Files identical despite different names*

### Comparing `infrahub_sync-0.3.0/potenda/potenda/__init__.py` & `infrahub_sync-0.4.0/potenda/potenda/__init__.py`

 * *Files identical despite different names*

### Comparing `infrahub_sync-0.3.0/pyproject.toml` & `infrahub_sync-0.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "infrahub-sync"
-version = "0.3.0"
+version = "0.4.0"
 description = ""
 authors = ["OpsMill <contact@opsmill.com>"]
 readme = "README.md"
 license = "Apache-2.0"
 homepage = "https://opsmill.io"
 repository = "https://opsmill.io"
 documentation = "https://opsmill.io"
@@ -18,32 +18,31 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: 3.12",
 ]
 
 [tool.poetry.dependencies]
-python = ">=3.8, < 3.13"
+python = ">=3.9, < 3.13"
 infrahub-sdk = {version = "^0,>=0.9.1", extras = ["all"]}
 structlog = "^22.3.0"
-diffsync = "^1.10.0"
+diffsync = { version = ">=1.10,<2.0 || >=2.0", extras = ["redis"] }
 
 [tool.poetry.group.dev.dependencies]
 pytest = "*"
 pytest-clarity = "^1.0.1"
 pytest-cov = "^4.0.0"
 pytest-httpx = "*"
 yamllint = "*"
 pylint = "*"
 mypy = "*"
 ipython = "*"
 pytest-asyncio = "*"
 requests = "*"
 pre-commit = "^2.20.0"
-autoflake = "*"
 types-toml = "*"
 types-ujson = "*"
 types-pyyaml = "*"
 typer-cli = "*"
 ruff = "0.3.3"
 pytest-xdist = "^3.3.1"
 types-python-slugify = "^8.0.0.3"
```

