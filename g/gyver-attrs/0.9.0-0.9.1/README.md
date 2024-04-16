# Comparing `tmp/gyver_attrs-0.9.0.tar.gz` & `tmp/gyver_attrs-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gyver_attrs-0.9.0.tar", max compression
+gzip compressed data, was "gyver_attrs-0.9.1.tar", max compression
```

## Comparing `gyver_attrs-0.9.0.tar` & `gyver_attrs-0.9.1.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0    11352 2024-03-28 22:15:25.253687 gyver_attrs-0.9.0/LICENSE
--rw-r--r--   0        0        0     5279 2024-03-28 22:15:25.253687 gyver_attrs-0.9.0/README.md
--rw-r--r--   0        0        0       80 2024-03-28 22:15:25.253687 gyver_attrs-0.9.0/gyver/__init__.py
--rw-r--r--   0        0        0      721 2024-03-28 22:20:32.217655 gyver_attrs-0.9.0/gyver/attrs/__init__.py
--rw-r--r--   0        0        0     3467 2024-03-28 22:15:25.253687 gyver_attrs-0.9.0/gyver/attrs/camel.py
--rw-r--r--   0        0        0      146 2024-03-28 22:15:25.253687 gyver_attrs-0.9.0/gyver/attrs/converters/__init__.py
--rw-r--r--   0        0        0      751 2024-03-28 22:15:25.253687 gyver_attrs-0.9.0/gyver/attrs/converters/json.py
--rw-r--r--   0        0        0     1463 2024-03-28 22:15:25.253687 gyver_attrs-0.9.0/gyver/attrs/converters/utils.py
--rw-r--r--   0        0        0     9316 2024-03-28 22:15:25.253687 gyver_attrs-0.9.0/gyver/attrs/field.py
--rw-r--r--   0        0        0     6142 2024-03-28 22:15:25.253687 gyver_attrs-0.9.0/gyver/attrs/helpers.py
--rw-r--r--   0        0        0    29147 2024-03-28 22:15:25.253687 gyver_attrs-0.9.0/gyver/attrs/main.py
--rw-r--r--   0        0        0     5072 2024-03-28 22:15:25.253687 gyver_attrs-0.9.0/gyver/attrs/methods.py
--rw-r--r--   0        0        0        0 2024-03-28 22:15:25.253687 gyver_attrs-0.9.0/gyver/attrs/py.typed
--rw-r--r--   0        0        0     4348 2024-03-28 22:15:25.253687 gyver_attrs-0.9.0/gyver/attrs/resolver.py
--rw-r--r--   0        0        0     4032 2024-03-28 22:15:25.253687 gyver_attrs-0.9.0/gyver/attrs/schema.py
--rw-r--r--   0        0        0     5653 2024-03-28 22:15:25.253687 gyver_attrs-0.9.0/gyver/attrs/shortcuts.py
--rw-r--r--   0        0        0        0 2024-03-28 22:15:25.253687 gyver_attrs-0.9.0/gyver/attrs/utils/__init__.py
--rw-r--r--   0        0        0      627 2024-03-28 22:15:25.253687 gyver_attrs-0.9.0/gyver/attrs/utils/factory.py
--rw-r--r--   0        0        0     5650 2024-03-28 22:15:25.253687 gyver_attrs-0.9.0/gyver/attrs/utils/functions.py
--rw-r--r--   0        0        0      641 2024-03-28 22:15:25.253687 gyver_attrs-0.9.0/gyver/attrs/utils/typedef.py
--rw-r--r--   0        0        0     1149 2024-03-28 22:20:32.224322 gyver_attrs-0.9.0/pyproject.toml
--rw-r--r--   0        0        0     5920 1970-01-01 00:00:00.000000 gyver_attrs-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0    11352 2024-03-28 22:15:25.253687 gyver_attrs-0.9.1/LICENSE
+-rw-r--r--   0        0        0     5279 2024-03-28 22:15:25.253687 gyver_attrs-0.9.1/README.md
+-rw-r--r--   0        0        0       80 2024-03-28 22:15:25.253687 gyver_attrs-0.9.1/gyver/__init__.py
+-rw-r--r--   0        0        0      721 2024-04-16 17:08:08.551174 gyver_attrs-0.9.1/gyver/attrs/__init__.py
+-rw-r--r--   0        0        0     3508 2024-04-16 17:07:30.546888 gyver_attrs-0.9.1/gyver/attrs/camel.py
+-rw-r--r--   0        0        0      146 2024-03-28 22:15:25.253687 gyver_attrs-0.9.1/gyver/attrs/converters/__init__.py
+-rw-r--r--   0        0        0      751 2024-03-28 22:15:25.253687 gyver_attrs-0.9.1/gyver/attrs/converters/json.py
+-rw-r--r--   0        0        0     1463 2024-03-28 22:15:25.253687 gyver_attrs-0.9.1/gyver/attrs/converters/utils.py
+-rw-r--r--   0        0        0     9316 2024-03-28 22:15:25.253687 gyver_attrs-0.9.1/gyver/attrs/field.py
+-rw-r--r--   0        0        0     6142 2024-03-28 22:15:25.253687 gyver_attrs-0.9.1/gyver/attrs/helpers.py
+-rw-r--r--   0        0        0    29147 2024-03-28 22:15:25.253687 gyver_attrs-0.9.1/gyver/attrs/main.py
+-rw-r--r--   0        0        0     5072 2024-03-28 22:15:25.253687 gyver_attrs-0.9.1/gyver/attrs/methods.py
+-rw-r--r--   0        0        0        0 2024-03-28 22:15:25.253687 gyver_attrs-0.9.1/gyver/attrs/py.typed
+-rw-r--r--   0        0        0     4348 2024-03-28 22:15:25.253687 gyver_attrs-0.9.1/gyver/attrs/resolver.py
+-rw-r--r--   0        0        0     4032 2024-03-28 22:15:25.253687 gyver_attrs-0.9.1/gyver/attrs/schema.py
+-rw-r--r--   0        0        0     5653 2024-03-28 22:15:25.253687 gyver_attrs-0.9.1/gyver/attrs/shortcuts.py
+-rw-r--r--   0        0        0        0 2024-03-28 22:15:25.253687 gyver_attrs-0.9.1/gyver/attrs/utils/__init__.py
+-rw-r--r--   0        0        0      627 2024-03-28 22:15:25.253687 gyver_attrs-0.9.1/gyver/attrs/utils/factory.py
+-rw-r--r--   0        0        0     5797 2024-04-16 17:06:15.778349 gyver_attrs-0.9.1/gyver/attrs/utils/functions.py
+-rw-r--r--   0        0        0      641 2024-03-28 22:15:25.253687 gyver_attrs-0.9.1/gyver/attrs/utils/typedef.py
+-rw-r--r--   0        0        0     1149 2024-04-16 17:08:08.561174 gyver_attrs-0.9.1/pyproject.toml
+-rw-r--r--   0        0        0     5920 1970-01-01 00:00:00.000000 gyver_attrs-0.9.1/PKG-INFO
```

### Comparing `gyver_attrs-0.9.0/LICENSE` & `gyver_attrs-0.9.1/LICENSE`

 * *Files identical despite different names*

### Comparing `gyver_attrs-0.9.0/README.md` & `gyver_attrs-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `gyver_attrs-0.9.0/gyver/attrs/__init__.py` & `gyver_attrs-0.9.1/gyver/attrs/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -23,9 +23,9 @@
     'mutable',
     'kw_only',
     'UNINITIALIZED',
     'update_ref',
     'update_refs',
 ]
 
-__version__ = '0.9.0'
+__version__ = '0.9.1'
 __version_info__ = tuple(map(int, __version__.split('.')))
```

### Comparing `gyver_attrs-0.9.0/gyver/attrs/camel.py` & `gyver_attrs-0.9.1/gyver/attrs/camel.py`

 * *Files 19% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from typing import Any, Literal, Optional, TypeVar, Union, overload
 
 import typing_extensions
 
 from gyver.attrs.main import define
 
 from .field import Field, FieldInfo, info
-from .utils.functions import to_camel, to_upper_camel
+from .utils.functions import to_camel, to_pascal, to_upper_camel
 from .utils.typedef import DisassembledType
 
 T = TypeVar('T')
 
 
 @typing_extensions.deprecated('Use the `alias_generator` parameter instead instead')
 class ToCamelField(Field):
@@ -71,15 +71,15 @@
 
 
 @overload
 def define_camel(
     maybe_cls: None = None,
     /,
     *,
-    style: Literal['upper', 'lower'] = 'lower',
+    style: Literal['upper', 'pascal', 'lower'] = 'lower',
     frozen: bool = True,
     kw_only: bool = False,
     slots: bool = True,
     repr: bool = True,
     eq: bool = True,
     order: bool = True,
     hash: Optional[bool] = None,
@@ -89,15 +89,15 @@
 
 
 @overload
 def define_camel(
     maybe_cls: type[T],
     /,
     *,
-    style: Literal['upper', 'lower'] = 'lower',
+    style: Literal['upper', 'pascal', 'lower'] = 'lower',
     frozen: bool = True,
     kw_only: bool = False,
     slots: bool = True,
     repr: bool = True,
     eq: bool = True,
     order: bool = True,
     hash: Optional[bool] = None,
@@ -112,32 +112,32 @@
     kw_only_default=False,
     field_specifiers=(FieldInfo, info),
 )
 def define_camel(
     maybe_cls: Optional[type[T]] = None,
     /,
     *,
-    style: Literal['upper', 'lower'] = 'lower',
+    style: Literal['pascal', 'upper', 'lower'] = 'lower',
     frozen: bool = True,
     kw_only: bool = False,
     slots: bool = True,
     repr: bool = True,
     eq: bool = True,
     order: bool = True,
     hash: Optional[bool] = None,
     pydantic: bool = True,
     dataclass_fields: bool = False,
 ) -> Union[Callable[[type[T]], type[T]], type[T]]:
-    field_class = ToCamelField if style == 'lower' else ToUpperCamelField
+    alias_generator = to_camel if style == 'lower' else to_pascal
     return define(
         maybe_cls,
         frozen=frozen,
         kw_only=kw_only,
         slots=slots,
         repr=repr,
         eq=eq,
         order=order,
         hash=hash,
         pydantic=pydantic,
         dataclass_fields=dataclass_fields,
-        field_class=field_class,
+        alias_generator=alias_generator,
     )
```

### Comparing `gyver_attrs-0.9.0/gyver/attrs/converters/json.py` & `gyver_attrs-0.9.1/gyver/attrs/converters/json.py`

 * *Files identical despite different names*

### Comparing `gyver_attrs-0.9.0/gyver/attrs/converters/utils.py` & `gyver_attrs-0.9.1/gyver/attrs/converters/utils.py`

 * *Files identical despite different names*

### Comparing `gyver_attrs-0.9.0/gyver/attrs/field.py` & `gyver_attrs-0.9.1/gyver/attrs/field.py`

 * *Files identical despite different names*

### Comparing `gyver_attrs-0.9.0/gyver/attrs/helpers.py` & `gyver_attrs-0.9.1/gyver/attrs/helpers.py`

 * *Files identical despite different names*

### Comparing `gyver_attrs-0.9.0/gyver/attrs/main.py` & `gyver_attrs-0.9.1/gyver/attrs/main.py`

 * *Files identical despite different names*

### Comparing `gyver_attrs-0.9.0/gyver/attrs/methods.py` & `gyver_attrs-0.9.1/gyver/attrs/methods.py`

 * *Files identical despite different names*

### Comparing `gyver_attrs-0.9.0/gyver/attrs/resolver.py` & `gyver_attrs-0.9.1/gyver/attrs/resolver.py`

 * *Files identical despite different names*

### Comparing `gyver_attrs-0.9.0/gyver/attrs/schema.py` & `gyver_attrs-0.9.1/gyver/attrs/schema.py`

 * *Files identical despite different names*

### Comparing `gyver_attrs-0.9.0/gyver/attrs/shortcuts.py` & `gyver_attrs-0.9.1/gyver/attrs/shortcuts.py`

 * *Files identical despite different names*

### Comparing `gyver_attrs-0.9.0/gyver/attrs/utils/factory.py` & `gyver_attrs-0.9.1/gyver/attrs/utils/factory.py`

 * *Files identical despite different names*

### Comparing `gyver_attrs-0.9.0/gyver/attrs/utils/functions.py` & `gyver_attrs-0.9.1/gyver/attrs/utils/functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 import re
 from collections.abc import Callable
 from typing import Any, ForwardRef, TypeVar, Union, get_args, get_origin
 
+import typing_extensions
+
 from .typedef import UNINITIALIZED, DisassembledType, TypeNode
 
 T = TypeVar('T')
 
 
 def disassemble_type(typ: Union[type, str]) -> DisassembledType:
     type_ = typ if not isinstance(typ, str) else ForwardRef(typ)
@@ -168,19 +170,24 @@
 _to_camel_regex = re.compile('_([a-zA-Z])')
 
 
 def to_camel(string: str) -> str:
     return _to_camel_regex.sub(lambda match: match[1].upper(), string.strip('_'))
 
 
-def to_upper_camel(string: str) -> str:
+def to_pascal(string: str) -> str:
     result = to_camel(string)
     return result[:1].upper() + result[1:]
 
 
+@typing_extensions.deprecated('Use to_pascal instead')
+def to_upper_camel(string: str) -> str:
+    return to_pascal(string)
+
+
 _dunder_regex = re.compile('__[a-zA-Z0-9_]__')
 
 
 def is_dunder(string: str) -> bool:
     return _dunder_regex.match(string) is not None
```

### Comparing `gyver_attrs-0.9.0/gyver/attrs/utils/typedef.py` & `gyver_attrs-0.9.1/gyver/attrs/utils/typedef.py`

 * *Files identical despite different names*

### Comparing `gyver_attrs-0.9.0/pyproject.toml` & `gyver_attrs-0.9.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "gyver-attrs"
-version = "0.9.0"
+version = "0.9.1"
 description = ""
 authors = ["Gustavo Cardoso <self.gustavocorrea@gmail.com>"]
 readme = "README.md"
 packages = [{ include = "gyver" }]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `gyver_attrs-0.9.0/PKG-INFO` & `gyver_attrs-0.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gyver-attrs
-Version: 0.9.0
+Version: 0.9.1
 Summary: 
 Author: Gustavo Cardoso
 Author-email: self.gustavocorrea@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

