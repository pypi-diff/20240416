# Comparing `tmp/dataspecs-0.2.0.tar.gz` & `tmp/dataspecs-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dataspecs-0.2.0.tar", max compression
+gzip compressed data, was "dataspecs-0.3.0.tar", max compression
```

## Comparing `dataspecs-0.2.0.tar` & `dataspecs-0.3.0.tar`

### file list

```diff
@@ -1,9 +1,12 @@
--rw-r--r--   0        0        0     1076 2024-04-12 18:28:21.633624 dataspecs-0.2.0/LICENSE
--rw-r--r--   0        0        0      876 2024-04-12 18:28:21.633624 dataspecs-0.2.0/README.md
--rw-r--r--   0        0        0      358 2024-04-12 18:28:21.633624 dataspecs-0.2.0/dataspecs/__init__.py
--rw-r--r--   0        0        0     5113 2024-04-12 18:28:21.633624 dataspecs-0.2.0/dataspecs/api.py
--rw-r--r--   0        0        0        0 2024-04-12 18:28:21.633624 dataspecs-0.2.0/dataspecs/py.typed
--rw-r--r--   0        0        0     5104 2024-04-12 18:28:21.633624 dataspecs-0.2.0/dataspecs/specs.py
--rw-r--r--   0        0        0     2633 2024-04-12 18:28:21.633624 dataspecs-0.2.0/dataspecs/typing.py
--rw-r--r--   0        0        0      891 2024-04-12 18:28:21.633624 dataspecs-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1643 1970-01-01 00:00:00.000000 dataspecs-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1076 2024-04-16 15:38:02.824623 dataspecs-0.3.0/LICENSE
+-rw-r--r--   0        0        0      876 2024-04-16 15:38:02.824623 dataspecs-0.3.0/README.md
+-rw-r--r--   0        0        0      344 2024-04-16 15:38:02.824623 dataspecs-0.3.0/dataspecs/__init__.py
+-rw-r--r--   0        0        0      111 2024-04-16 15:38:02.824623 dataspecs-0.3.0/dataspecs/core/__init__.py
+-rw-r--r--   0        0        0     5119 2024-04-16 15:38:02.824623 dataspecs-0.3.0/dataspecs/core/api.py
+-rw-r--r--   0        0        0     5109 2024-04-16 15:38:02.824623 dataspecs-0.3.0/dataspecs/core/specs.py
+-rw-r--r--   0        0        0     2938 2024-04-16 15:38:02.824623 dataspecs-0.3.0/dataspecs/core/typing.py
+-rw-r--r--   0        0        0      174 2024-04-16 15:38:02.824623 dataspecs-0.3.0/dataspecs/extras/__init__.py
+-rw-r--r--   0        0        0     1406 2024-04-16 15:38:02.824623 dataspecs-0.3.0/dataspecs/extras/replacement.py
+-rw-r--r--   0        0        0        0 2024-04-16 15:38:02.824623 dataspecs-0.3.0/dataspecs/py.typed
+-rw-r--r--   0        0        0      891 2024-04-16 15:38:02.824623 dataspecs-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1643 1970-01-01 00:00:00.000000 dataspecs-0.3.0/PKG-INFO
```

### Comparing `dataspecs-0.2.0/LICENSE` & `dataspecs-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `dataspecs-0.2.0/README.md` & `dataspecs-0.3.0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -7,9 +7,9 @@
 [![Tests](https://img.shields.io/github/actions/workflow/status/astropenguin/dataspecs/tests.yaml?label=Tests&style=flat-square)](https://github.com/astropenguin/dataspecs/actions)
 
 Data specifications by data classes
 
 ## Installation
 
 ```shell
-pip install dataspecs==0.2.0
+pip install dataspecs==0.3.0
 ```
```

### Comparing `dataspecs-0.2.0/dataspecs/api.py` & `dataspecs-0.3.0/dataspecs/core/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 
 # dependencies
 from .specs import ID, ROOT, Spec, Specs
 from .typing import (
     DataClass,
     StrPath,
+    get_annotated,
     get_dataclasses,
     get_final,
     get_first,
     get_subtypes,
     get_tags,
 )
 
@@ -82,15 +83,14 @@
 
         specs.append(
             spec_factory(
                 id=(child_id := ID(parent_id) / field.name),
                 tags=get_tags(reftype),
                 type=get_final(field.type, type_only),
                 data=getattr(obj, field.name, field.default),
-                origin=obj,
             )
         )
         specs.extend(
             from_typehint(
                 reftype,
                 parent_id=child_id,
                 first_only=first_only,
@@ -153,15 +153,15 @@
 
     Returns:
         Data specs created from the type hint.
 
     """
     specs: Specs[Any] = Specs()
 
-    for name, subtype in enumerate(get_subtypes(obj)):
+    for name, subtype in enumerate(get_subtypes(get_annotated(obj))):
         specs.append(
             spec_factory(
                 id=(child_id := ID(parent_id) / str(name)),
                 tags=get_tags(subtype),
                 type=get_final(subtype, type_only),
             )
         )
```

### Comparing `dataspecs-0.2.0/dataspecs/specs.py` & `dataspecs-0.3.0/dataspecs/core/specs.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 __all__ = ["ID", "ROOT", "Spec", "Specs"]
 
 
 # standard library
 from collections import UserList
 from collections.abc import Iterable
-from dataclasses import dataclass, field
+from dataclasses import dataclass
 from os import fspath
 from pathlib import PurePosixPath
 from re import Match, compile, escape, fullmatch
 from typing import Any, Optional, SupportsIndex, TypeVar, cast, overload
 
 
 # dependencies
 from typing_extensions import Self
-from .typing import DataClass, StrPath, TagBase, is_strpath, is_tag
+from .typing import StrPath, TagBase, is_strpath, is_tag
 
 
 # constants
 GLOB_PATTERN = compile(r"\\\*\\\*()|\\\*([^\\\*]|$)")
 GLOB_REPLS = r".*", r"[^/]*"
 ROOT_PATH = "/"
 
@@ -81,15 +81,14 @@
     """Data specification (data spec).
 
     Args:
         id: ID of the data spec.
         tags: Tags of the data spec.
         type: Type hint for the data of the data spec.
         data: Default or final data of the data spec.
-        origin: Original dataclass object of the data spec.
 
     """
 
     id: ID
     """ID of the data spec."""
 
     tags: tuple[TagBase, ...]
@@ -97,17 +96,14 @@
 
     type: Any
     """Type hint for the data of the data spec."""
 
     data: Optional[Any] = None
     """Default or final data of the data spec."""
 
-    origin: Optional[DataClass] = field(default=None, repr=False)
-    """Original dataclass object of the data spec."""
-
 
 class Specs(UserList[TSpec]):
     """Data specifications (data specs)."""
 
     @property
     def first(self) -> Optional[TSpec]:
         """Return the first data spec if it exists (``None`` otherwise)."""
@@ -119,14 +115,18 @@
         return self[-1] if len(self) else None
 
     @property
     def unique(self) -> Optional[TSpec]:
         """Return the data spec if it is unique (``None`` otherwise)."""
         return self[0] if len(self) == 1 else None
 
+    def replace(self, old: TSpec, new: TSpec, /) -> Self:
+        """Return data specs with old data spec replaced by new one."""
+        return type(self)(new if spec == old else spec for spec in self)
+
     @overload
     def __getitem__(self, index: None, /) -> Self: ...
 
     @overload
     def __getitem__(self, index: TagBase, /) -> Self: ...
 
     @overload
```

### Comparing `dataspecs-0.2.0/dataspecs/typing.py` & `dataspecs-0.3.0/dataspecs/core/typing.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 __all__ = ["TagBase"]
 
 
 # standard library
+import types
 from dataclasses import Field, is_dataclass
 from enum import Enum
 from os import PathLike
-from typing import Annotated, Any, ClassVar, Protocol, Union
+from typing import Annotated, Any, ClassVar, Literal, Protocol, Union
 
 
 # dependencies
 from typing_extensions import TypeGuard, get_args, get_origin, get_type_hints
 
 
 # type hints
@@ -68,33 +69,45 @@
 def get_first(obj: Any, /) -> Any:
     """Return the first type if a type hint is a union type."""
     return get_args(obj)[0] if is_union(obj) else obj
 
 
 def get_subtypes(obj: Any, /) -> tuple[Any, ...]:
     """Return subtypes of a type hint if they exist."""
-    return get_args(get_annotated(obj))
+    return get_args(obj) if not is_literal(obj) else ()
 
 
 def get_tags(obj: Any, /) -> tuple[TagBase, ...]:
     """Return tags that annotate a type hint."""
     return tuple(filter(is_tag, get_annotations(obj)))
 
 
 def is_annotated(obj: Any, /) -> bool:
     """Check if a type hint is annotated."""
     return get_origin(obj) is Annotated
 
 
+def is_literal(obj: Any, /) -> bool:
+    """Check if a type hint is a literal type."""
+    return get_origin(obj) is Literal
+
+
 def is_strpath(obj: Any, /) -> TypeGuard[StrPath]:
     """Check if an object is a string or a string path."""
     return isinstance(obj, (str, PathLike))
 
 
 def is_tag(obj: Any, /) -> TypeGuard[TagBase]:
     """Check if an object is a specification tag."""
     return isinstance(obj, TagBase)
 
 
 def is_union(obj: Any, /) -> bool:
     """Check if a type hint is a union type."""
-    return get_origin(Union[obj]) is Union  # type: ignore
+    if get_origin(obj) is Union:
+        return True
+
+    # Only for Python >= 3.10
+    if UnionType := getattr(types, "UnionType", None):
+        return isinstance(obj, UnionType)
+
+    return False
```

### Comparing `dataspecs-0.2.0/pyproject.toml` & `dataspecs-0.3.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dataspecs"
-version = "0.2.0"
+version = "0.3.0"
 description = "Data specifications by data classes"
 authors = ["Akio Taniguchi <taniguchi@a.phys.nagoya-u.ac.jp>"]
 documentation = "https://astropenguin.github.io/dataspecs/"
 homepage = "https://github.com/astropenguin/dataspecs/"
 keywords = ["dataclasses", "specifications", "typing"]
 license = "MIT"
 readme = "README.md"
```

### Comparing `dataspecs-0.2.0/PKG-INFO` & `dataspecs-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dataspecs
-Version: 0.2.0
+Version: 0.3.0
 Summary: Data specifications by data classes
 Home-page: https://github.com/astropenguin/dataspecs/
 License: MIT
 Keywords: dataclasses,specifications,typing
 Author: Akio Taniguchi
 Author-email: taniguchi@a.phys.nagoya-u.ac.jp
 Requires-Python: >=3.9,<3.13
@@ -27,10 +27,10 @@
 [![Tests](https://img.shields.io/github/actions/workflow/status/astropenguin/dataspecs/tests.yaml?label=Tests&style=flat-square)](https://github.com/astropenguin/dataspecs/actions)
 
 Data specifications by data classes
 
 ## Installation
 
 ```shell
-pip install dataspecs==0.2.0
+pip install dataspecs==0.3.0
 ```
```

