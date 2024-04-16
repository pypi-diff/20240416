# Comparing `tmp/py_transmuter-0.1.2.tar.gz` & `tmp/py_transmuter-0.2.0.tar.gz`

## Comparing `py_transmuter-0.1.2.tar` & `py_transmuter-0.2.0.tar`

### file list

```diff
@@ -1,18 +1,25 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 py_transmuter-0.1.2/CONTRIBUTING.md
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 py_transmuter-0.1.2/dev-requirements.txt
--rw-r--r--   0        0        0      204 2020-02-02 00:00:00.000000 py_transmuter-0.1.2/py_transmuter/__init__.py
--rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 py_transmuter-0.1.2/py_transmuter/self_inspector.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 py_transmuter-0.1.2/py_transmuter/base/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 py_transmuter-0.1.2/py_transmuter/pydantic_mapping/__init__.py
--rw-r--r--   0        0        0     9504 2020-02-02 00:00:00.000000 py_transmuter-0.1.2/py_transmuter/pydantic_mapping/aggregator.py
--rw-r--r--   0        0        0     4607 2020-02-02 00:00:00.000000 py_transmuter-0.1.2/py_transmuter/pydantic_mapping/mapper.py
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 py_transmuter-0.1.2/py_transmuter/pydantic_mapping/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 py_transmuter-0.1.2/test/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 py_transmuter-0.1.2/test/pydantic/__init__.py
--rw-r--r--   0        0        0     9902 2020-02-02 00:00:00.000000 py_transmuter-0.1.2/test/pydantic/test_aggregator.py
--rw-r--r--   0        0        0     4789 2020-02-02 00:00:00.000000 py_transmuter-0.1.2/test/pydantic/test_mapper.py
--rw-r--r--   0        0        0     3087 2020-02-02 00:00:00.000000 py_transmuter-0.1.2/.gitignore
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 py_transmuter-0.1.2/LICENSE
--rw-r--r--   0        0        0     9061 2020-02-02 00:00:00.000000 py_transmuter-0.1.2/README.md
--rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 py_transmuter-0.1.2/pyproject.toml
--rw-r--r--   0        0        0    11005 2020-02-02 00:00:00.000000 py_transmuter-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 py_transmuter-0.2.0/CONTRIBUTING.md
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 py_transmuter-0.2.0/dev-requirements.txt
+-rw-r--r--   0        0        0      174 2020-02-02 00:00:00.000000 py_transmuter-0.2.0/.vscode/settings.json
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 py_transmuter-0.2.0/py_transmuter/__init__.py
+-rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 py_transmuter-0.2.0/py_transmuter/self_inspector.py
+-rw-r--r--   0        0        0      190 2020-02-02 00:00:00.000000 py_transmuter-0.2.0/py_transmuter/dictionaries/__init__.py
+-rw-r--r--   0        0        0     8200 2020-02-02 00:00:00.000000 py_transmuter-0.2.0/py_transmuter/dictionaries/aggregator.py
+-rw-r--r--   0        0        0     3212 2020-02-02 00:00:00.000000 py_transmuter-0.2.0/py_transmuter/dictionaries/mapper.py
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 py_transmuter-0.2.0/py_transmuter/models/__init__.py
+-rw-r--r--   0        0        0     9400 2020-02-02 00:00:00.000000 py_transmuter-0.2.0/py_transmuter/models/aggregator.py
+-rw-r--r--   0        0        0     4503 2020-02-02 00:00:00.000000 py_transmuter-0.2.0/py_transmuter/models/mapper.py
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 py_transmuter-0.2.0/py_transmuter/models/types.py
+-rw-r--r--   0        0        0     1142 2020-02-02 00:00:00.000000 py_transmuter-0.2.0/py_transmuter/models/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 py_transmuter-0.2.0/test/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 py_transmuter-0.2.0/test/dictionaries/__init__.py
+-rw-r--r--   0        0        0     7323 2020-02-02 00:00:00.000000 py_transmuter-0.2.0/test/dictionaries/test_aggregator.py
+-rw-r--r--   0        0        0     2442 2020-02-02 00:00:00.000000 py_transmuter-0.2.0/test/dictionaries/test_mapper.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 py_transmuter-0.2.0/test/models/__init__.py
+-rw-r--r--   0        0        0    10608 2020-02-02 00:00:00.000000 py_transmuter-0.2.0/test/models/test_aggregator.py
+-rw-r--r--   0        0        0     5360 2020-02-02 00:00:00.000000 py_transmuter-0.2.0/test/models/test_mapper.py
+-rw-r--r--   0        0        0     3087 2020-02-02 00:00:00.000000 py_transmuter-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 py_transmuter-0.2.0/LICENSE
+-rw-r--r--   0        0        0     9964 2020-02-02 00:00:00.000000 py_transmuter-0.2.0/README.md
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 py_transmuter-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0    11877 2020-02-02 00:00:00.000000 py_transmuter-0.2.0/PKG-INFO
```

### Comparing `py_transmuter-0.1.2/py_transmuter/self_inspector.py` & `py_transmuter-0.2.0/py_transmuter/self_inspector.py`

 * *Files identical despite different names*

### Comparing `py_transmuter-0.1.2/py_transmuter/pydantic_mapping/aggregator.py` & `py_transmuter-0.2.0/py_transmuter/models/aggregator.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,27 +1,22 @@
 from collections import defaultdict
 from typing import (
     Any,
     Callable,
     Generic,
     Mapping,
-    TypeVar,
     get_args,
 )
 
-from pydantic import BaseModel
-from py_transmuter.pydantic_mapping.utils import get_required_fields
+from py_transmuter.models.types import TargetModel, SourceModel
+from py_transmuter.models.utils import get_required_fields
 from py_transmuter.self_inspector import SelfInspector
 
 
-SourceModel = TypeVar("SourceModel", bound=BaseModel)
-TargetModel = TypeVar("TargetModel", bound=BaseModel)
-
-
-class BaseModelAggregator(Generic[TargetModel, SourceModel], SelfInspector):
+class ModelAggregator(Generic[TargetModel, SourceModel], SelfInspector):
     """
     Aggregator class that transforms a list of objects of the source model
     into a list of objects of the target model.
 
     Attributes:
         group_by (tuple[str | Callable[[SourceModel], Any], ...] | None):
             The fields to group the data by or methods that can extract a value to group by
```

### Comparing `py_transmuter-0.1.2/py_transmuter/pydantic_mapping/mapper.py` & `py_transmuter-0.2.0/py_transmuter/models/mapper.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,15 @@
-from typing import Any, Callable, Generic, Mapping, TypeVar, get_args
+from typing import Any, Callable, Generic, Mapping, get_args
 
-from pydantic import BaseModel
-
-from py_transmuter.pydantic_mapping.utils import get_required_fields
+from py_transmuter.models.types import TargetModel, SourceModel
+from py_transmuter.models.utils import get_required_fields
 from py_transmuter.self_inspector import SelfInspector
 
-SourceModel = TypeVar("SourceModel", bound=BaseModel)
-TargetModel = TypeVar("TargetModel", bound=BaseModel)
-
 
-class BaseModelMapper(Generic[TargetModel, SourceModel], SelfInspector):
+class ModelMapper(Generic[TargetModel, SourceModel], SelfInspector):
     """
     A generic mapper class that maps data from a source model to a target model.
 
     Attributes:
         mapping (Mapping[str, str | tuple[str, Callable[[Any], Any]] | Callable[[SourceModel], Any]):
             A mapping dictionary that defines the mapping between the fields of
             the source model and the target model.
@@ -21,15 +17,15 @@
                 - A string that represents the name of the field in the source model
                 - A tuple with the name of a field in the source model and a callable
                     that takes the value of the field in the source model and returns
                     the value of the field in the target model.
                 - A callable that takes the source model as an argument and returns
                     the value of the field in the target model.
         context (Mapping[str, Any] | None):
-            A dictionary that allows passing specific attributes to the aggregator
+            A dictionary that allows passing specific attributes to the mapper
             if they are instance specific not class wide. Defaults to None.
 
     Methods:
         map(data: SourceModel) -> TargetModel:
             Maps the data from the source model to a target model using the
             mapping dictionary.
         map_list(data: list[SourceModel]) -> list[TargetModel]:
```

### Comparing `py_transmuter-0.1.2/py_transmuter/pydantic_mapping/utils.py` & `py_transmuter-0.2.0/py_transmuter/models/utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import inspect
 from types import UnionType
 from typing import Optional, Union, get_type_hints
-from pydantic import BaseModel
 
+from py_transmuter.models.types import SupportsTypeHints
 
-def get_required_fields(model_cls: type[BaseModel]) -> list[str]:
+
+def get_required_fields(model_cls: type[SupportsTypeHints]) -> list[str]:
     required_fields = list()
 
     type_hints = get_type_hints(model_cls)
     for field, field_type in type_hints.items():
         # For Python 3.10 and later: Check if field_type is UnionType and contains None
         if isinstance(field_type, UnionType):
             if type(None) not in field_type.__args__:
```

### Comparing `py_transmuter-0.1.2/test/pydantic/test_aggregator.py` & `py_transmuter-0.2.0/test/models/test_aggregator.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,79 +1,113 @@
+from dataclasses import dataclass
 from datetime import date, datetime, timedelta
 from statistics import mean
 from pydantic import BaseModel
+from pydantic.dataclasses import dataclass as py_dataclass
 from pytest import raises
-from py_transmuter.pydantic.aggregator import BaseModelAggregator
+from py_transmuter.models.aggregator import ModelAggregator
 
 
 def test_aggregator_field_direct_mappings():
     class A(BaseModel):
         id: int
 
     class B(BaseModel):
         ids: list[int]
 
-    class ABAggregator(BaseModelAggregator[B, A]):
+    class ABAggregator(ModelAggregator[B, A]):
         mappings = {"ids": "id"}
 
     assert ABAggregator().aggregate([A(id=1), A(id=2), A(id=3)]) == [B(ids=[1, 2, 3])]
 
 
+def test_aggregator_dataclasses():
+    @py_dataclass
+    class A:
+        id: int
+
+    @dataclass
+    class B:
+        ids: list[int]
+
+    class DataClassAggregator(ModelAggregator[B, A]):
+        mappings = {"ids": "id"}
+
+    assert DataClassAggregator().aggregate([A(id=1), A(id=2), A(id=3)]) == [B(ids=[1, 2, 3])]
+
+
 def test_aggregator_tuple_direct_mappings():
     class A(BaseModel):
         id: int
 
     class B(BaseModel):
         ids: list[str]
 
-    class ABAggregator(BaseModelAggregator[B, A]):
+    class ABAggregator(ModelAggregator[B, A]):
         mappings = {"ids": ("id", lambda id: str(id))}
 
     assert ABAggregator().aggregate([A(id=1), A(id=2), A(id=3)]) == [
         B(ids=["1", "2", "3"])
     ]
 
 
+def test_cross_model_type_aggregator():
+    class A(BaseModel):
+        id: int
+
+    @dataclass
+    class B:
+        ids: list[str]
+
+    class ABMapper(ModelAggregator[B, A]):
+        mappings = {"ids": ("id", lambda value: str(value))}
+
+    assert ABMapper().aggregate([A(id=1), A(id=2), A(id=3)]) == [
+        B(ids=["1", "2", "3"]),
+    ]
+
+
 def test_aggregator_model_callable_direct_mappings():
     class A(BaseModel):
         first_name: str
         last_name: str
 
     class B(BaseModel):
         full_names: list[str]
 
     def make_full_name(data: A) -> str:
         return f"{data.first_name} {data.last_name}"
 
-    class ABAggregator(BaseModelAggregator[B, A]):
+    class ABAggregator(ModelAggregator[B, A]):
         mappings = {"full_names": make_full_name}
 
     assert ABAggregator().aggregate(
         [
             A(first_name="Rodrigo", last_name="De Rosa"),
             A(first_name="Marcelo", last_name="Gallardo"),
             A(first_name="Super", last_name="Man"),
         ]
     ) == [B(full_names=["Rodrigo De Rosa", "Marcelo Gallardo", "Super Man"])]
 
 
 def test_aggregator_field_direct_mappings_with_grouping():
-    class Child(BaseModel):
+    @dataclass
+    class Child:
         parent: str
 
         first_name: str
         last_name: str
 
     class Parent(BaseModel):
         children_names: list[str]
 
     def make_full_name(data: Child) -> str:
         return f"{data.first_name} {data.last_name}"
 
-    class ChildParentAggregator(BaseModelAggregator[Parent, Child]):
+    class ChildParentAggregator(ModelAggregator[Parent, Child]):
         group_by = ("parent",)
 
         mappings = {"children_names": make_full_name}
 
     assert ChildParentAggregator().aggregate(
         [
             Child(parent="Patricio", first_name="Rodrigo", last_name="De Rosa"),
@@ -92,15 +126,15 @@
 
         first_name: str
         last_name: str
 
     class Parent(BaseModel):
         children_names: list[str]
 
-    class ChildParentAggregator(BaseModelAggregator[Parent, Child]):
+    class ChildParentAggregator(ModelAggregator[Parent, Child]):
         @staticmethod
         def parent_full_name(data: Child) -> str:
             return f"{data.parent} {data.last_name}"
 
         group_by = (parent_full_name,)
 
         mappings = {"children_names": "first_name"}
@@ -120,15 +154,15 @@
         timestamp: datetime
         value: float
 
     class DayValues(BaseModel):
         intervals: list[datetime]
         values: list[float]
 
-    class DailyMeasurementAggregator(BaseModelAggregator[DayValues, Measurement]):
+    class DailyMeasurementAggregator(ModelAggregator[DayValues, Measurement]):
         @staticmethod
         def timestamp_date(data: Measurement) -> date:
             return data.timestamp.date()
 
         group_by = ("machine", timestamp_date)
 
         mappings = {"intervals": "timestamp", "values": "value"}
@@ -161,15 +195,15 @@
 def test_aggregator_with_sort_by_field():
     class A(BaseModel):
         id: int
 
     class B(BaseModel):
         ids: list[int]
 
-    class ABAggregator(BaseModelAggregator[B, A]):
+    class ABAggregator(ModelAggregator[B, A]):
         sort_by = ("id",)
 
         mappings = {"ids": "id"}
 
     assert ABAggregator().aggregate([A(id=3), A(id=1), A(id=2)]) == [B(ids=[1, 2, 3])]
 
 
@@ -180,15 +214,15 @@
 
     class Parent(BaseModel):
         children_names: list[str]
 
     def make_full_name(data: Child) -> str:
         return f"{data.first_name} {data.last_name}"
 
-    class ChildParentAggregator(BaseModelAggregator[Parent, Child]):
+    class ChildParentAggregator(ModelAggregator[Parent, Child]):
         sort_by = (make_full_name,)
 
         mappings = {"children_names": make_full_name}
 
     assert ChildParentAggregator().aggregate(
         [
             Child(first_name="Paul", last_name="Smith"),
@@ -207,15 +241,15 @@
     class Parent(BaseModel):
         children_names: list[str]
         ages: list[int]
 
     def make_full_name(data: Child) -> str:
         return f"{data.first_name} {data.last_name}"
 
-    class ChildParentAggregator(BaseModelAggregator[Parent, Child]):
+    class ChildParentAggregator(ModelAggregator[Parent, Child]):
         sort_by = (make_full_name, "age")
 
         mappings = {"children_names": make_full_name, "ages": "age"}
 
     assert ChildParentAggregator().aggregate(
         [
             Child(first_name="Paul", last_name="Smith", age=17),
@@ -236,15 +270,15 @@
     class Horizontal(BaseModel):
         values: list[float]
 
     def aggregate_values(values: list[float]) -> float:
         average = sum(values) / len(values)
         return [value / average for value in values]
 
-    class VerticalToHorizontalAggregator(BaseModelAggregator[Horizontal, Vertical]):
+    class VerticalToHorizontalAggregator(ModelAggregator[Horizontal, Vertical]):
         aggregations = {
             "values": ("value", aggregate_values),
         }
 
     assert VerticalToHorizontalAggregator().aggregate(
         [Vertical(value=6), Vertical(value=4), Vertical(value=2)]
     ) == [Horizontal(values=[1.5, 1, 0.5])]
@@ -264,15 +298,15 @@
 
     def average_coordinates(turbines: list[Turbine]) -> Coordinates:
         return Coordinates(
             latitude=mean(turbine.latitude for turbine in turbines),
             longitude=mean(turbine.longitude for turbine in turbines),
         )
 
-    class TurbineParkAggregator(BaseModelAggregator[Park, Turbine]):
+    class TurbineParkAggregator(ModelAggregator[Park, Turbine]):
         aggregations = {
             "location": average_coordinates,
         }
 
     assert TurbineParkAggregator().aggregate(
         [
             Turbine(latitude=10, longitude=5), 
@@ -287,15 +321,15 @@
         parent_id: int
         value: float
 
     class B(BaseModel):
         id: int
         values: list[float]
 
-    class ABAggregator(BaseModelAggregator[B, A]):
+    class ABAggregator(ModelAggregator[B, A]):
         group_by = ("parent_id",)
 
         mappings = {"values": "value"}
         aggregations = {"id": ("parent_id", lambda ids: ids[0])}
 
     assert ABAggregator().aggregate(
         [A(parent_id=1, value=10), A(parent_id=1, value=20), A(parent_id=2, value=30)]
@@ -305,31 +339,31 @@
 def test_aggregator_with_overlapping_mappings_and_aggregations_fails_to_create():
     class A(BaseModel):
         parent_id: int
 
     class B(BaseModel):
         id: int
 
-    class ABAggregator(BaseModelAggregator[B, A]):
+    class ABAggregator(ModelAggregator[B, A]):
         mappings = {"id": "parent_id"}
         aggregations = {"id": ("parent_id", lambda ids: ids[0])}
 
 
     with raises(ValueError):
         ABAggregator()
 
 
-def test_aggregator_without_mappings_or_aggregations():
+def test_aggregator_without_mappings_or_aggregations_fails_to_create():
     class A(BaseModel):
         id: int
 
     class B(BaseModel):
         id: int
 
-    class ABAggregator(BaseModelAggregator[B, A]):
+    class ABAggregator(ModelAggregator[B, A]):
         pass
 
     with raises(ValueError):
         ABAggregator()
 
 
 def test_aggregator_missing_required_fields():
@@ -337,27 +371,27 @@
         id: int
         value: float
 
     class B(BaseModel):
         id: int
         values: list[float]
 
-    class ABAggregator(BaseModelAggregator[B, A]):
+    class ABAggregator(ModelAggregator[B, A]):
         aggregations = {"values": "value"}
 
     with raises(ValueError):
         ABAggregator()
 
 
 def test_aggregator_with_extra_fields():
     class A(BaseModel):
         id: int
         value: float
 
     class B(BaseModel):
         id: int
 
-    class ABAggregator(BaseModelAggregator[B, A]):
+    class ABAggregator(ModelAggregator[B, A]):
         aggregations = {"id": "id", "values": "value"}
 
     with raises(ValueError):
         ABAggregator()
```

### Comparing `py_transmuter-0.1.2/test/pydantic/test_mapper.py` & `py_transmuter-0.2.0/test/models/test_mapper.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,63 +1,95 @@
+from dataclasses import dataclass
 from datetime import datetime
 from pydantic import BaseModel
+from pydantic.dataclasses import dataclass as py_dataclass
 from pytest import raises
-from py_transmuter.pydantic_mapping.mapper import BaseModelMapper
+from py_transmuter.models.mapper import ModelMapper
 
 
 def test_map_with_field_name():
     class A(BaseModel):
         id: int
 
     class B(BaseModel):
         id: int
 
-    class ABMapper(BaseModelMapper[B, A]):
+    class ABMapper(ModelMapper[B, A]):
         mapping = {"id": "id"}
 
     assert ABMapper().map(A(id=1)) == B(id=1)
 
 
+def test_map_dataclasses():
+    @dataclass
+    class A:
+        id: int
+
+    @py_dataclass
+    class B:
+        id: int
+
+    class DataClassMapper(ModelMapper[B, A]):
+        mapping = {"id": "id"}
+
+    assert DataClassMapper().map(A(id=1)) == B(id=1)
+
+
 def test_map_with_lambda():
     class A(BaseModel):
         id: int
 
     class B(BaseModel):
         id: str
 
-    class ABMapper(BaseModelMapper[B, A]):
+    class ABMapper(ModelMapper[B, A]):
         mapping = {"id": lambda data: str(data.id)}
 
     assert ABMapper().map(A(id=1)) == B(id="1")
 
 
+def test_cross_model_type_mapping():
+    class A(BaseModel):
+        id: int
+
+    @dataclass
+    class B:
+        id: str
+
+    class ABMapper(ModelMapper[B, A]):
+        mapping = {"id": ("id", lambda value: str(value))}
+    
+    assert ABMapper().map(A(id=1)) == B(id="1")
+
+
+
 def test_map_with_function():
     class A(BaseModel):
         id: int
 
     class B(BaseModel):
         id: str
 
     def map_id(data: A) -> str:
         return str(data.id * 10)
 
-    class ABMapper(BaseModelMapper[B, A]):
+    class ABMapper(ModelMapper[B, A]):
         mapping = {"id": map_id}
 
     assert ABMapper().map(A(id=1)) == B(id="10")
 
 
 def test_map_with_context_and_self_inspection():
     class A(BaseModel):
         id: int
 
     class B(BaseModel):
         id: str
 
-    class ABMapper(BaseModelMapper[B, A]):
+    class ABMapper(ModelMapper[B, A]):
         def map_id(self, data: A) -> str:
             return str(data.id * self.context["factor"])
 
         mapping = {"id": map_id}
 
     assert ABMapper(context={"factor": 2}).map(A(id=1)) == B(id="2")
 
@@ -65,15 +97,15 @@
 def test_map_with_class_method():
     class A(BaseModel):
         id: int
 
     class B(BaseModel):
         id: int
 
-    class ABMapper(BaseModelMapper[B, A]):
+    class ABMapper(ModelMapper[B, A]):
         FACTOR = 10
 
         @classmethod
         def map_id(cls, data: A) -> int:
             return data.id * cls.FACTOR
 
         mapping = {"id": map_id}
@@ -84,130 +116,131 @@
 def test_map_with_tuple_accessor():
     class A(BaseModel):
         id: int
 
     class B(BaseModel):
         id: int
 
-    class ABMapper(BaseModelMapper[B, A]):
+    class ABMapper(ModelMapper[B, A]):
         mapping = {"id": ("id", lambda value: value * 10)}
 
     assert ABMapper().map(A(id=1)) == B(id=10)
 
 
 def test_map_list():
     class A(BaseModel):
         id: int
 
     class B(BaseModel):
         id: int
 
-    class ABMapper(BaseModelMapper[B, A]):
+    class ABMapper(ModelMapper[B, A]):
         mapping = {"id": "id"}
 
     assert ABMapper().map_list([A(id=1), A(id=2)]) == [B(id=1), B(id=2)]
 
 
 def test_map_without_optional_fields():
     class A(BaseModel):
         id: int
 
     class B(BaseModel):
         id: int
         name: str | None = None
 
-    class ABMapper(BaseModelMapper[B, A]):
+    class ABMapper(ModelMapper[B, A]):
         mapping = {"id": "id"}
 
     assert ABMapper().map(A(id=1)) == B(id=1)
 
 
 def test_map_missing_required_field_fails():
     class A(BaseModel):
         id: int
 
     class B(BaseModel):
         id: int
         name: str
 
-    class ABMapper(BaseModelMapper[B, A]):
+    class ABMapper(ModelMapper[B, A]):
         mapping = {"id": "id"}
 
     with raises(ValueError):
         ABMapper()
 
 
 def test_map_extra_field_fails():
     class A(BaseModel):
         id: int
 
     class B(BaseModel):
         id: int
 
-    class ABMapper(BaseModelMapper[B, A]):
+    class ABMapper(ModelMapper[B, A]):
         mapping = {"id": "id", "name": "name"}
 
     with raises(ValueError):
         ABMapper()
 
 
 def test_map_with_optional_field():
     class A(BaseModel):
         id: int
 
     class B(BaseModel):
         id: int
         name: str | None = None
 
-    class ABMapper(BaseModelMapper[B, A]):
+    class ABMapper(ModelMapper[B, A]):
         mapping = {"id": "id", "name": lambda data: "Rodrigo"}
 
     assert ABMapper().map(A(id=1)) == B(id=1, name="Rodrigo")
 
 
 def test_map_complex_models():
     class WeatherDataBackend(BaseModel):
         temperature_fahrenheit: float
         humidity_proportion: float
         timestamp: datetime
-        
+
         country: str | None = None
 
     class WeatherDataUI(BaseModel):
         temperature_celsius: float
         humidity_percentage: int
         date: str
         time: str
 
         language: str
 
-    class WeatherDataMapper(BaseModelMapper[WeatherDataBackend, WeatherDataUI]):
+    class WeatherDataMapper(ModelMapper[WeatherDataBackend, WeatherDataUI]):
         @staticmethod
         def celsius_to_fahrenheit(celsius: float) -> float:
             return (celsius * 9 / 5) + 32
 
         @staticmethod
         def parse_date_time_to_object(data: WeatherDataUI) -> datetime:
-            return datetime.strptime(
-                f"{data.date} {data.time}", "%Y-%m-%d %H:%M"
-            )
+            return datetime.strptime(f"{data.date} {data.time}", "%Y-%m-%d %H:%M")
 
         mapping = {
             "temperature_fahrenheit": ("temperature_celsius", celsius_to_fahrenheit),
-            "humidity_proportion": ("humidity_percentage", lambda humidity: float(humidity) / 100),
+            "humidity_proportion": (
+                "humidity_percentage",
+                lambda humidity: float(humidity) / 100,
+            ),
             "timestamp": parse_date_time_to_object,
         }
 
     to_map = WeatherDataUI(
         temperature_celsius=10,
         humidity_percentage=50,
-        date="2021-01-01", 
+        date="2021-01-01",
         time="12:00",
         language="en",
     )
 
     mapped = WeatherDataMapper().map(to_map)
     assert mapped == WeatherDataBackend(
         temperature_fahrenheit=50.0,
         humidity_proportion=0.5,
-        timestamp=datetime(2021, 1, 1, 12)
+        timestamp=datetime(2021, 1, 1, 12),
     )
```

### Comparing `py_transmuter-0.1.2/.gitignore` & `py_transmuter-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `py_transmuter-0.1.2/LICENSE` & `py_transmuter-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `py_transmuter-0.1.2/README.md` & `py_transmuter-0.2.0/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,62 +1,63 @@
 # PyTransmuter
 
-PyTransmuter is a Python library designed for efficient data mapping and aggregation 
-from source models to target models, leveraging the power of Pydantic for data validation
-and transformation. It simplifies the process of transforming data structures, making it 
-an essential tool for applications requiring data normalization, transformation, and aggregation.
+PyTransmuter is a Python library designed for efficient data mapping and aggregation from source 
+models to target models. It simplifies the process of transforming data structures, even between classes
+of different types (this is, you can transform from a `BaseModel` to a `@dataclass` if you need to) or 
+even transform data in Python dictionaries.
 
 ## Features
 
-- **Generic Mapping**: Utilizes generic typing to map data between different model structures.
+- **Generic Mapping**: Utilizes generic typing to map data between different model structures; for example, Python's `@dataclass`, 
+Pydantic's `BaseModel`, Pydantic's `@dataclass` or even plain dictionaries.
 - **Flexible Aggregation**: Supports complex data aggregation strategies, including grouping, 
 sorting, and custom aggregation functions.
 - **Self-Inspection**: Incorporates self-inspection capabilities for resolving callables related 
 to class instances.
-- **Pydantic Integration**: Leverages Pydantic models for input and output validation, ensuring 
-data integrity.
 - **Customizable Transformations**: Allows defining custom field transformations using callable 
 functions or lambdas.
 
 ## Installation
 
 To install the library, run the following command in your terminal:
 
 ```bash
 pip install py-transmuter
 ```
 
-## Usage of the Mapper
+## Usage of the ModelMapper
 
 ### Basic Setup
 
-Start by defining your source and target Pydantic models that represent the structure of your input and output data:
+Start by defining your source and target models that represent the structure of your input and output data:
 
 ```python
 from pydantic import BaseModel
+from dataclasses import dataclass
 
-class SourceModel(BaseModel):
+@dataclass
+class SourceModel:
     id: int
     temperature_celsius: float
     humidity_percentage: int
 
 class TargetModel(BaseModel):
     id: int
     temperature_fahrenheit: float
     humidity_proportion: float
 ```
 
-### Implementing a Mapper
+### Implementing a ModelMapper
 
-Define a mapper by inheriting from `BaseModelMapper`, specifying how each field in the source model maps to the target model:
+Define a mapper by inheriting from `ModelMapper`, specifying how each field in the source model maps to the target model:
 
 ```python
-from py_transmuter.pydantic.mapper import BaseModelMapper
+from py_transmuter.models.mapper import ModelMapper
 
-class MyMapper(BaseModelMapper[TargetModel, SourceModel]):
+class MyMapper(ModelMapper[TargetModel, SourceModel]):
     mapping = {
         "id": "id",
         "temperature_fahrenheit": ("temperature_celsius", lambda c: c * 9 / 5 + 32),
         "humidity_proportion": ("humidity_percentage", lambda h: h / 100.0),
     }
 ```
 
@@ -72,15 +73,15 @@
 
 print(target_data)
 # Output: TargetModel(id=1, temperature_fahrenheit=77.0, humidity_proportion=0.5)
 ```
 
 ### Mapping Lists of Data
 
-`BaseModelMapper` also supports mapping lists of data from source models to target models:
+`ModelMapper` also supports mapping lists of data from source models to target models:
 
 ```python
 source_list = [
     SourceModel(id=1, temperature_celsius=25, humidity_percentage=50),
     SourceModel(id=2, temperature_celsius=20, humidity_percentage=60),
 ]
 
@@ -88,44 +89,46 @@
 
 for item in mapped_list:
     print(item)
 # Output: List of TargetModel instances with mapped data
 ```
 
 
-## Usage of the Aggregator
+## Usage of the ModelAggregator
 
 ### Basic Setup
 
-First, define your source and target Pydantic models:
+First, define your source and target models:
 
 ```python
 from pydantic import BaseModel
+from pydantic.dataclasses import dataclass as pydantic_dataclass
 
 class SourceModel(BaseModel):
     id: int
     first_name: str
     last_name: str
 
-class TargetModel(BaseModel):
+@pydantic_dataclass
+class TargetModel:
     full_names: list[str]
 ```
 
 ### Aggregating Data
 
-To aggregate data from a list of `SourceModel` instances into a list of `TargetModel` instances, define an aggregator class by inheriting from `BaseModelAggregator`:
+To aggregate data from a list of `SourceModel` instances into a list of `TargetModel` instances, define an aggregator class by inheriting from `ModelAggregator`:
 
 ```python
-from py_transmuter.pydantic.aggregator import BaseModelAggregator
+from py_transmuter.models.aggregator import ModelAggregator
 
-class MyAggregator(BaseModelAggregator[TargetModel, SourceModel]):
+class MyAggregator(ModelAggregator[TargetModel, SourceModel]):
     mappings = {"full_names": lambda data: f"{data.first_name} {data.last_name}"}
 ```
 
-### Using the Aggregator
+### Using the ModelAggregator
 
 Once your aggregator is defined, you can use it to aggregate data as follows:
 
 ```python
 # Sample data
 source_data = [
     SourceModel(id=1, first_name="Jane", last_name="Doe"),
@@ -136,15 +139,15 @@
 aggregator = MyAggregator()
 target_data = aggregator.aggregate(source_data)
 
 print(target_data)
 # Output: [TargetModel(full_names=['Jane Doe', 'John Doe'])]
 ```
 
-### Advanced Usage of the Aggregator
+### Advanced Usage of the ModelAggregator
 
 For more complex scenarios, `py-transmuter` allows for advanced data transformation capabilities, including grouping, sorting, and using custom functions for mappings and aggregations. Here’s an elaborate example that showcases these features.
 
 #### Scenario
 
 Imagine you have a dataset of measurements taken by different sensors in a scientific experiment. Each measurement includes the sensor's ID, the timestamp of the measurement, and the measured value. Your goal is to aggregate these measurements by sensor ID and day, calculate the daily average value for each sensor, and sort the results by date.
 
@@ -163,23 +166,23 @@
 
 class DailyAverage(BaseModel):
     sensor_id: int
     date: date
     average_value: float
 ```
 
-#### Aggregator Class
+#### ModelAggregator Class
 
 Next, define the aggregator class that specifies how to group measurements, how to calculate the daily averages, and how to sort the results:
 
 ```python
-from py_transmuter.pydantic.aggregator import BaseModelAggregator
+from py_transmuter.models.aggregator import ModelAggregator
 from statistics import mean
 
-class MeasurementAggregator(BaseModelAggregator[DailyAverage, Measurement]):
+class MeasurementAggregator(ModelAggregator[DailyAverage, Measurement]):
     # Group by sensor ID and the date part of the timestamp
     group_by = (
         "sensor_id",
         lambda x: x.timestamp.date(),
     )
     
     # Define the aggregation to calculate the average value
@@ -211,30 +214,30 @@
 daily_averages = aggregator.aggregate(measurements)
 
 # Output the aggregated data
 print(daily_averages)
 # [DailyAverage(sensor_id=1, date=date(2024, 1, 1), average_value=15), DailyAverage(sensor_id=2, date=date(2024, 1, 1), value=30), ...]
 ```
 
-### Using mappings in the Aggregator
+### Using mappings in the ModelAggregator
 
 An `Aggregator` can have both `aggregation` and `mappings`; the former were explained above, but the latter serve a way simpler purpose: simply extract the value of field
 for every element in the group and store it in a list; for example:
 
 ```python
 class Child(BaseModel):
     parent: str
     first_name: str
     last_name: str
 
 class Parent(BaseModel):
     name: str
     children: list[str]
 
-class ChildParentAggregator(BaseModelAggregator[Parent, Child]):
+class ChildParentAggregator(ModelAggregator[Parent, Child]):
     group_by = ('parent',)
 
     mappings = {"children": lambda child: f"{child.first_name} {child.last_name}"}
     aggregations = {"name": ("parent": lambda names: names[0])}
 ```
 
 With this setup, we would then get:
@@ -249,40 +252,67 @@
 parents = ChildParentAggregator().aggregate(children)
 print(parents)
 # [Parent(name="Tom Smith", children=["Paul Smith", "Laura Smith"]), Parent(name="Anna Lopez", children=["Tupac Towers"])]
 ```
 
 ## Using self inspection
 
-There are many scenarios in which we need values that are known only in runtime and not when declaring the mappings and aggregations for our `Mapper` or `Aggregator` class;
+There are many scenarios in which we need values that are known only in runtime and not when declaring the mappings and aggregations for our `ModelMapper` or `ModelAggregator` class;
 for this, both these classes are capable of identifying methods that "belong to them" and it is possible to add them to the static definitions of `mappings` and `aggregations`,
 and can later access class or instance attributes in runtime.
 
 An example of this would be:
 
 ```python
-class A(BaseModel):
+@dataclass
+class A:
     id: int
 
-class B(BaseModel):
+@dataclass
+class B:
     id: str
 
-class ABMapper(BaseModelMapper[B, A]):
+class ABMapper(ModelMapper[B, A]):
     def map_id(self, data: A) -> str:
         return str(data.id * self.context["factor"])
 
     mapping = {"id": map_id}
 
 assert ABMapper(context={"factor": 2}).map(A(id=1)) == B(id="2")
 ```
 
-The `context` attribute is included by default in both the `Mapper` and the `Aggregator`, but you could define the class as you wish (with any attributes you'd want) and 
+The `context` attribute is included by default in both the `ModelMapper` and the `ModelAggregator`, but you could define the class as you wish (with any attributes you'd want) and 
 access them in the moment they are needed:
 
 ```python
-class Mapper(BaseModelMapper[B, A]):
+class Mapper(ModelMapper[B, A]):
     attribute: Any
 
     def __init__(self, attribute: Any, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.attribute = attribute
 ```
+
+## Dictionary Mapper and Aggregator
+
+Very similarly to what we can do with the `ModelMapper` and `ModelAggregator`, we can create a `DictionaryMapper` and `DictionaryAggregator`. These have the same functionalities
+we have seen above but allow for mapping and aggregation of dictionaries of type `dict[Any, Any]` (not restricted to `string` keys or JSON formats).
+
+An example of this would be:
+
+```python
+from py_transmuter.dictionaries.mapper import DictionaryMapper
+
+class Mapper(DictionaryMapper):
+    mapping = {
+        "id": 1,
+        ("march", 14): date(2021, 3, 14),
+    }
+
+mapper = Mapper()
+
+source = {1: "an_id", date(2021, 3, 14): "Tomorrow is Pi day!"}
+mapper.map(source)
+# {"id": "an_id", ("march, 14"): "Tomorrow is Pi day!"}
+```
+
+This seems quite odd, but who knows, maybe you're the one who finds it useful!
```

### Comparing `py_transmuter-0.1.2/pyproject.toml` & `py_transmuter-0.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,26 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "py-transmuter"
-version = "0.1.2"
+version = "0.2.0"
 authors = [
     {name="Rodrigo De Rosa", email="rodrigoderosa15@gmail.com"},
 ]
 description = "A library that facilitates mapping and aggregating objects from one model to another"
 readme = "README.md"
 license = {file = "LICENSE"}
 requires-python = ">=3.12.0"
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3.12",
     "Framework :: Pydantic :: 2",
 ]
-dependencies = [
-    "pydantic==2.5.3",
-]
+dependencies = []
 
 [project.urls]
 Homepage = "https://github.com/RodrigoDeRosa/py-transmuter"
 Issues = "https://github.com/RodrigoDeRosa/py-transmuter/issues"
```

### Comparing `py_transmuter-0.1.2/PKG-INFO` & `py_transmuter-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: py-transmuter
-Version: 0.1.2
+Version: 0.2.0
 Summary: A library that facilitates mapping and aggregating objects from one model to another
 Project-URL: Homepage, https://github.com/RodrigoDeRosa/py-transmuter
 Project-URL: Issues, https://github.com/RodrigoDeRosa/py-transmuter/issues
 Author-email: Rodrigo De Rosa <rodrigoderosa15@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 Rodrigo De Rosa
@@ -29,72 +29,72 @@
 License-File: LICENSE
 Classifier: Development Status :: 3 - Alpha
 Classifier: Framework :: Pydantic :: 2
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.12
 Requires-Python: >=3.12.0
-Requires-Dist: pydantic==2.5.3
 Description-Content-Type: text/markdown
 
 # PyTransmuter
 
-PyTransmuter is a Python library designed for efficient data mapping and aggregation 
-from source models to target models, leveraging the power of Pydantic for data validation
-and transformation. It simplifies the process of transforming data structures, making it 
-an essential tool for applications requiring data normalization, transformation, and aggregation.
+PyTransmuter is a Python library designed for efficient data mapping and aggregation from source 
+models to target models. It simplifies the process of transforming data structures, even between classes
+of different types (this is, you can transform from a `BaseModel` to a `@dataclass` if you need to) or 
+even transform data in Python dictionaries.
 
 ## Features
 
-- **Generic Mapping**: Utilizes generic typing to map data between different model structures.
+- **Generic Mapping**: Utilizes generic typing to map data between different model structures; for example, Python's `@dataclass`, 
+Pydantic's `BaseModel`, Pydantic's `@dataclass` or even plain dictionaries.
 - **Flexible Aggregation**: Supports complex data aggregation strategies, including grouping, 
 sorting, and custom aggregation functions.
 - **Self-Inspection**: Incorporates self-inspection capabilities for resolving callables related 
 to class instances.
-- **Pydantic Integration**: Leverages Pydantic models for input and output validation, ensuring 
-data integrity.
 - **Customizable Transformations**: Allows defining custom field transformations using callable 
 functions or lambdas.
 
 ## Installation
 
 To install the library, run the following command in your terminal:
 
 ```bash
 pip install py-transmuter
 ```
 
-## Usage of the Mapper
+## Usage of the ModelMapper
 
 ### Basic Setup
 
-Start by defining your source and target Pydantic models that represent the structure of your input and output data:
+Start by defining your source and target models that represent the structure of your input and output data:
 
 ```python
 from pydantic import BaseModel
+from dataclasses import dataclass
 
-class SourceModel(BaseModel):
+@dataclass
+class SourceModel:
     id: int
     temperature_celsius: float
     humidity_percentage: int
 
 class TargetModel(BaseModel):
     id: int
     temperature_fahrenheit: float
     humidity_proportion: float
 ```
 
-### Implementing a Mapper
+### Implementing a ModelMapper
 
-Define a mapper by inheriting from `BaseModelMapper`, specifying how each field in the source model maps to the target model:
+Define a mapper by inheriting from `ModelMapper`, specifying how each field in the source model maps to the target model:
 
 ```python
-from py_transmuter.pydantic.mapper import BaseModelMapper
+from py_transmuter.models.mapper import ModelMapper
 
-class MyMapper(BaseModelMapper[TargetModel, SourceModel]):
+class MyMapper(ModelMapper[TargetModel, SourceModel]):
     mapping = {
         "id": "id",
         "temperature_fahrenheit": ("temperature_celsius", lambda c: c * 9 / 5 + 32),
         "humidity_proportion": ("humidity_percentage", lambda h: h / 100.0),
     }
 ```
 
@@ -110,15 +110,15 @@
 
 print(target_data)
 # Output: TargetModel(id=1, temperature_fahrenheit=77.0, humidity_proportion=0.5)
 ```
 
 ### Mapping Lists of Data
 
-`BaseModelMapper` also supports mapping lists of data from source models to target models:
+`ModelMapper` also supports mapping lists of data from source models to target models:
 
 ```python
 source_list = [
     SourceModel(id=1, temperature_celsius=25, humidity_percentage=50),
     SourceModel(id=2, temperature_celsius=20, humidity_percentage=60),
 ]
 
@@ -126,44 +126,46 @@
 
 for item in mapped_list:
     print(item)
 # Output: List of TargetModel instances with mapped data
 ```
 
 
-## Usage of the Aggregator
+## Usage of the ModelAggregator
 
 ### Basic Setup
 
-First, define your source and target Pydantic models:
+First, define your source and target models:
 
 ```python
 from pydantic import BaseModel
+from pydantic.dataclasses import dataclass as pydantic_dataclass
 
 class SourceModel(BaseModel):
     id: int
     first_name: str
     last_name: str
 
-class TargetModel(BaseModel):
+@pydantic_dataclass
+class TargetModel:
     full_names: list[str]
 ```
 
 ### Aggregating Data
 
-To aggregate data from a list of `SourceModel` instances into a list of `TargetModel` instances, define an aggregator class by inheriting from `BaseModelAggregator`:
+To aggregate data from a list of `SourceModel` instances into a list of `TargetModel` instances, define an aggregator class by inheriting from `ModelAggregator`:
 
 ```python
-from py_transmuter.pydantic.aggregator import BaseModelAggregator
+from py_transmuter.models.aggregator import ModelAggregator
 
-class MyAggregator(BaseModelAggregator[TargetModel, SourceModel]):
+class MyAggregator(ModelAggregator[TargetModel, SourceModel]):
     mappings = {"full_names": lambda data: f"{data.first_name} {data.last_name}"}
 ```
 
-### Using the Aggregator
+### Using the ModelAggregator
 
 Once your aggregator is defined, you can use it to aggregate data as follows:
 
 ```python
 # Sample data
 source_data = [
     SourceModel(id=1, first_name="Jane", last_name="Doe"),
@@ -174,15 +176,15 @@
 aggregator = MyAggregator()
 target_data = aggregator.aggregate(source_data)
 
 print(target_data)
 # Output: [TargetModel(full_names=['Jane Doe', 'John Doe'])]
 ```
 
-### Advanced Usage of the Aggregator
+### Advanced Usage of the ModelAggregator
 
 For more complex scenarios, `py-transmuter` allows for advanced data transformation capabilities, including grouping, sorting, and using custom functions for mappings and aggregations. Here’s an elaborate example that showcases these features.
 
 #### Scenario
 
 Imagine you have a dataset of measurements taken by different sensors in a scientific experiment. Each measurement includes the sensor's ID, the timestamp of the measurement, and the measured value. Your goal is to aggregate these measurements by sensor ID and day, calculate the daily average value for each sensor, and sort the results by date.
 
@@ -201,23 +203,23 @@
 
 class DailyAverage(BaseModel):
     sensor_id: int
     date: date
     average_value: float
 ```
 
-#### Aggregator Class
+#### ModelAggregator Class
 
 Next, define the aggregator class that specifies how to group measurements, how to calculate the daily averages, and how to sort the results:
 
 ```python
-from py_transmuter.pydantic.aggregator import BaseModelAggregator
+from py_transmuter.models.aggregator import ModelAggregator
 from statistics import mean
 
-class MeasurementAggregator(BaseModelAggregator[DailyAverage, Measurement]):
+class MeasurementAggregator(ModelAggregator[DailyAverage, Measurement]):
     # Group by sensor ID and the date part of the timestamp
     group_by = (
         "sensor_id",
         lambda x: x.timestamp.date(),
     )
     
     # Define the aggregation to calculate the average value
@@ -249,30 +251,30 @@
 daily_averages = aggregator.aggregate(measurements)
 
 # Output the aggregated data
 print(daily_averages)
 # [DailyAverage(sensor_id=1, date=date(2024, 1, 1), average_value=15), DailyAverage(sensor_id=2, date=date(2024, 1, 1), value=30), ...]
 ```
 
-### Using mappings in the Aggregator
+### Using mappings in the ModelAggregator
 
 An `Aggregator` can have both `aggregation` and `mappings`; the former were explained above, but the latter serve a way simpler purpose: simply extract the value of field
 for every element in the group and store it in a list; for example:
 
 ```python
 class Child(BaseModel):
     parent: str
     first_name: str
     last_name: str
 
 class Parent(BaseModel):
     name: str
     children: list[str]
 
-class ChildParentAggregator(BaseModelAggregator[Parent, Child]):
+class ChildParentAggregator(ModelAggregator[Parent, Child]):
     group_by = ('parent',)
 
     mappings = {"children": lambda child: f"{child.first_name} {child.last_name}"}
     aggregations = {"name": ("parent": lambda names: names[0])}
 ```
 
 With this setup, we would then get:
@@ -287,40 +289,67 @@
 parents = ChildParentAggregator().aggregate(children)
 print(parents)
 # [Parent(name="Tom Smith", children=["Paul Smith", "Laura Smith"]), Parent(name="Anna Lopez", children=["Tupac Towers"])]
 ```
 
 ## Using self inspection
 
-There are many scenarios in which we need values that are known only in runtime and not when declaring the mappings and aggregations for our `Mapper` or `Aggregator` class;
+There are many scenarios in which we need values that are known only in runtime and not when declaring the mappings and aggregations for our `ModelMapper` or `ModelAggregator` class;
 for this, both these classes are capable of identifying methods that "belong to them" and it is possible to add them to the static definitions of `mappings` and `aggregations`,
 and can later access class or instance attributes in runtime.
 
 An example of this would be:
 
 ```python
-class A(BaseModel):
+@dataclass
+class A:
     id: int
 
-class B(BaseModel):
+@dataclass
+class B:
     id: str
 
-class ABMapper(BaseModelMapper[B, A]):
+class ABMapper(ModelMapper[B, A]):
     def map_id(self, data: A) -> str:
         return str(data.id * self.context["factor"])
 
     mapping = {"id": map_id}
 
 assert ABMapper(context={"factor": 2}).map(A(id=1)) == B(id="2")
 ```
 
-The `context` attribute is included by default in both the `Mapper` and the `Aggregator`, but you could define the class as you wish (with any attributes you'd want) and 
+The `context` attribute is included by default in both the `ModelMapper` and the `ModelAggregator`, but you could define the class as you wish (with any attributes you'd want) and 
 access them in the moment they are needed:
 
 ```python
-class Mapper(BaseModelMapper[B, A]):
+class Mapper(ModelMapper[B, A]):
     attribute: Any
 
     def __init__(self, attribute: Any, *args, **kwargs):
         super().__init__(*args, **kwargs)
         self.attribute = attribute
 ```
+
+## Dictionary Mapper and Aggregator
+
+Very similarly to what we can do with the `ModelMapper` and `ModelAggregator`, we can create a `DictionaryMapper` and `DictionaryAggregator`. These have the same functionalities
+we have seen above but allow for mapping and aggregation of dictionaries of type `dict[Any, Any]` (not restricted to `string` keys or JSON formats).
+
+An example of this would be:
+
+```python
+from py_transmuter.dictionaries.mapper import DictionaryMapper
+
+class Mapper(DictionaryMapper):
+    mapping = {
+        "id": 1,
+        ("march", 14): date(2021, 3, 14),
+    }
+
+mapper = Mapper()
+
+source = {1: "an_id", date(2021, 3, 14): "Tomorrow is Pi day!"}
+mapper.map(source)
+# {"id": "an_id", ("march, 14"): "Tomorrow is Pi day!"}
+```
+
+This seems quite odd, but who knows, maybe you're the one who finds it useful!
```

