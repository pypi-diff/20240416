# Comparing `tmp/lazy_type_hint-2.0.6.tar.gz` & `tmp/lazy_type_hint-2.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazy_type_hint-2.0.6.tar", max compression
+gzip compressed data, was "lazy_type_hint-2.0.7.tar", max compression
```

## Comparing `lazy_type_hint-2.0.6.tar` & `lazy_type_hint-2.0.7.tar`

### file list

```diff
@@ -1,39 +1,42 @@
--rw-r--r--   0        0        0      257 2024-04-03 13:39:39.210757 lazy_type_hint-2.0.6/lazy_type_hint/__init__.py
--rw-r--r--   0        0        0      495 2024-04-03 08:50:18.646693 lazy_type_hint-2.0.6/lazy_type_hint/data_type_tree/__init__.py
--rw-r--r--   0        0        0     9844 2024-04-14 13:10:15.517147 lazy_type_hint-2.0.6/lazy_type_hint/data_type_tree/data_type_tree.py
--rw-r--r--   0        0        0     5377 2024-04-14 12:56:14.695752 lazy_type_hint-2.0.6/lazy_type_hint/data_type_tree/factory.py
--rw-r--r--   0        0        0      833 2024-04-14 12:56:14.700751 lazy_type_hint-2.0.6/lazy_type_hint/data_type_tree/generic_type/__init__.py
--rw-r--r--   0        0        0    16935 2024-04-03 15:48:14.628513 lazy_type_hint-2.0.6/lazy_type_hint/data_type_tree/generic_type/dict_data_type_tree.py
--rw-r--r--   0        0        0     4020 2024-04-03 08:50:18.649845 lazy_type_hint-2.0.6/lazy_type_hint/data_type_tree/generic_type/generic_data_type_tree.py
--rw-r--r--   0        0        0     1131 2024-04-03 08:50:18.650845 lazy_type_hint-2.0.6/lazy_type_hint/data_type_tree/generic_type/list_data_type_tree.py
--rw-r--r--   0        0        0     4849 2024-04-14 10:52:55.353306 lazy_type_hint-2.0.6/lazy_type_hint/data_type_tree/generic_type/mapping_data_type_tree.py
--rw-r--r--   0        0        0      225 2024-04-03 08:50:18.651845 lazy_type_hint-2.0.6/lazy_type_hint/data_type_tree/generic_type/mapping_proxy_data_type_tree.py
--rw-r--r--   0        0        0     5631 2024-04-15 11:24:42.289742 lazy_type_hint-2.0.6/lazy_type_hint/data_type_tree/generic_type/pandas_data_frame_data_type_tree.py
--rw-r--r--   0        0        0      767 2024-04-03 08:50:18.652845 lazy_type_hint-2.0.6/lazy_type_hint/data_type_tree/generic_type/sequence_data_type_tree.py
--rw-r--r--   0        0        0     6525 2024-04-15 06:58:33.554062 lazy_type_hint-2.0.6/lazy_type_hint/data_type_tree/generic_type/set_and_sequence_operations.py
--rw-r--r--   0        0        0     1562 2024-04-03 08:50:18.652845 lazy_type_hint-2.0.6/lazy_type_hint/data_type_tree/generic_type/set_data_type_tree.py
--rw-r--r--   0        0        0     2138 2024-04-14 09:58:33.082160 lazy_type_hint-2.0.6/lazy_type_hint/data_type_tree/generic_type/tuple_data_type_tree.py
--rw-r--r--   0        0        0      798 2024-04-14 12:56:14.714038 lazy_type_hint-2.0.6/lazy_type_hint/data_type_tree/simple_data_type_tree/__init__.py
--rw-r--r--   0        0        0     2446 2024-04-03 08:50:18.654846 lazy_type_hint-2.0.6/lazy_type_hint/data_type_tree/simple_data_type_tree/function_data_type_tree.py
--rw-r--r--   0        0        0      993 2024-04-03 08:50:18.654846 lazy_type_hint-2.0.6/lazy_type_hint/data_type_tree/simple_data_type_tree/instance_data_type_tree.py
--rw-r--r--   0        0        0      436 2024-04-14 12:56:14.719035 lazy_type_hint-2.0.6/lazy_type_hint/data_type_tree/simple_data_type_tree/pandas_series_data_type_tree.py
--rw-r--r--   0        0        0     1003 2024-04-14 10:39:38.880313 lazy_type_hint-2.0.6/lazy_type_hint/data_type_tree/simple_data_type_tree/simple_data_type_tree.py
--rw-r--r--   0        0        0      752 2024-04-03 08:50:18.655845 lazy_type_hint-2.0.6/lazy_type_hint/data_type_tree/simple_data_type_tree/type_data_type_tree.py
--rw-r--r--   0        0        0      192 2024-04-03 08:50:18.656845 lazy_type_hint-2.0.6/lazy_type_hint/file_modifiers/__init__.py
--rw-r--r--   0        0        0    11392 2024-04-03 15:48:14.641664 lazy_type_hint-2.0.6/lazy_type_hint/file_modifiers/py_file_modifier.py
--rw-r--r--   0        0        0    17473 2024-04-03 08:50:18.657845 lazy_type_hint-2.0.6/lazy_type_hint/file_modifiers/yaml_file_modifier.py
--rw-r--r--   0        0        0     2340 2024-04-15 06:56:34.375018 lazy_type_hint-2.0.6/lazy_type_hint/generators/lazy_type_hint.py
--rw-r--r--   0        0        0     3137 2024-04-15 11:24:42.296743 lazy_type_hint-2.0.6/lazy_type_hint/generators/lazy_type_hint_abc.py
--rw-r--r--   0        0        0     8646 2024-04-15 11:24:42.302827 lazy_type_hint-2.0.6/lazy_type_hint/generators/lazy_type_hint_live.py
--rw-r--r--   0        0        0        0 2024-04-03 08:50:18.658845 lazy_type_hint-2.0.6/lazy_type_hint/py.typed
--rw-r--r--   0        0        0     1809 2024-04-15 11:24:42.310740 lazy_type_hint-2.0.6/lazy_type_hint/strategies.py
--rw-r--r--   0        0        0      706 2024-04-03 13:39:39.229769 lazy_type_hint-2.0.6/lazy_type_hint/utils/__init__.py
--rw-r--r--   0        0        0     2303 2024-04-03 08:50:18.660845 lazy_type_hint-2.0.6/lazy_type_hint/utils/docstring_formatter.py
--rw-r--r--   0        0        0     5458 2024-04-14 12:56:14.735213 lazy_type_hint-2.0.6/lazy_type_hint/utils/import_manager.py
--rw-r--r--   0        0        0     5008 2024-04-14 13:10:20.018341 lazy_type_hint-2.0.6/lazy_type_hint/utils/mypy.py
--rw-r--r--   0        0        0     1275 2024-04-03 08:50:18.662845 lazy_type_hint-2.0.6/lazy_type_hint/utils/ordered_set.py
--rw-r--r--   0        0        0      669 2024-04-03 08:50:18.662845 lazy_type_hint-2.0.6/lazy_type_hint/utils/test_ordered_set.py
--rw-r--r--   0        0        0     3770 2024-04-03 15:48:14.655819 lazy_type_hint-2.0.6/lazy_type_hint/utils/utils.py
--rw-r--r--   0        0        0     2397 2024-04-15 11:24:42.318741 lazy_type_hint-2.0.6/pyproject.toml
--rw-r--r--   0        0        0     6857 2024-04-15 06:41:49.885418 lazy_type_hint-2.0.6/README.md
--rw-r--r--   0        0        0     7246 1970-01-01 00:00:00.000000 lazy_type_hint-2.0.6/PKG-INFO
+-rw-r--r--   0        0        0      257 2024-04-03 13:39:39.210757 lazy_type_hint-2.0.7/lazy_type_hint/__init__.py
+-rw-r--r--   0        0        0      495 2024-04-03 08:50:18.646693 lazy_type_hint-2.0.7/lazy_type_hint/data_type_tree/__init__.py
+-rw-r--r--   0        0        0    10091 2024-04-15 15:41:02.041201 lazy_type_hint-2.0.7/lazy_type_hint/data_type_tree/data_type_tree.py
+-rw-r--r--   0        0        0     6810 2024-04-15 15:41:02.046201 lazy_type_hint-2.0.7/lazy_type_hint/data_type_tree/factory.py
+-rw-r--r--   0        0        0      969 2024-04-15 15:41:02.051201 lazy_type_hint-2.0.7/lazy_type_hint/data_type_tree/generic_type/__init__.py
+-rw-r--r--   0        0        0    16935 2024-04-03 15:48:14.628513 lazy_type_hint-2.0.7/lazy_type_hint/data_type_tree/generic_type/dict_data_type_tree.py
+-rw-r--r--   0        0        0     4020 2024-04-03 08:50:18.649845 lazy_type_hint-2.0.7/lazy_type_hint/data_type_tree/generic_type/generic_data_type_tree.py
+-rw-r--r--   0        0        0      772 2024-04-15 15:41:02.056201 lazy_type_hint-2.0.7/lazy_type_hint/data_type_tree/generic_type/iterator_data_type_tree.py
+-rw-r--r--   0        0        0     1091 2024-04-15 15:41:02.061200 lazy_type_hint-2.0.7/lazy_type_hint/data_type_tree/generic_type/list_data_type_tree.py
+-rw-r--r--   0        0        0     4803 2024-04-15 15:41:02.067200 lazy_type_hint-2.0.7/lazy_type_hint/data_type_tree/generic_type/mapping_data_type_tree.py
+-rw-r--r--   0        0        0      225 2024-04-03 08:50:18.651845 lazy_type_hint-2.0.7/lazy_type_hint/data_type_tree/generic_type/mapping_proxy_data_type_tree.py
+-rw-r--r--   0        0        0     5806 2024-04-15 15:41:02.072465 lazy_type_hint-2.0.7/lazy_type_hint/data_type_tree/generic_type/pandas_data_frame_data_type_tree.py
+-rw-r--r--   0        0        0      719 2024-04-15 15:41:02.076615 lazy_type_hint-2.0.7/lazy_type_hint/data_type_tree/generic_type/sequence_data_type_tree.py
+-rw-r--r--   0        0        0     6525 2024-04-15 06:58:33.554062 lazy_type_hint-2.0.7/lazy_type_hint/data_type_tree/generic_type/set_and_sequence_operations.py
+-rw-r--r--   0        0        0     1486 2024-04-15 15:41:02.081610 lazy_type_hint-2.0.7/lazy_type_hint/data_type_tree/generic_type/set_data_type_tree.py
+-rw-r--r--   0        0        0     2098 2024-04-15 15:41:02.086610 lazy_type_hint-2.0.7/lazy_type_hint/data_type_tree/generic_type/tuple_data_type_tree.py
+-rw-r--r--   0        0        0     1061 2024-04-15 15:41:02.091078 lazy_type_hint-2.0.7/lazy_type_hint/data_type_tree/simple_data_type_tree/__init__.py
+-rw-r--r--   0        0        0     2832 2024-04-15 15:41:02.092078 lazy_type_hint-2.0.7/lazy_type_hint/data_type_tree/simple_data_type_tree/function_data_type_tree.py
+-rw-r--r--   0        0        0     1060 2024-04-15 15:41:02.097066 lazy_type_hint-2.0.7/lazy_type_hint/data_type_tree/simple_data_type_tree/instance_data_type_tree.py
+-rw-r--r--   0        0        0      365 2024-04-15 15:41:02.101065 lazy_type_hint-2.0.7/lazy_type_hint/data_type_tree/simple_data_type_tree/io_data_type_tree.py
+-rw-r--r--   0        0        0      401 2024-04-15 15:41:02.105064 lazy_type_hint-2.0.7/lazy_type_hint/data_type_tree/simple_data_type_tree/module_data_type_tree.py
+-rw-r--r--   0        0        0      436 2024-04-14 12:56:14.719035 lazy_type_hint-2.0.7/lazy_type_hint/data_type_tree/simple_data_type_tree/pandas_series_data_type_tree.py
+-rw-r--r--   0        0        0     1003 2024-04-14 10:39:38.880313 lazy_type_hint-2.0.7/lazy_type_hint/data_type_tree/simple_data_type_tree/simple_data_type_tree.py
+-rw-r--r--   0        0        0      752 2024-04-03 08:50:18.655845 lazy_type_hint-2.0.7/lazy_type_hint/data_type_tree/simple_data_type_tree/type_data_type_tree.py
+-rw-r--r--   0        0        0      192 2024-04-03 08:50:18.656845 lazy_type_hint-2.0.7/lazy_type_hint/file_modifiers/__init__.py
+-rw-r--r--   0        0        0    11392 2024-04-03 15:48:14.641664 lazy_type_hint-2.0.7/lazy_type_hint/file_modifiers/py_file_modifier.py
+-rw-r--r--   0        0        0    17473 2024-04-03 08:50:18.657845 lazy_type_hint-2.0.7/lazy_type_hint/file_modifiers/yaml_file_modifier.py
+-rw-r--r--   0        0        0     2340 2024-04-15 06:56:34.375018 lazy_type_hint-2.0.7/lazy_type_hint/generators/lazy_type_hint.py
+-rw-r--r--   0        0        0     3137 2024-04-15 11:24:42.296743 lazy_type_hint-2.0.7/lazy_type_hint/generators/lazy_type_hint_abc.py
+-rw-r--r--   0        0        0     8646 2024-04-15 11:24:42.302827 lazy_type_hint-2.0.7/lazy_type_hint/generators/lazy_type_hint_live.py
+-rw-r--r--   0        0        0        0 2024-04-03 08:50:18.658845 lazy_type_hint-2.0.7/lazy_type_hint/py.typed
+-rw-r--r--   0        0        0     1809 2024-04-15 11:24:42.310740 lazy_type_hint-2.0.7/lazy_type_hint/strategies.py
+-rw-r--r--   0        0        0      706 2024-04-03 13:39:39.229769 lazy_type_hint-2.0.7/lazy_type_hint/utils/__init__.py
+-rw-r--r--   0        0        0     2303 2024-04-03 08:50:18.660845 lazy_type_hint-2.0.7/lazy_type_hint/utils/docstring_formatter.py
+-rw-r--r--   0        0        0     5655 2024-04-15 15:41:02.110072 lazy_type_hint-2.0.7/lazy_type_hint/utils/import_manager.py
+-rw-r--r--   0        0        0     5008 2024-04-14 13:10:20.018341 lazy_type_hint-2.0.7/lazy_type_hint/utils/mypy.py
+-rw-r--r--   0        0        0     1275 2024-04-03 08:50:18.662845 lazy_type_hint-2.0.7/lazy_type_hint/utils/ordered_set.py
+-rw-r--r--   0        0        0      669 2024-04-03 08:50:18.662845 lazy_type_hint-2.0.7/lazy_type_hint/utils/test_ordered_set.py
+-rw-r--r--   0        0        0     3770 2024-04-03 15:48:14.655819 lazy_type_hint-2.0.7/lazy_type_hint/utils/utils.py
+-rw-r--r--   0        0        0     2468 2024-04-15 15:41:14.843904 lazy_type_hint-2.0.7/pyproject.toml
+-rw-r--r--   0        0        0     6919 2024-04-15 15:41:02.034103 lazy_type_hint-2.0.7/README.md
+-rw-r--r--   0        0        0     7305 1970-01-01 00:00:00.000000 lazy_type_hint-2.0.7/PKG-INFO
```

### Comparing `lazy_type_hint-2.0.6/lazy_type_hint/data_type_tree/data_type_tree.py` & `lazy_type_hint-2.0.7/lazy_type_hint/data_type_tree/data_type_tree.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,22 +99,25 @@
         self.__pre_child_instantiation__()
         self.children = self._instantiate_children(data)
         self.height = self._get_height()
         self.__post_child_instantiation__()
 
     @classmethod
     def get_subclass(cls, data: object) -> Type[DataTypeTree]:
-        try:
-            return DataTypeTree.subclasses[type(data)]
-        except KeyError:
-            return DataTypeTree.subclasses[int]  # For instances created from any custom class.
+        for subclass in DataTypeTree.subclasses.values():
+            wraps = [subclass.wraps] if not isinstance(subclass.wraps, Iterable) else subclass.wraps
+            for wrap in wraps:
+                if isinstance(data, wrap):
+                    return subclass
+        return DataTypeTree.subclasses[int]  # For instances created from any custom class.
 
     def _check_tree_is_correct_one(self, data: object) -> None:
         wraps = self.wraps if isinstance(self.wraps, Iterable) else [self.wraps]
-        if type(data) not in wraps:
+        if not any(isinstance(data, wraps_) for wraps_ in wraps):
+            # if type(data) not in wraps:
             wraps_str = [element.__name__ for element in wraps]
             raise DataTypeTreeError(
                 f"The given parser ({type(self).__name__}) is meant to parse `{', '.join(wraps_str)}` data type but "
                 f"{type(data).__name__} was given"
             )
 
     def __pre_child_instantiation__(self) -> None:
```

### Comparing `lazy_type_hint-2.0.6/lazy_type_hint/data_type_tree/factory.py` & `lazy_type_hint-2.0.7/lazy_type_hint/data_type_tree/factory.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,44 +1,88 @@
-from typing import TYPE_CHECKING, overload
+from typing import TYPE_CHECKING, Iterator, overload
 
 from lazy_type_hint.data_type_tree.data_type_tree import DataTypeTree
 from lazy_type_hint.strategies import ParsingStrategies
 
 if TYPE_CHECKING:
-    from types import MappingProxyType
+    from types import MappingProxyType, ModuleType
     from typing import (
         Any,
         Dict,
         FrozenSet,
+        Iterator,
         List,
         Mapping,
         Optional,
         Sequence,
         Set,
+        TextIO,
         Tuple,
         Union,
     )
 
     import pandas as pd
 
     from lazy_type_hint.data_type_tree.generic_type.dict_data_type_tree import DictDataTypeTree
+    from lazy_type_hint.data_type_tree.generic_type.iterator_data_type_tree import IteratorDataTypeTree
     from lazy_type_hint.data_type_tree.generic_type.list_data_type_tree import ListDataTypeTree
     from lazy_type_hint.data_type_tree.generic_type.mapping_data_type_tree import MappingDataTypeTree
     from lazy_type_hint.data_type_tree.generic_type.pandas_data_frame_data_type_tree import PandasDataFrameDataTypeTree
     from lazy_type_hint.data_type_tree.generic_type.sequence_data_type_tree import SequenceDataTypeTree
     from lazy_type_hint.data_type_tree.generic_type.set_data_type_tree import SetDataTypeTree
     from lazy_type_hint.data_type_tree.generic_type.tuple_data_type_tree import TupleDataTypeTree
-    from lazy_type_hint.data_type_tree.simple_data_type_tree.simple_data_type_tree import SimpleDataTypeTree
+    from lazy_type_hint.data_type_tree.simple_data_type_tree.io_data_type_tree import IoDataTypeTree
+    from lazy_type_hint.data_type_tree.simple_data_type_tree.module_data_type_tree import ModuleTypeDataTypeTree
     from lazy_type_hint.data_type_tree.simple_data_type_tree.pandas_series_data_type_tree import (
         PandasSeriesDataTypeTree,
     )
+    from lazy_type_hint.data_type_tree.simple_data_type_tree.simple_data_type_tree import SimpleDataTypeTree
     from lazy_type_hint.utils import ImportManager
 
 
 @overload
+def data_type_tree_factory(  # type: ignore[overload-overlap]
+    data: "Iterator[Any]",
+    name: str,
+    *,
+    imports: "Optional[ImportManager]" = None,
+    depth: int = 0,
+    strategies: ParsingStrategies = ParsingStrategies(),  # noqa: B008
+    parent: "Optional[DataTypeTree]" = None,
+) -> "IteratorDataTypeTree":
+    ...
+
+
+@overload
+def data_type_tree_factory(  # type: ignore[overload-overlap]
+    data: "ModuleType",
+    name: str,
+    *,
+    imports: "Optional[ImportManager]" = None,
+    depth: int = 0,
+    strategies: ParsingStrategies = ParsingStrategies(),  # noqa: B008
+    parent: "Optional[DataTypeTree]" = None,
+) -> "ModuleTypeDataTypeTree":
+    ...
+
+
+@overload
+def data_type_tree_factory(  # type: ignore[overload-overlap]
+    data: "TextIO",
+    name: str,
+    *,
+    imports: "Optional[ImportManager]" = None,
+    depth: int = 0,
+    strategies: ParsingStrategies = ParsingStrategies(),  # noqa: B008
+    parent: "Optional[DataTypeTree]" = None,
+) -> "IoDataTypeTree":
+    ...
+
+
+@overload
 def data_type_tree_factory(
     data: "pd.Series",
     name: str,
     *,
     imports: "Optional[ImportManager]" = None,
     depth: int = 0,
     strategies: ParsingStrategies = ParsingStrategies(),  # noqa: B008
```

### Comparing `lazy_type_hint-2.0.6/lazy_type_hint/data_type_tree/generic_type/__init__.py` & `lazy_type_hint-2.0.7/lazy_type_hint/data_type_tree/generic_type/__init__.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,11 +6,14 @@
     MappingDataTypeTree as MappingDataTypeTree,
 )
 
 with suppress(ImportError):
     from lazy_type_hint.data_type_tree.generic_type.pandas_data_frame_data_type_tree import (
         PandasDataFrameDataTypeTree as PandasDataFrameDataTypeTree,
     )
+from lazy_type_hint.data_type_tree.generic_type.iterator_data_type_tree import (
+    IteratorDataTypeTree as IteratorDataTypeTree,
+)
 from lazy_type_hint.data_type_tree.generic_type.set_data_type_tree import SetDataTypeTree as SetDataTypeTree
 from lazy_type_hint.data_type_tree.generic_type.tuple_data_type_tree import (
     TupleDataTypeTree as TupleDataTypeTree,
 )
```

### Comparing `lazy_type_hint-2.0.6/lazy_type_hint/data_type_tree/generic_type/dict_data_type_tree.py` & `lazy_type_hint-2.0.7/lazy_type_hint/data_type_tree/generic_type/dict_data_type_tree.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.6/lazy_type_hint/data_type_tree/generic_type/generic_data_type_tree.py` & `lazy_type_hint-2.0.7/lazy_type_hint/data_type_tree/generic_type/generic_data_type_tree.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.6/lazy_type_hint/data_type_tree/generic_type/list_data_type_tree.py` & `lazy_type_hint-2.0.7/lazy_type_hint/data_type_tree/generic_type/list_data_type_tree.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,20 +1,19 @@
-from typing import Any, List, Sequence, Tuple
+from typing import Any, Sequence, Tuple
 
 from typing_extensions import override
 
 from lazy_type_hint.data_type_tree.data_type_tree import DataTypeTree, DataTypeTreeError
 from lazy_type_hint.data_type_tree.generic_type.sequence_data_type_tree import (
     SequenceDataTypeTree,
 )
 
 
 class ListDataTypeTree(SequenceDataTypeTree):
     wraps = list
-    original_data = List[object]
 
     @override
     def _instantiate_children(self, data: Sequence[Any]) -> Tuple[DataTypeTree, ...]:  # type: ignore
         return self.operations.instantiate_children(data, allow_repeated_children=False)
 
     @override
     def _get_str_top_node(self) -> str:
```

### Comparing `lazy_type_hint-2.0.6/lazy_type_hint/data_type_tree/generic_type/mapping_data_type_tree.py` & `lazy_type_hint-2.0.7/lazy_type_hint/data_type_tree/generic_type/mapping_data_type_tree.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,15 +9,14 @@
 from lazy_type_hint.data_type_tree.generic_type.generic_data_type_tree import GenericDataTypeTree
 from lazy_type_hint.file_modifiers.yaml_file_modifier import YamlFileModifier
 
 
 class MappingDataTypeTree(GenericDataTypeTree):
     children: Mapping[Hashable, DataTypeTree]
     wraps = MappingProxyType
-    original_data: Mapping[Hashable, object]
     hidden_keys_prefix: Final = YamlFileModifier.prefix
 
     # Iterable-protocol related
     _keys: Iterator[Hashable]
 
     @override
     def _instantiate_children(self, data: Mapping[Hashable, object]) -> Mapping[Hashable, DataTypeTree]:  # type: ignore
```

### Comparing `lazy_type_hint-2.0.6/lazy_type_hint/data_type_tree/generic_type/pandas_data_frame_data_type_tree.py` & `lazy_type_hint-2.0.7/lazy_type_hint/data_type_tree/generic_type/pandas_data_frame_data_type_tree.py`

 * *Files 2% similar despite different names*

```diff
@@ -104,14 +104,19 @@
         )
 
     @override
     def _instantiate_children(self, data: Mapping[str, object]) -> Mapping[str, DataTypeTree]:  # type: ignore
         children: Dict[str, DataTypeTree] = {}
         if not self.are_columns_either_all_str_or_all_tuple:
             return children
+
+        # Corner case to avoid infinite recursion
+        if all(isinstance(column, tuple) and len(column) == 1 for column in self.data.columns):
+            return {}
+
         for column in self.data.columns:
             if not self.can_be_accessed_multilevel:  # Here all columns will  be str
                 children[column] = self._create_child(column)
             else:  # Here all columns will be tuple
                 columns_processed: Set[str] = set()
                 for column in self.data.columns:
                     if column[0] not in columns_processed:
```

### Comparing `lazy_type_hint-2.0.6/lazy_type_hint/data_type_tree/generic_type/sequence_data_type_tree.py` & `lazy_type_hint-2.0.7/lazy_type_hint/data_type_tree/generic_type/sequence_data_type_tree.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,19 +1,18 @@
-from typing import Hashable, List, Sequence
+from typing import Hashable, List
 
 from typing_extensions import override
 
 from lazy_type_hint.data_type_tree.generic_type.generic_data_type_tree import (
     GenericDataTypeTree,
 )
 from lazy_type_hint.data_type_tree.generic_type.set_and_sequence_operations import SetAndSequenceOperations
 
 
 class SequenceDataTypeTree(GenericDataTypeTree):
-    original_data = Sequence[object]
     operations: SetAndSequenceOperations
 
     @override
     def __pre_child_instantiation__(self) -> None:
         self.operations = SetAndSequenceOperations(self)
 
     @override
```

### Comparing `lazy_type_hint-2.0.6/lazy_type_hint/data_type_tree/generic_type/set_and_sequence_operations.py` & `lazy_type_hint-2.0.7/lazy_type_hint/data_type_tree/generic_type/set_and_sequence_operations.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.6/lazy_type_hint/data_type_tree/generic_type/set_data_type_tree.py` & `lazy_type_hint-2.0.7/lazy_type_hint/data_type_tree/generic_type/set_data_type_tree.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,21 @@
-from typing import Any, FrozenSet, Hashable, Literal, Sequence, Set, Tuple, Union
+from typing import Any, Hashable, Literal, Sequence, Set, Tuple
 
 from typing_extensions import override
 
 from lazy_type_hint.data_type_tree.data_type_tree import DataTypeTree
 from lazy_type_hint.data_type_tree.generic_type.generic_data_type_tree import (
     GenericDataTypeTree,
 )
 from lazy_type_hint.data_type_tree.generic_type.set_and_sequence_operations import SetAndSequenceOperations
 
 
 class SetDataTypeTree(GenericDataTypeTree):
     wraps = (frozenset, set)
     children: Sequence[DataTypeTree]
-    original_data: Union[Set[object], FrozenSet[object]]
     operations: SetAndSequenceOperations
 
     @override
     def __pre_child_instantiation__(self) -> None:
         self.operations = SetAndSequenceOperations(self)
 
     @override
```

### Comparing `lazy_type_hint-2.0.6/lazy_type_hint/data_type_tree/generic_type/tuple_data_type_tree.py` & `lazy_type_hint-2.0.7/lazy_type_hint/data_type_tree/generic_type/tuple_data_type_tree.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,14 @@
 
 from lazy_type_hint.data_type_tree import DataTypeTree
 from lazy_type_hint.data_type_tree.generic_type.sequence_data_type_tree import SequenceDataTypeTree
 
 
 class TupleDataTypeTree(SequenceDataTypeTree):
     wraps = tuple
-    original_data = Tuple[object, ...]
 
     @override
     def _instantiate_children(self, data: Sequence[Any]) -> Tuple[DataTypeTree, ...]:  # type: ignore
         if self.strategies.tuple_size_strategy == "fixed":
             return self.operations.instantiate_children(data, allow_repeated_children=True)
         else:
             return self.operations.instantiate_children(data, allow_repeated_children=False)
```

### Comparing `lazy_type_hint-2.0.6/lazy_type_hint/data_type_tree/simple_data_type_tree/__init__.py` & `lazy_type_hint-2.0.7/lazy_type_hint/data_type_tree/simple_data_type_tree/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -7,13 +7,17 @@
     InstanceDataTypeTree as InstanceDataTypeTree,
 )
 
 with suppress(ImportError):
     from lazy_type_hint.data_type_tree.simple_data_type_tree.pandas_series_data_type_tree import (
         PandasSeriesDataTypeTree as PandasSeriesDataTypeTree,
     )
+from lazy_type_hint.data_type_tree.simple_data_type_tree.io_data_type_tree import IoDataTypeTree as IoDataTypeTree
+from lazy_type_hint.data_type_tree.simple_data_type_tree.module_data_type_tree import (
+    ModuleTypeDataTypeTree as ModuleTypeDataTypeTree,
+)
 from lazy_type_hint.data_type_tree.simple_data_type_tree.simple_data_type_tree import (
     SimpleDataTypeTree as SimpleDataTypeTree,
 )
 from lazy_type_hint.data_type_tree.simple_data_type_tree.type_data_type_tree import (
     TypeDataTypeTree as TypeDataTypeTree,
 )
```

### Comparing `lazy_type_hint-2.0.6/lazy_type_hint/data_type_tree/simple_data_type_tree/function_data_type_tree.py` & `lazy_type_hint-2.0.7/lazy_type_hint/data_type_tree/simple_data_type_tree/function_data_type_tree.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,36 +1,47 @@
 import ast
 import inspect
 import textwrap
 from inspect import Parameter
-from types import FunctionType, MappingProxyType
+from types import BuiltinFunctionType, FunctionType, MappingProxyType, MethodType
 from typing import Any, Callable, Hashable, Optional
 
 from typing_extensions import override
 
 from lazy_type_hint.data_type_tree.simple_data_type_tree.simple_data_type_tree import SimpleDataTypeTree
 from lazy_type_hint.utils import TAB
 
 
 class FunctionDataTypeTree(SimpleDataTypeTree):
-    wraps = (FunctionType, staticmethod, classmethod)
+    wraps = (FunctionType, staticmethod, classmethod, BuiltinFunctionType, MethodType)
     data: Callable[[Any], Any]
 
     @property
     def is_lambda(self) -> bool:
         return bool(self.data.__name__ == "<lambda>")
 
     @override
     @property
     def permission_to_be_created_as_type_alias(self) -> bool:
         if self.is_lambda or self.parent is None:
             return True
         return True
 
+    @property
+    def can_be_inspected(self) -> bool:
+        try:
+            inspect.signature(self.data)
+            return True
+        except ValueError:
+            return False
+
     def _get_str_top_node(self) -> str:
+        if not self.can_be_inspected:
+            self.imports.add("Callable")
+            return f"{self.name} = Callable"
         if self.is_lambda:
             return self._get_lambda_str()
         return self._get_protocol_str()
 
     def _get_protocol_str(self) -> str:
         args = str(inspect.signature(self.data))
         self.imports.add("Protocol")
```

### Comparing `lazy_type_hint-2.0.6/lazy_type_hint/data_type_tree/simple_data_type_tree/instance_data_type_tree.py` & `lazy_type_hint-2.0.7/lazy_type_hint/data_type_tree/simple_data_type_tree/instance_data_type_tree.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 from typing_extensions import override
 
 from lazy_type_hint.data_type_tree.simple_data_type_tree.simple_data_type_tree import SimpleDataTypeTree
 
 
 class InstanceDataTypeTree(SimpleDataTypeTree):
+    # Change it by `NoneType` once I drop support with Python 3.8
     wraps = (bool, int, float, range, slice, str, type(None))  # + Custom classes
 
     @override
     def _get_str_top_node(self) -> str:
         if self.holding_type == type(None):
             self.imports.add("Optional")
             return f"{self.name} = Optional[object]"
```

### Comparing `lazy_type_hint-2.0.6/lazy_type_hint/data_type_tree/simple_data_type_tree/simple_data_type_tree.py` & `lazy_type_hint-2.0.7/lazy_type_hint/data_type_tree/simple_data_type_tree/simple_data_type_tree.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.6/lazy_type_hint/data_type_tree/simple_data_type_tree/type_data_type_tree.py` & `lazy_type_hint-2.0.7/lazy_type_hint/data_type_tree/simple_data_type_tree/type_data_type_tree.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.6/lazy_type_hint/file_modifiers/py_file_modifier.py` & `lazy_type_hint-2.0.7/lazy_type_hint/file_modifiers/py_file_modifier.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.6/lazy_type_hint/file_modifiers/yaml_file_modifier.py` & `lazy_type_hint-2.0.7/lazy_type_hint/file_modifiers/yaml_file_modifier.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.6/lazy_type_hint/generators/lazy_type_hint.py` & `lazy_type_hint-2.0.7/lazy_type_hint/generators/lazy_type_hint.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.6/lazy_type_hint/generators/lazy_type_hint_abc.py` & `lazy_type_hint-2.0.7/lazy_type_hint/generators/lazy_type_hint_abc.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.6/lazy_type_hint/generators/lazy_type_hint_live.py` & `lazy_type_hint-2.0.7/lazy_type_hint/generators/lazy_type_hint_live.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.6/lazy_type_hint/strategies.py` & `lazy_type_hint-2.0.7/lazy_type_hint/strategies.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.6/lazy_type_hint/utils/__init__.py` & `lazy_type_hint-2.0.7/lazy_type_hint/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.6/lazy_type_hint/utils/docstring_formatter.py` & `lazy_type_hint-2.0.7/lazy_type_hint/utils/docstring_formatter.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.6/lazy_type_hint/utils/import_manager.py` & `lazy_type_hint-2.0.7/lazy_type_hint/utils/import_manager.py`

 * *Files 9% similar despite different names*

```diff
@@ -26,20 +26,23 @@
     "Any",
     "Union",
     "Optional",
     "NotRequired",
     "ReadOnly",
     "Callable",
     "Protocol",
+    "Iterator",
     "Literal",
     "overload",
     "pandas",
     "pd.Scalar",
     "npt",
     "numpy",
+    "ModuleType",
+    "TextIO",
 ]
 
 
 @dataclass(frozen=True)
 class ImportManager:
     _set: Set[KEYWORDS_AVAILABLE] = field(default_factory=set)
 
@@ -59,22 +62,25 @@
             "TypedDict": ("typing", "TypedDict"),
             "Any": ("typing", "Any"),
             "Union": ("typing", "Union"),
             "Optional": ("typing", "Optional"),
             "NotRequired": ("typing_extensions", "NotRequired"),
             "ReadOnly": ("typing_extensions", "ReadOnly"),
             "Callable": ("typing", "Callable"),
+            "ModuleType": ("types", "ModuleType"),
             "Protocol": ("typing", "Protocol"),
             "Literal": ("typing", "Literal"),
             "overload": ("typing", "overload"),
             "pandas": ("pandas", "pandas"),
             "npt": ("npt", "npt"),
             "numpy": ("numpy", "numpy"),
             "TypeAlias": ("typing_extenions", "TypeAlias"),
             "pd.Scalar": ("pandas._typing", "Scalar"),
+            "TextIO": ("typing", "TextIO"),
+            "Iterator": ("typing", "Iterator"),
         }
     )
 
     def add(self, keyword: KEYWORDS_AVAILABLE) -> "Self":
         self._set.add(keyword)
         return self
```

### Comparing `lazy_type_hint-2.0.6/lazy_type_hint/utils/mypy.py` & `lazy_type_hint-2.0.7/lazy_type_hint/utils/mypy.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.6/lazy_type_hint/utils/ordered_set.py` & `lazy_type_hint-2.0.7/lazy_type_hint/utils/ordered_set.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.6/lazy_type_hint/utils/test_ordered_set.py` & `lazy_type_hint-2.0.7/lazy_type_hint/utils/test_ordered_set.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.6/lazy_type_hint/utils/utils.py` & `lazy_type_hint-2.0.7/lazy_type_hint/utils/utils.py`

 * *Files identical despite different names*

### Comparing `lazy_type_hint-2.0.6/pyproject.toml` & `lazy_type_hint-2.0.7/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "lazy-type-hint"
-version = "2.0.6"
+version = "2.0.7"
 description = "Automate type hint generation in an easy way."
 authors = ["Manuel Floriano Vázquez <mflovaa@gmail.com>"]
 readme = "README.md"
 
 [tool.poetry.urls]
 Source = "https://github.com/mflova/lazy-type-hint"
 
@@ -65,9 +65,10 @@
 "lazy_type_hint/**/lazy_type_hint*.py" = ["ARG002"]
 
 [tool.codespell]
 ignore-words-list = "bu"  # Comma separated
 
 [tool.pytest.ini_options]
 # addopts = "-vv"
-addopts = "-n auto"
+# addopts = ["-n", "auto", "-m", "not integration"]
+addopts = ["-n", "auto"]  # All tests
 testpaths = ["tests"]
```

### Comparing `lazy_type_hint-2.0.6/README.md` & `lazy_type_hint-2.0.7/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -199,9 +199,12 @@
  
 Structures that can be type hinted:
  - Sequences: list, tuples
  - Sets: sets, frozensets
  - Dictionaries: dict, MappingProxyType
  - Pandas DataFrame: Full support for string-based columns and `MultiIndex` columns
  - Simple built-in types: bool, int, float, range, slice, None, str
- - Callables: lambdas, functions, staticmethods, classmethods
+ - Callables: lambdas, functions, staticmethods, classmethods, built-in functions
+ - Module types
+ - IOBase
+ - Iterators
  - Custom objects: instances and classes
```

### Comparing `lazy_type_hint-2.0.6/PKG-INFO` & `lazy_type_hint-2.0.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazy-type-hint
-Version: 2.0.6
+Version: 2.0.7
 Summary: Automate type hint generation in an easy way.
 Author: Manuel Floriano Vázquez
 Author-email: mflovaa@gmail.com
 Requires-Python: >=3.8,<=3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -215,9 +215,12 @@
  
 Structures that can be type hinted:
  - Sequences: list, tuples
  - Sets: sets, frozensets
  - Dictionaries: dict, MappingProxyType
  - Pandas DataFrame: Full support for string-based columns and `MultiIndex` columns
  - Simple built-in types: bool, int, float, range, slice, None, str
- - Callables: lambdas, functions, staticmethods, classmethods
+ - Callables: lambdas, functions, staticmethods, classmethods, built-in functions
+ - Module types
+ - IOBase
+ - Iterators
  - Custom objects: instances and classes
```

