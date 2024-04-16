# Comparing `tmp/graphemy-1.0.0b3.tar.gz` & `tmp/graphemy-1.0.0b4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphemy-1.0.0b3.tar", max compression
+gzip compressed data, was "graphemy-1.0.0b4.tar", max compression
```

## Comparing `graphemy-1.0.0b3.tar` & `graphemy-1.0.0b4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
--rw-r--r--   0        0        0      669 2024-04-11 13:36:54.239602 graphemy-1.0.0b3/graphemy/__init__.py
--rw-r--r--   0        0        0        0 2024-04-03 15:13:51.585025 graphemy-1.0.0b3/graphemy/database/__init__.py
--rw-r--r--   0        0        0     5632 2024-03-03 14:45:13.570971 graphemy-1.0.0b3/graphemy/database/operations.py
--rw-r--r--   0        0        0     1394 2024-03-02 04:18:14.625389 graphemy-1.0.0b3/graphemy/database/utils.py
--rw-r--r--   0        0        0     2227 2024-03-03 14:45:12.700973 graphemy-1.0.0b3/graphemy/dl.py
--rw-r--r--   0        0        0     1356 2024-03-03 14:45:39.241519 graphemy-1.0.0b3/graphemy/models.py
--rw-r--r--   0        0        0     5359 2024-04-03 15:55:25.323324 graphemy-1.0.0b3/graphemy/router.py
--rw-r--r--   0        0        0        0 2024-04-03 15:13:51.585025 graphemy-1.0.0b3/graphemy/schemas/__init__.py
--rw-r--r--   0        0        0     6886 2024-04-11 13:30:51.675271 graphemy-1.0.0b3/graphemy/schemas/generators.py
--rw-r--r--   0        0        0      193 2024-03-02 04:18:14.640390 graphemy-1.0.0b3/graphemy/schemas/models.py
--rw-r--r--   0        0        0     2699 2024-03-03 14:44:06.277319 graphemy-1.0.0b3/graphemy/setup.py
--rw-r--r--   0        0        0     1100 2023-11-14 12:13:24.784243 graphemy-1.0.0b3/LICENSE
--rw-r--r--   0        0        0     2123 2024-04-11 13:38:46.365606 graphemy-1.0.0b3/pyproject.toml
--rw-r--r--   0        0        0     3607 2023-11-14 11:57:04.869280 graphemy-1.0.0b3/README.md
--rw-r--r--   0        0        0     4746 1970-01-01 00:00:00.000000 graphemy-1.0.0b3/PKG-INFO
+-rw-r--r--   0        0        0      717 2024-04-16 19:11:37.721195 graphemy-1.0.0b4/graphemy/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-03 15:13:51.585025 graphemy-1.0.0b4/graphemy/database/__init__.py
+-rw-r--r--   0        0        0     5630 2024-04-16 19:11:37.723473 graphemy-1.0.0b4/graphemy/database/operations.py
+-rw-r--r--   0        0        0     1574 2024-04-16 19:13:26.518773 graphemy-1.0.0b4/graphemy/database/utils.py
+-rw-r--r--   0        0        0     2367 2024-04-16 19:13:25.548615 graphemy-1.0.0b4/graphemy/dl.py
+-rw-r--r--   0        0        0     1356 2024-04-16 17:05:21.552951 graphemy-1.0.0b4/graphemy/models.py
+-rw-r--r--   0        0        0     5420 2024-04-16 18:53:26.124888 graphemy-1.0.0b4/graphemy/router.py
+-rw-r--r--   0        0        0        0 2024-04-03 15:13:51.585025 graphemy-1.0.0b4/graphemy/schemas/__init__.py
+-rw-r--r--   0        0        0     7679 2024-04-16 19:13:26.540872 graphemy-1.0.0b4/graphemy/schemas/generators.py
+-rw-r--r--   0        0        0      193 2024-03-02 04:18:14.640390 graphemy-1.0.0b4/graphemy/schemas/models.py
+-rw-r--r--   0        0        0     2699 2024-03-03 14:44:06.277319 graphemy-1.0.0b4/graphemy/setup.py
+-rw-r--r--   0        0        0     1100 2023-11-14 12:13:24.784243 graphemy-1.0.0b4/LICENSE
+-rw-r--r--   0        0        0     2182 2024-04-16 19:16:09.045356 graphemy-1.0.0b4/pyproject.toml
+-rw-r--r--   0        0        0     3607 2023-11-14 11:57:04.869280 graphemy-1.0.0b4/README.md
+-rw-r--r--   0        0        0     4746 1970-01-01 00:00:00.000000 graphemy-1.0.0b4/PKG-INFO
```

### Comparing `graphemy-1.0.0b3/graphemy/__init__.py` & `graphemy-1.0.0b4/graphemy/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,21 @@
+import os
+
 from sqlmodel import Field
 
 from graphemy.dl import Dl
 from graphemy.models import Graphemy
 from graphemy.router import GraphemyRouter
 from graphemy.setup import Setup
-import os
+
+
 def import_files(path):
     for root, dirs, files in os.walk(path):
         for file in files:
             if file.endswith('.py') and file != '__init__.py':
                 module_name = os.path.splitext(file)[0]
                 module_path = os.path.join(root, module_name)
-                module_path_rel = os.path.relpath(os.path.join(root, module_name))
+                module_path_rel = os.path.relpath(
+                    os.path.join(root, module_name)
+                )
                 module_path = module_path_rel.replace(os.path.sep, '.')
-                exec(f'import {module_path}')
+                exec(f'import {module_path}')
```

### Comparing `graphemy-1.0.0b3/graphemy/database/operations.py` & `graphemy-1.0.0b4/graphemy/database/operations.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,29 +60,30 @@
             and_(*filter_temp, get_filter(model, filters[f], id, params, i))
         )
     results = await Setup.execute_query(
         query.where(or_(*query_filters)).params(**params), model.__enginename__
     )
     for r in results:
         temp = id_groups[get_keys(r, id)]
+
         if len(temp) == 1:
             key = temp[0]
             if many:
                 groups[key].append(r)
             else:
                 groups[key] = r
         else:
             for t in temp:
                 if not t[0][1] or all(
                     [getattr(r, k) in v for k, v in t[0][1] if v]
                 ):
                     if many:
-                        groups[key].append(r)
+                        groups[t].append(r)
                     else:
-                        groups[key] = r
+                        groups[t] = r
     return groups.values()
 
 
 async def get_all(model: 'Graphemy', filters, query_filter):
     query = select(model).where(query_filter)
     if filters:
         filters = vars(filters)
```

### Comparing `graphemy-1.0.0b3/graphemy/database/utils.py` & `graphemy-1.0.0b4/graphemy/database/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from datetime import date
 from typing import TYPE_CHECKING
 
+from sqlalchemy.sql.elements import BinaryExpression
 from sqlmodel import and_, bindparam, or_
 
 if TYPE_CHECKING:
     from ..models import Graphemy
 
 
 def get_keys(model: 'Graphemy', id: str | list[str]) -> tuple | str:
@@ -18,15 +19,15 @@
 
 def get_filter(
     model: 'Graphemy',
     keys,
     id,
     params: dict,
     i: int,
-):
+) -> BinaryExpression:
     if isinstance(id, list):
         filter = []
         for j, key in enumerate(keys):
             f = []
             if None not in key:
                 for k in range(len(id)):
                     f.append(
@@ -40,10 +41,13 @@
                 filter.append(and_(*f))
             else:
                 filter.append(False)
         return or_(*filter)
     elif None in keys:
         keys.remove(None)
     params[f'p{i}'] = keys
+    a = getattr(model, id).in_(
+        bindparam(f'p{i}', expanding=True, literal_execute=True)
+    )
     return getattr(model, id).in_(
         bindparam(f'p{i}', expanding=True, literal_execute=True)
     )
```

### Comparing `graphemy-1.0.0b3/graphemy/dl.py` & `graphemy-1.0.0b4/graphemy/dl.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,28 +2,35 @@
 
 from .schemas.models import DateFilter
 
 
 class Dl:
     source: str | list[str]
     target: str | list[str]
+    foreign_key: bool = True
 
-    def __init__(self, source: str | list[str], target: str | list[str]):
+    def __init__(
+        self,
+        source: str | list[str],
+        target: str | list[str],
+        foreign_key: bool = True,
+    ):
         if type(source) != type(target):
             raise 'source and target must have same type'
         if type(source) == list:
             if len(source) != len(target):
                 raise 'source and target must have same length'
             ids = {}
             for i, id in enumerate(target):
                 ids[id] = source[i]
             target.sort()
             source = [ids[id] for id in target]
         self.source = source
         self.target = target
+        self.foreign_key = foreign_key
 
 
 class GraphemyDataLoader(DataLoader):
     def __init__(self, filter_method=None, request=None, **kwargs):
         self.filter_method = filter_method
         self.request = request
         super().__init__(**kwargs)
```

### Comparing `graphemy-1.0.0b3/graphemy/models.py` & `graphemy-1.0.0b4/graphemy/models.py`

 * *Files identical despite different names*

### Comparing `graphemy-1.0.0b3/graphemy/router.py` & `graphemy-1.0.0b4/graphemy/router.py`

 * *Files 1% similar despite different names*

```diff
@@ -54,26 +54,27 @@
         dl_filter: Callable | None = None,
         query_filter: Callable | None = None,
         engine: Engine | Dict[str, Engine] = None,
         extensions: list = [],
         enable_queries: bool = True,
         enable_put_mutations: bool = False,
         enable_delete_mutations: bool = False,
+        auto_foreign_keys: bool = False,
         **kwargs,
     ):
         functions: Dict[str, tuple] = {}
         Setup.setup(
             engine=engine,
             get_perm=permission_getter,
             query_filter=query_filter,
         )
         need_query = True
         need_mutation = True
         for cls in Setup.classes.values():
-            set_schema(cls, functions)
+            set_schema(cls, functions, auto_foreign_keys)
             if cls.__enable_query__ == None:
                 cls.__enable_query__ = enable_queries
             if cls.__enable_put_mutation__ == None:
                 cls.__enable_put_mutation__ = enable_put_mutations
             if cls.__enable_delete_mutation__ == None:
                 cls.__enable_delete_mutation__ = enable_delete_mutations
             cls_query, cls_filter = get_query(cls)
```

### Comparing `graphemy-1.0.0b3/graphemy/schemas/generators.py` & `graphemy-1.0.0b4/graphemy/schemas/generators.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     TypeVar,
     Union,
     get_args,
     get_origin,
 )
 
 import strawberry
+from sqlalchemy import ForeignKeyConstraint
 from sqlalchemy.inspection import inspect
 from strawberry.field import StrawberryField
 from strawberry.tools import merge_types
 from strawberry.types import Info
 
 from ..database.operations import delete_item, get_all, get_items, put_item
 from ..dl import Dl
@@ -26,22 +27,25 @@
 if TYPE_CHECKING:
     from ..models import Graphemy
 
 T = TypeVar('T')
 
 
 def set_schema(
-    cls: 'Graphemy', functions: Dict[str, Tuple[Callable, 'Graphemy']]
+    cls: 'Graphemy',
+    functions: Dict[str, Tuple[Callable, 'Graphemy']],
+    auto_foreign_keys,
 ) -> None:
     """Set the Strawberry schema for a Graphemy class."""
 
     # Define a class to hold Strawberry schema fields
     class Schema:
         pass
 
+    foreign_keys_info = []
     for attr in [
         attr for attr in cls.__dict__.values() if hasattr(attr, 'dl')
     ]:
         returned_class: 'Graphemy' = Setup.classes[attr.dl]
         setattr(
             Schema,
             attr.__name__,
@@ -51,44 +55,60 @@
                     Setup.get_auth(
                         returned_class,
                         'query',
                     )
                 ],
             ),
         )
+        if auto_foreign_keys and not attr.many and attr.foreign_key:
+            source = (
+                attr.source if isinstance(attr.source, list) else [attr.source]
+            )
+            target = (
+                attr.target if isinstance(attr.target, list) else [attr.target]
+            )
+            target = [returned_class.__tablename__ + '.' + t for t in target]
+            cls.__table__.append_constraint(
+                ForeignKeyConstraint(source, target)
+            )
+            foreign_keys_info.append((source, target))
         if not attr.dl_name in functions:
-            functions[attr.dl_name] = (get_dl_field(attr,returned_class ), returned_class)
+            functions[attr.dl_name] = (
+                get_dl_field(attr, returned_class),
+                returned_class,
+            )
     extra_schema = strawberry.type(
         cls.Strawberry, name=f'{cls.__name__}Schema2'
     )
     strawberry_schema = strawberry.experimental.pydantic.type(
         cls, all_fields=True, name=f'{cls.__name__}Schema'
     )(Schema)
     if extra_schema.__annotations__:
         strawberry_schema = merge_types(
             f'{cls.__name__}Schema', (strawberry_schema, extra_schema)
         )
     cls.__strawberry_schema__ = strawberry_schema
 
 
-def get_dl_field(attr,returned_class:"Graphemy"):
+def get_dl_field(attr, returned_class: 'Graphemy'):
     returned_schema = returned_class.__strawberry_schema__
     if attr.many:
         returned_schema = list[returned_schema]
     else:
         returned_schema = Optional[returned_schema]
+
     async def dataloader(
         keys: list[tuple],
     ) -> returned_schema:
-        return await get_items(
-            returned_class, keys, attr.target, attr.many
-        )
+        return await get_items(returned_class, keys, attr.target, attr.many)
+
     dataloader.__name__ = attr.dl_name
     return dataloader
 
+
 def get_dl_function(
     field_name: str,
     field_type: T,
     field_value: Dl,
 ) -> Callable[[], Union['Graphemy', list['Graphemy']]]:
     """Generates a DataLoader function dynamically based on the field's specifications."""
     # Determine if the field_type is a list and extract the inner type
@@ -106,15 +126,15 @@
     # Define the return type using Strawberry's lazy type resolution
     return_type = Annotated[
         f'{class_type}Schema',
         strawberry.lazy('graphemy.router'),
     ]
     if is_list:
         return_type = list[return_type]
-    
+
     else:
         return_type = Optional[return_type]
 
     async def loader_func(
         self,
         info: Info,
         filters: Annotated[
@@ -135,14 +155,16 @@
         )
 
     # Customize the function attributes for introspection or other purposes
     loader_func.__name__ = field_name
     loader_func.dl = class_type
     loader_func.many = is_list
     loader_func.target = field_value.target
+    loader_func.source = field_value.source
+    loader_func.foreign_key = field_value.foreign_key
     loader_func.dl_name = dl_name
 
     return loader_func
 
 
 def get_query(cls: 'Graphemy') -> StrawberryField:
     class Filter:
```

### Comparing `graphemy-1.0.0b3/graphemy/setup.py` & `graphemy-1.0.0b4/graphemy/setup.py`

 * *Files identical despite different names*

### Comparing `graphemy-1.0.0b3/LICENSE` & `graphemy-1.0.0b4/LICENSE`

 * *Files identical despite different names*

### Comparing `graphemy-1.0.0b3/pyproject.toml` & `graphemy-1.0.0b4/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "graphemy"
-version = "1.0.0-beta.3"
+version = "1.0.0-beta.4"
 description = "A Python library for integrating SQLModel and Strawberry, providing a seamless GraphQL integration with FastAPI and advanced features for database interactions."
 authors = ["Matheus Doreto <matheusdoreto.md@gmail.com>"]
 readme = "README.md"
 packages = [{include = "graphemy"}]
 homepage = "https://github.com/MDoreto/graphemy"
 documentation = "https://graphemy.readthedocs.io/en/latest/"
 repository = "https://github.com/MDoreto/graphemy"
@@ -36,14 +36,15 @@
 pytest-cov = "^4.1.0"
 blue = "^0.9.1"
 isort = "^5.12.0"
 taskipy = "^1.12.0"
 pytest-asyncio = "^0.21.1"
 httpx = "^0.25.0"
 pytest-env = "^1.1.1"
+aiosqlite = "^0.20.0"
 
 
 [tool.poetry.group.doc.dependencies]
 mkdocs-material = "^9.4.7"
 mkdocstrings = "^0.23.0"
 mkdocstrings-python = "^1.7.3"
 mkdocs-macros-plugin = "^1.0.5"
@@ -66,7 +67,8 @@
 [tool.taskipy.tasks]
 example = "uvicorn examples.tutorial.main:app --reload --port 8001"
 lint = "blue . && isort ."
 docs = "mkdocs serve"
 pre_test = "task lint"
 test = "pytest -s -x --cov=graphemy -vv -W ignore::DeprecationWarning"
 post_test = "coverage html"
+publish = "poetry publish --build"
```

### Comparing `graphemy-1.0.0b3/README.md` & `graphemy-1.0.0b4/README.md`

 * *Files identical despite different names*

### Comparing `graphemy-1.0.0b3/PKG-INFO` & `graphemy-1.0.0b4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: graphemy
-Version: 1.0.0b3
+Version: 1.0.0b4
 Summary: A Python library for integrating SQLModel and Strawberry, providing a seamless GraphQL integration with FastAPI and advanced features for database interactions.
 Home-page: https://github.com/MDoreto/graphemy
 License: MIT
 Author: Matheus Doreto
 Author-email: matheusdoreto.md@gmail.com
 Requires-Python: >=3.12,<4.0
 Classifier: Development Status :: 4 - Beta
```

